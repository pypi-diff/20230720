# Comparing `tmp/aleksis_app_csvimport-3.0.1.tar.gz` & `tmp/aleksis_app_csvimport-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_csvimport-3.0.1.tar", max compression
+gzip compressed data, was "aleksis_app_csvimport-3.0b0.tar", max compression
```

## Comparing `aleksis_app_csvimport-3.0.1.tar` & `aleksis_app_csvimport-3.0b0.tar`

### file list

```diff
@@ -1,89 +1,91 @@
--rw-r--r--   0        0        0     6353 2023-07-20 19:12:37.728159 aleksis_app_csvimport-3.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-07-20 19:12:37.728159 aleksis_app_csvimport-3.0.1/LICENCE.rst
--rw-r--r--   0        0        0     1594 2023-07-20 19:12:37.728159 aleksis_app_csvimport-3.0.1/README.rst
--rw-r--r--   0        0        0      155 2023-07-20 19:12:37.728159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__init__.py
--rw-r--r--   0        0        0      454 2023-07-20 19:14:58.817481 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      421 2023-07-20 19:15:02.853633 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0     1666 2023-07-20 19:15:00.777555 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    30686 2023-07-20 19:15:02.729628 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/field_types.cpython-311.pyc
--rw-r--r--   0        0        0      704 2023-07-20 19:15:02.969637 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/model_extensions.cpython-311.pyc
--rw-r--r--   0        0        0    11854 2023-07-20 19:15:02.725628 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     2891 2023-07-20 19:15:03.089642 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1134 2023-07-20 19:15:02.897635 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0      435 2023-07-20 19:14:59.021489 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0      129 2023-07-20 19:12:37.728159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/admin.py
--rw-r--r--   0        0        0      993 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/apps.py
--rw-r--r--   0        0        0      603 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/default_templates.py
--rw-r--r--   0        0        0     4758 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/default_templates.yaml
--rw-r--r--   0        0        0    15681 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/field_types.py
--rw-r--r--   0        0        0     1946 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/forms.py
--rw-r--r--   0        0        0     1469 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/frontend/index.js
--rw-r--r--   0        0        0      187 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/frontend/messages/de.json
--rw-r--r--   0        0        0      182 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/frontend/messages/en.json
--rw-r--r--   0        0        0      225 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/frontend/messages/ru.json
--rw-r--r--   0        0        0      221 2023-07-20 19:12:37.732159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/frontend/messages/uk.json
--rw-r--r--   0        0        0      463 2023-07-20 19:15:03.493657 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9782 2023-07-20 19:12:37.736159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8154 2023-07-20 19:15:03.605661 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15409 2023-07-20 19:12:37.740159 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-07-20 19:15:03.477657 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9698 2023-07-20 19:12:37.744160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-20 19:15:03.605661 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9652 2023-07-20 19:12:37.748160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-20 19:15:03.473657 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9652 2023-07-20 19:12:37.748160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10410 2023-07-20 19:15:03.501658 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15141 2023-07-20 19:12:37.748160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-20 19:15:03.481657 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9652 2023-07-20 19:12:37.756160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10209 2023-07-20 19:15:03.481657 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14940 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/management/commands/__init__.py
--rw-r--r--   0        0        0     1875 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/management/commands/csv_import.py
--rw-r--r--   0        0        0      718 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/menus.py
--rw-r--r--   0        0        0     7500 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0001_initial.py
--rw-r--r--   0        0        0     1549 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0002_importjob.py
--rw-r--r--   0        0        0      510 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0003_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      540 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0004_args.py
--rw-r--r--   0        0        0      479 2023-07-20 19:12:37.760160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0005_optional_index_col.py
--rw-r--r--   0        0        0      438 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0006_from_default_field.py
--rw-r--r--   0        0        0      709 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0007_virtual_template_field.py
--rw-r--r--   0        0        0      486 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0008_configurable_quotechar.py
--rw-r--r--   0        0        0        0 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/__init__.py
--rw-r--r--   0        0        0      274 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/model_extensions.py
--rw-r--r--   0        0        0     7679 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/models.py
--rw-r--r--   0        0        0     1573 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/preferences.py
--rw-r--r--   0        0        0      851 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/rules.py
--rw-r--r--   0        0        0      239 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/settings.py
--rw-r--r--   0        0        0      340 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tables.py
--rw-r--r--   0        0        0      373 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tasks.py
--rw-r--r--   0        0        0      934 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/templates/csv_import/csv_import.html
--rw-r--r--   0        0        0      709 2023-07-20 19:12:37.764160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/templates/csv_import/import_template/list.html
--rw-r--r--   0        0        0      518 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/templates/csv_import/import_template/upload.html
--rw-r--r--   0        0        0     1067 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/models/test_template.py
--rw-r--r--   0        0        0     3259 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/models/test_template_load.py
--rw-r--r--   0        0        0     2954 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/test_field_types.py
--rw-r--r--   0        0        0     3358 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/util/test_class_range_helpers.py
--rw-r--r--   0        0        0     2876 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/util/test_converters.py
--rw-r--r--   0        0        0      365 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/util/test_import_helpers.py
--rw-r--r--   0        0        0      334 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/urls.py
--rw-r--r--   0        0        0     5561 2023-07-20 19:15:02.733629 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/__pycache__/class_range_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     4549 2023-07-20 19:15:02.733629 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/__pycache__/converters.cpython-311.pyc
--rw-r--r--   0        0        0      732 2023-07-20 19:15:02.733629 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/__pycache__/import_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     3824 2023-07-20 19:12:37.768160 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/class_range_helpers.py
--rw-r--r--   0        0        0     2287 2023-07-20 19:12:37.772161 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/converters.py
--rw-r--r--   0        0        0      359 2023-07-20 19:12:37.772161 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/import_helpers.py
--rw-r--r--   0        0        0    12182 2023-07-20 19:12:37.772161 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/process.py
--rw-r--r--   0        0        0     2867 2023-07-20 19:12:37.772161 aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/views.py
--rw-r--r--   0        0        0      581 2023-07-20 19:12:37.772161 aleksis_app_csvimport-3.0.1/docs/Makefile
--rw-r--r--   0        0        0      104 2023-07-20 19:12:37.776161 aleksis_app_csvimport-3.0.1/docs/admin/00_index.rst
--rw-r--r--   0        0        0     1355 2023-07-20 19:12:37.776161 aleksis_app_csvimport-3.0.1/docs/admin/01_concept.rst
--rw-r--r--   0        0        0      836 2023-07-20 19:12:37.776161 aleksis_app_csvimport-3.0.1/docs/admin/05_configuration.rst
--rw-r--r--   0        0        0      619 2023-07-20 19:12:37.776161 aleksis_app_csvimport-3.0.1/docs/admin/10_exporting_data.rst
--rw-r--r--   0        0        0     1076 2023-07-20 19:12:37.776161 aleksis_app_csvimport-3.0.1/docs/admin/20_import_data.rst
--rw-r--r--   0        0        0     6402 2023-07-20 19:12:37.776161 aleksis_app_csvimport-3.0.1/docs/conf.py
--rw-r--r--   0        0        0      532 2023-07-20 19:12:37.776161 aleksis_app_csvimport-3.0.1/docs/index.rst
--rw-r--r--   0        0        0      787 2023-07-20 19:12:37.776161 aleksis_app_csvimport-3.0.1/docs/make.bat
--rw-r--r--   0        0        0     2540 2023-07-20 19:13:13.633513 aleksis_app_csvimport-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-07-20 19:12:37.780161 aleksis_app_csvimport-3.0.1/tox.ini
--rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 aleksis_app_csvimport-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5835 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1594 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/README.rst
+-rw-r--r--   0        0        0      155 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__init__.py
+-rw-r--r--   0        0        0      454 2023-02-27 16:45:50.770732 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      421 2023-02-27 16:45:52.554729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0     1977 2023-02-27 16:45:51.310732 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     1525 2023-02-27 16:45:52.766729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/default_templates.cpython-311.pyc
+-rw-r--r--   0        0        0    30602 2023-02-27 16:45:52.098730 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/field_types.cpython-311.pyc
+-rw-r--r--   0        0        0      704 2023-02-27 16:45:52.594729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/model_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0    11426 2023-02-27 16:45:52.090730 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     2891 2023-02-27 16:45:52.626729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1134 2023-02-27 16:45:52.570729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0      435 2023-02-27 16:45:50.778732 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/admin.py
+-rw-r--r--   0        0        0     1258 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/apps.py
+-rw-r--r--   0        0        0      603 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/default_templates.py
+-rw-r--r--   0        0        0     4758 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/default_templates.yaml
+-rw-r--r--   0        0        0    15561 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/field_types.py
+-rw-r--r--   0        0        0     1946 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/forms.py
+-rw-r--r--   0        0        0     1469 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/index.js
+-rw-r--r--   0        0        0      187 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/messages/de.json
+-rw-r--r--   0        0        0      182 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/messages/en.json
+-rw-r--r--   0        0        0      225 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/messages/ru.json
+-rw-r--r--   0        0        0      221 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/messages/uk.json
+-rw-r--r--   0        0        0      463 2023-02-27 16:45:52.858729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9782 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8154 2023-02-27 16:45:52.850729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15409 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-02-27 16:45:52.846729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9698 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:45:52.858729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9652 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:45:52.838729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9652 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10397 2023-02-27 16:45:52.846729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15137 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:45:52.854729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9652 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10206 2023-02-27 16:45:52.842728 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14949 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/management/commands/__init__.py
+-rw-r--r--   0        0        0     1875 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/management/commands/csv_import.py
+-rw-r--r--   0        0        0      718 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/menus.py
+-rw-r--r--   0        0        0     7500 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1549 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0002_importjob.py
+-rw-r--r--   0        0        0      510 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0003_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      540 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0004_args.py
+-rw-r--r--   0        0        0      479 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0005_optional_index_col.py
+-rw-r--r--   0        0        0      438 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0006_from_default_field.py
+-rw-r--r--   0        0        0      709 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0007_virtual_template_field.py
+-rw-r--r--   0        0        0      486 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0008_configurable_quotechar.py
+-rw-r--r--   0        0        0        0 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/__init__.py
+-rw-r--r--   0        0        0      274 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/model_extensions.py
+-rw-r--r--   0        0        0     7521 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/models.py
+-rw-r--r--   0        0        0     1573 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/preferences.py
+-rw-r--r--   0        0        0      851 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/rules.py
+-rw-r--r--   0        0        0      239 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/settings.py
+-rw-r--r--   0        0        0      340 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tables.py
+-rw-r--r--   0        0        0      373 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tasks.py
+-rw-r--r--   0        0        0      934 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/csv_import.html
+-rw-r--r--   0        0        0      709 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/import_template/list.html
+-rw-r--r--   0        0        0      518 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/import_template/upload.html
+-rw-r--r--   0        0        0     1067 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/models/test_template.py
+-rw-r--r--   0        0        0     3217 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/models/test_template_load.py
+-rw-r--r--   0        0        0     2954 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/test_field_types.py
+-rw-r--r--   0        0        0     3358 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_class_range_helpers.py
+-rw-r--r--   0        0        0     2934 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_converters.py
+-rw-r--r--   0        0        0      365 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_import_helpers.py
+-rw-r--r--   0        0        0      334 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/urls.py
+-rw-r--r--   0        0        0     5561 2023-02-27 16:45:52.102730 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/class_range_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     4528 2023-02-27 16:45:52.102730 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/converters.cpython-311.pyc
+-rw-r--r--   0        0        0      732 2023-02-27 16:45:52.518729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/import_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     3824 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/class_range_helpers.py
+-rw-r--r--   0        0        0     2295 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/converters.py
+-rw-r--r--   0        0        0      359 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/import_helpers.py
+-rw-r--r--   0        0        0    12255 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/process.py
+-rw-r--r--   0        0        0     2867 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/views.py
+-rw-r--r--   0        0        0      581 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/Makefile
+-rw-r--r--   0        0        0      104 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     1355 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/01_concept.rst
+-rw-r--r--   0        0        0      836 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/05_configuration.rst
+-rw-r--r--   0        0        0      619 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/10_exporting_data.rst
+-rw-r--r--   0        0        0     1076 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/20_import_data.rst
+-rw-r--r--   0        0        0     6402 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/conf.py
+-rw-r--r--   0        0        0      532 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/make.bat
+-rw-r--r--   0        0        0     1576 2023-02-27 16:43:10.143036 aleksis_app_csvimport-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/tox.ini
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 aleksis_app_csvimport-3.0b0/setup.py
+-rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 aleksis_app_csvimport-3.0b0/PKG-INFO
```

### Comparing `aleksis_app_csvimport-3.0.1/CHANGELOG.rst` & `aleksis_app_csvimport-3.0b0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,33 +2,16 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0.1`_ - 2023-07-20
----------------------
-
-Fixed
-~~~~~
-
-* CSV import app caused long delay on AlekSIS startup
-
-`3.0`_ - 2023-05-12
--------------------
-
-Changed
-~~~~~~~
-
-* Ukrainian translations were updated.
-* Phonenumber country is now configured using the `PHONENUMBER_DEFAULT_REGION` setting.
-
-`3.0b0`_ - 2023-02-22
----------------------
+`3.0b0` - 2023-02-22
+--------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 Removed
 ~~~~~~~
 
@@ -41,15 +24,14 @@
 * If activated, imports with regex field types will show error messages
   when there is no match.
 
 Fixed
 ~~~~~
 
 * The reg ex field type wasn't usable with own templates.
-* Import failed if a file columns was empty.
 
 `2.3`_ - 2022-06-25
 -------------------
 
 Added
 ~~~~~
 
@@ -212,21 +194,19 @@
 ~~~~~
 
 * Use bootstrap buttons everywhere.
 
 .. _Keep a Changelog: https://keepachangelog.com/en/1.0.0/
 .. _Semantic Versioning: https://semver.org/spec/v2.0.0.html
 
-.. _1.0a1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/1.0a1
-.. _1.0a2: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/1.0a2
-.. _2.0b0: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0b0
-.. _2.0b1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0b1
-.. _2.0rc1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0rc1
-.. _2.0rc2: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0rc2
-.. _2.0: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0
-.. _2.1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.1
-.. _2.2: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.2
-.. _2.2.1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.2.1
-.. _2.3: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.3
-.. _3.0b0: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/3.0b0
-.. _3.0: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/3.0
-.. _3.0.1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/3.0.1
+.. _1.0a1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/1.0a1
+.. _1.0a2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/1.0a2
+.. _2.0b0: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0b0
+.. _2.0b1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0b1
+.. _2.0rc1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0rc1
+.. _2.0rc2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0rc2
+.. _2.0: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0
+.. _2.1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.1
+.. _2.2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.2
+.. _2.2.1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.2.1
+.. _2.3: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.3
+.. _3.0b0: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/3.0b0
```

### Comparing `aleksis_app_csvimport-3.0.1/LICENCE.rst` & `aleksis_app_csvimport-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/README.rst` & `aleksis_app_csvimport-3.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/apps.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/apps.cpython-311.pyc`

 * *Files 26% similar despite different names*

#### Python bytecode

```diff
@@ -1,117 +1,136 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
-files sz: 993
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
+files sz: 1258
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a010100020047006402840064036501a60300
-      00ab0300000000000000005a0264045300
+      0x9700640064016c006d015a010100640064026c026d035a036d045a0401
+      00640064036c056d065a060100020047006404840064056506a6030000ab
+      0300000000000000005a0764065300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('AppConfig',))
-                 6 IMPORT_NAME              0 (aleksis.core.util.apps)
-                 8 IMPORT_FROM              1 (AppConfig)
-                10 STORE_NAME               1 (AppConfig)
+                 4 LOAD_CONST               1 (('ImproperlyConfigured',))
+                 6 IMPORT_NAME              0 (django.core.exceptions)
+                 8 IMPORT_FROM              1 (ImproperlyConfigured)
+                10 STORE_NAME               1 (ImproperlyConfigured)
                 12 POP_TOP
    
-     4          14 PUSH_NULL
-                16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object CSVImportConfig, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/apps.py", line 4>)
-                20 MAKE_FUNCTION            0
-                22 LOAD_CONST               3 ('CSVImportConfig')
-                24 LOAD_NAME                1 (AppConfig)
-                26 PRECALL                  3
-                30 CALL                     3
-                40 STORE_NAME               2 (CSVImportConfig)
-                42 LOAD_CONST               4 (None)
-                44 RETURN_VALUE
+     2          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('OperationalError', 'ProgrammingError'))
+                18 IMPORT_NAME              2 (django.db)
+                20 IMPORT_FROM              3 (OperationalError)
+                22 STORE_NAME               3 (OperationalError)
+                24 IMPORT_FROM              4 (ProgrammingError)
+                26 STORE_NAME               4 (ProgrammingError)
+                28 POP_TOP
+   
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('AppConfig',))
+                34 IMPORT_NAME              5 (aleksis.core.util.apps)
+                36 IMPORT_FROM              6 (AppConfig)
+                38 STORE_NAME               6 (AppConfig)
+                40 POP_TOP
+   
+     7          42 PUSH_NULL
+                44 LOAD_BUILD_CLASS
+                46 LOAD_CONST               4 (<code object CSVImportConfig, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/apps.py", line 7>)
+                48 MAKE_FUNCTION            0
+                50 LOAD_CONST               5 ('CSVImportConfig')
+                52 LOAD_NAME                6 (AppConfig)
+                54 PRECALL                  3
+                58 CALL                     3
+                68 STORE_NAME               7 (CSVImportConfig)
+                70 LOAD_CONST               6 (None)
+                72 RETURN_VALUE
    consts
       0
+      ('ImproperlyConfigured',)
+      ('OperationalError', 'ProgrammingError')
       ('AppConfig',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364025a0464035a056404640569
             015a0664065a0767006407a2016408640966036700640aa201640b640c66
             03640d6701640e640f6603640d6701641064116603641267016413641466
             0366055a0888006601641584085a09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-           4           2 RESUME                   0
+           7           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('CSVImportConfig')
                       10 STORE_NAME               2 (__qualname__)
          
-           5          12 LOAD_CONST               1 ('aleksis.apps.csv_import')
+           8          12 LOAD_CONST               1 ('aleksis.apps.csv_import')
                       14 STORE_NAME               3 (name)
          
-           6          16 LOAD_CONST               2 ('AlekSIS-App-CSVImport')
+           9          16 LOAD_CONST               2 ('AlekSIS-App-CSVImport')
                       18 STORE_NAME               4 (dist_name)
          
-           7          20 LOAD_CONST               3 ('AlekSIS —\u200aCSV import')
+          10          20 LOAD_CONST               3 ('AlekSIS —\u200aCSV import')
                       22 STORE_NAME               5 (verbose_name)
          
-          10          24 LOAD_CONST               4 ('Repository')
+          13          24 LOAD_CONST               4 ('Repository')
                       26 LOAD_CONST               5 ('https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/')
          
-           9          28 BUILD_MAP                1
+          12          28 BUILD_MAP                1
                       30 STORE_NAME               6 (urls)
          
-          12          32 LOAD_CONST               6 ('EUPL-1.2+')
+          15          32 LOAD_CONST               6 ('EUPL-1.2+')
                       34 STORE_NAME               7 (licence)
          
-          14          36 BUILD_LIST               0
+          17          36 BUILD_LIST               0
                       38 LOAD_CONST               7 ((2019, 2020, 2022))
                       40 LIST_EXTEND              1
                       42 LOAD_CONST               8 ('Dominik George')
                       44 LOAD_CONST               9 ('dominik.george@teckids.org')
                       46 BUILD_TUPLE              3
          
-          15          48 BUILD_LIST               0
+          18          48 BUILD_LIST               0
                       50 LOAD_CONST              10 ((2020, 2021, 2022))
                       52 LIST_EXTEND              1
                       54 LOAD_CONST              11 ('Jonathan Weth')
                       56 LOAD_CONST              12 ('dev@jonathanweth.de')
                       58 BUILD_TUPLE              3
          
-          16          60 LOAD_CONST              13 (2019)
+          19          60 LOAD_CONST              13 (2019)
                       62 BUILD_LIST               1
                       64 LOAD_CONST              14 ('mirabilos')
                       66 LOAD_CONST              15 ('thorsten.glaser@teckids.org')
                       68 BUILD_TUPLE              3
          
-          17          70 LOAD_CONST              13 (2019)
+          20          70 LOAD_CONST              13 (2019)
                       72 BUILD_LIST               1
                       74 LOAD_CONST              16 ('Tom Teichler')
                       76 LOAD_CONST              17 ('tom.teichler@teckids.org')
                       78 BUILD_TUPLE              3
          
-          18          80 LOAD_CONST              18 (2022)
+          21          80 LOAD_CONST              18 (2022)
                       82 BUILD_LIST               1
                       84 LOAD_CONST              19 ('magicfelix')
                       86 LOAD_CONST              20 ('felix@felix-zauberer.de')
                       88 BUILD_TUPLE              3
          
-          13          90 BUILD_TUPLE              5
+          16          90 BUILD_TUPLE              5
                       92 STORE_NAME               8 (copyright_info)
          
-          21          94 LOAD_CLOSURE             0 (__class__)
+          24          94 LOAD_CLOSURE             0 (__class__)
                       96 BUILD_TUPLE              1
-                      98 LOAD_CONST              21 (<code object _maintain_default_data, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/apps.py", line 21>)
+                      98 LOAD_CONST              21 (<code object ready, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/apps.py", line 24>)
                      100 MAKE_FUNCTION            8 (closure)
-                     102 STORE_NAME               9 (_maintain_default_data)
+                     102 STORE_NAME               9 (ready)
                      104 LOAD_CLOSURE             0 (__class__)
                      106 COPY                     1
                      108 STORE_NAME              10 (__classcell__)
                      110 RETURN_VALUE
          consts
             'CSVImportConfig'
             'aleksis.apps.csv_import'
@@ -132,71 +151,105 @@
             'Tom Teichler'
             'tom.teichler@teckids.org'
             2022
             'magicfelix'
             'felix@felix-zauberer.de'
             code
                argcount  : 1
-               nlocals   : 2
-               stacksize : 2
+               nlocals   : 3
+               stacksize : 5
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a0010000000000000000000000000000000000000000a6000000ab0000
-                  000000000000000100640164026c026d037d01010002007c01a6000000ab
-                  000000000000000000010064005300
+                  0000000000000001000900640164026c026d037d01010002007c01a60000
+                  00ab00000000000000000001006400530023007408000000000000000000
+                  00740a00000000000000000000740c000000000000000000006603240072
+                  0b7d02590064007d027e026400530064007d027e02770177007803590077
+                  01
                              0 COPY_FREE_VARS           1
                
-                21           2 RESUME                   0
+                24           2 RESUME                   0
                
-                22           4 LOAD_GLOBAL              1 (NULL + super)
+                25           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
-                            30 LOAD_METHOD              1 (_maintain_default_data)
+                            30 LOAD_METHOD              1 (ready)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 POP_TOP
                
-                25          68 LOAD_CONST               1 (0)
-                            70 LOAD_CONST               2 (('update_or_create_default_templates',))
-                            72 IMPORT_NAME              2 (aleksis.apps.csv_import.default_templates)
-                            74 IMPORT_FROM              3 (update_or_create_default_templates)
-                            76 STORE_FAST               1 (update_or_create_default_templates)
-                            78 POP_TOP
-               
-                29          80 PUSH_NULL
-                            82 LOAD_FAST                1 (update_or_create_default_templates)
-                            84 PRECALL                  0
-                            88 CALL                     0
-                            98 POP_TOP
-                           100 LOAD_CONST               0 (None)
-                           102 RETURN_VALUE
+                28          68 NOP
+               
+                29          70 LOAD_CONST               1 (0)
+                            72 LOAD_CONST               2 (('update_or_create_default_templates',))
+                            74 IMPORT_NAME              2 (aleksis.apps.csv_import.default_templates)
+                            76 IMPORT_FROM              3 (update_or_create_default_templates)
+                            78 STORE_FAST               1 (update_or_create_default_templates)
+                            80 POP_TOP
+               
+                33          82 PUSH_NULL
+                            84 LOAD_FAST                1 (update_or_create_default_templates)
+                            86 PRECALL                  0
+                            90 CALL                     0
+                           100 POP_TOP
+                           102 LOAD_CONST               0 (None)
+                           104 RETURN_VALUE
+                       >>  106 PUSH_EXC_INFO
+               
+                34         108 LOAD_GLOBAL              8 (ProgrammingError)
+                           120 LOAD_GLOBAL             10 (OperationalError)
+                           132 LOAD_GLOBAL             12 (ImproperlyConfigured)
+                           144 BUILD_TUPLE              3
+                           146 CHECK_EXC_MATCH
+                           148 POP_JUMP_FORWARD_IF_FALSE    11 (to 172)
+                           150 STORE_FAST               2 (e)
+               
+                36         152 POP_EXCEPT
+                           154 LOAD_CONST               0 (None)
+                           156 STORE_FAST               2 (e)
+                           158 DELETE_FAST              2 (e)
+                           160 LOAD_CONST               0 (None)
+                           162 RETURN_VALUE
+                           164 LOAD_CONST               0 (None)
+                           166 STORE_FAST               2 (e)
+                           168 DELETE_FAST              2 (e)
+                           170 RERAISE                  1
+               
+                34     >>  172 RERAISE                  0
+                       >>  174 COPY                     3
+                           176 POP_EXCEPT
+                           178 RERAISE                  1
+               ExceptionTable:
+                 70 to 100 -> 106 [0]
+                 106 to 150 -> 174 [1] lasti
+                 164 to 172 -> 174 [1] lasti
                consts
                   None
                   0
                   ('update_or_create_default_templates',)
-               names      ('super', '_maintain_default_data', 'aleksis.apps.csv_import.default_templates', 'update_or_create_default_templates')
-               varnames   ('self', 'update_or_create_default_templates')
+               names      ('super', 'ready', 'aleksis.apps.csv_import.default_templates', 'update_or_create_default_templates', 'ProgrammingError', 'OperationalError', 'ImproperlyConfigured')
+               varnames   ('self', 'update_or_create_default_templates', 'e')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/apps.py'
-               name       '_maintain_default_data'
-               firstlineno 21
-               lnotab 0x040140030c04
-         names      ('__name__', '__module__', '__qualname__', 'name', 'dist_name', 'verbose_name', 'urls', 'licence', 'copyright_info', '_maintain_default_data', '__classcell__')
+               name       'ready'
+               firstlineno 24
+               lnotab 0x0401400302010c041a012c0214fe
+         names      ('__name__', '__module__', '__qualname__', 'name', 'dist_name', 'verbose_name', 'urls', 'licence', 'copyright_info', 'ready', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/apps.py'
          name       'CSVImportConfig'
-         firstlineno 4
+         firstlineno 7
          lnotab 0x0c0104010401040304ff040304020c010c010a010a010afb0408
       'CSVImportConfig'
       None
-   names      ('aleksis.core.util.apps', 'AppConfig', 'CSVImportConfig')
+   names      ('django.core.exceptions', 'ImproperlyConfigured', 'django.db', 'OperationalError', 'ProgrammingError', 'aleksis.core.util.apps', 'AppConfig', 'CSVImportConfig')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/apps.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c03
+   lnotab 0x00ff02010c0110020c03
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/field_types.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/field_types.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
-files sz: 15681
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
+files sz: 15561
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a036d
@@ -735,47 +735,47 @@
               1912 CALL                     3
    
    475        1922 PRECALL                  0
               1926 CALL                     0
    
    476        1936 STORE_NAME              70 (FileFieldType)
    
-   498        1938 LOAD_NAME               37 (field_type_registry)
+   493        1938 LOAD_NAME               37 (field_type_registry)
               1940 LOAD_ATTR               38 (register)
    
-   499        1950 PUSH_NULL
+   494        1950 PUSH_NULL
               1952 LOAD_BUILD_CLASS
-              1954 LOAD_CONST              81 (<code object AvatarFieldType, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py", line 498>)
+              1954 LOAD_CONST              81 (<code object AvatarFieldType, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py", line 493>)
               1956 MAKE_FUNCTION            0
               1958 LOAD_CONST              82 ('AvatarFieldType')
               1960 LOAD_NAME               70 (FileFieldType)
               1962 PRECALL                  3
               1966 CALL                     3
    
-   498        1976 PRECALL                  0
+   493        1976 PRECALL                  0
               1980 CALL                     0
    
-   499        1990 STORE_NAME              71 (AvatarFieldType)
+   494        1990 STORE_NAME              71 (AvatarFieldType)
    
-   504        1992 LOAD_NAME               37 (field_type_registry)
+   499        1992 LOAD_NAME               37 (field_type_registry)
               1994 LOAD_ATTR               38 (register)
    
-   505        2004 PUSH_NULL
+   500        2004 PUSH_NULL
               2006 LOAD_BUILD_CLASS
-              2008 LOAD_CONST              83 (<code object PhotoFieldType, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py", line 504>)
+              2008 LOAD_CONST              83 (<code object PhotoFieldType, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py", line 499>)
               2010 MAKE_FUNCTION            0
               2012 LOAD_CONST              84 ('PhotoFieldType')
               2014 LOAD_NAME               70 (FileFieldType)
               2016 PRECALL                  3
               2020 CALL                     3
    
-   504        2030 PRECALL                  0
+   499        2030 PRECALL                  0
               2034 CALL                     0
    
-   505        2044 STORE_NAME              72 (PhotoFieldType)
+   500        2044 STORE_NAME              72 (PhotoFieldType)
               2046 LOAD_CONST               1 (None)
               2048 RETURN_VALUE
    consts
       0
       None
       ('Any', 'Callable', 'Optional', 'Sequence', 'Tuple', 'Type', 'Union')
       ('uuid4',)
@@ -4338,127 +4338,115 @@
             'value'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 9
                flags     : 3
                code
-                  0x97007c00a0000000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007d037403000000000000000000007c017c03a6
-                  020000ab0200000000000000007d047c0272af7404000000000000000000
-                  006a030000000000000000a0040000000000000000000000000000000000
-                  0000007c02a6010000ab0100000000000000007d057c006a050000000000
-                  0000007404000000000000000000006a030000000000000000a006000000
-                  00000000000000000000000000000000007c006a0500000000000000007c
-                  056602a6010000ab0100000000000000006b02000000007312740f000000
-                  0000000000000064017c029b009d02a6010000ab01000000000000000082
-                  017c04a00800000000000000000000000000000000000000007404000000
-                  000000000000006a030000000000000000a0090000000000000000000000
-                  0000000000000000007c05a6010000ab0100000000000000007415000000
-                  000000000000007417000000000000000000007c056402a6020000ab0200
-                  00000000000000a6010000ab010000000000000000a6020000ab02000000
-                  000000000001006e147c04a00c0000000000000000000000000000000000
-                  000000a6000000ab00000000000000000001007c01a00800000000000000
-                  00000000000000000000000000a6000000ab000000000000000000010064
-                  005300
+                  0x97007400000000000000000000006a010000000000000000a002000000
+                  00000000000000000000000000000000007c02a6010000ab010000000000
+                  0000007d037c006a0300000000000000007400000000000000000000006a
+                  010000000000000000a00400000000000000000000000000000000000000
+                  007c006a0300000000000000007c036602a6010000ab0100000000000000
+                  006b02000000007312740b0000000000000000000064017c029b009d02a6
+                  010000ab01000000000000000082017c00a0060000000000000000000000
+                  000000000000000000a6000000ab0000000000000000007d04740f000000
+                  000000000000007c017c04a6020000ab0200000000000000007d057c05a0
+                  080000000000000000000000000000000000000000740000000000000000
+                  0000006a010000000000000000a009000000000000000000000000000000
+                  00000000007c03a6010000ab010000000000000000741500000000000000
+                  0000007417000000000000000000007c036402a6020000ab020000000000
+                  000000a6010000ab010000000000000000a6020000ab0200000000000000
+                  0001007c01a0080000000000000000000000000000000000000000a60000
+                  00ab000000000000000000010064005300
                479           0 RESUME                   0
                
-               481           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (get_db_field)
-                            26 PRECALL                  0
-                            30 CALL                     0
-                            40 STORE_FAST               3 (field_name)
-               
-               482          42 LOAD_GLOBAL              3 (NULL + getattr)
-                            54 LOAD_FAST                1 (instance)
-                            56 LOAD_FAST                3 (field_name)
-                            58 PRECALL                  2
-                            62 CALL                     2
-                            72 STORE_FAST               4 (file_field)
-               
-               484          74 LOAD_FAST                2 (value)
-                            76 POP_JUMP_FORWARD_IF_FALSE   175 (to 428)
-               
-               486          78 LOAD_GLOBAL              4 (os)
-                            90 LOAD_ATTR                3 (path)
-                           100 LOAD_METHOD              4 (realpath)
-                           122 LOAD_FAST                2 (value)
-                           124 PRECALL                  1
-                           128 CALL                     1
-                           138 STORE_FAST               5 (abs_path)
-               
-               487         140 LOAD_FAST                0 (self)
-                           142 LOAD_ATTR                5 (base_path)
-                           152 LOAD_GLOBAL              4 (os)
-                           164 LOAD_ATTR                3 (path)
-                           174 LOAD_METHOD              6 (commonpath)
-                           196 LOAD_FAST                0 (self)
-                           198 LOAD_ATTR                5 (base_path)
-                           208 LOAD_FAST                5 (abs_path)
-                           210 BUILD_TUPLE              2
-                           212 PRECALL                  1
-                           216 CALL                     1
-                           226 COMPARE_OP               2 (==)
-                           232 POP_JUMP_FORWARD_IF_TRUE    18 (to 270)
-               
-               488         234 LOAD_GLOBAL             15 (NULL + ValueError)
-                           246 LOAD_CONST               1 ('Disallowed path traversal importing file from ')
-                           248 LOAD_FAST                2 (value)
-                           250 FORMAT_VALUE             0
-                           252 BUILD_STRING             2
-                           254 PRECALL                  1
-                           258 CALL                     1
-                           268 RAISE_VARARGS            1
-               
-               490     >>  270 LOAD_FAST                4 (file_field)
-                           272 LOAD_METHOD              8 (save)
-                           294 LOAD_GLOBAL              4 (os)
-                           306 LOAD_ATTR                3 (path)
-                           316 LOAD_METHOD              9 (basename)
-                           338 LOAD_FAST                5 (abs_path)
-                           340 PRECALL                  1
-                           344 CALL                     1
-                           354 LOAD_GLOBAL             21 (NULL + File)
-                           366 LOAD_GLOBAL             23 (NULL + open)
-                           378 LOAD_FAST                5 (abs_path)
-                           380 LOAD_CONST               2 ('rb')
-                           382 PRECALL                  2
-                           386 CALL                     2
-                           396 PRECALL                  1
-                           400 CALL                     1
-                           410 PRECALL                  2
-                           414 CALL                     2
-                           424 POP_TOP
-                           426 JUMP_FORWARD            20 (to 468)
-               
-               493     >>  428 LOAD_FAST                4 (file_field)
-                           430 LOAD_METHOD             12 (delete)
-                           452 PRECALL                  0
-                           456 CALL                     0
-                           466 POP_TOP
-               
-               495     >>  468 LOAD_FAST                1 (instance)
-                           470 LOAD_METHOD              8 (save)
-                           492 PRECALL                  0
-                           496 CALL                     0
-                           506 POP_TOP
-                           508 LOAD_CONST               0 (None)
-                           510 RETURN_VALUE
+               481           2 LOAD_GLOBAL              0 (os)
+                            14 LOAD_ATTR                1 (path)
+                            24 LOAD_METHOD              2 (realpath)
+                            46 LOAD_FAST                2 (value)
+                            48 PRECALL                  1
+                            52 CALL                     1
+                            62 STORE_FAST               3 (abs_path)
+               
+               482          64 LOAD_FAST                0 (self)
+                            66 LOAD_ATTR                3 (base_path)
+                            76 LOAD_GLOBAL              0 (os)
+                            88 LOAD_ATTR                1 (path)
+                            98 LOAD_METHOD              4 (commonpath)
+                           120 LOAD_FAST                0 (self)
+                           122 LOAD_ATTR                3 (base_path)
+                           132 LOAD_FAST                3 (abs_path)
+                           134 BUILD_TUPLE              2
+                           136 PRECALL                  1
+                           140 CALL                     1
+                           150 COMPARE_OP               2 (==)
+                           156 POP_JUMP_FORWARD_IF_TRUE    18 (to 194)
+               
+               483         158 LOAD_GLOBAL             11 (NULL + ValueError)
+                           170 LOAD_CONST               1 ('Disallowed path traversal importing file from ')
+                           172 LOAD_FAST                2 (value)
+                           174 FORMAT_VALUE             0
+                           176 BUILD_STRING             2
+                           178 PRECALL                  1
+                           182 CALL                     1
+                           192 RAISE_VARARGS            1
+               
+               486     >>  194 LOAD_FAST                0 (self)
+                           196 LOAD_METHOD              6 (get_db_field)
+                           218 PRECALL                  0
+                           222 CALL                     0
+                           232 STORE_FAST               4 (field_name)
+               
+               487         234 LOAD_GLOBAL             15 (NULL + getattr)
+                           246 LOAD_FAST                1 (instance)
+                           248 LOAD_FAST                4 (field_name)
+                           250 PRECALL                  2
+                           254 CALL                     2
+                           264 STORE_FAST               5 (file_field)
+               
+               488         266 LOAD_FAST                5 (file_field)
+                           268 LOAD_METHOD              8 (save)
+                           290 LOAD_GLOBAL              0 (os)
+                           302 LOAD_ATTR                1 (path)
+                           312 LOAD_METHOD              9 (basename)
+                           334 LOAD_FAST                3 (abs_path)
+                           336 PRECALL                  1
+                           340 CALL                     1
+                           350 LOAD_GLOBAL             21 (NULL + File)
+                           362 LOAD_GLOBAL             23 (NULL + open)
+                           374 LOAD_FAST                3 (abs_path)
+                           376 LOAD_CONST               2 ('rb')
+                           378 PRECALL                  2
+                           382 CALL                     2
+                           392 PRECALL                  1
+                           396 CALL                     1
+                           406 PRECALL                  2
+                           410 CALL                     2
+                           420 POP_TOP
+               
+               490         422 LOAD_FAST                1 (instance)
+                           424 LOAD_METHOD              8 (save)
+                           446 PRECALL                  0
+                           450 CALL                     0
+                           460 POP_TOP
+                           462 LOAD_CONST               0 (None)
+                           464 RETURN_VALUE
                consts
                   None
                   'Disallowed path traversal importing file from '
                   'rb'
-               names      ('get_db_field', 'getattr', 'os', 'path', 'realpath', 'base_path', 'commonpath', 'ValueError', 'save', 'basename', 'File', 'open', 'delete')
-               varnames   ('self', 'instance', 'value', 'field_name', 'file_field', 'abs_path')
+               names      ('os', 'path', 'realpath', 'base_path', 'commonpath', 'ValueError', 'get_db_field', 'getattr', 'save', 'basename', 'File', 'open')
+               varnames   ('self', 'instance', 'value', 'abs_path', 'field_name', 'file_field')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py'
                name       'process'
                firstlineno 479
-               lnotab 0x02022801200204023e015e0124029e032802
+               lnotab 0x02023e015e012403280120019c02
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Model', 'str', 'process')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py'
          name       'FileFieldType'
@@ -4467,70 +4455,70 @@
       'FileFieldType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364015a0464025300
-         498           0 RESUME                   0
+         493           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AvatarFieldType')
                        8 STORE_NAME               2 (__qualname__)
          
-         500          10 LOAD_CONST               1 ('avatar')
+         495          10 LOAD_CONST               1 ('avatar')
                       12 STORE_NAME               3 (name)
          
-         501          14 LOAD_CONST               1 ('avatar')
+         496          14 LOAD_CONST               1 ('avatar')
                       16 STORE_NAME               4 (db_field)
                       18 LOAD_CONST               2 (None)
                       20 RETURN_VALUE
          consts
             'AvatarFieldType'
             'avatar'
             None
          names      ('__name__', '__module__', '__qualname__', 'name', 'db_field')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py'
          name       'AvatarFieldType'
-         firstlineno 498
+         firstlineno 493
          lnotab 0x0a020401
       'AvatarFieldType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364015a0464025300
-         504           0 RESUME                   0
+         499           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PhotoFieldType')
                        8 STORE_NAME               2 (__qualname__)
          
-         506          10 LOAD_CONST               1 ('photo')
+         501          10 LOAD_CONST               1 ('photo')
                       12 STORE_NAME               3 (name)
          
-         507          14 LOAD_CONST               1 ('photo')
+         502          14 LOAD_CONST               1 ('photo')
                       16 STORE_NAME               4 (db_field)
                       18 LOAD_CONST               2 (None)
                       20 RETURN_VALUE
          consts
             'PhotoFieldType'
             'photo'
             None
          names      ('__name__', '__module__', '__qualname__', 'name', 'db_field')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py'
          name       'PhotoFieldType'
-         firstlineno 504
+         firstlineno 499
          lnotab 0x0a020401
       'PhotoFieldType'
    names      ('os', 're', 'typing', 'Any', 'Callable', 'Optional', 'Sequence', 'Tuple', 'Type', 'Union', 'uuid', 'uuid4', 'django.apps', 'apps', 'django.core.files', 'File', 'django.db.models', 'Model', 'django.utils.translation', 'gettext', '_', 'aleksis.apps.csv_import.util.class_range_helpers', 'get_classes_per_grade', 'get_classes_per_short_name', 'parse_class_range', 'aleksis.apps.csv_import.util.converters', 'converter_registry', 'aleksis.apps.csv_import.util.import_helpers', 'with_prefix', 'aleksis.core.models', 'Group', 'Person', 'SchoolTerm', 'aleksis.core.util.core_helpers', 'get_site_preferences', 'FieldType', 'FieldTypeRegistry', 'field_type_registry', 'register', 'MatchFieldType', 'DirectMappingFieldType', 'ProcessFieldType', 'RegExFieldType', 'UniqueReferenceFieldType', 'NameFieldType', 'FirstNameFieldType', 'LastNameFieldType', 'AdditionalNameFieldType', 'ShortNameFieldType', 'EmailFieldType', 'DateOfBirthFieldType', 'SexFieldType', 'StreetFieldType', 'HouseNumberFieldType', 'StreetAndHouseNumberFieldType', 'PostalCodeFieldType', 'PlaceFieldType', 'PhoneNumberFieldType', 'MobileNumberFieldType', 'IgnoreFieldType', 'DepartmentsFieldType', 'GroupSubjectByShortNameFieldType', 'ClassRangeFieldType', 'PrimaryGroupByShortNameFieldType', 'PrimaryGroupOwnerByShortNameFieldType', 'GroupOwnerByShortNameFieldType', 'GroupMembershipByShortNameFieldType', 'ParentGroupByShortNameFieldType', 'MemberOfByNameFieldType', 'ChildByUniqueReference', 'FileFieldType', 'AvatarFieldType', 'PhotoFieldType')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/field_types.py'
@@ -4542,8 +4530,8 @@
       ff0e0102070c011aff0e0102070c011aff0e0102060c011aff0e0102060c
       011aff0e0102060c011aff0e0102080c011aff0e0102130c011aff0e0102
       070c011aff0e0102070c011aff0e0102060c011aff0e0102060c011aff0e
       0102060c011aff0e0102060c011aff0e0102060c011aff0e0102070c011a
       ff0e0102070c011aff0e0102050c011aff0e0102290c011aff0e01020d0c
       011aff0e0102140c011aff0e01020d0c011aff0e01020a0c011aff0e0102
       0f0c011aff0e01020c0c011aff0e01020c0c011aff0e01020a0c011aff0e
-      0102090c011aff0e0102160c011aff0e0102050c011aff0e01
+      0102090c011aff0e0102110c011aff0e0102050c011aff0e01
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/model_extensions.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/model_extensions.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 274
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/models.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/models.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
-files sz: 7679
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
+files sz: 7521
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
@@ -121,17 +121,17 @@
                188 MAKE_FUNCTION            0
                190 LOAD_CONST              16 ('ImportTemplateField')
                192 LOAD_NAME               20 (ExtensibleModel)
                194 PRECALL                  3
                198 CALL                     3
                208 STORE_NAME              29 (ImportTemplateField)
    
-   207         210 PUSH_NULL
+   204         210 PUSH_NULL
                212 LOAD_BUILD_CLASS
-               214 LOAD_CONST              17 (<code object ImportJob, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 207>)
+               214 LOAD_CONST              17 (<code object ImportJob, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 204>)
                216 MAKE_FUNCTION            0
                218 LOAD_CONST              18 ('ImportJob')
                220 LOAD_NAME               20 (ExtensibleModel)
                222 PRECALL                  3
                226 CALL                     3
                236 STORE_NAME              30 (ImportJob)
                238 LOAD_CONST               1 (None)
@@ -173,21 +173,21 @@
             056410020065096411a6010000ab010000000000000000ac12a6030000ab
             0300000000000000005a11020065036a060000000000000000651265036a
             13000000000000000064086408020065096413a6010000ab010000000000
             000000020065096414a6010000ab010000000000000000ac15a6060000ab
             0600000000000000005a14020065036a060000000000000000651565036a
             13000000000000000064086408020065096416a6010000ab010000000000
             000000020065096417a6010000ab010000000000000000ac15a6060000ab
-            0600000000000000005a1602004700641884006419a6020000ab02000000
-            00000000005a17641a84005a1888006601641b84085a19651a641c8400a6
-            000000ab0000000000000000005a1b651a641d8400a6000000ab00000000
-            00000000005a1c651d641e651e641f651f6420651f642165206422652165
-            2265236524651f65256602190000000000000000006526651f6604190000
-            0000000000000019000000000000000000660a64238404a6000000ab0000
-            000000000000005a27651d642664246526660264258405a6000000ab0000
+            0600000000000000005a16651764188400a6000000ab0000000000000000
+            005a18651764198400a6000000ab0000000000000000005a198800660164
+            1a84085a1a651b641b651c641c651d641d651d641e651e641f651f652065
+            216522651d65236602190000000000000000006524651d66041900000000
+            000000000019000000000000000000660a64208404a6000000ab00000000
+            00000000005a25651b642664216524660264228405a6000000ab00000000
+            00000000005a26642384005a2702004700642484006425a6020000ab0200
             000000000000005a28880078015a295300
                        0 MAKE_CELL                0 (__class__)
          
           17           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ImportTemplate')
@@ -386,109 +386,109 @@
                      612 CALL                     1
          
           55         622 KW_NAMES                21
                      624 PRECALL                  6
                      628 CALL                     6
                      638 STORE_NAME              22 (group_type)
          
-          66         640 PUSH_NULL
-                     642 LOAD_BUILD_CLASS
-                     644 LOAD_CONST              24 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 66>)
-                     646 MAKE_FUNCTION            0
-                     648 LOAD_CONST              25 ('Meta')
-                     650 PRECALL                  2
-                     654 CALL                     2
-                     664 STORE_NAME              23 (Meta)
+          66         640 LOAD_NAME               23 (property)
          
-          76         666 LOAD_CONST              26 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 76>)
-                     668 MAKE_FUNCTION            0
-                     670 STORE_NAME              24 (__str__)
+          67         642 LOAD_CONST              24 (<code object parsed_separator, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 66>)
+                     644 MAKE_FUNCTION            0
          
-          79         672 LOAD_CLOSURE             0 (__class__)
-                     674 BUILD_TUPLE              1
-                     676 LOAD_CONST              27 (<code object save, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 79>)
-                     678 MAKE_FUNCTION            8 (closure)
-                     680 STORE_NAME              25 (save)
+          66         646 PRECALL                  0
+                     650 CALL                     0
          
-          86         682 LOAD_NAME               26 (property)
+          67         660 STORE_NAME              24 (parsed_separator)
          
-          87         684 LOAD_CONST              28 (<code object parsed_separator, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 86>)
-                     686 MAKE_FUNCTION            0
+          70         662 LOAD_NAME               23 (property)
          
-          86         688 PRECALL                  0
-                     692 CALL                     0
+          71         664 LOAD_CONST              25 (<code object parsed_quotechar, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 70>)
+                     666 MAKE_FUNCTION            0
          
-          87         702 STORE_NAME              27 (parsed_separator)
+          70         668 PRECALL                  0
+                     672 CALL                     0
          
-          90         704 LOAD_NAME               26 (property)
+          71         682 STORE_NAME              25 (parsed_quotechar)
          
-          91         706 LOAD_CONST              29 (<code object parsed_quotechar, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 90>)
-                     708 MAKE_FUNCTION            0
+          74         684 LOAD_CLOSURE             0 (__class__)
+                     686 BUILD_TUPLE              1
+                     688 LOAD_CONST              26 (<code object save, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 74>)
+                     690 MAKE_FUNCTION            8 (closure)
+                     692 STORE_NAME              26 (save)
          
-          90         710 PRECALL                  0
-                     714 CALL                     0
+          81         694 LOAD_NAME               27 (classmethod)
          
-          91         724 STORE_NAME              28 (parsed_quotechar)
+          82         696 LOAD_CONST              27 ('model')
          
-          94         726 LOAD_NAME               29 (classmethod)
+          84         698 LOAD_NAME               28 (Model)
          
-          95         728 LOAD_CONST              30 ('model')
+          82         700 LOAD_CONST              28 ('name')
          
-          97         730 LOAD_NAME               30 (Model)
+          85         702 LOAD_NAME               29 (str)
          
-          95         732 LOAD_CONST              31 ('name')
+          82         704 LOAD_CONST              29 ('verbose_name')
          
-          98         734 LOAD_NAME               31 (str)
+          86         706 LOAD_NAME               29 (str)
          
-          95         736 LOAD_CONST              32 ('verbose_name')
+          82         708 LOAD_CONST              30 ('extra_args')
          
-          99         738 LOAD_NAME               31 (str)
+          87         710 LOAD_NAME               30 (dict)
          
-          95         740 LOAD_CONST              33 ('extra_args')
+          82         712 LOAD_CONST              31 ('fields')
          
-         100         742 LOAD_NAME               32 (dict)
+          88         714 LOAD_NAME               31 (Sequence)
+                     716 LOAD_NAME               32 (Tuple)
+                     718 LOAD_NAME               33 (FieldType)
+                     720 LOAD_NAME               34 (Dict)
+                     722 LOAD_NAME               29 (str)
+                     724 LOAD_NAME               35 (Any)
+                     726 BUILD_TUPLE              2
+                     728 BINARY_SUBSCR
+                     738 LOAD_NAME               36 (bool)
+                     740 LOAD_NAME               29 (str)
+                     742 BUILD_TUPLE              4
+                     744 BINARY_SUBSCR
+                     754 BINARY_SUBSCR
          
-          95         744 LOAD_CONST              34 ('fields')
+          82         764 BUILD_TUPLE             10
+                     766 LOAD_CONST              32 (<code object update_or_create, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 81>)
+                     768 MAKE_FUNCTION            4 (annotations)
          
-         101         746 LOAD_NAME               33 (Sequence)
-                     748 LOAD_NAME               34 (Tuple)
-                     750 LOAD_NAME               35 (FieldType)
-                     752 LOAD_NAME               36 (Dict)
-                     754 LOAD_NAME               31 (str)
-                     756 LOAD_NAME               37 (Any)
-                     758 BUILD_TUPLE              2
-                     760 BINARY_SUBSCR
-                     770 LOAD_NAME               38 (bool)
-                     772 LOAD_NAME               31 (str)
-                     774 BUILD_TUPLE              4
-                     776 BINARY_SUBSCR
-                     786 BINARY_SUBSCR
+          81         770 PRECALL                  0
+                     774 CALL                     0
          
-          95         796 BUILD_TUPLE             10
-                     798 LOAD_CONST              35 (<code object update_or_create, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 94>)
-                     800 MAKE_FUNCTION            4 (annotations)
+          82         784 STORE_NAME              37 (update_or_create)
          
-          94         802 PRECALL                  0
-                     806 CALL                     0
+         115         786 LOAD_NAME               27 (classmethod)
          
-          95         816 STORE_NAME              39 (update_or_create)
+         116         788 LOAD_CONST              38 ((False,))
+                     790 LOAD_CONST              33 ('from_default')
+                     792 LOAD_NAME               36 (bool)
+                     794 BUILD_TUPLE              2
+                     796 LOAD_CONST              34 (<code object update_or_create_templates, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 115>)
+                     798 MAKE_FUNCTION            5 (defaults, annotations)
          
-         128         818 LOAD_NAME               29 (classmethod)
+         115         800 PRECALL                  0
+                     804 CALL                     0
          
-         129         820 LOAD_CONST              38 ((False,))
-                     822 LOAD_CONST              36 ('from_default')
-                     824 LOAD_NAME               38 (bool)
-                     826 BUILD_TUPLE              2
-                     828 LOAD_CONST              37 (<code object update_or_create_templates, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 128>)
-                     830 MAKE_FUNCTION            5 (defaults, annotations)
+         116         814 STORE_NAME              38 (update_or_create_templates)
          
-         128         832 PRECALL                  0
-                     836 CALL                     0
+         149         816 LOAD_CONST              35 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 149>)
+                     818 MAKE_FUNCTION            0
+                     820 STORE_NAME              39 (__str__)
          
-         129         846 STORE_NAME              40 (update_or_create_templates)
+         152         822 PUSH_NULL
+                     824 LOAD_BUILD_CLASS
+                     826 LOAD_CONST              36 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 152>)
+                     828 MAKE_FUNCTION            0
+                     830 LOAD_CONST              37 ('Meta')
+                     832 PRECALL                  2
+                     836 CALL                     2
+                     846 STORE_NAME              40 (Meta)
                      848 LOAD_CLOSURE             0 (__class__)
                      850 COPY                     1
                      852 STORE_NAME              41 (__classcell__)
                      854 RETURN_VALUE
          consts
             'ImportTemplate'
             False
@@ -511,178 +511,27 @@
             ('max_length', 'default', 'verbose_name')
             'Base group'
             'If imported objects are persons, they all will be members of this group after import.'
             ('on_delete', 'blank', 'null', 'verbose_name', 'help_text')
             'Group type'
             'If imported objects are groups, they all will get this group type after import.'
             code
-               argcount  : 0
-               nlocals   : 0
-               stacksize : 4
-               flags     : 0
-               code
-                  0x970065005a0164005a02640167015a03020065046402a6010000ab0100
-                  000000000000005a05020065046403a6010000ab0100000000000000005a
-                  06020065076a08000000000000000064046405ac06a6020000ab02000000
-                  000000000067015a0964075300
-                66           0 RESUME                   0
-                             2 LOAD_NAME                0 (__name__)
-                             4 STORE_NAME               1 (__module__)
-                             6 LOAD_CONST               0 ('ImportTemplate.Meta')
-                             8 STORE_NAME               2 (__qualname__)
-               
-                67          10 LOAD_CONST               1 ('name')
-                            12 BUILD_LIST               1
-                            14 STORE_NAME               3 (ordering)
-               
-                68          16 PUSH_NULL
-                            18 LOAD_NAME                4 (_)
-                            20 LOAD_CONST               2 ('Import template')
-                            22 PRECALL                  1
-                            26 CALL                     1
-                            36 STORE_NAME               5 (verbose_name)
-               
-                69          38 PUSH_NULL
-                            40 LOAD_NAME                4 (_)
-                            42 LOAD_CONST               3 ('Import templates')
-                            44 PRECALL                  1
-                            48 CALL                     1
-                            58 STORE_NAME               6 (verbose_name_plural)
-               
-                71          60 PUSH_NULL
-                            62 LOAD_NAME                7 (models)
-                            64 LOAD_ATTR                8 (UniqueConstraint)
-               
-                72          74 LOAD_CONST               4 (('site_id', 'name'))
-                            76 LOAD_CONST               5 ('unique_template_name_per_site')
-               
-                71          78 KW_NAMES                 6
-                            80 PRECALL                  2
-                            84 CALL                     2
-               
-                70          94 BUILD_LIST               1
-                            96 STORE_NAME               9 (constraints)
-                            98 LOAD_CONST               7 (None)
-                           100 RETURN_VALUE
-               consts
-                  'ImportTemplate.Meta'
-                  'name'
-                  'Import template'
-                  'Import templates'
-                  ('site_id', 'name')
-                  'unique_template_name_per_site'
-                  ('fields', 'name')
-                  None
-               names      ('__name__', '__module__', '__qualname__', 'ordering', '_', 'verbose_name', 'verbose_name_plural', 'models', 'UniqueConstraint', 'constraints')
-               varnames   ()
-               freevars   ()
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
-               name       'Meta'
-               firstlineno 66
-               lnotab 0x0a010601160116020e0104ff10ff
-            'Meta'
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 1
-               flags     : 3
-               code 0x97007c006a0000000000000000005300
-                76           0 RESUME                   0
-               
-                77           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (verbose_name)
-                            14 RETURN_VALUE
-               consts
-                  None
-               names      ('verbose_name',)
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
-               name       '__str__'
-               firstlineno 76
-               lnotab 0x0201
-            code
-               argcount  : 1
-               nlocals   : 3
-               stacksize : 5
-               flags     : 15
-               code
-                  0x950197007c006a0000000000000000006a01000000000000000064016b
-                  0200000000730764007c005f0200000000000000007c006a000000000000
-                  0000006a01000000000000000064026b0200000000730764007c005f0300
-                  000000000000000200740900000000000000000000a6000000ab00000000
-                  00000000006a0500000000000000007c0169007c02a4018e010100640053
-                  00
-                             0 COPY_FREE_VARS           1
-               
-                79           2 RESUME                   0
-               
-                80           4 LOAD_FAST                0 (self)
-                             6 LOAD_ATTR                0 (content_type)
-                            16 LOAD_ATTR                1 (model)
-                            26 LOAD_CONST               1 ('person')
-                            28 COMPARE_OP               2 (==)
-                            34 POP_JUMP_FORWARD_IF_TRUE     7 (to 50)
-               
-                81          36 LOAD_CONST               0 (None)
-                            38 LOAD_FAST                0 (self)
-                            40 STORE_ATTR               2 (group)
-               
-                82     >>   50 LOAD_FAST                0 (self)
-                            52 LOAD_ATTR                0 (content_type)
-                            62 LOAD_ATTR                1 (model)
-                            72 LOAD_CONST               2 ('group')
-                            74 COMPARE_OP               2 (==)
-                            80 POP_JUMP_FORWARD_IF_TRUE     7 (to 96)
-               
-                83          82 LOAD_CONST               0 (None)
-                            84 LOAD_FAST                0 (self)
-                            86 STORE_ATTR               3 (group_type)
-               
-                84     >>   96 PUSH_NULL
-                            98 LOAD_GLOBAL              9 (NULL + super)
-                           110 PRECALL                  0
-                           114 CALL                     0
-                           124 LOAD_ATTR                5 (save)
-                           134 LOAD_FAST                1 (args)
-                           136 BUILD_MAP                0
-                           138 LOAD_FAST                2 (kwargs)
-                           140 DICT_MERGE               1
-                           142 CALL_FUNCTION_EX         1
-                           144 POP_TOP
-                           146 LOAD_CONST               0 (None)
-                           148 RETURN_VALUE
-               consts
-                  None
-                  'person'
-                  'group'
-               names      ('content_type', 'model', 'group', 'group_type', 'super', 'save')
-               varnames   ('self', 'args', 'kwargs')
-               freevars   ('__class__',)
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
-               name       'save'
-               firstlineno 79
-               lnotab 0x040120010e0120010e01
-            code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000007c006a0300000000000000006401a6020000ab02000000
                   0000000000a6010000ab0100000000000000006402190000000000000000
                   00a00400000000000000000000000000000000000000006401a6010000ab
                   0100000000000000005300
-                86           0 RESUME                   0
+                66           0 RESUME                   0
                
-                88           2 LOAD_GLOBAL              1 (NULL + codecs)
+                68           2 LOAD_GLOBAL              1 (NULL + codecs)
                             14 LOAD_ATTR                1 (escape_decode)
                             24 LOAD_GLOBAL              5 (NULL + bytes)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                3 (separator)
                             48 LOAD_CONST               1 ('utf-8')
                             50 PRECALL                  2
                             54 CALL                     2
@@ -701,30 +550,30 @@
                   0
                names      ('codecs', 'escape_decode', 'bytes', 'separator', 'decode')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
                name       'parsed_separator'
-               firstlineno 86
+               firstlineno 66
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000007c006a0300000000000000006401a6020000ab02000000
                   0000000000a6010000ab0100000000000000006402190000000000000000
                   00a00400000000000000000000000000000000000000006401a6010000ab
                   0100000000000000005300
-                90           0 RESUME                   0
+                70           0 RESUME                   0
                
-                92           2 LOAD_GLOBAL              1 (NULL + codecs)
+                72           2 LOAD_GLOBAL              1 (NULL + codecs)
                             14 LOAD_ATTR                1 (escape_decode)
                             24 LOAD_GLOBAL              5 (NULL + bytes)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                3 (quotechar)
                             48 LOAD_CONST               1 ('utf-8')
                             50 PRECALL                  2
                             54 CALL                     2
@@ -743,16 +592,79 @@
                   0
                names      ('codecs', 'escape_decode', 'bytes', 'quotechar', 'decode')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
                name       'parsed_quotechar'
-               firstlineno 90
+               firstlineno 70
                lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x950197007c006a0000000000000000006a01000000000000000064016b
+                  0200000000730764007c005f0200000000000000007c006a000000000000
+                  0000006a01000000000000000064026b0200000000730764007c005f0300
+                  000000000000000200740900000000000000000000a6000000ab00000000
+                  00000000006a0500000000000000007c0169007c02a4018e010100640053
+                  00
+                             0 COPY_FREE_VARS           1
+               
+                74           2 RESUME                   0
+               
+                75           4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (content_type)
+                            16 LOAD_ATTR                1 (model)
+                            26 LOAD_CONST               1 ('person')
+                            28 COMPARE_OP               2 (==)
+                            34 POP_JUMP_FORWARD_IF_TRUE     7 (to 50)
+               
+                76          36 LOAD_CONST               0 (None)
+                            38 LOAD_FAST                0 (self)
+                            40 STORE_ATTR               2 (group)
+               
+                77     >>   50 LOAD_FAST                0 (self)
+                            52 LOAD_ATTR                0 (content_type)
+                            62 LOAD_ATTR                1 (model)
+                            72 LOAD_CONST               2 ('group')
+                            74 COMPARE_OP               2 (==)
+                            80 POP_JUMP_FORWARD_IF_TRUE     7 (to 96)
+               
+                78          82 LOAD_CONST               0 (None)
+                            84 LOAD_FAST                0 (self)
+                            86 STORE_ATTR               3 (group_type)
+               
+                79     >>   96 PUSH_NULL
+                            98 LOAD_GLOBAL              9 (NULL + super)
+                           110 PRECALL                  0
+                           114 CALL                     0
+                           124 LOAD_ATTR                5 (save)
+                           134 LOAD_FAST                1 (args)
+                           136 BUILD_MAP                0
+                           138 LOAD_FAST                2 (kwargs)
+                           140 DICT_MERGE               1
+                           142 CALL_FUNCTION_EX         1
+                           144 POP_TOP
+                           146 LOAD_CONST               0 (None)
+                           148 RETURN_VALUE
+               consts
+                  None
+                  'person'
+                  'group'
+               names      ('content_type', 'model', 'group', 'group_type', 'super', 'save')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ('__class__',)
+               cellvars   ()
+               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
+               name       'save'
+               firstlineno 74
+               lnotab 0x040120010e0120010e01
             'model'
             'name'
             'verbose_name'
             'extra_args'
             'fields'
             code
                argcount  : 6
@@ -770,104 +682,104 @@
                   00000000000000a00300000000000000000000000000000000000000007c
                   077c097c0b6a0600000000000000007c0c7c0d7c0e64049c04ac05a60300
                   00ab03000000000000000001008c39740a000000000000000000006a0100
                   00000000000000a00700000000000000000000000000000000000000007c
                   077c09ac06a6020000ab020000000000000000a008000000000000000000
                   0000000000000000000000a6000000ab00000000000000000001007c0753
                   00
-                94           0 RESUME                   0
+                81           0 RESUME                   0
                
-               104           2 LOAD_GLOBAL              0 (ContentType)
+                91           2 LOAD_GLOBAL              0 (ContentType)
                             14 LOAD_ATTR                1 (objects)
                             24 LOAD_METHOD              2 (get_for_model)
                             46 LOAD_FAST                1 (model)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               6 (ct)
                
-               105          64 LOAD_FAST                0 (cls)
+                92          64 LOAD_FAST                0 (cls)
                             66 LOAD_ATTR                1 (objects)
                             76 LOAD_METHOD              3 (update_or_create)
                
-               106          98 LOAD_FAST                2 (name)
+                93          98 LOAD_FAST                2 (name)
                
-               107         100 LOAD_FAST                3 (verbose_name)
+                94         100 LOAD_FAST                3 (verbose_name)
                            102 LOAD_FAST                6 (ct)
                            104 LOAD_CONST               1 (('verbose_name', 'content_type'))
                            106 BUILD_CONST_KEY_MAP      2
                            108 LOAD_FAST                4 (extra_args)
                            110 DICT_UPDATE              1
                
-               105         112 KW_NAMES                 2
+                92         112 KW_NAMES                 2
                            114 PRECALL                  2
                            118 CALL                     2
                            128 UNPACK_SEQUENCE          2
                            132 STORE_FAST               7 (template)
                            134 STORE_FAST               8 (updated)
                
-               110         136 LOAD_CONST               3 (0)
+                97         136 LOAD_CONST               3 (0)
                            138 STORE_FAST               9 (i)
                
-               111         140 LOAD_GLOBAL              9 (NULL + enumerate)
+                98         140 LOAD_GLOBAL              9 (NULL + enumerate)
                            152 LOAD_FAST                5 (fields)
                            154 PRECALL                  1
                            158 CALL                     1
                            168 GET_ITER
                        >>  170 FOR_ITER                56 (to 284)
                            172 UNPACK_SEQUENCE          2
                            176 STORE_FAST               9 (i)
                            178 STORE_FAST              10 (field)
                
-               112         180 LOAD_FAST               10 (field)
+                99         180 LOAD_FAST               10 (field)
                            182 UNPACK_SEQUENCE          4
                            186 STORE_FAST              11 (field_type)
                            188 STORE_FAST              12 (args)
                            190 STORE_FAST              13 (virtual)
                            192 STORE_FAST              14 (virtual_tmpl)
                
-               113         194 LOAD_GLOBAL             10 (ImportTemplateField)
+               100         194 LOAD_GLOBAL             10 (ImportTemplateField)
                            206 LOAD_ATTR                1 (objects)
                            216 LOAD_METHOD              3 (update_or_create)
                
-               114         238 LOAD_FAST                7 (template)
+               101         238 LOAD_FAST                7 (template)
                
-               115         240 LOAD_FAST                9 (i)
+               102         240 LOAD_FAST                9 (i)
                
-               117         242 LOAD_FAST               11 (field_type)
+               104         242 LOAD_FAST               11 (field_type)
                            244 LOAD_ATTR                6 (name)
                
-               118         254 LOAD_FAST               12 (args)
+               105         254 LOAD_FAST               12 (args)
                
-               119         256 LOAD_FAST               13 (virtual)
+               106         256 LOAD_FAST               13 (virtual)
                
-               120         258 LOAD_FAST               14 (virtual_tmpl)
+               107         258 LOAD_FAST               14 (virtual_tmpl)
                
-               116         260 LOAD_CONST               4 (('field_type', 'args', 'virtual', 'virtual_tmpl'))
+               103         260 LOAD_CONST               4 (('field_type', 'args', 'virtual', 'virtual_tmpl'))
                            262 BUILD_CONST_KEY_MAP      4
                
-               113         264 KW_NAMES                 5
+               100         264 KW_NAMES                 5
                            266 PRECALL                  3
                            270 CALL                     3
                            280 POP_TOP
                            282 JUMP_BACKWARD           57 (to 170)
                
-               124     >>  284 LOAD_GLOBAL             10 (ImportTemplateField)
+               111     >>  284 LOAD_GLOBAL             10 (ImportTemplateField)
                            296 LOAD_ATTR                1 (objects)
                            306 LOAD_METHOD              7 (filter)
                            328 LOAD_FAST                7 (template)
                            330 LOAD_FAST                9 (i)
                            332 KW_NAMES                 6
                            334 PRECALL                  2
                            338 CALL                     2
                            348 LOAD_METHOD              8 (delete)
                            370 PRECALL                  0
                            374 CALL                     0
                            384 POP_TOP
                
-               126         386 LOAD_FAST                7 (template)
+               113         386 LOAD_FAST                7 (template)
                            388 RETURN_VALUE
                consts
                   'Update or create an import template in database.'
                   ('verbose_name', 'content_type')
                   ('name', 'defaults')
                   0
                   ('field_type', 'args', 'virtual', 'virtual_tmpl')
@@ -875,15 +787,15 @@
                   ('template', 'index__gt')
                names      ('ContentType', 'objects', 'get_for_model', 'update_or_create', 'enumerate', 'ImportTemplateField', 'name', 'filter', 'delete')
                varnames   ('cls', 'model', 'name', 'verbose_name', 'extra_args', 'fields', 'ct', 'template', 'updated', 'i', 'field', 'field_type', 'args', 'virtual', 'virtual_tmpl')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
                name       'update_or_create'
-               firstlineno 94
+               firstlineno 81
                lnotab
                   0x020a3e01220102010cfe1805040128010e012c01020102020c01020102
                   0102fc04fd140b6602
             'from_default'
             code
                argcount  : 3
                nlocals   : 13
@@ -907,153 +819,153 @@
                   007c087c0b7c097c0a6604a6010000ab01000000000000000001008ca17c
                   04a009000000000000000000000000000000000000000064086900a60200
                   00ab0200000000000000007d0c7c027c0c64093c0000007c00a00a000000
                   00000000000000000000000000000000007c057c037c04a0090000000000
                   000000000000000000000000000000640a6404a6020000ab020000000000
                   0000007c0c7c06ac0ba6050000ab050000000000000000010090018c1664
                   0c5300
-               128           0 RESUME                   0
+               115           0 RESUME                   0
                
-               131           2 LOAD_FAST                1 (template_defs)
+               118           2 LOAD_FAST                1 (template_defs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 EXTENDED_ARG             1
                             44 FOR_ITER               276 (to 598)
                             46 UNPACK_SEQUENCE          2
                             50 STORE_FAST               3 (name)
                             52 STORE_FAST               4 (defs)
                
-               132          54 LOAD_GLOBAL              3 (NULL + apps)
+               119          54 LOAD_GLOBAL              3 (NULL + apps)
                             66 LOAD_ATTR                2 (get_model)
                             76 LOAD_FAST                4 (defs)
                             78 LOAD_CONST               1 ('model')
                             80 BINARY_SUBSCR
                             90 PRECALL                  1
                             94 CALL                     1
                            104 STORE_FAST               5 (model)
                
-               134         106 BUILD_LIST               0
+               121         106 BUILD_LIST               0
                            108 STORE_FAST               6 (fields)
                
-               135         110 LOAD_FAST                4 (defs)
+               122         110 LOAD_FAST                4 (defs)
                            112 LOAD_CONST               2 ('fields')
                            114 BINARY_SUBSCR
                            124 GET_ITER
                        >>  126 FOR_ITER               160 (to 448)
                            128 STORE_FAST               7 (field_definition)
                
-               136         130 LOAD_GLOBAL              7 (NULL + isinstance)
+               123         130 LOAD_GLOBAL              7 (NULL + isinstance)
                            142 LOAD_FAST                7 (field_definition)
                            144 LOAD_GLOBAL              8 (str)
                            156 PRECALL                  2
                            160 CALL                     2
                            170 POP_JUMP_FORWARD_IF_FALSE    27 (to 226)
                
-               137         172 LOAD_GLOBAL             11 (NULL + field_type_registry)
+               124         172 LOAD_GLOBAL             11 (NULL + field_type_registry)
                            184 LOAD_ATTR                6 (get_from_name)
                            194 LOAD_FAST                7 (field_definition)
                            196 PRECALL                  1
                            200 CALL                     1
                            210 STORE_FAST               8 (field_type)
                
-               138         212 LOAD_CONST               3 (False)
+               125         212 LOAD_CONST               3 (False)
                            214 STORE_FAST               9 (virtual)
                
-               139         216 LOAD_CONST               4 ('')
+               126         216 LOAD_CONST               4 ('')
                            218 STORE_FAST              10 (template)
                
-               140         220 BUILD_MAP                0
+               127         220 BUILD_MAP                0
                            222 STORE_FAST              11 (args)
                            224 JUMP_FORWARD            85 (to 396)
                
-               142     >>  226 LOAD_GLOBAL             11 (NULL + field_type_registry)
+               129     >>  226 LOAD_GLOBAL             11 (NULL + field_type_registry)
                            238 LOAD_ATTR                6 (get_from_name)
                
-               143         248 LOAD_FAST                7 (field_definition)
+               130         248 LOAD_FAST                7 (field_definition)
                            250 LOAD_METHOD              7 (pop)
                            272 LOAD_CONST               5 ('field_type')
                            274 PRECALL                  1
                            278 CALL                     1
                
-               142         288 PRECALL                  1
+               129         288 PRECALL                  1
                            292 CALL                     1
                            302 STORE_FAST               8 (field_type)
                
-               145         304 LOAD_FAST                7 (field_definition)
+               132         304 LOAD_FAST                7 (field_definition)
                            306 LOAD_METHOD              7 (pop)
                            328 LOAD_CONST               6 ('virtual')
                            330 LOAD_CONST               3 (False)
                            332 PRECALL                  2
                            336 CALL                     2
                            346 STORE_FAST               9 (virtual)
                
-               146         348 LOAD_FAST                7 (field_definition)
+               133         348 LOAD_FAST                7 (field_definition)
                            350 LOAD_METHOD              7 (pop)
                            372 LOAD_CONST               7 ('template')
                            374 LOAD_CONST               4 ('')
                            376 PRECALL                  2
                            380 CALL                     2
                            390 STORE_FAST              10 (template)
                
-               147         392 LOAD_FAST                7 (field_definition)
+               134         392 LOAD_FAST                7 (field_definition)
                            394 STORE_FAST              11 (args)
                
-               149     >>  396 LOAD_FAST                6 (fields)
+               136     >>  396 LOAD_FAST                6 (fields)
                            398 LOAD_METHOD              8 (append)
                            420 LOAD_FAST                8 (field_type)
                            422 LOAD_FAST               11 (args)
                            424 LOAD_FAST                9 (virtual)
                            426 LOAD_FAST               10 (template)
                            428 BUILD_TUPLE              4
                            430 PRECALL                  1
                            434 CALL                     1
                            444 POP_TOP
                            446 JUMP_BACKWARD          161 (to 126)
                
-               151     >>  448 LOAD_FAST                4 (defs)
+               138     >>  448 LOAD_FAST                4 (defs)
                            450 LOAD_METHOD              9 (get)
                            472 LOAD_CONST               8 ('extra_args')
                            474 BUILD_MAP                0
                            476 PRECALL                  2
                            480 CALL                     2
                            490 STORE_FAST              12 (extra_args)
                
-               152         492 LOAD_FAST                2 (from_default)
+               139         492 LOAD_FAST                2 (from_default)
                            494 LOAD_FAST               12 (extra_args)
                            496 LOAD_CONST               9 ('from_default')
                            498 STORE_SUBSCR
                
-               154         502 LOAD_FAST                0 (cls)
+               141         502 LOAD_FAST                0 (cls)
                            504 LOAD_METHOD             10 (update_or_create)
                
-               155         526 LOAD_FAST                5 (model)
+               142         526 LOAD_FAST                5 (model)
                
-               156         528 LOAD_FAST                3 (name)
+               143         528 LOAD_FAST                3 (name)
                
-               157         530 LOAD_FAST                4 (defs)
+               144         530 LOAD_FAST                4 (defs)
                            532 LOAD_METHOD              9 (get)
                            554 LOAD_CONST              10 ('verbose_name')
                            556 LOAD_CONST               4 ('')
                            558 PRECALL                  2
                            562 CALL                     2
                
-               158         572 LOAD_FAST               12 (extra_args)
+               145         572 LOAD_FAST               12 (extra_args)
                
-               159         574 LOAD_FAST                6 (fields)
+               146         574 LOAD_FAST                6 (fields)
                
-               154         576 KW_NAMES                11
+               141         576 KW_NAMES                11
                            578 PRECALL                  5
                            582 CALL                     5
                            592 POP_TOP
                            594 EXTENDED_ARG             1
                            596 JUMP_BACKWARD          278 (to 42)
                
-               131     >>  598 LOAD_CONST              12 (None)
+               118     >>  598 LOAD_CONST              12 (None)
                            600 RETURN_VALUE
                consts
                   'Update or create import templates.'
                   'model'
                   'fields'
                   False
                   ''
@@ -1067,32 +979,120 @@
                   None
                names      ('items', 'apps', 'get_model', 'isinstance', 'str', 'field_type_registry', 'get_from_name', 'pop', 'append', 'get', 'update_or_create')
                varnames   ('cls', 'template_defs', 'from_default', 'name', 'defs', 'model', 'fields', 'field_definition', 'field_type', 'virtual', 'template', 'args', 'extra_args')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
                name       'update_or_create_templates'
-               firstlineno 128
+               firstlineno 115
                lnotab
                   0x020334013402040114012a012801040104010602160128ff10032c012c
                   01040234022c010a021801020102012a01020102fb16e9
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x97007c006a0000000000000000005300
+               149           0 RESUME                   0
+               
+               150           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (verbose_name)
+                            14 RETURN_VALUE
+               consts
+                  None
+               names      ('verbose_name',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
+               name       '__str__'
+               firstlineno 149
+               lnotab 0x0201
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 4
+               flags     : 0
+               code
+                  0x970065005a0164005a02640167015a03020065046402a6010000ab0100
+                  000000000000005a05020065046403a6010000ab0100000000000000005a
+                  06020065076a08000000000000000064046405ac06a6020000ab02000000
+                  000000000067015a0964075300
+               152           0 RESUME                   0
+                             2 LOAD_NAME                0 (__name__)
+                             4 STORE_NAME               1 (__module__)
+                             6 LOAD_CONST               0 ('ImportTemplate.Meta')
+                             8 STORE_NAME               2 (__qualname__)
+               
+               153          10 LOAD_CONST               1 ('name')
+                            12 BUILD_LIST               1
+                            14 STORE_NAME               3 (ordering)
+               
+               154          16 PUSH_NULL
+                            18 LOAD_NAME                4 (_)
+                            20 LOAD_CONST               2 ('Import template')
+                            22 PRECALL                  1
+                            26 CALL                     1
+                            36 STORE_NAME               5 (verbose_name)
+               
+               155          38 PUSH_NULL
+                            40 LOAD_NAME                4 (_)
+                            42 LOAD_CONST               3 ('Import templates')
+                            44 PRECALL                  1
+                            48 CALL                     1
+                            58 STORE_NAME               6 (verbose_name_plural)
+               
+               157          60 PUSH_NULL
+                            62 LOAD_NAME                7 (models)
+                            64 LOAD_ATTR                8 (UniqueConstraint)
+               
+               158          74 LOAD_CONST               4 (('site_id', 'name'))
+                            76 LOAD_CONST               5 ('unique_template_name_per_site')
+               
+               157          78 KW_NAMES                 6
+                            80 PRECALL                  2
+                            84 CALL                     2
+               
+               156          94 BUILD_LIST               1
+                            96 STORE_NAME               9 (constraints)
+                            98 LOAD_CONST               7 (None)
+                           100 RETURN_VALUE
+               consts
+                  'ImportTemplate.Meta'
+                  'name'
+                  'Import template'
+                  'Import templates'
+                  ('site_id', 'name')
+                  'unique_template_name_per_site'
+                  ('fields', 'name')
+                  None
+               names      ('__name__', '__module__', '__qualname__', 'ordering', '_', 'verbose_name', 'verbose_name_plural', 'models', 'UniqueConstraint', 'constraints')
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
+               name       'Meta'
+               firstlineno 152
+               lnotab 0x0a010601160116020e0104ff10ff
+            'Meta'
             (False,)
-         names      ('__name__', '__module__', '__qualname__', 'models', 'BooleanField', 'from_default', 'ForeignKey', 'ContentType', 'CASCADE', '_', 'content_type', 'CharField', 'name', 'verbose_name', 'has_header_row', 'has_index_col', 'separator', 'quotechar', 'Group', 'SET_NULL', 'group', 'GroupType', 'group_type', 'Meta', '__str__', 'save', 'property', 'parsed_separator', 'parsed_quotechar', 'classmethod', 'Model', 'str', 'dict', 'Sequence', 'Tuple', 'FieldType', 'Dict', 'Any', 'bool', 'update_or_create', 'update_or_create_templates', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'BooleanField', 'from_default', 'ForeignKey', 'ContentType', 'CASCADE', '_', 'content_type', 'CharField', 'name', 'verbose_name', 'has_header_row', 'has_index_col', 'separator', 'quotechar', 'Group', 'SET_NULL', 'group', 'GroupType', 'group_type', 'property', 'parsed_separator', 'parsed_quotechar', 'save', 'classmethod', 'Model', 'str', 'dict', 'Sequence', 'Tuple', 'FieldType', 'Dict', 'Any', 'bool', 'update_or_create', 'update_or_create_templates', '__str__', 'Meta', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
          name       'ImportTemplate'
          firstlineno 17
          lnotab
             0x0c0122010e0102010c0114fd1205360136020e0116ff12030e0116ff12
             030e0102010201140114fc12060e010201020114fd12060e0102010c0102
             0102011401040102ff0efa120a0e0102010c01020102011401040102ff0e
-            fa120b1a0a06030a07020104ff0e010203020104ff0e0102030201020202
-            fe020302fd020402fc020502fb020632fa06ff0e01022102010cff0e01
+            fa120b020104ff0e010203020104ff0e0102030a070201020202fe020302
+            fd020402fc020502fb020632fa06ff0e01022102010cff0e0102210603
       'ImportTemplate'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
@@ -1104,17 +1104,16 @@
             056407a6010000ab010000000000000000650c6a0d0000000000000000ac
             08a6030000ab0300000000000000005a0e020065036a0f00000000000000
             00020065056409a6010000ab0100000000000000006900ac0aa6020000ab
             0200000000000000005a10020065036a1100000000000000000200650564
             0ba6010000ab010000000000000000640c640cac0da6030000ab03000000
             00000000005a12020065036a13000000000000000002006505640ea60100
             00ab010000000000000000640fac10a6020000ab0200000000000000005a
-            1402004700641184006412a6020000ab0200000000000000005a15641384
-            005a16651764148400a6000000ab0000000000000000005a18641584005a
-            1964165300
+            14651564118400a6000000ab0000000000000000005a16641284005a1702
+            004700641384006414a6020000ab0200000000000000005a1864155300
          163           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ImportTemplateField')
                        8 STORE_NAME               2 (__qualname__)
          
          164          10 PUSH_NULL
@@ -1213,42 +1212,38 @@
                      340 LOAD_CONST              15 (True)
          
          179         342 KW_NAMES                16
                      344 PRECALL                  2
                      348 CALL                     2
                      358 STORE_NAME              20 (virtual_tmpl)
          
-         183         360 PUSH_NULL
-                     362 LOAD_BUILD_CLASS
-                     364 LOAD_CONST              17 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 183>)
-                     366 MAKE_FUNCTION            0
-                     368 LOAD_CONST              18 ('Meta')
-                     370 PRECALL                  2
-                     374 CALL                     2
-                     384 STORE_NAME              21 (Meta)
-         
-         189         386 LOAD_CONST              19 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 189>)
-                     388 MAKE_FUNCTION            0
-                     390 STORE_NAME              22 (__str__)
-         
-         192         392 LOAD_NAME               23 (property)
-         
-         193         394 LOAD_CONST              20 (<code object field_type_class, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 192>)
-                     396 MAKE_FUNCTION            0
-         
-         192         398 PRECALL                  0
-                     402 CALL                     0
-         
-         193         412 STORE_NAME              24 (field_type_class)
-         
-         197         414 LOAD_CONST              21 (<code object clean, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 197>)
-                     416 MAKE_FUNCTION            0
-                     418 STORE_NAME              25 (clean)
-                     420 LOAD_CONST              22 (None)
-                     422 RETURN_VALUE
+         183         360 LOAD_NAME               21 (property)
+         
+         184         362 LOAD_CONST              17 (<code object field_type_class, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 183>)
+                     364 MAKE_FUNCTION            0
+         
+         183         366 PRECALL                  0
+                     370 CALL                     0
+         
+         184         380 STORE_NAME              22 (field_type_class)
+         
+         188         382 LOAD_CONST              18 (<code object clean, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 188>)
+                     384 MAKE_FUNCTION            0
+                     386 STORE_NAME              23 (clean)
+         
+         197         388 PUSH_NULL
+                     390 LOAD_BUILD_CLASS
+                     392 LOAD_CONST              19 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 197>)
+                     394 MAKE_FUNCTION            0
+                     396 LOAD_CONST              20 ('Meta')
+                     398 PRECALL                  2
+                     402 CALL                     2
+                     412 STORE_NAME              24 (Meta)
+                     414 LOAD_CONST              21 (None)
+                     416 RETURN_VALUE
          consts
             'ImportTemplateField'
             'Index'
             ('verbose_name',)
             'Import template'
             'fields'
             ('verbose_name', 'related_name')
@@ -1260,133 +1255,42 @@
             'Virtual field'
             False
             ('verbose_name', 'default', 'null')
             'Django template to generate virtual field from'
             True
             ('verbose_name', 'blank')
             code
-               argcount  : 0
-               nlocals   : 0
-               stacksize : 3
-               flags     : 0
-               code
-                  0x970065005a0164005a026401640267025a036401640267025a04020065
-                  056403a6010000ab0100000000000000005a06020065056404a6010000ab
-                  0100000000000000005a0764055300
-               183           0 RESUME                   0
-                             2 LOAD_NAME                0 (__name__)
-                             4 STORE_NAME               1 (__module__)
-                             6 LOAD_CONST               0 ('ImportTemplateField.Meta')
-                             8 STORE_NAME               2 (__qualname__)
-               
-               184          10 LOAD_CONST               1 ('template')
-                            12 LOAD_CONST               2 ('index')
-                            14 BUILD_LIST               2
-                            16 STORE_NAME               3 (ordering)
-               
-               185          18 LOAD_CONST               1 ('template')
-                            20 LOAD_CONST               2 ('index')
-                            22 BUILD_LIST               2
-                            24 STORE_NAME               4 (unique_together)
-               
-               186          26 PUSH_NULL
-                            28 LOAD_NAME                5 (_)
-                            30 LOAD_CONST               3 ('Import template field')
-                            32 PRECALL                  1
-                            36 CALL                     1
-                            46 STORE_NAME               6 (verbose_name)
-               
-               187          48 PUSH_NULL
-                            50 LOAD_NAME                5 (_)
-                            52 LOAD_CONST               4 ('Import template fields')
-                            54 PRECALL                  1
-                            58 CALL                     1
-                            68 STORE_NAME               7 (verbose_name_plural)
-                            70 LOAD_CONST               5 (None)
-                            72 RETURN_VALUE
-               consts
-                  'ImportTemplateField.Meta'
-                  'template'
-                  'index'
-                  'Import template field'
-                  'Import template fields'
-                  None
-               names      ('__name__', '__module__', '__qualname__', 'ordering', 'unique_together', '_', 'verbose_name', 'verbose_name_plural')
-               varnames   ()
-               freevars   ()
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
-               name       'Meta'
-               firstlineno 183
-               lnotab 0x0a01080108011601
-            'Meta'
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 5
-               flags     : 3
-               code
-                  0x97007c006a0000000000000000009b0064017c006a0100000000000000
-                  009b0064027c006a0200000000000000009b009d055300
-               189           0 RESUME                   0
-               
-               190           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (template)
-                            14 FORMAT_VALUE             0
-                            16 LOAD_CONST               1 ('/')
-                            18 LOAD_FAST                0 (self)
-                            20 LOAD_ATTR                1 (index)
-                            30 FORMAT_VALUE             0
-                            32 LOAD_CONST               2 (': ')
-                            34 LOAD_FAST                0 (self)
-                            36 LOAD_ATTR                2 (field_type)
-                            46 FORMAT_VALUE             0
-                            48 BUILD_STRING             5
-                            50 RETURN_VALUE
-               consts
-                  None
-                  '/'
-                  ': '
-               names      ('template', 'index', 'field_type')
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
-               name       '__str__'
-               firstlineno 189
-               lnotab 0x0201
-            code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   00000000000000a6010000ab0100000000000000007d017c015300
-               192           0 RESUME                   0
+               183           0 RESUME                   0
                
-               194           2 LOAD_GLOBAL              1 (NULL + field_type_registry)
+               185           2 LOAD_GLOBAL              1 (NULL + field_type_registry)
                             14 LOAD_ATTR                1 (get_from_name)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (field_type)
                             36 PRECALL                  1
                             40 CALL                     1
                             50 STORE_FAST               1 (field_type)
                
-               195          52 LOAD_FAST                1 (field_type)
+               186          52 LOAD_FAST                1 (field_type)
                             54 RETURN_VALUE
                consts
                   None
                names      ('field_type_registry', 'get_from_name', 'field_type')
                varnames   ('self', 'field_type')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
                name       'field_type_class'
-               firstlineno 192
+               firstlineno 183
                lnotab 0x02023201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -1394,172 +1298,224 @@
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   007d017c006a0300000000000000007408000000000000000000006a0500
                   000000000000007c01190000000000000000007601722f7c006a03000000
                   00000000007408000000000000000000006a060000000000000000760172
                   1e740f000000000000000000007411000000000000000000006401a60100
                   00ab010000000000000000a6010000ab0100000000000000008201640253
                   0064025300
-               197           0 RESUME                   0
+               188           0 RESUME                   0
                
-               199           2 LOAD_FAST                0 (self)
+               190           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (template)
                             14 LOAD_ATTR                1 (content_type)
                             24 LOAD_METHOD              2 (model_class)
                             46 PRECALL                  0
                             50 CALL                     0
                             60 STORE_FAST               1 (model)
                
-               201          62 LOAD_FAST                0 (self)
+               192          62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (field_type)
                             74 LOAD_GLOBAL              8 (field_type_registry)
                             86 LOAD_ATTR                5 (allowed_field_types_for_models)
                             96 LOAD_FAST                1 (model)
                             98 BINARY_SUBSCR
                            108 CONTAINS_OP              1
                            110 POP_JUMP_FORWARD_IF_FALSE    47 (to 206)
                
-               202         112 LOAD_FAST                0 (self)
+               193         112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                3 (field_type)
                            124 LOAD_GLOBAL              8 (field_type_registry)
                            136 LOAD_ATTR                6 (allowed_field_types_for_all_models)
                            146 CONTAINS_OP              1
                            148 POP_JUMP_FORWARD_IF_FALSE    30 (to 210)
                
-               204         150 LOAD_GLOBAL             15 (NULL + ValidationError)
+               195         150 LOAD_GLOBAL             15 (NULL + ValidationError)
                            162 LOAD_GLOBAL             17 (NULL + _)
                            174 LOAD_CONST               1 ('You are not allowed to use this field type in this model.')
                            176 PRECALL                  1
                            180 CALL                     1
                            190 PRECALL                  1
                            194 CALL                     1
                            204 RAISE_VARARGS            1
                
-               201     >>  206 LOAD_CONST               2 (None)
+               192     >>  206 LOAD_CONST               2 (None)
                            208 RETURN_VALUE
                
-               202     >>  210 LOAD_CONST               2 (None)
+               193     >>  210 LOAD_CONST               2 (None)
                            212 RETURN_VALUE
                consts
                   'Validate correct usage of field types.'
                   'You are not allowed to use this field type in this model.'
                   None
                names      ('template', 'content_type', 'model_class', 'field_type', 'field_type_registry', 'allowed_field_types_for_models', 'allowed_field_types_for_all_models', 'ValidationError', '_')
                varnames   ('self', 'model')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
                name       'clean'
-               firstlineno 197
+               firstlineno 188
                lnotab 0x02023c023201260238fd0401
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 3
+               flags     : 0
+               code
+                  0x970065005a0164005a026401640267025a036401640267025a04020065
+                  056403a6010000ab0100000000000000005a06020065056404a6010000ab
+                  0100000000000000005a0764055300
+               197           0 RESUME                   0
+                             2 LOAD_NAME                0 (__name__)
+                             4 STORE_NAME               1 (__module__)
+                             6 LOAD_CONST               0 ('ImportTemplateField.Meta')
+                             8 STORE_NAME               2 (__qualname__)
+               
+               198          10 LOAD_CONST               1 ('template')
+                            12 LOAD_CONST               2 ('index')
+                            14 BUILD_LIST               2
+                            16 STORE_NAME               3 (ordering)
+               
+               199          18 LOAD_CONST               1 ('template')
+                            20 LOAD_CONST               2 ('index')
+                            22 BUILD_LIST               2
+                            24 STORE_NAME               4 (unique_together)
+               
+               200          26 PUSH_NULL
+                            28 LOAD_NAME                5 (_)
+                            30 LOAD_CONST               3 ('Import template field')
+                            32 PRECALL                  1
+                            36 CALL                     1
+                            46 STORE_NAME               6 (verbose_name)
+               
+               201          48 PUSH_NULL
+                            50 LOAD_NAME                5 (_)
+                            52 LOAD_CONST               4 ('Import template fields')
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 STORE_NAME               7 (verbose_name_plural)
+                            70 LOAD_CONST               5 (None)
+                            72 RETURN_VALUE
+               consts
+                  'ImportTemplateField.Meta'
+                  'template'
+                  'index'
+                  'Import template field'
+                  'Import template fields'
+                  None
+               names      ('__name__', '__module__', '__qualname__', 'ordering', 'unique_together', '_', 'verbose_name', 'verbose_name_plural')
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
+               name       'Meta'
+               firstlineno 197
+               lnotab 0x0a01080108011601
+            'Meta'
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'IntegerField', '_', 'index', 'ForeignKey', 'ImportTemplate', 'CASCADE', 'template', 'CharField', 'field_type_registry', 'choices', 'field_type', 'JSONField', 'args', 'BooleanField', 'virtual', 'TextField', 'virtual_tmpl', 'Meta', '__str__', 'property', 'field_type_class', 'clean')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'IntegerField', '_', 'index', 'ForeignKey', 'ImportTemplate', 'CASCADE', 'template', 'CharField', 'field_type_registry', 'choices', 'field_type', 'JSONField', 'args', 'BooleanField', 'virtual', 'TextField', 'virtual_tmpl', 'property', 'field_type_class', 'clean', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
          name       'ImportTemplateField'
          firstlineno 163
          lnotab
             0x0a0134010e0102010c01140102fc12060e01020114010cfd1205360238
-            010e0116ff12041a060603020104ff0e010204
+            010e0116ff1204020104ff0e0102040609
       'ImportTemplateField'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
          code
             0x970065005a0164005a0264015a03020065046a05000000000000000065
             0665046a070000000000000000020065086402a6010000ab010000000000
             0000006403ac04a6040000ab0400000000000000005a09020065046a0a00
             000000000000006405ac06a6010000ab0100000000000000005a0b020065
             046a050000000000000000650c65046a0700000000000000000200650864
             07a6010000ab010000000000000000640364086408ac09a6060000ab0600
             000000000000005a0d02004700640a8400640ba6020000ab020000000000
-            0000005a0e640c84005a0f640d5300
-         207           0 RESUME                   0
+            0000005a0e640c5300
+         204           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ImportJob')
                        8 STORE_NAME               2 (__qualname__)
          
-         208          10 LOAD_CONST               1 ('Job definition for one import, to track import history and files.')
+         205          10 LOAD_CONST               1 ('Job definition for one import, to track import history and files.')
                       12 STORE_NAME               3 (__doc__)
          
-         210          14 PUSH_NULL
+         207          14 PUSH_NULL
                       16 LOAD_NAME                4 (models)
                       18 LOAD_ATTR                5 (ForeignKey)
          
-         211          28 LOAD_NAME                6 (ImportTemplate)
+         208          28 LOAD_NAME                6 (ImportTemplate)
          
-         212          30 LOAD_NAME                4 (models)
+         209          30 LOAD_NAME                4 (models)
                       32 LOAD_ATTR                7 (CASCADE)
          
-         213          42 PUSH_NULL
+         210          42 PUSH_NULL
                       44 LOAD_NAME                8 (_)
                       46 LOAD_CONST               2 ('Import template')
                       48 PRECALL                  1
                       52 CALL                     1
          
-         214          62 LOAD_CONST               3 ('import_jobs')
+         211          62 LOAD_CONST               3 ('import_jobs')
          
-         210          64 KW_NAMES                 4
+         207          64 KW_NAMES                 4
                       66 PRECALL                  4
                       70 CALL                     4
                       80 STORE_NAME               9 (template)
          
-         216          82 PUSH_NULL
+         213          82 PUSH_NULL
                       84 LOAD_NAME                4 (models)
                       86 LOAD_ATTR               10 (FileField)
                       96 LOAD_CONST               5 ('csv_import/')
                       98 KW_NAMES                 6
                      100 PRECALL                  1
                      104 CALL                     1
                      114 STORE_NAME              11 (data_file)
          
-         217         116 PUSH_NULL
+         214         116 PUSH_NULL
                      118 LOAD_NAME                4 (models)
                      120 LOAD_ATTR                5 (ForeignKey)
          
-         218         130 LOAD_NAME               12 (SchoolTerm)
+         215         130 LOAD_NAME               12 (SchoolTerm)
          
-         219         132 LOAD_NAME                4 (models)
+         216         132 LOAD_NAME                4 (models)
                      134 LOAD_ATTR                7 (CASCADE)
          
-         220         144 PUSH_NULL
+         217         144 PUSH_NULL
                      146 LOAD_NAME                8 (_)
                      148 LOAD_CONST               7 ('School term')
                      150 PRECALL                  1
                      154 CALL                     1
          
-         221         164 LOAD_CONST               3 ('import_jobs')
+         218         164 LOAD_CONST               3 ('import_jobs')
          
-         222         166 LOAD_CONST               8 (True)
+         219         166 LOAD_CONST               8 (True)
          
-         223         168 LOAD_CONST               8 (True)
+         220         168 LOAD_CONST               8 (True)
          
-         217         170 KW_NAMES                 9
+         214         170 KW_NAMES                 9
                      172 PRECALL                  6
                      176 CALL                     6
                      186 STORE_NAME              13 (school_term)
          
-         226         188 PUSH_NULL
+         223         188 PUSH_NULL
                      190 LOAD_BUILD_CLASS
-                     192 LOAD_CONST              10 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 226>)
+                     192 LOAD_CONST              10 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 223>)
                      194 MAKE_FUNCTION            0
                      196 LOAD_CONST              11 ('Meta')
                      198 PRECALL                  2
                      202 CALL                     2
                      212 STORE_NAME              14 (Meta)
-         
-         230         214 LOAD_CONST              12 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py", line 230>)
-                     216 MAKE_FUNCTION            0
-                     218 STORE_NAME              15 (__str__)
-                     220 LOAD_CONST              13 (None)
-                     222 RETURN_VALUE
+                     214 LOAD_CONST              12 (None)
+                     216 RETURN_VALUE
          consts
             'ImportJob'
             'Job definition for one import, to track import history and files.'
             'Import template'
             'import_jobs'
             ('on_delete', 'verbose_name', 'related_name')
             'csv_import/'
@@ -1571,28 +1527,28 @@
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               226           0 RESUME                   0
+               223           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('ImportJob.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               227          10 PUSH_NULL
+               224          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('Import job')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               228          32 PUSH_NULL
+               225          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('Import jobs')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                             54 LOAD_CONST               3 (None)
                             56 RETURN_VALUE
@@ -1603,62 +1559,32 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
                name       'Meta'
-               firstlineno 226
+               firstlineno 223
                lnotab 0x0a011601
             'Meta'
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 3
-               flags     : 3
-               code
-                  0x97007c006a0000000000000000009b0064017c006a0100000000000000
-                  009b009d035300
-               230           0 RESUME                   0
-               
-               231           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (template)
-                            14 FORMAT_VALUE             0
-                            16 LOAD_CONST               1 ('#')
-                            18 LOAD_FAST                0 (self)
-                            20 LOAD_ATTR                1 (pk)
-                            30 FORMAT_VALUE             0
-                            32 BUILD_STRING             3
-                            34 RETURN_VALUE
-               consts
-                  None
-                  '#'
-               names      ('template', 'pk')
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
-               name       '__str__'
-               firstlineno 230
-               lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'ImportTemplate', 'CASCADE', '_', 'template', 'FileField', 'data_file', 'SchoolTerm', 'school_term', 'Meta', '__str__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'ImportTemplate', 'CASCADE', '_', 'template', 'FileField', 'data_file', 'SchoolTerm', 'school_term', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
          name       'ImportJob'
-         firstlineno 207
+         firstlineno 204
          lnotab
             0x0a0104020e0102010c01140102fc120622010e0102010c011401020102
-            0102fa12091a04
+            0102fa1209
       'ImportJob'
    names      ('codecs', 'typing', 'Any', 'Dict', 'Sequence', 'Tuple', 'django.apps', 'apps', 'django.contrib.contenttypes.models', 'ContentType', 'django.core.exceptions', 'ValidationError', 'django.db', 'models', 'django.db.models', 'Model', 'django.utils.translation', 'gettext', '_', 'aleksis.core.mixins', 'ExtensibleModel', 'aleksis.core.models', 'Group', 'GroupType', 'SchoolTerm', 'field_types', 'FieldType', 'field_type_registry', 'ImportTemplate', 'ImportTemplateField', 'ImportJob')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080118020c010c010c010c010c010c020c01140210031c7f00
-      131c2c
+      131c29
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/preferences.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/preferences.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 1573
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/__pycache__/rules.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/rules.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 851
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/default_templates.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/default_templates.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/default_templates.yaml` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/default_templates.yaml`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/field_types.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/field_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -473,28 +473,23 @@
 
 
 @field_type_registry.register
 class FileFieldType(ProcessFieldType):
     """Field type that stores a referenced file on a file field."""
 
     def process(self, instance: Model, value: str):
+        # Test path for unwanted path traversal
+        abs_path = os.path.realpath(value)
+        if not self.base_path == os.path.commonpath((self.base_path, abs_path)):
+            raise ValueError(f"Disallowed path traversal importing file from {value}")
+
         # Get target FileField and save content
         field_name = self.get_db_field()
         file_field = getattr(instance, field_name)
-
-        if value:
-            # Test path for unwanted path traversal
-            abs_path = os.path.realpath(value)
-            if not self.base_path == os.path.commonpath((self.base_path, abs_path)):
-                raise ValueError(f"Disallowed path traversal importing file from {value}")
-
-            file_field.save(os.path.basename(abs_path), File(open(abs_path, "rb")))
-        else:
-            # Clear the file field
-            file_field.delete()
+        file_field.save(os.path.basename(abs_path), File(open(abs_path, "rb")))
 
         instance.save()
 
 
 @field_type_registry.register
 class AvatarFieldType(FileFieldType):
     name = "avatar"
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/forms.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/frontend/index.js` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-05-26 04:38+0000\n"
+"PO-Revision-Date: 2022-07-03 06:13+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
 "Language-Team: Russian <https://translate.edugit.org/projects/aleksis/"
 "aleksis-app-csvimport/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -190,15 +190,15 @@
 msgid "Missing unique reference or other matching fields."
 msgstr "Остутствует уникальная ссылка или другие поля для сравнения."
 
 msgid "Mobile number"
 msgstr "Номер мобильного"
 
 msgid "Name"
-msgstr "Полное имя"
+msgstr "Имя"
 
 msgid "Name of a group the person is a member of"
 msgstr "Название группы, к которой принадлежит физлицо"
 
 msgid "Name of import template which should be used"
 msgstr "Название шаблона, который нужно использовать"
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-06-21 12:14+0200\n"
-"PO-Revision-Date: 2023-05-26 04:38+0000\n"
+"PO-Revision-Date: 2022-07-03 06:13+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
-"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/aleksis-app-csvimport/ru/>\n"
+"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/"
+"aleksis-app-csvimport/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
+"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
+"%100>=11 && n%100<=14)? 2 : 3);\n"
 "X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/csv_import/field_types.py:162
 msgid "Unique reference"
 msgstr "Уникальная ссылка"
 
 #: aleksis/apps/csv_import/field_types.py:170
 #: aleksis/apps/csv_import/models.py:24 aleksis/apps/csv_import/models.py:25
 msgid "Name"
-msgstr "Полное имя"
+msgstr "Имя"
 
 #: aleksis/apps/csv_import/field_types.py:178
 msgid "First name"
 msgstr "Имя"
 
 #: aleksis/apps/csv_import/field_types.py:185
 msgid "Last name"
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,24 +1,24 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-01-25 05:57+0000\n"
+"PO-Revision-Date: 2022-05-07 01:36+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
 "Language-Team: Ukrainian <https://translate.edugit.org/projects/aleksis/"
 "aleksis-app-csvimport/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
-"X-Generator: Weblate 4.12.1\n"
+"X-Generator: Weblate 4.8\n"
 
 msgid ""
 "\n"
 "        You can import data from several school administration software "
 "using this CSV importer. Please read the notes\n"
 "        according to your software in the documentation! Sometimes there is "
 "needed a special procedure to import the data correctly.\n"
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-06-21 12:14+0200\n"
-"PO-Revision-Date: 2023-01-25 05:57+0000\n"
+"PO-Revision-Date: 2022-05-07 01:36+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
-"Language-Team: Ukrainian <https://translate.edugit.org/projects/aleksis/aleksis-app-csvimport/uk/>\n"
+"Language-Team: Ukrainian <https://translate.edugit.org/projects/aleksis/"
+"aleksis-app-csvimport/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
-"X-Generator: Weblate 4.12.1\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
+"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
+"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
+"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"X-Generator: Weblate 4.8\n"
 
 #: aleksis/apps/csv_import/field_types.py:162
 msgid "Unique reference"
 msgstr "Унікальне посилання"
 
 #: aleksis/apps/csv_import/field_types.py:170
 #: aleksis/apps/csv_import/models.py:24 aleksis/apps/csv_import/models.py:25
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/management/commands/csv_import.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/management/commands/csv_import.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/menus.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/menus.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0001_initial.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0002_importjob.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0002_importjob.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0004_args.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0004_args.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/migrations/0007_virtual_template_field.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0007_virtual_template_field.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/models.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,42 +59,29 @@
         null=True,
         verbose_name=_("Group type"),
         help_text=_(
             "If imported objects are groups, they all will get this group type after import."
         ),
     )
 
-    class Meta:
-        ordering = ["name"]
-        verbose_name = _("Import template")
-        verbose_name_plural = _("Import templates")
-        constraints = [
-            models.UniqueConstraint(
-                fields=("site_id", "name"), name="unique_template_name_per_site"
-            ),
-        ]
+    @property
+    def parsed_separator(self):
+        return codecs.escape_decode(bytes(self.separator, "utf-8"))[0].decode("utf-8")
 
-    def __str__(self):
-        return self.verbose_name
+    @property
+    def parsed_quotechar(self):
+        return codecs.escape_decode(bytes(self.quotechar, "utf-8"))[0].decode("utf-8")
 
     def save(self, *args, **kwargs):
         if not self.content_type.model == "person":
             self.group = None
         if not self.content_type.model == "group":
             self.group_type = None
         super().save(*args, **kwargs)
 
-    @property
-    def parsed_separator(self):
-        return codecs.escape_decode(bytes(self.separator, "utf-8"))[0].decode("utf-8")
-
-    @property
-    def parsed_quotechar(self):
-        return codecs.escape_decode(bytes(self.quotechar, "utf-8"))[0].decode("utf-8")
-
     @classmethod
     def update_or_create(
         cls,
         model: Model,
         name: str,
         verbose_name: str,
         extra_args: dict,
@@ -155,14 +142,27 @@
                 model,
                 name=name,
                 verbose_name=defs.get("verbose_name", ""),
                 extra_args=extra_args,
                 fields=fields,
             )
 
+    def __str__(self):
+        return self.verbose_name
+
+    class Meta:
+        ordering = ["name"]
+        verbose_name = _("Import template")
+        verbose_name_plural = _("Import templates")
+        constraints = [
+            models.UniqueConstraint(
+                fields=("site_id", "name"), name="unique_template_name_per_site"
+            ),
+        ]
+
 
 class ImportTemplateField(ExtensibleModel):
     index = models.IntegerField(verbose_name=_("Index"))
     template = models.ForeignKey(
         ImportTemplate,
         models.CASCADE,
         verbose_name=_("Import template"),
@@ -176,37 +176,34 @@
     args = models.JSONField(verbose_name=_("Optional arguments passed to field type"), default={})
 
     virtual = models.BooleanField(verbose_name=_("Virtual field"), default=False, null=False)
     virtual_tmpl = models.TextField(
         verbose_name=_("Django template to generate virtual field from"), blank=True
     )
 
-    class Meta:
-        ordering = ["template", "index"]
-        unique_together = ["template", "index"]
-        verbose_name = _("Import template field")
-        verbose_name_plural = _("Import template fields")
-
-    def __str__(self):
-        return f"{self.template}/{self.index}: {self.field_type}"
-
     @property
     def field_type_class(self):
         field_type = field_type_registry.get_from_name(self.field_type)
         return field_type
 
     def clean(self):
         """Validate correct usage of field types."""
         model = self.template.content_type.model_class()
         if (
             self.field_type not in field_type_registry.allowed_field_types_for_models[model]
             and self.field_type not in field_type_registry.allowed_field_types_for_all_models
         ):
             raise ValidationError(_("You are not allowed to use this field type in this model."))
 
+    class Meta:
+        ordering = ["template", "index"]
+        unique_together = ["template", "index"]
+        verbose_name = _("Import template field")
+        verbose_name_plural = _("Import template fields")
+
 
 class ImportJob(ExtensibleModel):
     """Job definition for one import, to track import history and files."""
 
     template = models.ForeignKey(
         ImportTemplate,
         on_delete=models.CASCADE,
@@ -222,10 +219,7 @@
         blank=True,
         null=True,
     )
 
     class Meta:
         verbose_name = _("Import job")
         verbose_name_plural = _("Import jobs")
-
-    def __str__(self):
-        return f"{self.template}#{self.pk}"
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/preferences.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/rules.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/templates/csv_import/csv_import.html` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/csv_import.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/templates/csv_import/import_template/list.html` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/import_template/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/templates/csv_import/import_template/upload.html` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/import_template/upload.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/models/test_template.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/models/test_template.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/models/test_template_load.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/models/test_template_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
 
 def test_load_sample_template(tmp_path):
     test_filename = os.path.join(tmp_path, "templates.yaml")
     with open(test_filename, "w") as f:
         f.write(TEST_FILE_1)
 
-    ImportTemplate.objects.all().delete()
     assert ImportTemplate.objects.all().count() == 0
 
     update_or_create_templates_from_yaml(test_filename)
 
     assert ImportTemplate.objects.all().count() == 1
     assert ImportTemplateField.objects.all().count() == 7
     template = ImportTemplate.objects.all()[0]
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/test_field_types.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/test_field_types.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/util/test_class_range_helpers.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_class_range_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/tests/util/test_converters.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     parse_sex,
 )
 from aleksis.core.util.core_helpers import get_site_preferences
 
 pytestmark = pytest.mark.django_db
 
 
-def test_parse_phone_number(settings):
-    settings.PHONENUMBER_DEFAULT_REGION = "DE"
+def test_parse_phone_number():
+    get_site_preferences()["internationalisation__phone_number_country"] = "DE"
     fake_number = PhoneNumber(country_code=49, national_number=1635550217)
     assert parse_phone_number("+49-163-555-0217") == fake_number
     assert parse_phone_number("+491635550217") == fake_number
     assert parse_phone_number("0163-555-0217") == fake_number
     assert parse_phone_number("01635550217") == fake_number
-    settings.PHONENUMBER_DEFAULT_REGION = "GB"
+    get_site_preferences()["internationalisation__phone_number_country"] = "GB"
     assert parse_phone_number("0163-555-0217") != fake_number
     assert parse_phone_number("01635550217") != fake_number
 
 
 def test_parse_phone_number_none():
     assert parse_phone_number("") == ""
     assert parse_phone_number("foo") == ""
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/__pycache__/class_range_helpers.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/class_range_helpers.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 3824
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/__pycache__/converters.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/converters.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,31 +1,31 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
-files sz: 2287
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
+files sz: 2295
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
-      055a056d065a060100640064036c076d085a080100640064046c096d0a5a
-      0a0100640064056c0b6d0c5a0c0100640064066c0d6d0e5a0e0100640064
-      076c0f6d105a10010002004700640884006409a6020000ab020000000000
-      0000005a1102006511a6000000ab0000000000000000005a1265126a1300
-      00000000000000640a6514640b6506650865146602190000000000000000
-      006604640c8404a6000000ab0000000000000000005a1565126a13000000
-      0000000000640a6514640b65146604640d8404a6000000ab000000000000
-      0000005a1665126a130000000000000000640a6514640b65066501640e66
-      02190000000000000000006604640f8404a6000000ab0000000000000000
-      005a1765126a130000000000000000640a6514640b650565141900000000
-      0000000000660464108404a6000000ab0000000000000000005a18641144
-      005d215a196512a013000000000000000000000000000000000000000002
-      00651a65146519a6020000ab020000000000000000a6010000ab01000000
-      000000000001008c22640e5300
+      055a056d065a060100640064036c075a07640064046c086d095a09010064
+      0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d0100640064076c0e6d
+      0f5a0f010002004700640884006409a6020000ab0200000000000000005a
+      1002006510a6000000ab0000000000000000005a1165116a120000000000
+      000000640a6513640b650665096513660219000000000000000000660464
+      0c8404a6000000ab0000000000000000005a1465116a1200000000000000
+      00640a6513640b65136604640d8404a6000000ab0000000000000000005a
+      1565116a120000000000000000640a6513640b6506650164036602190000
+      000000000000006604640e8404a6000000ab0000000000000000005a1665
+      116a120000000000000000640a6513640b65056513190000000000000000
+      006604640f8404a6000000ab0000000000000000005a17641044005d215a
+      186511a01200000000000000000000000000000000000000000200651965
+      136518a6020000ab020000000000000000a6010000ab0100000000000000
+      0001008c2264035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('date',))
                  6 IMPORT_NAME              0 (datetime)
                  8 IMPORT_FROM              1 (date)
                 10 STORE_NAME               1 (date)
@@ -41,165 +41,163 @@
                 28 IMPORT_FROM              5 (Sequence)
                 30 STORE_NAME               5 (Sequence)
                 32 IMPORT_FROM              6 (Union)
                 34 STORE_NAME               6 (Union)
                 36 POP_TOP
    
      4          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (('PhoneNumber',))
-                42 IMPORT_NAME              7 (phonenumber_field.phonenumber)
-                44 IMPORT_FROM              8 (PhoneNumber)
-                46 STORE_NAME               8 (PhoneNumber)
-                48 POP_TOP
-   
-     5          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('NumberParseException',))
-                54 IMPORT_NAME              9 (phonenumbers)
-                56 IMPORT_FROM             10 (NumberParseException)
-                58 STORE_NAME              10 (NumberParseException)
-                60 POP_TOP
-   
-     7          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('SEXES',))
-                66 IMPORT_NAME             11 (aleksis.apps.csv_import.settings)
-                68 IMPORT_FROM             12 (SEXES)
-                70 STORE_NAME              12 (SEXES)
-                72 POP_TOP
-   
-     8          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               6 (('settings',))
-                78 IMPORT_NAME             13 (aleksis.core)
-                80 IMPORT_FROM             14 (settings)
-                82 STORE_NAME              14 (settings)
-                84 POP_TOP
-   
-     9          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               7 (('get_site_preferences',))
-                90 IMPORT_NAME             15 (aleksis.core.util.core_helpers)
-                92 IMPORT_FROM             16 (get_site_preferences)
-                94 STORE_NAME              16 (get_site_preferences)
-                96 POP_TOP
-   
-    12          98 PUSH_NULL
-               100 LOAD_BUILD_CLASS
-               102 LOAD_CONST               8 (<code object ConverterRegistry, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 12>)
-               104 MAKE_FUNCTION            0
-               106 LOAD_CONST               9 ('ConverterRegistry')
-               108 PRECALL                  2
-               112 CALL                     2
-               122 STORE_NAME              17 (ConverterRegistry)
-   
-    31         124 PUSH_NULL
-               126 LOAD_NAME               17 (ConverterRegistry)
-               128 PRECALL                  0
-               132 CALL                     0
-               142 STORE_NAME              18 (converter_registry)
-   
-    34         144 LOAD_NAME               18 (converter_registry)
-               146 LOAD_ATTR               19 (register)
-   
-    35         156 LOAD_CONST              10 ('value')
-               158 LOAD_NAME               20 (str)
-               160 LOAD_CONST              11 ('return')
-               162 LOAD_NAME                6 (Union)
-               164 LOAD_NAME                8 (PhoneNumber)
-               166 LOAD_NAME               20 (str)
-               168 BUILD_TUPLE              2
-               170 BINARY_SUBSCR
-               180 BUILD_TUPLE              4
-               182 LOAD_CONST              12 (<code object parse_phone_number, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 34>)
-               184 MAKE_FUNCTION            4 (annotations)
-   
-    34         186 PRECALL                  0
-               190 CALL                     0
-   
-    35         200 STORE_NAME              21 (parse_phone_number)
-   
-    46         202 LOAD_NAME               18 (converter_registry)
-               204 LOAD_ATTR               19 (register)
-   
-    47         214 LOAD_CONST              10 ('value')
-               216 LOAD_NAME               20 (str)
-               218 LOAD_CONST              11 ('return')
-               220 LOAD_NAME               20 (str)
-               222 BUILD_TUPLE              4
-               224 LOAD_CONST              13 (<code object parse_sex, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 46>)
-               226 MAKE_FUNCTION            4 (annotations)
-   
-    46         228 PRECALL                  0
-               232 CALL                     0
-   
-    47         242 STORE_NAME              22 (parse_sex)
-   
-    56         244 LOAD_NAME               18 (converter_registry)
-               246 LOAD_ATTR               19 (register)
-   
-    57         256 LOAD_CONST              10 ('value')
-               258 LOAD_NAME               20 (str)
-               260 LOAD_CONST              11 ('return')
-               262 LOAD_NAME                6 (Union)
-               264 LOAD_NAME                1 (date)
-               266 LOAD_CONST              14 (None)
-               268 BUILD_TUPLE              2
-               270 BINARY_SUBSCR
-               280 BUILD_TUPLE              4
-               282 LOAD_CONST              15 (<code object parse_date, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 56>)
-               284 MAKE_FUNCTION            4 (annotations)
-   
-    56         286 PRECALL                  0
-               290 CALL                     0
-   
-    57         300 STORE_NAME              23 (parse_date)
-   
-    69         302 LOAD_NAME               18 (converter_registry)
-               304 LOAD_ATTR               19 (register)
-   
-    70         314 LOAD_CONST              10 ('value')
-               316 LOAD_NAME               20 (str)
-               318 LOAD_CONST              11 ('return')
-               320 LOAD_NAME                5 (Sequence)
-               322 LOAD_NAME               20 (str)
-               324 BINARY_SUBSCR
-               334 BUILD_TUPLE              4
-               336 LOAD_CONST              16 (<code object parse_comma_separated_data, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 69>)
-               338 MAKE_FUNCTION            4 (annotations)
-   
-    69         340 PRECALL                  0
-               344 CALL                     0
-   
-    70         354 STORE_NAME              24 (parse_comma_separated_data)
-   
-    75         356 LOAD_CONST              17 (('capitalize', 'lstrip', 'strip', 'rstrip', 'lower', 'upper', 'title'))
-               358 GET_ITER
-           >>  360 FOR_ITER                33 (to 428)
-               362 STORE_NAME              25 (str_converter)
-   
-    76         364 LOAD_NAME               18 (converter_registry)
-               366 LOAD_METHOD             19 (register)
-               388 PUSH_NULL
-               390 LOAD_NAME               26 (getattr)
-               392 LOAD_NAME               20 (str)
-               394 LOAD_NAME               25 (str_converter)
-               396 PRECALL                  2
-               400 CALL                     2
-               410 PRECALL                  1
-               414 CALL                     1
-               424 POP_TOP
-               426 JUMP_BACKWARD           34 (to 360)
+                40 LOAD_CONST               3 (None)
+                42 IMPORT_NAME              7 (dateparser)
+                44 STORE_NAME               7 (dateparser)
+   
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('PhoneNumber',))
+                50 IMPORT_NAME              8 (phonenumber_field.phonenumber)
+                52 IMPORT_FROM              9 (PhoneNumber)
+                54 STORE_NAME               9 (PhoneNumber)
+                56 POP_TOP
+   
+     6          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               5 (('NumberParseException',))
+                62 IMPORT_NAME             10 (phonenumbers)
+                64 IMPORT_FROM             11 (NumberParseException)
+                66 STORE_NAME              11 (NumberParseException)
+                68 POP_TOP
+   
+     8          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               6 (('SEXES',))
+                74 IMPORT_NAME             12 (aleksis.apps.csv_import.settings)
+                76 IMPORT_FROM             13 (SEXES)
+                78 STORE_NAME              13 (SEXES)
+                80 POP_TOP
+   
+     9          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               7 (('get_site_preferences',))
+                86 IMPORT_NAME             14 (aleksis.core.util.core_helpers)
+                88 IMPORT_FROM             15 (get_site_preferences)
+                90 STORE_NAME              15 (get_site_preferences)
+                92 POP_TOP
+   
+    12          94 PUSH_NULL
+                96 LOAD_BUILD_CLASS
+                98 LOAD_CONST               8 (<code object ConverterRegistry, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 12>)
+               100 MAKE_FUNCTION            0
+               102 LOAD_CONST               9 ('ConverterRegistry')
+               104 PRECALL                  2
+               108 CALL                     2
+               118 STORE_NAME              16 (ConverterRegistry)
+   
+    31         120 PUSH_NULL
+               122 LOAD_NAME               16 (ConverterRegistry)
+               124 PRECALL                  0
+               128 CALL                     0
+               138 STORE_NAME              17 (converter_registry)
+   
+    34         140 LOAD_NAME               17 (converter_registry)
+               142 LOAD_ATTR               18 (register)
+   
+    35         152 LOAD_CONST              10 ('value')
+               154 LOAD_NAME               19 (str)
+               156 LOAD_CONST              11 ('return')
+               158 LOAD_NAME                6 (Union)
+               160 LOAD_NAME                9 (PhoneNumber)
+               162 LOAD_NAME               19 (str)
+               164 BUILD_TUPLE              2
+               166 BINARY_SUBSCR
+               176 BUILD_TUPLE              4
+               178 LOAD_CONST              12 (<code object parse_phone_number, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 34>)
+               180 MAKE_FUNCTION            4 (annotations)
+   
+    34         182 PRECALL                  0
+               186 CALL                     0
+   
+    35         196 STORE_NAME              20 (parse_phone_number)
+   
+    48         198 LOAD_NAME               17 (converter_registry)
+               200 LOAD_ATTR               18 (register)
+   
+    49         210 LOAD_CONST              10 ('value')
+               212 LOAD_NAME               19 (str)
+               214 LOAD_CONST              11 ('return')
+               216 LOAD_NAME               19 (str)
+               218 BUILD_TUPLE              4
+               220 LOAD_CONST              13 (<code object parse_sex, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 48>)
+               222 MAKE_FUNCTION            4 (annotations)
+   
+    48         224 PRECALL                  0
+               228 CALL                     0
+   
+    49         238 STORE_NAME              21 (parse_sex)
+   
+    58         240 LOAD_NAME               17 (converter_registry)
+               242 LOAD_ATTR               18 (register)
+   
+    59         252 LOAD_CONST              10 ('value')
+               254 LOAD_NAME               19 (str)
+               256 LOAD_CONST              11 ('return')
+               258 LOAD_NAME                6 (Union)
+               260 LOAD_NAME                1 (date)
+               262 LOAD_CONST               3 (None)
+               264 BUILD_TUPLE              2
+               266 BINARY_SUBSCR
+               276 BUILD_TUPLE              4
+               278 LOAD_CONST              14 (<code object parse_date, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 58>)
+               280 MAKE_FUNCTION            4 (annotations)
+   
+    58         282 PRECALL                  0
+               286 CALL                     0
+   
+    59         296 STORE_NAME              22 (parse_date)
+   
+    69         298 LOAD_NAME               17 (converter_registry)
+               300 LOAD_ATTR               18 (register)
+   
+    70         310 LOAD_CONST              10 ('value')
+               312 LOAD_NAME               19 (str)
+               314 LOAD_CONST              11 ('return')
+               316 LOAD_NAME                5 (Sequence)
+               318 LOAD_NAME               19 (str)
+               320 BINARY_SUBSCR
+               330 BUILD_TUPLE              4
+               332 LOAD_CONST              15 (<code object parse_comma_separated_data, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 69>)
+               334 MAKE_FUNCTION            4 (annotations)
+   
+    69         336 PRECALL                  0
+               340 CALL                     0
+   
+    70         350 STORE_NAME              23 (parse_comma_separated_data)
+   
+    75         352 LOAD_CONST              16 (('capitalize', 'lstrip', 'strip', 'rstrip', 'lower', 'upper', 'title'))
+               354 GET_ITER
+           >>  356 FOR_ITER                33 (to 424)
+               358 STORE_NAME              24 (str_converter)
+   
+    76         360 LOAD_NAME               17 (converter_registry)
+               362 LOAD_METHOD             18 (register)
+               384 PUSH_NULL
+               386 LOAD_NAME               25 (getattr)
+               388 LOAD_NAME               19 (str)
+               390 LOAD_NAME               24 (str_converter)
+               392 PRECALL                  2
+               396 CALL                     2
+               406 PRECALL                  1
+               410 CALL                     1
+               420 POP_TOP
+               422 JUMP_BACKWARD           34 (to 356)
    
-    75     >>  428 LOAD_CONST              14 (None)
-               430 RETURN_VALUE
+    75     >>  424 LOAD_CONST               3 (None)
+               426 RETURN_VALUE
    consts
       0
       ('date',)
       ('Any', 'Callable', 'Sequence', 'Union')
+      None
       ('PhoneNumber',)
       ('NumberParseException',)
       ('SEXES',)
-      ('settings',)
       ('get_site_preferences',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
@@ -368,207 +366,207 @@
          lnotab 0x0a01040206033408
       'ConverterRegistry'
       'value'
       'return'
       code
          argcount  : 1
          nlocals   : 2
-         stacksize : 4
+         stacksize : 5
          flags     : 3
          code
             0x970009007401000000000000000000006a0100000000000000007c0074
-            04000000000000000000006a030000000000000000a6020000ab02000000
-            00000000007d017c01a00400000000000000000000000000000000000000
-            00a6000000ab00000000000000000072027c0153006e102300740a000000
-            0000000000000024007203010059006e04770078035900770164015300
+            0500000000000000000000a6000000ab0000000000000000006401190000
+            00000000000000a6020000ab0200000000000000007d017c01a003000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            0072027c0153006e10230074080000000000000000000024007203010059
+            006e04770078035900770164025300
           34           0 RESUME                   0
          
           37           2 NOP
          
           38           4 LOAD_GLOBAL              1 (NULL + PhoneNumber)
                       16 LOAD_ATTR                1 (from_string)
-                      26 LOAD_FAST                0 (value)
-                      28 LOAD_GLOBAL              4 (settings)
-                      40 LOAD_ATTR                3 (PHONENUMBER_DEFAULT_REGION)
-                      50 PRECALL                  2
-                      54 CALL                     2
-                      64 STORE_FAST               1 (number)
-         
-          39          66 LOAD_FAST                1 (number)
-                      68 LOAD_METHOD              4 (is_valid)
-                      90 PRECALL                  0
-                      94 CALL                     0
-                     104 POP_JUMP_FORWARD_IF_FALSE     2 (to 110)
-         
-          40         106 LOAD_FAST                1 (number)
-                     108 RETURN_VALUE
          
-          39     >>  110 JUMP_FORWARD            16 (to 144)
-                 >>  112 PUSH_EXC_INFO
+          39          26 LOAD_FAST                0 (value)
+                      28 LOAD_GLOBAL              5 (NULL + get_site_preferences)
+                      40 PRECALL                  0
+                      44 CALL                     0
+                      54 LOAD_CONST               1 ('internationalisation__phone_number_country')
+                      56 BINARY_SUBSCR
+         
+          38          66 PRECALL                  2
+                      70 CALL                     2
+                      80 STORE_FAST               1 (number)
+         
+          41          82 LOAD_FAST                1 (number)
+                      84 LOAD_METHOD              3 (is_valid)
+                     106 PRECALL                  0
+                     110 CALL                     0
+                     120 POP_JUMP_FORWARD_IF_FALSE     2 (to 126)
+         
+          42         122 LOAD_FAST                1 (number)
+                     124 RETURN_VALUE
+         
+          41     >>  126 JUMP_FORWARD            16 (to 160)
+                 >>  128 PUSH_EXC_INFO
+         
+          43         130 LOAD_GLOBAL              8 (NumberParseException)
+                     142 CHECK_EXC_MATCH
+                     144 POP_JUMP_FORWARD_IF_FALSE     3 (to 152)
+                     146 POP_TOP
+         
+          44         148 POP_EXCEPT
+                     150 JUMP_FORWARD             4 (to 160)
+         
+          43     >>  152 RERAISE                  0
+                 >>  154 COPY                     3
+                     156 POP_EXCEPT
+                     158 RERAISE                  1
          
-          41         114 LOAD_GLOBAL             10 (NumberParseException)
-                     126 CHECK_EXC_MATCH
-                     128 POP_JUMP_FORWARD_IF_FALSE     3 (to 136)
-                     130 POP_TOP
-         
-          42         132 POP_EXCEPT
-                     134 JUMP_FORWARD             4 (to 144)
-         
-          41     >>  136 RERAISE                  0
-                 >>  138 COPY                     3
-                     140 POP_EXCEPT
-                     142 RERAISE                  1
-         
-          43     >>  144 LOAD_CONST               1 ('')
-                     146 RETURN_VALUE
+          45     >>  160 LOAD_CONST               2 ('')
+                     162 RETURN_VALUE
          ExceptionTable:
-           4 to 106 -> 112 [0]
-           112 to 130 -> 138 [1] lasti
-           136 to 136 -> 138 [1] lasti
+           4 to 122 -> 128 [0]
+           128 to 146 -> 154 [1] lasti
+           152 to 152 -> 154 [1] lasti
          consts
             'Parse a phone number.'
+            'internationalisation__phone_number_country'
             ''
-         names      ('PhoneNumber', 'from_string', 'settings', 'PHONENUMBER_DEFAULT_REGION', 'is_valid', 'NumberParseException')
+         names      ('PhoneNumber', 'from_string', 'get_site_preferences', 'is_valid', 'NumberParseException')
          varnames   ('value', 'number')
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'parse_phone_number'
          firstlineno 34
-         lnotab 0x020302013e01280104ff0402120104ff0802
+         lnotab 0x02030201160128ff1003280104ff0402120104ff0802
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code
             0x97007c00a0000000000000000000000000000000000000000000a60000
             00ab0000000000000000007d007c00740200000000000000000000760072
             0d7402000000000000000000007c00190000000000000000005300640153
             00
-          46           0 RESUME                   0
+          48           0 RESUME                   0
          
-          49           2 LOAD_FAST                0 (value)
+          51           2 LOAD_FAST                0 (value)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               0 (value)
          
-          50          42 LOAD_FAST                0 (value)
+          52          42 LOAD_FAST                0 (value)
                       44 LOAD_GLOBAL              2 (SEXES)
                       56 CONTAINS_OP              0
                       58 POP_JUMP_FORWARD_IF_FALSE    13 (to 86)
          
-          51          60 LOAD_GLOBAL              2 (SEXES)
+          53          60 LOAD_GLOBAL              2 (SEXES)
                       72 LOAD_FAST                0 (value)
                       74 BINARY_SUBSCR
                       84 RETURN_VALUE
          
-          53     >>   86 LOAD_CONST               1 ('')
+          55     >>   86 LOAD_CONST               1 ('')
                       88 RETURN_VALUE
          consts
             'Parse sex via SEXES dictionary.'
             ''
          names      ('lower', 'SEXES')
          varnames   ('value',)
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'parse_sex'
-         firstlineno 46
+         firstlineno 48
          lnotab 0x0203280112011a02
-      None
       code
          argcount  : 1
-         nlocals   : 4
+         nlocals   : 3
          stacksize : 4
          flags     : 3
          code
-            0x9700640164026c007d01740300000000000000000000a6000000ab0000
-            000000000000006403190000000000000000007d027c0272157c02a00200
-            000000000000000000000000000000000000006404a6010000ab01000000
-            00000000006e0167007d0309007c01a00300000000000000000000000000
-            000000000000007c007c03ac05a6020000ab020000000000000000a00400
-            00000000000000000000000000000000000000a6000000ab000000000000
-            00000053002300740a00000000000000000000740c000000000000000000
-            0066022400720401005900640253007700780359007701
-          56           0 RESUME                   0
-         
-          59           2 LOAD_CONST               1 (0)
-                       4 LOAD_CONST               2 (None)
-                       6 IMPORT_NAME              0 (dateparser)
-                       8 STORE_FAST               1 (dateparser)
-         
-          61          10 LOAD_GLOBAL              3 (NULL + get_site_preferences)
-                      22 PRECALL                  0
-                      26 CALL                     0
-                      36 LOAD_CONST               3 ('csv_import__date_languages')
-                      38 BINARY_SUBSCR
-                      48 STORE_FAST               2 (languages_raw)
-         
-          62          50 LOAD_FAST                2 (languages_raw)
-                      52 POP_JUMP_FORWARD_IF_FALSE    21 (to 96)
-                      54 LOAD_FAST                2 (languages_raw)
-                      56 LOAD_METHOD              2 (split)
-                      78 LOAD_CONST               4 (',')
-                      80 PRECALL                  1
-                      84 CALL                     1
-                      94 JUMP_FORWARD             1 (to 98)
-                 >>   96 BUILD_LIST               0
-                 >>   98 STORE_FAST               3 (languages)
-         
-          63         100 NOP
-         
-          64         102 LOAD_FAST                1 (dateparser)
-                     104 LOAD_METHOD              3 (parse)
-                     126 LOAD_FAST                0 (value)
-                     128 LOAD_FAST                3 (languages)
-                     130 KW_NAMES                 5
-                     132 PRECALL                  2
-                     136 CALL                     2
-                     146 LOAD_METHOD              4 (date)
-                     168 PRECALL                  0
-                     172 CALL                     0
-                     182 RETURN_VALUE
-                 >>  184 PUSH_EXC_INFO
-         
-          65         186 LOAD_GLOBAL             10 (ValueError)
-                     198 LOAD_GLOBAL             12 (AttributeError)
-                     210 BUILD_TUPLE              2
-                     212 CHECK_EXC_MATCH
-                     214 POP_JUMP_FORWARD_IF_FALSE     4 (to 224)
-                     216 POP_TOP
-         
-          66         218 POP_EXCEPT
-                     220 LOAD_CONST               2 (None)
-                     222 RETURN_VALUE
-         
-          65     >>  224 RERAISE                  0
-                 >>  226 COPY                     3
-                     228 POP_EXCEPT
-                     230 RERAISE                  1
+            0x9700740100000000000000000000a6000000ab00000000000000000064
+            01190000000000000000007d017c0172157c01a001000000000000000000
+            00000000000000000000006402a6010000ab0100000000000000006e0167
+            007d0209007405000000000000000000006a0300000000000000007c007c
+            02ac03a6020000ab020000000000000000a0040000000000000000000000
+            000000000000000000a6000000ab00000000000000000053002300740a00
+            000000000000000000740c00000000000000000000660224007204010059
+            00640453007700780359007701
+          58           0 RESUME                   0
+         
+          61           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
+                      14 PRECALL                  0
+                      18 CALL                     0
+                      28 LOAD_CONST               1 ('csv_import__date_languages')
+                      30 BINARY_SUBSCR
+                      40 STORE_FAST               1 (languages_raw)
+         
+          62          42 LOAD_FAST                1 (languages_raw)
+                      44 POP_JUMP_FORWARD_IF_FALSE    21 (to 88)
+                      46 LOAD_FAST                1 (languages_raw)
+                      48 LOAD_METHOD              1 (split)
+                      70 LOAD_CONST               2 (',')
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 JUMP_FORWARD             1 (to 90)
+                 >>   88 BUILD_LIST               0
+                 >>   90 STORE_FAST               2 (languages)
+         
+          63          92 NOP
+         
+          64          94 LOAD_GLOBAL              5 (NULL + dateparser)
+                     106 LOAD_ATTR                3 (parse)
+                     116 LOAD_FAST                0 (value)
+                     118 LOAD_FAST                2 (languages)
+                     120 KW_NAMES                 3
+                     122 PRECALL                  2
+                     126 CALL                     2
+                     136 LOAD_METHOD              4 (date)
+                     158 PRECALL                  0
+                     162 CALL                     0
+                     172 RETURN_VALUE
+                 >>  174 PUSH_EXC_INFO
+         
+          65         176 LOAD_GLOBAL             10 (ValueError)
+                     188 LOAD_GLOBAL             12 (AttributeError)
+                     200 BUILD_TUPLE              2
+                     202 CHECK_EXC_MATCH
+                     204 POP_JUMP_FORWARD_IF_FALSE     4 (to 214)
+                     206 POP_TOP
+         
+          66         208 POP_EXCEPT
+                     210 LOAD_CONST               4 (None)
+                     212 RETURN_VALUE
+         
+          65     >>  214 RERAISE                  0
+                 >>  216 COPY                     3
+                     218 POP_EXCEPT
+                     220 RERAISE                  1
          ExceptionTable:
-           102 to 180 -> 184 [0]
-           184 to 216 -> 226 [1] lasti
-           224 to 224 -> 226 [1] lasti
+           94 to 170 -> 174 [0]
+           174 to 206 -> 216 [1] lasti
+           214 to 214 -> 216 [1] lasti
          consts
             'Parse string date.'
-            0
-            None
             'csv_import__date_languages'
             ','
             ('languages',)
-         names      ('dateparser', 'get_site_preferences', 'split', 'parse', 'date', 'ValueError', 'AttributeError')
-         varnames   ('value', 'dateparser', 'languages_raw', 'languages')
+            None
+         names      ('get_site_preferences', 'split', 'dateparser', 'parse', 'date', 'ValueError', 'AttributeError')
+         varnames   ('value', 'languages_raw', 'languages')
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'parse_date'
-         firstlineno 56
-         lnotab 0x020308022801320102015401200106ff
+         firstlineno 58
+         lnotab 0x02032801320102015201200106ff
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 8
          flags     : 3
          code
             0x9700740100000000000000000000740300000000000000000000640184
@@ -618,17 +616,17 @@
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'parse_comma_separated_data'
          firstlineno 69
          lnotab 0x0203
       ('capitalize', 'lstrip', 'strip', 'rstrip', 'lower', 'upper', 'title')
-   names      ('datetime', 'date', 'typing', 'Any', 'Callable', 'Sequence', 'Union', 'phonenumber_field.phonenumber', 'PhoneNumber', 'phonenumbers', 'NumberParseException', 'aleksis.apps.csv_import.settings', 'SEXES', 'aleksis.core', 'settings', 'aleksis.core.util.core_helpers', 'get_site_preferences', 'ConverterRegistry', 'converter_registry', 'register', 'str', 'parse_phone_number', 'parse_sex', 'parse_date', 'parse_comma_separated_data', 'str_converter', 'getattr')
+   names      ('datetime', 'date', 'typing', 'Any', 'Callable', 'Sequence', 'Union', 'dateparser', 'phonenumber_field.phonenumber', 'PhoneNumber', 'phonenumbers', 'NumberParseException', 'aleksis.apps.csv_import.settings', 'SEXES', 'aleksis.core.util.core_helpers', 'get_site_preferences', 'ConverterRegistry', 'converter_registry', 'register', 'str', 'parse_phone_number', 'parse_sex', 'parse_date', 'parse_comma_separated_data', 'str_converter', 'getattr')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0118020c010c020c010c010c031a1314030c011eff0e0102
-      0b0c010eff0e0102090c011eff0e01020c0c011aff0e010205080140ff
+      0x00ff02010c01180208010c010c020c010c031a1314030c011eff0e0102
+      0d0c010eff0e0102090c011eff0e01020a0c011aff0e010205080140ff
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/__pycache__/import_helpers.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/import_helpers.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2587b964 (Thu Jul 20 19:12:37 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 359
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/class_range_helpers.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/class_range_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/converters.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/converters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import date
 from typing import Any, Callable, Sequence, Union
 
+import dateparser
 from phonenumber_field.phonenumber import PhoneNumber
 from phonenumbers import NumberParseException
 
 from aleksis.apps.csv_import.settings import SEXES
-from aleksis.core import settings
 from aleksis.core.util.core_helpers import get_site_preferences
 
 
 class ConverterRegistry:
     """Registry of known conversion functions."""
 
     def __init__(self):
@@ -31,15 +31,17 @@
 converter_registry = ConverterRegistry()
 
 
 @converter_registry.register
 def parse_phone_number(value: str) -> Union[PhoneNumber, str]:
     """Parse a phone number."""
     try:
-        number = PhoneNumber.from_string(value, settings.PHONENUMBER_DEFAULT_REGION)
+        number = PhoneNumber.from_string(
+            value, get_site_preferences()["internationalisation__phone_number_country"]
+        )
         if number.is_valid():
             return number
     except NumberParseException:
         pass
     return ""
 
 
@@ -52,16 +54,14 @@
 
     return ""
 
 
 @converter_registry.register
 def parse_date(value: str) -> Union[date, None]:
     """Parse string date."""
-    import dateparser  # noqa
-
     languages_raw = get_site_preferences()["csv_import__date_languages"]
     languages = languages_raw.split(",") if languages_raw else []
     try:
         return dateparser.parse(value, languages=languages).date()
     except (ValueError, AttributeError):
         return None
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/util/process.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,18 @@
                     # Set group type for imported groups if defined in template globally
                     if template.group_type and model == Group:
                         update_dict["group_type"] = template.group_type
 
                     # Determine available fields for finding existing instances
                     get_dict = {}
                     match_field_priority = 0
-                    for column_name, field_type in sorted(
+                    for (
+                        column_name,
+                        field_type,
+                    ) in sorted(
                         filter(lambda f: isinstance(f[1], MatchFieldType), field_types.items()),
                         key=lambda f: f[1].priority,
                     ):
                         if match_field_priority and match_field_priority < field_type.priority:
                             # We found a match field, but with less important priority than
                             # those before, so we write data from the field
                             update_dict[field_type.get_db_field()] = row[column_name]
```

### Comparing `aleksis_app_csvimport-3.0.1/aleksis/apps/csv_import/views.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/docs/Makefile` & `aleksis_app_csvimport-3.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/docs/admin/01_concept.rst` & `aleksis_app_csvimport-3.0b0/docs/admin/01_concept.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/docs/admin/05_configuration.rst` & `aleksis_app_csvimport-3.0b0/docs/admin/05_configuration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/docs/admin/10_exporting_data.rst` & `aleksis_app_csvimport-3.0b0/docs/admin/10_exporting_data.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/docs/admin/20_import_data.rst` & `aleksis_app_csvimport-3.0b0/docs/admin/20_import_data.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/docs/conf.py` & `aleksis_app_csvimport-3.0b0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-CSVImport"
 copyright = "2018-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0.1"
+release = "3.0b0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_app_csvimport-3.0.1/docs/index.rst` & `aleksis_app_csvimport-3.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/docs/make.bat` & `aleksis_app_csvimport-3.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/tox.ini` & `aleksis_app_csvimport-3.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0.1/PKG-INFO` & `aleksis_app_csvimport-3.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: aleksis-app-csvimport
-Version: 3.0.1
+Version: 3.0b0
 Summary: AlekSIS (School Information System) — App for CSV import
-Home-page: https://aleksis.org
-License: EUPL-1.2-or-later
+Home-page: https://aleksis.org/
+License: EUPL-1.2
 Author: Dominik George
 Author-email: dominik.george@teckids.org
-Maintainer: Jonathan Weth
-Maintainer-email: dev@jonathanweth.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=3.0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Requires-Dist: chardet (>=5.0.0,<6.0.0)
 Requires-Dist: dateparser (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
 Requires-Dist: phonenumbers (>=8.10,<9.0)
 Requires-Dist: ruamel.yaml (>=0.17.19,<0.18.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Documentation, https://aleksis.edugit.io/AlekSIS/docs/html/
```

