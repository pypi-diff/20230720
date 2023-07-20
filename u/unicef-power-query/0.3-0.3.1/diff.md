# Comparing `tmp/unicef-power-query-0.3.tar.gz` & `tmp/unicef-power-query-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicef-power-query-0.3.tar", last modified: Wed Jul 19 07:39:20 2023, max compression
+gzip compressed data, was "unicef-power-query-0.3.1.tar", last modified: Thu Jul 20 09:46:13 2023, max compression
```

## Comparing `unicef-power-query-0.3.tar` & `unicef-power-query-0.3.1.tar`

### file list

```diff
@@ -1,191 +1,195 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.226723 unicef-power-query-0.3/
--rw-r--r--   0 jojo       (501) staff       (20)      289 2023-07-19 07:39:05.000000 unicef-power-query-0.3/CHANGES
--rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:28:14.000000 unicef-power-query-0.3/LICENSE
--rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-power-query-0.3/MANIFEST.in
--rw-r--r--   0 jojo       (501) staff       (20)      527 2023-07-19 07:39:20.226942 unicef-power-query-0.3/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     2190 2023-07-04 08:17:12.000000 unicef-power-query-0.3/README.rst
--rw-r--r--   0 jojo       (501) staff       (20)       82 2023-07-19 07:39:20.227660 unicef-power-query-0.3/setup.cfg
--rwxr-xr-x   0 jojo       (501) staff       (20)     1852 2023-07-04 08:17:12.000000 unicef-power-query-0.3/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.040243 unicef-power-query-0.3/src/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.069692 unicef-power-query-0.3/src/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)       58 2023-07-19 07:39:05.000000 unicef-power-query-0.3/src/power_query/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.104759 unicef-power-query-0.3/src/power_query/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      248 2023-07-18 14:47:17.000000 unicef-power-query-0.3/src/power_query/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      223 2023-07-18 09:30:04.000000 unicef-power-query-0.3/src/power_query/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    27954 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    15713 2023-07-13 10:19:49.000000 unicef-power-query-0.3/src/power_query/__pycache__/admin.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      522 2023-07-18 14:47:17.000000 unicef-power-query-0.3/src/power_query/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      411 2023-07-13 10:19:44.000000 unicef-power-query-0.3/src/power_query/__pycache__/apps.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     6185 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/__pycache__/celery_tasks.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     3741 2023-07-13 10:19:49.000000 unicef-power-query-0.3/src/power_query/__pycache__/celery_tasks.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1105 2023-07-13 12:04:32.000000 unicef-power-query-0.3/src/power_query/__pycache__/defaults.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1161 2023-07-18 14:47:17.000000 unicef-power-query-0.3/src/power_query/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      816 2023-07-13 10:19:47.000000 unicef-power-query-0.3/src/power_query/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     6621 2023-07-18 09:30:08.000000 unicef-power-query-0.3/src/power_query/__pycache__/fixtures.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2347 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1494 2023-07-13 10:19:49.000000 unicef-power-query-0.3/src/power_query/__pycache__/forms.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1519 2023-07-18 14:47:17.000000 unicef-power-query-0.3/src/power_query/__pycache__/json.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      947 2023-07-13 10:19:47.000000 unicef-power-query-0.3/src/power_query/__pycache__/json.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1130 2023-07-13 10:19:49.000000 unicef-power-query-0.3/src/power_query/__pycache__/mixin.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    29741 2023-07-18 14:47:17.000000 unicef-power-query-0.3/src/power_query/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    16511 2023-07-13 10:19:47.000000 unicef-power-query-0.3/src/power_query/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      713 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      508 2023-07-13 10:20:35.000000 unicef-power-query-0.3/src/power_query/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     9981 2023-07-18 14:47:17.000000 unicef-power-query-0.3/src/power_query/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     5157 2023-07-13 10:19:47.000000 unicef-power-query-0.3/src/power_query/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1213 2023-07-18 14:47:17.000000 unicef-power-query-0.3/src/power_query/__pycache__/validators.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      840 2023-07-13 10:19:47.000000 unicef-power-query-0.3/src/power_query/__pycache__/validators.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     5028 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2800 2023-07-13 10:20:35.000000 unicef-power-query-0.3/src/power_query/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     5600 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/__pycache__/widget.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     3645 2023-07-13 10:19:49.000000 unicef-power-query-0.3/src/power_query/__pycache__/widget.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    16001 2023-07-13 09:21:20.000000 unicef-power-query-0.3/src/power_query/admin.py
--rw-r--r--   0 jojo       (501) staff       (20)      119 2023-07-13 07:16:39.000000 unicef-power-query-0.3/src/power_query/apps.py
--rw-r--r--   0 jojo       (501) staff       (20)     3009 2023-07-13 07:25:13.000000 unicef-power-query-0.3/src/power_query/celery_tasks.py
--rw-r--r--   0 jojo       (501) staff       (20)     1051 2023-07-13 07:22:15.000000 unicef-power-query-0.3/src/power_query/defaults.py
--rw-r--r--   0 jojo       (501) staff       (20)      404 2023-07-13 07:14:46.000000 unicef-power-query-0.3/src/power_query/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)     4351 2023-07-18 09:06:00.000000 unicef-power-query-0.3/src/power_query/fixtures.py
--rw-r--r--   0 jojo       (501) staff       (20)     1438 2023-07-13 07:24:44.000000 unicef-power-query-0.3/src/power_query/forms.py
--rw-r--r--   0 jojo       (501) staff       (20)      572 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/json.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.106537 unicef-power-query-0.3/src/power_query/management/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/management/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.107098 unicef-power-query-0.3/src/power_query/management/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:07.000000 unicef-power-query-0.3/src/power_query/management/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.110463 unicef-power-query-0.3/src/power_query/management/commands/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/management/commands/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     3595 2023-07-13 07:17:04.000000 unicef-power-query-0.3/src/power_query/management/commands/pq.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.114807 unicef-power-query-0.3/src/power_query/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)    15211 2023-07-18 09:06:00.000000 unicef-power-query-0.3/src/power_query/migrations/0001_migration_squashed_0014_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)     1003 2023-07-18 14:51:26.000000 unicef-power-query-0.3/src/power_query/migrations/0015_alter_dataset_description_and_more.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/migrations/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.120652 unicef-power-query-0.3/src/power_query/migrations/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)    10802 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     5436 2023-07-18 09:30:10.000000 unicef-power-query-0.3/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      923 2023-07-18 14:48:37.000000 unicef-power-query-0.3/src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      188 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:08.000000 unicef-power-query-0.3/src/power_query/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      753 2023-07-13 07:18:11.000000 unicef-power-query-0.3/src/power_query/mixin.py
--rw-r--r--   0 jojo       (501) staff       (20)    17447 2023-07-19 07:39:05.000000 unicef-power-query-0.3/src/power_query/models.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/notify.py
--rw-r--r--   0 jojo       (501) staff       (20)       91 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/signals.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.124891 unicef-power-query-0.3/src/power_query/static/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.034094 unicef-power-query-0.3/src/power_query/static/admin/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.128897 unicef-power-query-0.3/src/power_query/static/admin/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)     3628 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/code.css
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.151426 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/
--rw-r--r--   0 jojo       (501) staff       (20)     1969 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/abcdef.css
--rw-r--r--   0 jojo       (501) staff       (20)     2507 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/active-line.js
--rw-r--r--   0 jojo       (501) staff       (20)     8706 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/codemirror.css
--rw-r--r--   0 jojo       (501) staff       (20)   400161 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/codemirror.js
--rw-r--r--   0 jojo       (501) staff       (20)    11792 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/django.js
--rw-r--r--   0 jojo       (501) staff       (20)     4983 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/foldcode.js
--rw-r--r--   0 jojo       (501) staff       (20)      435 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/foldgutter.css
--rw-r--r--   0 jojo       (501) staff       (20)     5368 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/foldgutter.js
--rw-r--r--   0 jojo       (501) staff       (20)      118 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/fullscreen.css
--rw-r--r--   0 jojo       (501) staff       (20)     1495 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/fullscreen.js
--rw-r--r--   0 jojo       (501) staff       (20)     1674 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/indent-fold.js
--rw-r--r--   0 jojo       (501) staff       (20)     6816 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/matchbrackets.js
--rw-r--r--   0 jojo       (501) staff       (20)     1856 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/midnight.css
--rw-r--r--   0 jojo       (501) staff       (20)     3241 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/overlay.js
--rw-r--r--   0 jojo       (501) staff       (20)    14924 2023-05-08 13:33:06.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/python.js
--rw-r--r--   0 jojo       (501) staff       (20)    13351 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/xml.js
--rw-r--r--   0 jojo       (501) staff       (20)     3733 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/yaml.js
--rw-r--r--   0 jojo       (501) staff       (20)     5122 2023-07-04 08:17:12.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/colorful.css
--rw-r--r--   0 jojo       (501) staff       (20)      760 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/diff.css
--rw-r--r--   0 jojo       (501) staff       (20)    16556 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/admin/power_query/editor.png
--rw-r--r--   0 jojo       (501) staff       (20)      292 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/power_query.css
--rw-r--r--   0 jojo       (501) staff       (20)      204 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/power_query.css.map
--rw-r--r--   0 jojo       (501) staff       (20)      355 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/power_query.scss
--rw-r--r--   0 jojo       (501) staff       (20)     6742 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/redo.png
--rw-r--r--   0 jojo       (501) staff       (20)     6554 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/static/undo.png
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.038384 unicef-power-query-0.3/src/power_query/templates/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.036022 unicef-power-query-0.3/src/power_query/templates/admin/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.037967 unicef-power-query-0.3/src/power_query/templates/admin/power_query/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.156592 unicef-power-query-0.3/src/power_query/templates/admin/power_query/dataset/
--rw-r--r--   0 jojo       (501) staff       (20)      109 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/dataset/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/dataset/export.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.169316 unicef-power-query-0.3/src/power_query/templates/admin/power_query/formatter/
--rw-r--r--   0 jojo       (501) staff       (20)     2750 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/formatter/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/formatter/change_list.html
--rw-r--r--   0 jojo       (501) staff       (20)      489 2023-07-13 07:30:38.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/formatter/test.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.172466 unicef-power-query-0.3/src/power_query/templates/admin/power_query/query/
--rw-r--r--   0 jojo       (501) staff       (20)      407 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/query/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/query/export.html
--rw-r--r--   0 jojo       (501) staff       (20)      822 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/query/monitor.html
--rw-r--r--   0 jojo       (501) staff       (20)     2003 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/query/preview.html
--rw-r--r--   0 jojo       (501) staff       (20)      490 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/query/run_result.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.173844 unicef-power-query-0.3/src/power_query/templates/admin/power_query/queryargs/
--rw-r--r--   0 jojo       (501) staff       (20)     1559 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/queryargs/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      479 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/queryargs/preview.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.175081 unicef-power-query-0.3/src/power_query/templates/admin/power_query/report/
--rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/report/change_list.html
--rw-r--r--   0 jojo       (501) staff       (20)      743 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/admin/power_query/report/monitor.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.177270 unicef-power-query-0.3/src/power_query/templates/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)      532 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/power_query/base.html
--rw-r--r--   0 jojo       (501) staff       (20)      762 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/power_query/detail.html
--rw-r--r--   0 jojo       (501) staff       (20)      339 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/power_query/list.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.178286 unicef-power-query-0.3/src/power_query/templates/power_query/widgets/
--rw-r--r--   0 jojo       (501) staff       (20)     1235 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templates/power_query/widgets/codewidget.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.179684 unicef-power-query-0.3/src/power_query/templatetags/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3/src/power_query/templatetags/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.183608 unicef-power-query-0.3/src/power_query/templatetags/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      190 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      172 2023-07-13 10:20:43.000000 unicef-power-query-0.3/src/power_query/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2150 2023-07-18 14:47:18.000000 unicef-power-query-0.3/src/power_query/templatetags/__pycache__/power_query.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1295 2023-07-13 10:20:43.000000 unicef-power-query-0.3/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      814 2023-07-13 07:18:11.000000 unicef-power-query-0.3/src/power_query/templatetags/power_query.py
--rw-r--r--   0 jojo       (501) staff       (20)      368 2023-07-13 07:19:25.000000 unicef-power-query-0.3/src/power_query/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)     5041 2023-07-13 07:19:03.000000 unicef-power-query-0.3/src/power_query/utils.py
--rw-r--r--   0 jojo       (501) staff       (20)      453 2023-07-13 07:17:09.000000 unicef-power-query-0.3/src/power_query/validators.py
--rw-r--r--   0 jojo       (501) staff       (20)     3360 2023-07-13 09:21:39.000000 unicef-power-query-0.3/src/power_query/views.py
--rw-r--r--   0 jojo       (501) staff       (20)     3111 2023-07-13 07:15:15.000000 unicef-power-query-0.3/src/power_query/widget.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.195334 unicef-power-query-0.3/src/unicef_power_query.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      527 2023-07-19 07:39:19.000000 unicef-power-query-0.3/src/unicef_power_query.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     7505 2023-07-19 07:39:20.000000 unicef-power-query-0.3/src/unicef_power_query.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-19 07:39:19.000000 unicef-power-query-0.3/src/unicef_power_query.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)      319 2023-07-19 07:39:19.000000 unicef-power-query-0.3/src/unicef_power_query.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       12 2023-07-19 07:39:19.000000 unicef-power-query-0.3/src/unicef_power_query.egg-info/top_level.txt
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.205270 unicef-power-query-0.3/tests/
--rw-r--r--   0 jojo       (501) staff       (20)      214 2023-05-16 13:30:33.000000 unicef-power-query-0.3/tests/.coveragerc
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3/tests/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.210927 unicef-power-query-0.3/tests/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)    36910 2023-06-12 09:22:39.000000 unicef-power-query-0.3/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     3607 2023-06-12 07:29:10.000000 unicef-power-query-0.3/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     7475 2023-06-12 07:29:10.000000 unicef-power-query-0.3/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1408 2023-06-12 07:29:10.000000 unicef-power-query-0.3/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     4525 2023-06-12 07:29:10.000000 unicef-power-query-0.3/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1502 2023-06-12 07:29:10.000000 unicef-power-query-0.3/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    11905 2023-05-16 12:47:07.000000 unicef-power-query-0.3/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.214973 unicef-power-query-0.3/tests/demoproject/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-02 15:31:56.000000 unicef-power-query-0.3/tests/demoproject/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)   278528 2023-05-31 15:10:33.000000 unicef-power-query-0.3/tests/demoproject/db.sqlite3
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.219400 unicef-power-query-0.3/tests/demoproject/demo/
--rw-r--r--   0 jojo       (501) staff       (20)       65 2023-07-04 08:17:12.000000 unicef-power-query-0.3/tests/demoproject/demo/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.223704 unicef-power-query-0.3/tests/demoproject/demo/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      267 2023-07-18 14:47:16.000000 unicef-power-query-0.3/tests/demoproject/demo/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      691 2023-07-18 14:47:16.000000 unicef-power-query-0.3/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      738 2023-05-16 12:44:40.000000 unicef-power-query-0.3/tests/demoproject/demo/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2690 2023-07-18 14:47:16.000000 unicef-power-query-0.3/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      525 2023-05-31 11:57:14.000000 unicef-power-query-0.3/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      699 2023-05-16 13:01:06.000000 unicef-power-query-0.3/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      245 2023-07-04 08:17:12.000000 unicef-power-query-0.3/tests/demoproject/demo/celery.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.225031 unicef-power-query-0.3/tests/demoproject/demo/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-power-query-0.3/tests/demoproject/demo/migrations/0001_initial.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-power-query-0.3/tests/demoproject/demo/migrations/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-19 07:39:20.226023 unicef-power-query-0.3/tests/demoproject/demo/migrations/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)     3923 2023-05-16 13:01:06.000000 unicef-power-query-0.3/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      195 2023-05-16 13:01:06.000000 unicef-power-query-0.3/tests/demoproject/demo/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      142 2023-05-16 12:43:15.000000 unicef-power-query-0.3/tests/demoproject/demo/models.py
--rw-r--r--   0 jojo       (501) staff       (20)     2590 2023-07-04 08:17:12.000000 unicef-power-query-0.3/tests/demoproject/demo/settings.py
--rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-16 14:04:29.000000 unicef-power-query-0.3/tests/demoproject/demo/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-power-query-0.3/tests/demoproject/demo/wsgi.py
--rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-power-query-0.3/tests/demoproject/factories.py
--rwxr-xr-x   0 jojo       (501) staff       (20)      246 2023-07-04 08:17:12.000000 unicef-power-query-0.3/tests/demoproject/manage.py
--rw-r--r--   0 jojo       (501) staff       (20)    10380 2023-07-18 09:06:00.000000 unicef-power-query-0.3/tests/test_admin.py
--rw-r--r--   0 jojo       (501) staff       (20)     1719 2023-07-18 09:06:00.000000 unicef-power-query-0.3/tests/test_auth.py
--rw-r--r--   0 jojo       (501) staff       (20)     2097 2023-07-18 09:06:00.000000 unicef-power-query-0.3/tests/test_celery.py
--rw-r--r--   0 jojo       (501) staff       (20)      441 2023-07-18 09:06:00.000000 unicef-power-query-0.3/tests/test_params.py
--rw-r--r--   0 jojo       (501) staff       (20)     1989 2023-07-18 09:06:00.000000 unicef-power-query-0.3/tests/test_queries.py
--rw-r--r--   0 jojo       (501) staff       (20)      829 2023-07-13 09:09:33.000000 unicef-power-query-0.3/tests/test_utils.py
--rw-r--r--   0 jojo       (501) staff       (20)     1772 2023-07-18 09:06:00.000000 unicef-power-query-0.3/tests/test_views.py
--rw-r--r--   0 jojo       (501) staff       (20)     1022 2023-07-04 08:17:12.000000 unicef-power-query-0.3/tox.ini
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.572956 unicef-power-query-0.3.1/
+-rw-r--r--   0 jojo       (501) staff       (20)      351 2023-07-20 09:45:52.000000 unicef-power-query-0.3.1/CHANGES
+-rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:28:14.000000 unicef-power-query-0.3.1/LICENSE
+-rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-power-query-0.3.1/MANIFEST.in
+-rw-r--r--   0 jojo       (501) staff       (20)      529 2023-07-20 09:46:13.573162 unicef-power-query-0.3.1/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     2190 2023-07-04 08:17:12.000000 unicef-power-query-0.3.1/README.rst
+-rw-r--r--   0 jojo       (501) staff       (20)       82 2023-07-20 09:46:13.574430 unicef-power-query-0.3.1/setup.cfg
+-rwxr-xr-x   0 jojo       (501) staff       (20)     1852 2023-07-04 08:17:12.000000 unicef-power-query-0.3.1/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.274392 unicef-power-query-0.3.1/src/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.311542 unicef-power-query-0.3.1/src/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)       60 2023-07-20 09:45:52.000000 unicef-power-query-0.3.1/src/power_query/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.365701 unicef-power-query-0.3.1/src/power_query/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      248 2023-07-19 09:25:59.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      225 2023-07-20 09:45:59.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    28562 2023-07-19 09:50:40.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    15905 2023-07-20 09:46:04.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/admin.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      522 2023-07-19 09:25:59.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      411 2023-07-20 09:12:56.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/apps.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     6185 2023-07-19 09:26:06.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/celery_tasks.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3741 2023-07-20 09:13:05.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/celery_tasks.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1565 2023-07-19 09:26:07.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/defaults.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1161 2023-07-19 09:26:00.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      816 2023-07-20 09:13:01.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    10719 2023-07-19 09:26:07.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/fixtures.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     6621 2023-07-18 09:30:08.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/fixtures.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2347 2023-07-19 09:26:06.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1494 2023-07-20 09:13:05.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/forms.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1519 2023-07-19 09:26:00.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/json.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      947 2023-07-20 09:13:01.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1130 2023-07-20 09:13:03.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/mixin.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    30343 2023-07-19 09:56:12.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    16825 2023-07-20 09:13:01.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      713 2023-07-19 09:26:22.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      508 2023-07-20 09:13:22.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     9981 2023-07-19 09:26:03.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5157 2023-07-20 09:13:01.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1213 2023-07-19 09:26:03.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/validators.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      840 2023-07-20 09:13:01.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/validators.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5028 2023-07-19 09:26:22.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2800 2023-07-20 09:13:22.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/views.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5600 2023-07-19 09:26:06.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/widget.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3619 2023-07-20 09:46:04.000000 unicef-power-query-0.3.1/src/power_query/__pycache__/widget.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    16148 2023-07-20 09:45:52.000000 unicef-power-query-0.3.1/src/power_query/admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)      119 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/apps.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3009 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/celery_tasks.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1051 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/defaults.py
+-rw-r--r--   0 jojo       (501) staff       (20)      404 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4351 2023-07-18 09:06:00.000000 unicef-power-query-0.3.1/src/power_query/fixtures.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1438 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/forms.py
+-rw-r--r--   0 jojo       (501) staff       (20)      572 2023-07-19 07:55:05.000000 unicef-power-query-0.3.1/src/power_query/json.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.368699 unicef-power-query-0.3.1/src/power_query/management/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/management/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.370479 unicef-power-query-0.3.1/src/power_query/management/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      188 2023-07-19 09:26:07.000000 unicef-power-query-0.3.1/src/power_query/management/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:07.000000 unicef-power-query-0.3.1/src/power_query/management/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.372295 unicef-power-query-0.3.1/src/power_query/management/commands/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/management/commands/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3595 2023-07-13 07:17:04.000000 unicef-power-query-0.3.1/src/power_query/management/commands/pq.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.375565 unicef-power-query-0.3.1/src/power_query/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)    15211 2023-07-18 09:06:00.000000 unicef-power-query-0.3.1/src/power_query/migrations/0001_migration_squashed_0014_migration.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1003 2023-07-18 14:51:26.000000 unicef-power-query-0.3.1/src/power_query/migrations/0015_alter_dataset_description_and_more.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/migrations/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.385770 unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)    10802 2023-07-18 14:47:18.000000 unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5436 2023-07-18 09:30:10.000000 unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1409 2023-07-19 09:26:07.000000 unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      923 2023-07-20 09:13:33.000000 unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      188 2023-07-18 14:47:18.000000 unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:08.000000 unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      753 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/mixin.py
+-rw-r--r--   0 jojo       (501) staff       (20)    17447 2023-07-19 09:57:17.000000 unicef-power-query-0.3.1/src/power_query/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-19 07:55:05.000000 unicef-power-query-0.3.1/src/power_query/notify.py
+-rw-r--r--   0 jojo       (501) staff       (20)       91 2023-07-19 07:55:05.000000 unicef-power-query-0.3.1/src/power_query/signals.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.391762 unicef-power-query-0.3.1/src/power_query/static/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.269512 unicef-power-query-0.3.1/src/power_query/static/admin/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.402266 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)     3628 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/code.css
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.457575 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/
+-rw-r--r--   0 jojo       (501) staff       (20)     1969 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/abcdef.css
+-rw-r--r--   0 jojo       (501) staff       (20)     2507 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/active-line.js
+-rw-r--r--   0 jojo       (501) staff       (20)     8706 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/codemirror.css
+-rw-r--r--   0 jojo       (501) staff       (20)   400161 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/codemirror.js
+-rw-r--r--   0 jojo       (501) staff       (20)    11792 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/django.js
+-rw-r--r--   0 jojo       (501) staff       (20)     4983 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/foldcode.js
+-rw-r--r--   0 jojo       (501) staff       (20)      435 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/foldgutter.css
+-rw-r--r--   0 jojo       (501) staff       (20)     5368 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/foldgutter.js
+-rw-r--r--   0 jojo       (501) staff       (20)      118 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/fullscreen.css
+-rw-r--r--   0 jojo       (501) staff       (20)     1495 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/fullscreen.js
+-rw-r--r--   0 jojo       (501) staff       (20)     1674 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/indent-fold.js
+-rw-r--r--   0 jojo       (501) staff       (20)     6816 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/matchbrackets.js
+-rw-r--r--   0 jojo       (501) staff       (20)     1856 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/midnight.css
+-rw-r--r--   0 jojo       (501) staff       (20)     3241 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/overlay.js
+-rw-r--r--   0 jojo       (501) staff       (20)    14924 2023-05-08 13:33:06.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/python.js
+-rw-r--r--   0 jojo       (501) staff       (20)    13351 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/xml.js
+-rw-r--r--   0 jojo       (501) staff       (20)     3733 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/yaml.js
+-rw-r--r--   0 jojo       (501) staff       (20)     5122 2023-07-04 08:17:12.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/colorful.css
+-rw-r--r--   0 jojo       (501) staff       (20)      760 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/diff.css
+-rw-r--r--   0 jojo       (501) staff       (20)    16556 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/admin/power_query/editor.png
+-rw-r--r--   0 jojo       (501) staff       (20)      292 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/power_query.css
+-rw-r--r--   0 jojo       (501) staff       (20)      204 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/power_query.css.map
+-rw-r--r--   0 jojo       (501) staff       (20)      355 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/power_query.scss
+-rw-r--r--   0 jojo       (501) staff       (20)     6742 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/redo.png
+-rw-r--r--   0 jojo       (501) staff       (20)     6554 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/static/undo.png
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.273447 unicef-power-query-0.3.1/src/power_query/templates/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.270453 unicef-power-query-0.3.1/src/power_query/templates/admin/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.273198 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.461128 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/dataset/
+-rw-r--r--   0 jojo       (501) staff       (20)      109 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/dataset/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/dataset/export.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.465125 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/formatter/
+-rw-r--r--   0 jojo       (501) staff       (20)     2750 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/formatter/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/formatter/change_list.html
+-rw-r--r--   0 jojo       (501) staff       (20)      489 2023-07-13 07:30:38.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/formatter/test.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.471950 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/query/
+-rw-r--r--   0 jojo       (501) staff       (20)      407 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/query/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/query/export.html
+-rw-r--r--   0 jojo       (501) staff       (20)      822 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/query/monitor.html
+-rw-r--r--   0 jojo       (501) staff       (20)     2003 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/query/preview.html
+-rw-r--r--   0 jojo       (501) staff       (20)      490 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/query/run_result.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.473620 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/queryargs/
+-rw-r--r--   0 jojo       (501) staff       (20)     1559 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/queryargs/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      479 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/queryargs/preview.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.476553 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/report/
+-rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/report/change_list.html
+-rw-r--r--   0 jojo       (501) staff       (20)      743 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/report/monitor.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.481722 unicef-power-query-0.3.1/src/power_query/templates/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)      532 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/power_query/base.html
+-rw-r--r--   0 jojo       (501) staff       (20)      762 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/power_query/detail.html
+-rw-r--r--   0 jojo       (501) staff       (20)      339 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templates/power_query/list.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.483528 unicef-power-query-0.3.1/src/power_query/templates/power_query/widgets/
+-rw-r--r--   0 jojo       (501) staff       (20)     2661 2023-07-20 09:45:52.000000 unicef-power-query-0.3.1/src/power_query/templates/power_query/widgets/codewidget.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.485123 unicef-power-query-0.3.1/src/power_query/templatetags/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/src/power_query/templatetags/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.494357 unicef-power-query-0.3.1/src/power_query/templatetags/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      190 2023-07-18 14:47:18.000000 unicef-power-query-0.3.1/src/power_query/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      172 2023-07-13 10:20:43.000000 unicef-power-query-0.3.1/src/power_query/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2150 2023-07-18 14:47:18.000000 unicef-power-query-0.3.1/src/power_query/templatetags/__pycache__/power_query.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1295 2023-07-13 10:20:43.000000 unicef-power-query-0.3.1/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      814 2023-07-13 07:18:11.000000 unicef-power-query-0.3.1/src/power_query/templatetags/power_query.py
+-rw-r--r--   0 jojo       (501) staff       (20)      368 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5041 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)      453 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/validators.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3360 2023-07-19 07:59:09.000000 unicef-power-query-0.3.1/src/power_query/views.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2987 2023-07-20 09:45:52.000000 unicef-power-query-0.3.1/src/power_query/widget.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.497248 unicef-power-query-0.3.1/src/unicef_power_query.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      529 2023-07-20 09:46:13.000000 unicef-power-query-0.3.1/src/unicef_power_query.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     7761 2023-07-20 09:46:13.000000 unicef-power-query-0.3.1/src/unicef_power_query.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-20 09:46:13.000000 unicef-power-query-0.3.1/src/unicef_power_query.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      319 2023-07-20 09:46:13.000000 unicef-power-query-0.3.1/src/unicef_power_query.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       12 2023-07-20 09:46:13.000000 unicef-power-query-0.3.1/src/unicef_power_query.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.508210 unicef-power-query-0.3.1/tests/
+-rw-r--r--   0 jojo       (501) staff       (20)      214 2023-05-16 13:30:33.000000 unicef-power-query-0.3.1/tests/.coveragerc
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.3.1/tests/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.517887 unicef-power-query-0.3.1/tests/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      167 2023-07-19 09:26:06.000000 unicef-power-query-0.3.1/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     4942 2023-07-19 09:50:41.000000 unicef-power-query-0.3.1/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3607 2023-06-12 07:29:10.000000 unicef-power-query-0.3.1/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     7475 2023-06-12 07:29:10.000000 unicef-power-query-0.3.1/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1408 2023-06-12 07:29:10.000000 unicef-power-query-0.3.1/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     4525 2023-06-12 07:29:10.000000 unicef-power-query-0.3.1/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1502 2023-06-12 07:29:10.000000 unicef-power-query-0.3.1/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    11905 2023-05-16 12:47:07.000000 unicef-power-query-0.3.1/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.543006 unicef-power-query-0.3.1/tests/demoproject/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-02 15:31:56.000000 unicef-power-query-0.3.1/tests/demoproject/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)   278528 2023-05-31 15:10:33.000000 unicef-power-query-0.3.1/tests/demoproject/db.sqlite3
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.555013 unicef-power-query-0.3.1/tests/demoproject/demo/
+-rw-r--r--   0 jojo       (501) staff       (20)       65 2023-07-04 08:17:12.000000 unicef-power-query-0.3.1/tests/demoproject/demo/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.568018 unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      267 2023-07-18 14:47:16.000000 unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      691 2023-07-18 14:47:16.000000 unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      738 2023-05-16 12:44:40.000000 unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2731 2023-07-19 09:25:58.000000 unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      525 2023-05-31 11:57:14.000000 unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      699 2023-05-16 13:01:06.000000 unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      245 2023-07-04 08:17:12.000000 unicef-power-query-0.3.1/tests/demoproject/demo/celery.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.570506 unicef-power-query-0.3.1/tests/demoproject/demo/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-power-query-0.3.1/tests/demoproject/demo/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-power-query-0.3.1/tests/demoproject/demo/migrations/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-20 09:46:13.572136 unicef-power-query-0.3.1/tests/demoproject/demo/migrations/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)     3923 2023-05-16 13:01:06.000000 unicef-power-query-0.3.1/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      195 2023-05-16 13:01:06.000000 unicef-power-query-0.3.1/tests/demoproject/demo/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      142 2023-05-16 12:43:15.000000 unicef-power-query-0.3.1/tests/demoproject/demo/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2626 2023-07-20 09:45:52.000000 unicef-power-query-0.3.1/tests/demoproject/demo/settings.py
+-rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-16 14:04:29.000000 unicef-power-query-0.3.1/tests/demoproject/demo/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-power-query-0.3.1/tests/demoproject/demo/wsgi.py
+-rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-power-query-0.3.1/tests/demoproject/factories.py
+-rwxr-xr-x   0 jojo       (501) staff       (20)      246 2023-07-04 08:17:12.000000 unicef-power-query-0.3.1/tests/demoproject/manage.py
+-rw-r--r--   0 jojo       (501) staff       (20)    10643 2023-07-20 09:45:52.000000 unicef-power-query-0.3.1/tests/test_admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1719 2023-07-19 08:26:00.000000 unicef-power-query-0.3.1/tests/test_auth.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2097 2023-07-19 08:26:00.000000 unicef-power-query-0.3.1/tests/test_celery.py
+-rw-r--r--   0 jojo       (501) staff       (20)      441 2023-07-19 08:26:00.000000 unicef-power-query-0.3.1/tests/test_params.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1989 2023-07-19 08:26:00.000000 unicef-power-query-0.3.1/tests/test_queries.py
+-rw-r--r--   0 jojo       (501) staff       (20)      829 2023-07-19 08:26:00.000000 unicef-power-query-0.3.1/tests/test_utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1772 2023-07-19 08:26:00.000000 unicef-power-query-0.3.1/tests/test_views.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1022 2023-07-04 08:17:12.000000 unicef-power-query-0.3.1/tox.ini
```

### Comparing `unicef-power-query-0.3/LICENSE` & `unicef-power-query-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/PKG-INFO` & `unicef-power-query-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-power-query
-Version: 0.3
+Version: 0.3.1
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `unicef-power-query-0.3/README.rst` & `unicef-power-query-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/setup.py` & `unicef-power-query-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/admin.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/admin.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x10c2af64 (Thu Jul 13 09:21:20 2023 UTC)
-files sz: 16001
+moddate:  0xc0b1b764 (Wed Jul 19 09:49:52 2023 UTC)
+files sz: 16193
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
@@ -481,45 +481,45 @@
                896 CALL                     7
    
    395         906 PRECALL                  0
                910 CALL                     0
    
    396         920 STORE_NAME              86 (QueryArgsAdmin)
    
-   416         922 PUSH_NULL
+   421         922 PUSH_NULL
                924 LOAD_NAME               15 (register)
                926 LOAD_NAME               68 (ReportDocument)
                928 PRECALL                  1
                932 CALL                     1
    
-   417         942 PUSH_NULL
+   422         942 PUSH_NULL
                944 LOAD_BUILD_CLASS
-               946 LOAD_CONST              46 (<code object ReportDocumentAdmin, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 416>)
+               946 LOAD_CONST              46 (<code object ReportDocumentAdmin, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 421>)
                948 MAKE_FUNCTION            0
                950 LOAD_CONST              47 ('ReportDocumentAdmin')
    
-   418         952 LOAD_NAME               42 (AdminFiltersMixin)
+   423         952 LOAD_NAME               42 (AdminFiltersMixin)
    
-   419         954 LOAD_NAME               54 (LinkedObjectsMixin)
+   424         954 LOAD_NAME               54 (LinkedObjectsMixin)
    
-   420         956 LOAD_NAME               36 (ExtraButtonsMixin)
+   425         956 LOAD_NAME               36 (ExtraButtonsMixin)
    
-   421         958 LOAD_NAME               53 (DisplayAllMixin)
+   426         958 LOAD_NAME               53 (DisplayAllMixin)
    
-   422         960 LOAD_NAME               38 (AdminActionPermMixin)
+   427         960 LOAD_NAME               38 (AdminActionPermMixin)
    
-   423         962 LOAD_NAME               14 (ModelAdmin)
+   428         962 LOAD_NAME               14 (ModelAdmin)
    
-   417         964 PRECALL                  8
+   422         964 PRECALL                  8
                968 CALL                     8
    
-   416         978 PRECALL                  0
+   421         978 PRECALL                  0
                982 CALL                     0
    
-   417         992 STORE_NAME              87 (ReportDocumentAdmin)
+   422         992 STORE_NAME              87 (ReportDocumentAdmin)
                994 LOAD_CONST               1 (None)
                996 RETURN_VALUE
    consts
       0
       None
       ('Any', 'Dict', 'Optional', 'Sequence', 'TYPE_CHECKING')
       ('forms',)
@@ -3776,15 +3776,17 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06020065
             07a6000000ab00000000000000000064056508640665096407650a660664
-            088404a6000000ab0000000000000000005a0b64095300
+            088404a6000000ab0000000000000000005a0b0200650764098400ac0aa6
+            010000ab01000000000000000064056508640665096407640b6606640c84
+            04a6000000ab0000000000000000005a0c640b5300
          395           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('QueryArgsAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
          403          10 LOAD_CONST               1 (('name', 'code', 'system'))
@@ -3814,16 +3816,39 @@
                       58 LOAD_CONST               8 (<code object preview, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 408>)
                       60 MAKE_FUNCTION            4 (annotations)
          
          408          62 PRECALL                  0
                       66 CALL                     0
          
          409          76 STORE_NAME              11 (preview)
-                      78 LOAD_CONST               9 (None)
-                      80 RETURN_VALUE
+         
+         415          78 PUSH_NULL
+                      80 LOAD_NAME                7 (button)
+                      82 LOAD_CONST               9 (<code object <lambda>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 415>)
+                      84 MAKE_FUNCTION            0
+                      86 KW_NAMES                10
+                      88 PRECALL                  1
+                      92 CALL                     1
+         
+         416         102 LOAD_CONST               5 ('request')
+                     104 LOAD_NAME                8 (HttpRequest)
+                     106 LOAD_CONST               6 ('pk')
+                     108 LOAD_NAME                9 (int)
+                     110 LOAD_CONST               7 ('return')
+                     112 LOAD_CONST              11 (None)
+                     114 BUILD_TUPLE              6
+                     116 LOAD_CONST              12 (<code object refresh, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 415>)
+                     118 MAKE_FUNCTION            4 (annotations)
+         
+         415         120 PRECALL                  0
+                     124 CALL                     0
+         
+         416         134 STORE_NAME              12 (refresh)
+                     136 LOAD_CONST              11 (None)
+                     138 RETURN_VALUE
          consts
             'QueryArgsAdmin'
             ('name', 'code', 'system')
             ('system',)
             ('name', 'code')
             True
             'request'
@@ -3868,23 +3893,90 @@
                varnames   ('self', 'request', 'pk', 'context')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
                name       'preview'
                firstlineno 408
                lnotab 0x020230010c0106ff
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c006a0100000000000000006a0200
+                  00000000000000a6010000ab0100000000000000005300
+               415           0 RESUME                   0
+                             2 LOAD_GLOBAL              1 (NULL + bool)
+                            14 LOAD_FAST                0 (btn)
+                            16 LOAD_ATTR                1 (original)
+                            26 LOAD_ATTR                2 (source)
+                            36 PRECALL                  1
+                            40 CALL                     1
+                            50 RETURN_VALUE
+               consts
+                  None
+               names      ('bool', 'original', 'source')
+               varnames   ('btn',)
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
+               name       '<lambda>'
+               firstlineno 415
+               lnotab 0x
+            ('visible',)
             None
-         names      ('__name__', '__module__', '__qualname__', 'list_display', 'list_filter', 'search_fields', 'json_enabled', 'button', 'HttpRequest', 'int', 'TemplateResponse', 'preview')
+            code
+               argcount  : 3
+               nlocals   : 4
+               stacksize : 6
+               flags     : 3
+               code
+                  0x97007c00a00000000000000000000000000000000000000000007c0174
+                  03000000000000000000007c02a6010000ab010000000000000000a60200
+                  00ab0200000000000000007d037c03a00200000000000000000000000000
+                  00000000000000a6000000ab000000000000000000010064005300
+               415           0 RESUME                   0
+               
+               417           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (get_object)
+                            26 LOAD_FAST                1 (request)
+                            28 LOAD_GLOBAL              3 (NULL + str)
+                            40 LOAD_FAST                2 (pk)
+                            42 PRECALL                  1
+                            46 CALL                     1
+                            56 PRECALL                  2
+                            60 CALL                     2
+                            70 STORE_FAST               3 (obj)
+               
+               418          72 LOAD_FAST                3 (obj)
+                            74 LOAD_METHOD              2 (refresh)
+                            96 PRECALL                  0
+                           100 CALL                     0
+                           110 POP_TOP
+                           112 LOAD_CONST               0 (None)
+                           114 RETURN_VALUE
+               consts
+                  None
+               names      ('get_object', 'str', 'refresh')
+               varnames   ('self', 'request', 'pk', 'obj')
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
+               name       'refresh'
+               firstlineno 415
+               lnotab 0x02024601
+         names      ('__name__', '__module__', '__qualname__', 'list_display', 'list_filter', 'search_fields', 'json_enabled', 'button', 'HttpRequest', 'int', 'TemplateResponse', 'preview', 'refresh')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
          name       'QueryArgsAdmin'
          firstlineno 395
-         lnotab 0x0a080401040104010402120112ff0e01
+         lnotab 0x0a080401040104010402120112ff0e010206180112ff0e01
       'QueryArgsAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
@@ -3892,83 +3984,83 @@
             0664045a076405650864066509650a190000000000000000006604880066
             016407840c5a0b6408650a6406650c6604640984045a0d0200650ea60000
             00ab00000000000000000064056508640a650c6406650f6606640b8404a6
             000000ab0000000000000000005a1064056508640665116604640c84045a
             12880078015a135300
                        0 MAKE_CELL                0 (__class__)
          
-         416           2 RESUME                   0
+         421           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ReportDocumentAdmin')
                       10 STORE_NAME               2 (__qualname__)
          
-         425          12 LOAD_CONST               1 (('title', 'content_type', 'arguments', 'size'))
+         430          12 LOAD_CONST               1 (('title', 'content_type', 'arguments', 'size'))
                       14 STORE_NAME               3 (list_display)
          
-         426          16 LOAD_CONST               2 ('report')
+         431          16 LOAD_CONST               2 ('report')
                       18 LOAD_NAME                4 (AutoCompleteFilter)
                       20 BUILD_TUPLE              2
                       22 BUILD_TUPLE              1
                       24 STORE_NAME               5 (list_filter)
          
-         427          26 LOAD_CONST               3 (('limit_access_to',))
+         432          26 LOAD_CONST               3 (('limit_access_to',))
                       28 STORE_NAME               6 (filter_horizontal)
          
-         428          30 LOAD_CONST               4 (('arguments', 'report', 'dataset', 'content_type'))
+         433          30 LOAD_CONST               4 (('arguments', 'report', 'dataset', 'content_type'))
                       32 STORE_NAME               7 (readonly_fields)
          
-         430          34 LOAD_CONST               5 ('request')
+         435          34 LOAD_CONST               5 ('request')
                       36 LOAD_NAME                8 (HttpRequest)
                       38 LOAD_CONST               6 ('return')
                       40 LOAD_NAME                9 (QuerySet)
                       42 LOAD_NAME               10 (ReportDocument)
                       44 BINARY_SUBSCR
                       54 BUILD_TUPLE              4
                       56 LOAD_CLOSURE             0 (__class__)
                       58 BUILD_TUPLE              1
-                      60 LOAD_CONST               7 (<code object get_queryset, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 430>)
+                      60 LOAD_CONST               7 (<code object get_queryset, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 435>)
                       62 MAKE_FUNCTION           12 (annotations, closure)
                       64 STORE_NAME              11 (get_queryset)
          
-         433          66 LOAD_CONST               8 ('obj')
+         438          66 LOAD_CONST               8 ('obj')
                       68 LOAD_NAME               10 (ReportDocument)
                       70 LOAD_CONST               6 ('return')
                       72 LOAD_NAME               12 (int)
                       74 BUILD_TUPLE              4
-                      76 LOAD_CONST               9 (<code object size, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 433>)
+                      76 LOAD_CONST               9 (<code object size, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 438>)
                       78 MAKE_FUNCTION            4 (annotations)
                       80 STORE_NAME              13 (size)
          
-         436          82 PUSH_NULL
+         441          82 PUSH_NULL
                       84 LOAD_NAME               14 (button)
                       86 PRECALL                  0
                       90 CALL                     0
          
-         437         100 LOAD_CONST               5 ('request')
+         442         100 LOAD_CONST               5 ('request')
                      102 LOAD_NAME                8 (HttpRequest)
                      104 LOAD_CONST              10 ('pk')
                      106 LOAD_NAME               12 (int)
                      108 LOAD_CONST               6 ('return')
                      110 LOAD_NAME               15 (HttpResponseRedirect)
                      112 BUILD_TUPLE              6
-                     114 LOAD_CONST              11 (<code object view, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 436>)
+                     114 LOAD_CONST              11 (<code object view, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 441>)
                      116 MAKE_FUNCTION            4 (annotations)
          
-         436         118 PRECALL                  0
+         441         118 PRECALL                  0
                      122 CALL                     0
          
-         437         132 STORE_NAME              16 (view)
+         442         132 STORE_NAME              16 (view)
          
-         443         134 LOAD_CONST               5 ('request')
+         448         134 LOAD_CONST               5 ('request')
                      136 LOAD_NAME                8 (HttpRequest)
                      138 LOAD_CONST               6 ('return')
                      140 LOAD_NAME               17 (bool)
                      142 BUILD_TUPLE              4
-                     144 LOAD_CONST              12 (<code object has_add_permission, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 443>)
+                     144 LOAD_CONST              12 (<code object has_add_permission, file "/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py", line 448>)
                      146 MAKE_FUNCTION            4 (annotations)
                      148 STORE_NAME              18 (has_add_permission)
                      150 LOAD_CLOSURE             0 (__class__)
                      152 COPY                     1
                      154 STORE_NAME              19 (__classcell__)
                      156 RETURN_VALUE
          consts
@@ -3987,17 +4079,17 @@
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000005300
                              0 COPY_FREE_VARS           1
                
-               430           2 RESUME                   0
+               435           2 RESUME                   0
                
-               431           4 LOAD_GLOBAL              1 (NULL + super)
+               436           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (get_queryset)
                             52 LOAD_FAST                1 (request)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 LOAD_METHOD              2 (defer)
@@ -4010,28 +4102,28 @@
                   'output'
                names      ('super', 'get_queryset', 'defer')
                varnames   ('self', 'request')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
                name       'get_queryset'
-               firstlineno 430
+               firstlineno 435
                lnotab 0x0401
             'obj'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c016a010000000000000000700164
                   01a6010000ab0100000000000000005300
-               433           0 RESUME                   0
+               438           0 RESUME                   0
                
-               434           2 LOAD_GLOBAL              1 (NULL + len)
+               439           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                1 (obj)
                             16 LOAD_ATTR                1 (output)
                             26 JUMP_IF_TRUE_OR_POP      1 (to 30)
                             28 LOAD_CONST               1 ('')
                        >>   30 PRECALL                  1
                             34 CALL                     1
                             44 RETURN_VALUE
@@ -4040,15 +4132,15 @@
                   ''
                names      ('len', 'output')
                varnames   ('self', 'obj')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
                name       'size'
-               firstlineno 433
+               firstlineno 438
                lnotab 0x0201
             'pk'
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 6
                flags     : 3
@@ -4056,48 +4148,48 @@
                   0x97007c00a00000000000000000000000000000000000000000007c0174
                   03000000000000000000007c02a6010000ab010000000000000000a60200
                   00ab02000000000000000078017d03730f74050000000000000000000064
                   01a6010000ab010000000000000000820174070000000000000000000064
                   027c036a0400000000000000006a0500000000000000007c026702ac03a6
                   020000ab0200000000000000007d04740d000000000000000000007c04a6
                   010000ab0100000000000000005300
-               436           0 RESUME                   0
+               441           0 RESUME                   0
                
-               438           2 LOAD_FAST                0 (self)
+               443           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_object)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_GLOBAL              3 (NULL + str)
                             40 LOAD_FAST                2 (pk)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 PRECALL                  2
                             60 CALL                     2
                             70 COPY                     1
                             72 STORE_FAST               3 (obj)
                             74 POP_JUMP_FORWARD_IF_TRUE    15 (to 106)
                
-               439          76 LOAD_GLOBAL              5 (NULL + Exception)
+               444          76 LOAD_GLOBAL              5 (NULL + Exception)
                             88 LOAD_CONST               1 ('Report document not found')
                             90 PRECALL                  1
                             94 CALL                     1
                            104 RAISE_VARARGS            1
                
-               440     >>  106 LOAD_GLOBAL              7 (NULL + reverse)
+               445     >>  106 LOAD_GLOBAL              7 (NULL + reverse)
                            118 LOAD_CONST               2 ('power_query:document')
                            120 LOAD_FAST                3 (obj)
                            122 LOAD_ATTR                4 (report)
                            132 LOAD_ATTR                5 (pk)
                            142 LOAD_FAST                2 (pk)
                            144 BUILD_LIST               2
                            146 KW_NAMES                 3
                            148 PRECALL                  2
                            152 CALL                     2
                            162 STORE_FAST               4 (url)
                
-               441         164 LOAD_GLOBAL             13 (NULL + HttpResponseRedirect)
+               446         164 LOAD_GLOBAL             13 (NULL + HttpResponseRedirect)
                            176 LOAD_FAST                4 (url)
                            178 PRECALL                  1
                            182 CALL                     1
                            192 RETURN_VALUE
                consts
                   None
                   'Report document not found'
@@ -4105,44 +4197,44 @@
                   ('args',)
                names      ('get_object', 'str', 'Exception', 'reverse', 'report', 'pk', 'HttpResponseRedirect')
                varnames   ('self', 'request', 'pk', 'obj', 'url')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
                name       'view'
-               firstlineno 436
+               firstlineno 441
                lnotab 0x02024a011e013a01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064015300
-               443           0 RESUME                   0
+               448           0 RESUME                   0
                
-               444           2 LOAD_CONST               1 (False)
+               449           2 LOAD_CONST               1 (False)
                              4 RETURN_VALUE
                consts
                   None
                   False
                names      ()
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
                name       'has_add_permission'
-               firstlineno 443
+               firstlineno 448
                lnotab 0x0201
          names      ('__name__', '__module__', '__qualname__', 'list_display', 'AutoCompleteFilter', 'list_filter', 'filter_horizontal', 'readonly_fields', 'HttpRequest', 'QuerySet', 'ReportDocument', 'get_queryset', 'int', 'size', 'button', 'HttpResponseRedirect', 'view', 'bool', 'has_add_permission', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
          name       'ReportDocumentAdmin'
-         firstlineno 416
+         firstlineno 421
          lnotab 0x0c0904010a010401040220031003120112ff0e010206
       'ReportDocumentAdmin'
    names      ('logging', 'typing', 'Any', 'Dict', 'Optional', 'Sequence', 'TYPE_CHECKING', 'django', 'forms', 'django.conf', 'settings', 'django.contrib', 'messages', 'django.contrib.admin', 'ModelAdmin', 'register', 'django.contrib.contenttypes.models', 'ContentType', 'django.db', 'models', 'django.db.models', 'QuerySet', 'django.http', 'HttpRequest', 'HttpResponse', 'HttpResponseRedirect', 'django.shortcuts', 'render', 'django.template.response', 'TemplateResponse', 'django.urls', 'reverse', 'tablib', 'admin_extra_buttons.decorators', 'button', 'admin_extra_buttons.mixins', 'ExtraButtonsMixin', 'adminactions.helpers', 'AdminActionPermMixin', 'adminfilters.autocomplete', 'AutoCompleteFilter', 'adminfilters.mixin', 'AdminFiltersMixin', 'celery.result', 'AsyncResult', 'import_export', 'fields', 'resources', 'import_export.admin', 'ImportExportMixin', 'import_export.widgets', 'ForeignKeyWidget', 'smart_admin.mixins', 'DisplayAllMixin', 'LinkedObjectsMixin', 'power_query.celery_tasks', 'refresh_report', 'refresh_reports', 'run_background_query', 'power_query.forms', 'FormatterTestForm', 'power_query.models', 'CeleryEnabled', 'Dataset', 'Formatter', 'Parametrizer', 'Query', 'Report', 'ReportDocument', 'power_query.utils', 'to_dataset', 'power_query.widget', 'FormatterEditor', 'PythonFormatterEditor', 'getLogger', '__name__', 'logger', '_ModelT', 'CeleryEnabledMixin', 'QueryAdmin', 'DatasetAdmin', 'ModelResource', 'FormatterResource', 'FormatterAdmin', 'ReportResource', 'ReportAdmin', 'QueryArgsAdmin', 'ReportDocumentAdmin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/admin.py'
@@ -4151,8 +4243,8 @@
    lnotab
       0x00ff020108011c020c010c010c0110010c010c010c0114010c010c010c
       0208010c010c010c010c010c010c0110010c010c01100214050c0124090c
       011002200204010c031a2714010a0102010201020102010201020102f90e
       ff0e01026d14010a01020102010201020102fb0eff0e010234260714010a
       01020102010201020102fb0eff0e010230260a14010a0102010201020102
       010201020102f90eff0e01024a14010a01020102010201020102fb0eff0e
-      01021414010a010201020102010201020102fa0eff0e01
+      01021914010a010201020102010201020102fa0eff0e01
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/admin.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/admin.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 09:21:20 2023 UTC, .py size: 16001 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 10c2 af64 813e 0000  a..........d.>..
+00000000: 610d 0d0a 0000 0000 5002 b964 143f 0000  a.......P..d.?..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 b802 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -814,170 +814,182 @@
 000032d0: 0000 72ec 0000 0072 f100 0000 723e 0000  ..r....r....r>..
 000032e0: 0072 3e00 0000 723e 0000 0072 3f00 0000  .r>...r>...r?...
 000032f0: 72e3 0000 0040 0100 0073 3200 0000 080a  r....@...s2.....
 00003300: 0401 0401 0601 0402 0601 0601 0601 02fc  ................
 00003310: 0406 0401 0403 00ff 0201 0801 02fe 0c05  ................
 00003320: 1009 0c01 1409 0c01 1410 0201 06ff 0403  ................
 00003330: 72e3 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00003340: 0000 0000 0000 0500 0000 4000 0000 7334  ..........@...s4
+00003340: 0000 0000 0000 0500 0000 4000 0000 734c  ..........@...sL
 00003350: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
 00003360: 025a 0464 035a 0564 045a 0665 0783 0065  .Z.d.Z.d.Z.e...e
 00003370: 0865 0965 0a64 059c 0364 0664 0784 0483  .e.e.d...d.d....
-00003380: 015a 0b64 0853 0029 09da 0e51 7565 7279  .Z.d.S.)...Query
-00003390: 4172 6773 4164 6d69 6e29 0372 6700 0000  ArgsAdmin).rg...
-000033a0: 7276 0000 00da 0673 7973 7465 6d29 0172  rv.....system).r
-000033b0: f400 0000 2902 7267 0000 0072 7600 0000  ....).rg...rv...
-000033c0: 5472 5600 0000 6303 0000 0000 0000 0000  TrV...c.........
-000033d0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-000033e0: 1c00 0000 7c00 6a00 7c01 7c02 6401 6402  ....|.j.|.|.d.d.
-000033f0: 8d03 7d03 7401 7c01 6403 7c03 8303 5300  ..}.t.|.d.|...S.
-00003400: 2904 4e7a 0e45 7865 6375 7469 6f6e 2050  ).Nz.Execution P
-00003410: 6c61 6e72 4900 0000 7a28 6164 6d69 6e2f  lanrI...z(admin/
-00003420: 706f 7765 725f 7175 6572 792f 7175 6572  power_query/quer
-00003430: 7961 7267 732f 7072 6576 6965 772e 6874  yargs/preview.ht
-00003440: 6d6c 2902 724d 0000 0072 1300 0000 2904  ml).rM...r....).
-00003450: 723a 0000 0072 3200 0000 7257 0000 0072  r:...r2...rW...r
-00003460: 9f00 0000 723e 0000 0072 3e00 0000 723f  ....r>...r>...r?
-00003470: 0000 0072 a200 0000 9801 0000 7308 0000  ...r........s...
-00003480: 0000 0210 0102 0106 ff7a 1651 7565 7279  .........z.Query
-00003490: 4172 6773 4164 6d69 6e2e 7072 6576 6965  ArgsAdmin.previe
-000034a0: 774e 290c 725e 0000 0072 6100 0000 7262  wN).r^...ra...rb
-000034b0: 0000 0072 aa00 0000 72ac 0000 0072 ab00  ...r....r....r..
-000034c0: 0000 da0c 6a73 6f6e 5f65 6e61 626c 6564  ....json_enabled
-000034d0: 7215 0000 0072 0f00 0000 7264 0000 0072  r....r....rd...r
-000034e0: 1300 0000 72a2 0000 0072 3e00 0000 723e  ....r....r>...r>
-000034f0: 0000 0072 3e00 0000 723f 0000 0072 f300  ...r>...r?...r..
-00003500: 0000 8b01 0000 730c 0000 0008 0804 0104  ......s.........
-00003510: 0104 0104 0204 0172 f300 0000 6300 0000  .......r....c...
-00003520: 0000 0000 0000 0000 0000 0000 0005 0000  ................
-00003530: 0000 0000 0073 7600 0000 6500 5a01 6400  .....sv...e.Z.d.
-00003540: 5a02 6401 5a03 6402 6504 6602 6601 5a05  Z.d.Z.d.e.f.f.Z.
-00003550: 6403 5a06 6404 5a07 6508 6509 650a 1900  d.Z.d.Z.e.e.e...
-00003560: 6405 9c02 8700 6601 6406 6407 840c 5a0b  d.....f.d.d...Z.
-00003570: 650a 650c 6408 9c02 6409 640a 8404 5a0d  e.e.d...d.d...Z.
-00003580: 650e 8300 6508 650c 650f 640b 9c03 640c  e...e.e.e.d...d.
-00003590: 640d 8404 8301 5a10 6508 6511 6405 9c02  d.....Z.e.e.d...
-000035a0: 640e 640f 8404 5a12 8700 0400 5a13 5300  d.d...Z.....Z.S.
-000035b0: 2910 da13 5265 706f 7274 446f 6375 6d65  )...ReportDocume
-000035c0: 6e74 4164 6d69 6e29 0472 4a00 0000 72cb  ntAdmin).rJ...r.
-000035d0: 0000 0072 b600 0000 72b5 0000 0072 d500  ...r....r....r..
-000035e0: 0000 2901 72e5 0000 0029 0472 b600 0000  ..).r....).r....
-000035f0: 72d5 0000 0072 9600 0000 72cb 0000 0072  r....r....r....r
-00003600: 4200 0000 6302 0000 0000 0000 0000 0000  B...c...........
-00003610: 0002 0000 0003 0000 0003 0000 0073 1200  .............s..
-00003620: 0000 7400 8300 a001 7c01 a101 a002 6401  ..t.....|.....d.
-00003630: a101 5300 2902 4e72 db00 0000 72b8 0000  ..S.).Nr....r...
-00003640: 0072 ba00 0000 723c 0000 0072 3e00 0000  .r....r<...r>...
-00003650: 723f 0000 0072 4400 0000 ae01 0000 7302  r?...rD.......s.
-00003660: 0000 0000 017a 2052 6570 6f72 7444 6f63  .....z ReportDoc
-00003670: 756d 656e 7441 646d 696e 2e67 6574 5f71  umentAdmin.get_q
-00003680: 7565 7279 7365 7472 7100 0000 6302 0000  uerysetrq...c...
-00003690: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-000036a0: 0043 0000 0073 0e00 0000 7400 7c01 6a01  .C...s....t.|.j.
-000036b0: 700a 6401 8301 5300 2902 4eda 0029 0272  p.d...S.).N..).r
-000036c0: ed00 0000 72db 0000 0072 7300 0000 723e  ....r....rs...r>
-000036d0: 0000 0072 3e00 0000 723f 0000 0072 b500  ...r>...r?...r..
-000036e0: 0000 b101 0000 7302 0000 0000 017a 1852  ......s......z.R
-000036f0: 6570 6f72 7444 6f63 756d 656e 7441 646d  eportDocumentAdm
-00003700: 696e 2e73 697a 6572 5600 0000 6303 0000  in.sizerV...c...
-00003710: 0000 0000 0000 0000 0005 0000 0005 0000  ................
-00003720: 0043 0000 0073 3800 0000 7c00 a000 7c01  .C...s8...|...|.
-00003730: 7401 7c02 8301 a102 0400 7d03 731c 7402  t.|.......}.s.t.
-00003740: 6401 8301 8201 7403 6402 7c03 6a04 6a05  d.....t.d.|.j.j.
-00003750: 7c02 6702 6403 8d02 7d04 7406 7c04 8301  |.g.d...}.t.|...
-00003760: 5300 2904 4e7a 1952 6570 6f72 7420 646f  S.).Nz.Report do
-00003770: 6375 6d65 6e74 206e 6f74 2066 6f75 6e64  cument not found
-00003780: 7a14 706f 7765 725f 7175 6572 793a 646f  z.power_query:do
-00003790: 6375 6d65 6e74 2901 72a0 0000 0029 0772  cument).r....).r
-000037a0: 5900 0000 725a 0000 0072 5d00 0000 7214  Y...rZ...r]...r.
-000037b0: 0000 0072 d500 0000 7257 0000 0072 1100  ...r....rW...r..
-000037c0: 0000 2905 723a 0000 0072 3200 0000 7257  ..).r:...r2...rW
-000037d0: 0000 0072 3300 0000 7284 0000 0072 3e00  ...r3...r....r>.
-000037e0: 0000 723e 0000 0072 3f00 0000 da04 7669  ..r>...r?.....vi
-000037f0: 6577 b401 0000 7308 0000 0000 0214 0108  ew....s.........
-00003800: 0114 017a 1852 6570 6f72 7444 6f63 756d  ...z.ReportDocum
-00003810: 656e 7441 646d 696e 2e76 6965 7763 0200  entAdmin.viewc..
-00003820: 0000 0000 0000 0000 0000 0200 0000 0100  ................
-00003830: 0000 4300 0000 7304 0000 0064 0153 0072  ..C...s....d.S.r
-00003840: bb00 0000 723e 0000 0072 ba00 0000 723e  ....r>...r....r>
-00003850: 0000 0072 3e00 0000 723f 0000 0072 bc00  ...r>...r?...r..
-00003860: 0000 bb01 0000 7302 0000 0000 017a 2652  ......s......z&R
-00003870: 6570 6f72 7444 6f63 756d 656e 7441 646d  eportDocumentAdm
-00003880: 696e 2e68 6173 5f61 6464 5f70 6572 6d69  in.has_add_permi
-00003890: 7373 696f 6e29 1472 5e00 0000 7261 0000  ssion).r^...ra..
-000038a0: 0072 6200 0000 72aa 0000 0072 1800 0000  .rb...r....r....
-000038b0: 72ac 0000 0072 f200 0000 72ae 0000 0072  r....r....r....r
-000038c0: 0f00 0000 720e 0000 0072 2b00 0000 7244  ....r....r+...rD
-000038d0: 0000 0072 6400 0000 72b5 0000 0072 1500  ...rd...r....r..
-000038e0: 0000 7211 0000 0072 f800 0000 7272 0000  ..r....r....rr..
-000038f0: 0072 bc00 0000 7265 0000 0072 3e00 0000  .r....re...r>...
-00003900: 723e 0000 0072 3c00 0000 723f 0000 0072  r>...r<...r?...r
-00003910: f600 0000 a001 0000 7312 0000 0008 0904  ........s.......
-00003920: 010a 0104 0104 0218 0310 0304 0114 0672  ...............r
-00003930: f600 0000 2958 da07 6c6f 6767 696e 67da  ....)X..logging.
-00003940: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-00003950: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-00003960: da06 646a 616e 676f 7207 0000 00da 0b64  ..djangor......d
-00003970: 6a61 6e67 6f2e 636f 6e66 7208 0000 005a  jango.confr....Z
-00003980: 0e64 6a61 6e67 6f2e 636f 6e74 7269 6272  .django.contribr
-00003990: 0900 0000 da14 646a 616e 676f 2e63 6f6e  ......django.con
-000039a0: 7472 6962 2e61 646d 696e 720a 0000 0072  trib.adminr....r
-000039b0: 0b00 0000 da22 646a 616e 676f 2e63 6f6e  ....."django.con
-000039c0: 7472 6962 2e63 6f6e 7465 6e74 7479 7065  trib.contenttype
-000039d0: 732e 6d6f 6465 6c73 720c 0000 00da 0964  s.modelsr......d
-000039e0: 6a61 6e67 6f2e 6462 720d 0000 00da 1064  jango.dbr......d
-000039f0: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 7372  jango.db.modelsr
-00003a00: 0e00 0000 da0b 646a 616e 676f 2e68 7474  ......django.htt
-00003a10: 7072 0f00 0000 7210 0000 0072 1100 0000  pr....r....r....
-00003a20: da10 646a 616e 676f 2e73 686f 7274 6375  ..django.shortcu
-00003a30: 7473 7212 0000 00da 1864 6a61 6e67 6f2e  tsr......django.
-00003a40: 7465 6d70 6c61 7465 2e72 6573 706f 6e73  template.respons
-00003a50: 6572 1300 0000 da0b 646a 616e 676f 2e75  er......django.u
-00003a60: 726c 7372 1400 0000 729c 0000 005a 1e61  rlsr....r....Z.a
-00003a70: 646d 696e 5f65 7874 7261 5f62 7574 746f  dmin_extra_butto
-00003a80: 6e73 2e64 6563 6f72 6174 6f72 7372 1500  ns.decoratorsr..
-00003a90: 0000 5a1a 6164 6d69 6e5f 6578 7472 615f  ..Z.admin_extra_
-00003aa0: 6275 7474 6f6e 732e 6d69 7869 6e73 7216  buttons.mixinsr.
-00003ab0: 0000 00da 1461 646d 696e 6163 7469 6f6e  .....adminaction
-00003ac0: 732e 6865 6c70 6572 7372 1700 0000 5a19  s.helpersr....Z.
-00003ad0: 6164 6d69 6e66 696c 7465 7273 2e61 7574  adminfilters.aut
-00003ae0: 6f63 6f6d 706c 6574 6572 1800 0000 da12  ocompleter......
-00003af0: 6164 6d69 6e66 696c 7465 7273 2e6d 6978  adminfilters.mix
-00003b00: 696e 7219 0000 00da 0d63 656c 6572 792e  inr......celery.
-00003b10: 7265 7375 6c74 721a 0000 00da 0d69 6d70  resultr......imp
-00003b20: 6f72 745f 6578 706f 7274 721b 0000 0072  ort_exportr....r
-00003b30: 1c00 0000 5a13 696d 706f 7274 5f65 7870  ....Z.import_exp
-00003b40: 6f72 742e 6164 6d69 6e72 1d00 0000 5a15  ort.adminr....Z.
-00003b50: 696d 706f 7274 5f65 7870 6f72 742e 7769  import_export.wi
-00003b60: 6467 6574 7372 1e00 0000 da12 736d 6172  dgetsr......smar
-00003b70: 745f 6164 6d69 6e2e 6d69 7869 6e73 721f  t_admin.mixinsr.
-00003b80: 0000 0072 2000 0000 da18 706f 7765 725f  ...r .....power_
-00003b90: 7175 6572 792e 6365 6c65 7279 5f74 6173  query.celery_tas
-00003ba0: 6b73 7221 0000 0072 2200 0000 7223 0000  ksr!...r"...r#..
-00003bb0: 005a 1170 6f77 6572 5f71 7565 7279 2e66  .Z.power_query.f
-00003bc0: 6f72 6d73 7224 0000 005a 1270 6f77 6572  ormsr$...Z.power
-00003bd0: 5f71 7565 7279 2e6d 6f64 656c 7372 2500  _query.modelsr%.
-00003be0: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
-00003bf0: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
-00003c00: da11 706f 7765 725f 7175 6572 792e 7574  ..power_query.ut
-00003c10: 696c 7372 2c00 0000 5a12 706f 7765 725f  ilsr,...Z.power_
-00003c20: 7175 6572 792e 7769 6467 6574 722d 0000  query.widgetr-..
-00003c30: 0072 2e00 0000 da09 6765 744c 6f67 6765  .r......getLogge
-00003c40: 7272 5e00 0000 72c7 0000 0072 2f00 0000  rr^...r....r/...
-00003c50: 7230 0000 0072 6600 0000 72b2 0000 00da  r0...rf...r.....
-00003c60: 0d4d 6f64 656c 5265 736f 7572 6365 72ca  .ModelResourcer.
-00003c70: 0000 0072 cf00 0000 72e1 0000 0072 e300  ...r....r....r..
-00003c80: 0000 72f3 0000 0072 f600 0000 723e 0000  ..r....r....r>..
-00003c90: 0072 3e00 0000 723e 0000 0072 3f00 0000  .r>...r>...r?...
-00003ca0: da08 3c6d 6f64 756c 653e 0100 0000 73ae  ..<module>....s.
-00003cb0: 0000 0008 011c 020c 010c 010c 0110 010c  ................
-00003cc0: 010c 010c 0114 010c 010c 010c 0208 010c  ................
-00003cd0: 010c 010c 010c 010c 010c 0110 010c 010c  ................
-00003ce0: 0110 0214 050c 0124 090c 0110 020a 0206  .......$........
-00003cf0: 010c 030e 2706 010a 0102 0102 0102 0102  ....'...........
-00003d00: 0102 0102 0102 f906 6d06 010a 0102 0102  ........m.......
-00003d10: 0102 0102 0102 fb06 3412 0706 010a 0102  ........4.......
-00003d20: 0102 0102 0102 0102 fb06 3012 0a06 010a  ..........0.....
-00003d30: 0102 0102 0102 0102 0102 0102 0102 f906  ................
-00003d40: 4a06 010a 0102 0102 0102 0102 0102 fb06  J...............
-00003d50: 1406 010a 0102 0102 0102 0102 0102 0102  ................
-00003d60: fa                                       .
+00003380: 015a 0b65 0783 0065 0865 0964 0864 059c  .Z.e...e.e.d.d..
+00003390: 0364 0964 0a84 0483 015a 0c64 0853 0029  .d.d.....Z.d.S.)
+000033a0: 0bda 0e51 7565 7279 4172 6773 4164 6d69  ...QueryArgsAdmi
+000033b0: 6e29 0372 6700 0000 7276 0000 00da 0673  n).rg...rv.....s
+000033c0: 7973 7465 6d29 0172 f400 0000 2902 7267  ystem).r....).rg
+000033d0: 0000 0072 7600 0000 5472 5600 0000 6303  ...rv...TrV...c.
+000033e0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+000033f0: 0000 0043 0000 0073 1c00 0000 7c00 6a00  ...C...s....|.j.
+00003400: 7c01 7c02 6401 6402 8d03 7d03 7401 7c01  |.|.d.d...}.t.|.
+00003410: 6403 7c03 8303 5300 2904 4e7a 0e45 7865  d.|...S.).Nz.Exe
+00003420: 6375 7469 6f6e 2050 6c61 6e72 4900 0000  cution PlanrI...
+00003430: 7a28 6164 6d69 6e2f 706f 7765 725f 7175  z(admin/power_qu
+00003440: 6572 792f 7175 6572 7961 7267 732f 7072  ery/queryargs/pr
+00003450: 6576 6965 772e 6874 6d6c 2902 724d 0000  eview.html).rM..
+00003460: 0072 1300 0000 2904 723a 0000 0072 3200  .r....).r:...r2.
+00003470: 0000 7257 0000 0072 9f00 0000 723e 0000  ..rW...r....r>..
+00003480: 0072 3e00 0000 723f 0000 0072 a200 0000  .r>...r?...r....
+00003490: 9801 0000 7308 0000 0000 0210 0102 0106  ....s...........
+000034a0: ff7a 1651 7565 7279 4172 6773 4164 6d69  .z.QueryArgsAdmi
+000034b0: 6e2e 7072 6576 6965 774e 6303 0000 0000  n.previewNc.....
+000034c0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+000034d0: 0000 0073 1c00 0000 7c00 a000 7c01 7401  ...s....|...|.t.
+000034e0: 7c02 8301 a102 7d03 7c03 a002 a100 0100  |.....}.|.......
+000034f0: 6400 5300 7243 0000 0029 0372 5900 0000  d.S.rC...).rY...
+00003500: 725a 0000 0072 f100 0000 2904 723a 0000  rZ...r....).r:..
+00003510: 0072 3200 0000 7257 0000 0072 3300 0000  .r2...rW...r3...
+00003520: 723e 0000 0072 3e00 0000 723f 0000 0072  r>...r>...r?...r
+00003530: f100 0000 9f01 0000 7304 0000 0000 0210  ........s.......
+00003540: 017a 1651 7565 7279 4172 6773 4164 6d69  .z.QueryArgsAdmi
+00003550: 6e2e 7265 6672 6573 6829 0d72 5e00 0000  n.refresh).r^...
+00003560: 7261 0000 0072 6200 0000 72aa 0000 0072  ra...rb...r....r
+00003570: ac00 0000 72ab 0000 00da 0c6a 736f 6e5f  ....r......json_
+00003580: 656e 6162 6c65 6472 1500 0000 720f 0000  enabledr....r...
+00003590: 0072 6400 0000 7213 0000 0072 a200 0000  .rd...r....r....
+000035a0: 72f1 0000 0072 3e00 0000 723e 0000 0072  r....r>...r>...r
+000035b0: 3e00 0000 723f 0000 0072 f300 0000 8b01  >...r?...r......
+000035c0: 0000 7310 0000 0008 0804 0104 0104 0104  ..s.............
+000035d0: 0204 0114 0604 0172 f300 0000 6300 0000  .......r....c...
+000035e0: 0000 0000 0000 0000 0000 0000 0005 0000  ................
+000035f0: 0000 0000 0073 7600 0000 6500 5a01 6400  .....sv...e.Z.d.
+00003600: 5a02 6401 5a03 6402 6504 6602 6601 5a05  Z.d.Z.d.e.f.f.Z.
+00003610: 6403 5a06 6404 5a07 6508 6509 650a 1900  d.Z.d.Z.e.e.e...
+00003620: 6405 9c02 8700 6601 6406 6407 840c 5a0b  d.....f.d.d...Z.
+00003630: 650a 650c 6408 9c02 6409 640a 8404 5a0d  e.e.d...d.d...Z.
+00003640: 650e 8300 6508 650c 650f 640b 9c03 640c  e...e.e.e.d...d.
+00003650: 640d 8404 8301 5a10 6508 6511 6405 9c02  d.....Z.e.e.d...
+00003660: 640e 640f 8404 5a12 8700 0400 5a13 5300  d.d...Z.....Z.S.
+00003670: 2910 da13 5265 706f 7274 446f 6375 6d65  )...ReportDocume
+00003680: 6e74 4164 6d69 6e29 0472 4a00 0000 72cb  ntAdmin).rJ...r.
+00003690: 0000 0072 b600 0000 72b5 0000 0072 d500  ...r....r....r..
+000036a0: 0000 2901 72e5 0000 0029 0472 b600 0000  ..).r....).r....
+000036b0: 72d5 0000 0072 9600 0000 72cb 0000 0072  r....r....r....r
+000036c0: 4200 0000 6302 0000 0000 0000 0000 0000  B...c...........
+000036d0: 0002 0000 0003 0000 0003 0000 0073 1200  .............s..
+000036e0: 0000 7400 8300 a001 7c01 a101 a002 6401  ..t.....|.....d.
+000036f0: a101 5300 2902 4e72 db00 0000 72b8 0000  ..S.).Nr....r...
+00003700: 0072 ba00 0000 723c 0000 0072 3e00 0000  .r....r<...r>...
+00003710: 723f 0000 0072 4400 0000 b301 0000 7302  r?...rD.......s.
+00003720: 0000 0000 017a 2052 6570 6f72 7444 6f63  .....z ReportDoc
+00003730: 756d 656e 7441 646d 696e 2e67 6574 5f71  umentAdmin.get_q
+00003740: 7565 7279 7365 7472 7100 0000 6302 0000  uerysetrq...c...
+00003750: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00003760: 0043 0000 0073 0e00 0000 7400 7c01 6a01  .C...s....t.|.j.
+00003770: 700a 6401 8301 5300 2902 4eda 0029 0272  p.d...S.).N..).r
+00003780: ed00 0000 72db 0000 0072 7300 0000 723e  ....r....rs...r>
+00003790: 0000 0072 3e00 0000 723f 0000 0072 b500  ...r>...r?...r..
+000037a0: 0000 b601 0000 7302 0000 0000 017a 1852  ......s......z.R
+000037b0: 6570 6f72 7444 6f63 756d 656e 7441 646d  eportDocumentAdm
+000037c0: 696e 2e73 697a 6572 5600 0000 6303 0000  in.sizerV...c...
+000037d0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+000037e0: 0043 0000 0073 3800 0000 7c00 a000 7c01  .C...s8...|...|.
+000037f0: 7401 7c02 8301 a102 0400 7d03 731c 7402  t.|.......}.s.t.
+00003800: 6401 8301 8201 7403 6402 7c03 6a04 6a05  d.....t.d.|.j.j.
+00003810: 7c02 6702 6403 8d02 7d04 7406 7c04 8301  |.g.d...}.t.|...
+00003820: 5300 2904 4e7a 1952 6570 6f72 7420 646f  S.).Nz.Report do
+00003830: 6375 6d65 6e74 206e 6f74 2066 6f75 6e64  cument not found
+00003840: 7a14 706f 7765 725f 7175 6572 793a 646f  z.power_query:do
+00003850: 6375 6d65 6e74 2901 72a0 0000 0029 0772  cument).r....).r
+00003860: 5900 0000 725a 0000 0072 5d00 0000 7214  Y...rZ...r]...r.
+00003870: 0000 0072 d500 0000 7257 0000 0072 1100  ...r....rW...r..
+00003880: 0000 2905 723a 0000 0072 3200 0000 7257  ..).r:...r2...rW
+00003890: 0000 0072 3300 0000 7284 0000 0072 3e00  ...r3...r....r>.
+000038a0: 0000 723e 0000 0072 3f00 0000 da04 7669  ..r>...r?.....vi
+000038b0: 6577 b901 0000 7308 0000 0000 0214 0108  ew....s.........
+000038c0: 0114 017a 1852 6570 6f72 7444 6f63 756d  ...z.ReportDocum
+000038d0: 656e 7441 646d 696e 2e76 6965 7763 0200  entAdmin.viewc..
+000038e0: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+000038f0: 0000 4300 0000 7304 0000 0064 0153 0072  ..C...s....d.S.r
+00003900: bb00 0000 723e 0000 0072 ba00 0000 723e  ....r>...r....r>
+00003910: 0000 0072 3e00 0000 723f 0000 0072 bc00  ...r>...r?...r..
+00003920: 0000 c001 0000 7302 0000 0000 017a 2652  ......s......z&R
+00003930: 6570 6f72 7444 6f63 756d 656e 7441 646d  eportDocumentAdm
+00003940: 696e 2e68 6173 5f61 6464 5f70 6572 6d69  in.has_add_permi
+00003950: 7373 696f 6e29 1472 5e00 0000 7261 0000  ssion).r^...ra..
+00003960: 0072 6200 0000 72aa 0000 0072 1800 0000  .rb...r....r....
+00003970: 72ac 0000 0072 f200 0000 72ae 0000 0072  r....r....r....r
+00003980: 0f00 0000 720e 0000 0072 2b00 0000 7244  ....r....r+...rD
+00003990: 0000 0072 6400 0000 72b5 0000 0072 1500  ...rd...r....r..
+000039a0: 0000 7211 0000 0072 f800 0000 7272 0000  ..r....r....rr..
+000039b0: 0072 bc00 0000 7265 0000 0072 3e00 0000  .r....re...r>...
+000039c0: 723e 0000 0072 3c00 0000 723f 0000 0072  r>...r<...r?...r
+000039d0: f600 0000 a501 0000 7312 0000 0008 0904  ........s.......
+000039e0: 010a 0104 0104 0218 0310 0304 0114 0672  ...............r
+000039f0: f600 0000 2958 da07 6c6f 6767 696e 67da  ....)X..logging.
+00003a00: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
+00003a10: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+00003a20: da06 646a 616e 676f 7207 0000 00da 0b64  ..djangor......d
+00003a30: 6a61 6e67 6f2e 636f 6e66 7208 0000 005a  jango.confr....Z
+00003a40: 0e64 6a61 6e67 6f2e 636f 6e74 7269 6272  .django.contribr
+00003a50: 0900 0000 da14 646a 616e 676f 2e63 6f6e  ......django.con
+00003a60: 7472 6962 2e61 646d 696e 720a 0000 0072  trib.adminr....r
+00003a70: 0b00 0000 da22 646a 616e 676f 2e63 6f6e  ....."django.con
+00003a80: 7472 6962 2e63 6f6e 7465 6e74 7479 7065  trib.contenttype
+00003a90: 732e 6d6f 6465 6c73 720c 0000 00da 0964  s.modelsr......d
+00003aa0: 6a61 6e67 6f2e 6462 720d 0000 00da 1064  jango.dbr......d
+00003ab0: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 7372  jango.db.modelsr
+00003ac0: 0e00 0000 da0b 646a 616e 676f 2e68 7474  ......django.htt
+00003ad0: 7072 0f00 0000 7210 0000 0072 1100 0000  pr....r....r....
+00003ae0: da10 646a 616e 676f 2e73 686f 7274 6375  ..django.shortcu
+00003af0: 7473 7212 0000 00da 1864 6a61 6e67 6f2e  tsr......django.
+00003b00: 7465 6d70 6c61 7465 2e72 6573 706f 6e73  template.respons
+00003b10: 6572 1300 0000 da0b 646a 616e 676f 2e75  er......django.u
+00003b20: 726c 7372 1400 0000 729c 0000 005a 1e61  rlsr....r....Z.a
+00003b30: 646d 696e 5f65 7874 7261 5f62 7574 746f  dmin_extra_butto
+00003b40: 6e73 2e64 6563 6f72 6174 6f72 7372 1500  ns.decoratorsr..
+00003b50: 0000 5a1a 6164 6d69 6e5f 6578 7472 615f  ..Z.admin_extra_
+00003b60: 6275 7474 6f6e 732e 6d69 7869 6e73 7216  buttons.mixinsr.
+00003b70: 0000 00da 1461 646d 696e 6163 7469 6f6e  .....adminaction
+00003b80: 732e 6865 6c70 6572 7372 1700 0000 5a19  s.helpersr....Z.
+00003b90: 6164 6d69 6e66 696c 7465 7273 2e61 7574  adminfilters.aut
+00003ba0: 6f63 6f6d 706c 6574 6572 1800 0000 da12  ocompleter......
+00003bb0: 6164 6d69 6e66 696c 7465 7273 2e6d 6978  adminfilters.mix
+00003bc0: 696e 7219 0000 00da 0d63 656c 6572 792e  inr......celery.
+00003bd0: 7265 7375 6c74 721a 0000 00da 0d69 6d70  resultr......imp
+00003be0: 6f72 745f 6578 706f 7274 721b 0000 0072  ort_exportr....r
+00003bf0: 1c00 0000 5a13 696d 706f 7274 5f65 7870  ....Z.import_exp
+00003c00: 6f72 742e 6164 6d69 6e72 1d00 0000 5a15  ort.adminr....Z.
+00003c10: 696d 706f 7274 5f65 7870 6f72 742e 7769  import_export.wi
+00003c20: 6467 6574 7372 1e00 0000 da12 736d 6172  dgetsr......smar
+00003c30: 745f 6164 6d69 6e2e 6d69 7869 6e73 721f  t_admin.mixinsr.
+00003c40: 0000 0072 2000 0000 da18 706f 7765 725f  ...r .....power_
+00003c50: 7175 6572 792e 6365 6c65 7279 5f74 6173  query.celery_tas
+00003c60: 6b73 7221 0000 0072 2200 0000 7223 0000  ksr!...r"...r#..
+00003c70: 005a 1170 6f77 6572 5f71 7565 7279 2e66  .Z.power_query.f
+00003c80: 6f72 6d73 7224 0000 005a 1270 6f77 6572  ormsr$...Z.power
+00003c90: 5f71 7565 7279 2e6d 6f64 656c 7372 2500  _query.modelsr%.
+00003ca0: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
+00003cb0: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
+00003cc0: da11 706f 7765 725f 7175 6572 792e 7574  ..power_query.ut
+00003cd0: 696c 7372 2c00 0000 5a12 706f 7765 725f  ilsr,...Z.power_
+00003ce0: 7175 6572 792e 7769 6467 6574 722d 0000  query.widgetr-..
+00003cf0: 0072 2e00 0000 da09 6765 744c 6f67 6765  .r......getLogge
+00003d00: 7272 5e00 0000 72c7 0000 0072 2f00 0000  rr^...r....r/...
+00003d10: 7230 0000 0072 6600 0000 72b2 0000 00da  r0...rf...r.....
+00003d20: 0d4d 6f64 656c 5265 736f 7572 6365 72ca  .ModelResourcer.
+00003d30: 0000 0072 cf00 0000 72e1 0000 0072 e300  ...r....r....r..
+00003d40: 0000 72f3 0000 0072 f600 0000 723e 0000  ..r....r....r>..
+00003d50: 0072 3e00 0000 723e 0000 0072 3f00 0000  .r>...r>...r?...
+00003d60: da08 3c6d 6f64 756c 653e 0100 0000 73ae  ..<module>....s.
+00003d70: 0000 0008 011c 020c 010c 010c 0110 010c  ................
+00003d80: 010c 010c 0114 010c 010c 010c 0208 010c  ................
+00003d90: 010c 010c 010c 010c 010c 0110 010c 010c  ................
+00003da0: 0110 0214 050c 0124 090c 0110 020a 0206  .......$........
+00003db0: 010c 030e 2706 010a 0102 0102 0102 0102  ....'...........
+00003dc0: 0102 0102 0102 f906 6d06 010a 0102 0102  ........m.......
+00003dd0: 0102 0102 0102 fb06 3412 0706 010a 0102  ........4.......
+00003de0: 0102 0102 0102 0102 fb06 3012 0a06 010a  ..........0.....
+00003df0: 0102 0102 0102 0102 0102 0102 0102 f906  ................
+00003e00: 4a06 010a 0102 0102 0102 0102 0102 fb06  J...............
+00003e10: 1906 010a 0102 0102 0102 0102 0102 0102  ................
+00003e20: fa                                       .
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/apps.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/apps.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd7a4af64 (Thu Jul 13 07:16:39 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 119
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/celery_tasks.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/celery_tasks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd9a6af64 (Thu Jul 13 07:25:13 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 3009
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/celery_tasks.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/celery_tasks.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:25:13 2023 UTC, .py size: 3009 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d9a6 af64 c10b 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 cd97 b764 c10b 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2a01 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6401 6c07 5a07 6400 6403 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6400 6404 6c07 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/exceptions.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/exceptions.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x66a4af64 (Thu Jul 13 07:14:46 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 404
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/exceptions.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/exceptions.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:14:46 2023 UTC, .py size: 404 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 66a4 af64 9401 0000  a.......f..d....
+00000000: 610d 0d0a 0000 0000 cd97 b764 9401 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 8303 5a03 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0341 6e79 6300 0000  .....)...Anyc...
 00000060: 0000 0000 0000 0000 0000 0000 0007 0000  ................
 00000070: 0040 0000 0073 3200 0000 6500 5a01 6400  .@...s2...e.Z.d.
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/fixtures.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/fixtures.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/forms.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/forms.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xbca6af64 (Thu Jul 13 07:24:44 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 1438
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/forms.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/forms.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:24:44 2023 UTC, .py size: 1438 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 bca6 af64 9e05 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 cd97 b764 9e05 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6501 6a0a 8303 5a0b 4700 6407 6408 8400  e.j...Z.G.d.d...
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/json.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/json.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x49a2af64 (Thu Jul 13 07:05:45 2023 UTC)
+moddate:  0xd996b764 (Wed Jul 19 07:55:05 2023 UTC)
 files sz: 572
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/json.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/json.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:05:45 2023 UTC, .py size: 572 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 49a2 af64 3c02 0000  a.......I..d<...
+00000000: 610d 0d0a 0000 0000 d996 b764 3c02 0000  a..........d<...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6403 6c07 6d05 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/mixin.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/mixin.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:18:11 2023 UTC, .py size: 753 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 33a5 af64 f102 0000  a.......3..d....
+00000000: 610d 0d0a 0000 0000 cd97 b764 f102 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 4700 6407 6408  d.l.m.Z...G.d.d.
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/models.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/models.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,46 +1,47 @@
 magic:    0xa70d0d0a
-moddate:  0x72a7af64 (Thu Jul 13 07:27:46 2023 UTC)
-files sz: 17115
+moddate:  0x37b3b764 (Wed Jul 19 09:56:07 2023 UTC)
+files sz: 17472
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       026c036d045a046d055a056d065a066d075a076d085a086d095a09010064
-      0064036c0a6d0b5a0b0100640064046c0c6d0d5a0d0100640064056c0e6d
-      0f5a0f0100640064066c106d115a110100640064076c126d135a136d145a
-      140100640064086c156d165a160100640064096c176d185a186d195a1901
-      006400640a6c1a6d1b5a1b01006400640b6c1c6d1d5a1d01006400640c6c
-      1e6d1f5a1f01006400640d6c206d215a2101006400640e6c226d235a2301
-      00640064016c245a246400640f6c246d255a250100640064106c266d275a
-      270100640064116c286d295a290100640064126c2a6d2b5a2b6d2c5a2c01
-      00640064136c2d6d2e5a2e0100640064146c2f6d305a300100640064156c
-      316d325a326d335a330100640064166c346d355a350100020065016a3600
-      000000000000006537a6010000ab0100000000000000005a386417641864
-      19641a641b641c641d641e9c075a39641f84006539a03a00000000000000
-      00000000000000000000000000a6000000ab0000000000000000004400a6
-      000000ab0000000000000000005a3b6508653c6509653d653c6602190000
-      000000000000006602190000000000000000005a3e65066509653e650465
-      3d660319000000000000000000190000000000000000005a3f6508650465
-      046602190000000000000000005a406505653d6509653c653d6602190000
-      000000000000006602190000000000000000005a41642065046421640166
-      04642284045a420200470064238400642465136a430000000000000000a6
-      030000ab0300000000000000005a4402004700642584006426652965136a
-      430000000000000000a6040000ab0400000000000000005a450200470064
-      27840064286529654465136a430000000000000000a6050000ab05000000
-      00000000005a460200470064298400642a652965136a4300000000000000
-      00a6040000ab0400000000000000005a4702004700642b8400642c652965
-      136a430000000000000000a6040000ab0400000000000000005a48020047
-      00642d8400642e6529654465136a430000000000000000a6050000ab0500
-      000000000000005a4902004700642f8400643065136a4a00000000000000
-      00a6030000ab0300000000000000005a4b0200470064318400643265136a
-      430000000000000000a6030000ab0300000000000000005a4c64015300
+      0064036c0a6d0b5a0c0100640064046c0d6d0e5a0e0100640064056c0f6d
+      105a100100640064066c116d125a120100640064076c136d145a14010064
+      0064086c156d165a166d175a170100640064096c186d195a190100640064
+      0a6c1a6d1b5a1b6d1c5a1c01006400640b6c1d6d1e5a1e01006400640c6c
+      1f6d205a2001006400640d6c216d225a2201006400640e6c236d245a2401
+      006400640f6c256d265a260100640064016c275a27640064106c276d285a
+      280100640064116c296d2a5a2a0100640064126c2b6d2c5a2c0100640064
+      136c2d6d2e5a2e6d2f5a2f0100640064146c306d315a310100640064156c
+      326d335a330100640064166c346d355a356d365a360100640064176c376d
+      385a380100020065016a390000000000000000653aa6010000ab01000000
+      00000000005a3b64186419641a641b641c641d641e641f9c075a3c642084
+      00653ca03d0000000000000000000000000000000000000000a6000000ab
+      0000000000000000004400a6000000ab0000000000000000005a3e650865
+      3f65096540653f6602190000000000000000006602190000000000000000
+      005a41650665096541650465406603190000000000000000001900000000
+      00000000005a426508650465046602190000000000000000005a43650565
+      406509653f65406602190000000000000000006602190000000000000000
+      005a4464216504642264016604642384045a450200470064248400642565
+      166a460000000000000000a6030000ab0300000000000000005a47020047
+      00642684006427652c65166a460000000000000000a6040000ab04000000
+      00000000005a4802004700642884006429652c654765166a460000000000
+      000000a6050000ab0500000000000000005a4902004700642a8400642b65
+      2c65166a460000000000000000a6040000ab0400000000000000005a4a02
+      004700642c8400642d652c65166a460000000000000000a6040000ab0400
+      000000000000005a4b02004700642e8400642f652c654765166a46000000
+      0000000000a6050000ab0500000000000000005a4c020047006430840064
+      3165166a4d0000000000000000a6030000ab0300000000000000005a4e02
+      00470064328400643365166a460000000000000000a6030000ab03000000
+      00000000005a4f64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (itertools)
                  8 STORE_NAME               0 (itertools)
    
@@ -68,351 +69,359 @@
                 48 IMPORT_FROM              8 (Tuple)
                 50 STORE_NAME               8 (Tuple)
                 52 IMPORT_FROM              9 (Union)
                 54 STORE_NAME               9 (Union)
                 56 POP_TOP
    
      6          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               3 (('settings',))
-                62 IMPORT_NAME             10 (django.conf)
-                64 IMPORT_FROM             11 (settings)
-                66 STORE_NAME              11 (settings)
+                60 LOAD_CONST               3 (('apps',))
+                62 IMPORT_NAME             10 (django.apps)
+                64 IMPORT_FROM             11 (apps)
+                66 STORE_NAME              12 (django_apps)
                 68 POP_TOP
    
      7          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               4 (('get_user_model',))
-                74 IMPORT_NAME             12 (django.contrib.auth)
-                76 IMPORT_FROM             13 (get_user_model)
-                78 STORE_NAME              13 (get_user_model)
+                72 LOAD_CONST               4 (('settings',))
+                74 IMPORT_NAME             13 (django.conf)
+                76 IMPORT_FROM             14 (settings)
+                78 STORE_NAME              14 (settings)
                 80 POP_TOP
    
      8          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               5 (('ContentType',))
-                86 IMPORT_NAME             14 (django.contrib.contenttypes.models)
-                88 IMPORT_FROM             15 (ContentType)
-                90 STORE_NAME              15 (ContentType)
+                84 LOAD_CONST               5 (('get_user_model',))
+                86 IMPORT_NAME             15 (django.contrib.auth)
+                88 IMPORT_FROM             16 (get_user_model)
+                90 STORE_NAME              16 (get_user_model)
                 92 POP_TOP
    
      9          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               6 (('ValidationError',))
-                98 IMPORT_NAME             16 (django.core.exceptions)
-               100 IMPORT_FROM             17 (ValidationError)
-               102 STORE_NAME              17 (ValidationError)
+                96 LOAD_CONST               6 (('ContentType',))
+                98 IMPORT_NAME             17 (django.contrib.contenttypes.models)
+               100 IMPORT_FROM             18 (ContentType)
+               102 STORE_NAME              18 (ContentType)
                104 POP_TOP
    
     10         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               7 (('models', 'transaction'))
-               110 IMPORT_NAME             18 (django.db)
-               112 IMPORT_FROM             19 (models)
-               114 STORE_NAME              19 (models)
-               116 IMPORT_FROM             20 (transaction)
-               118 STORE_NAME              20 (transaction)
-               120 POP_TOP
-   
-    11         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST               8 (('JSONField',))
-               126 IMPORT_NAME             21 (django.db.models)
-               128 IMPORT_FROM             22 (JSONField)
-               130 STORE_NAME              22 (JSONField)
+               108 LOAD_CONST               7 (('ValidationError',))
+               110 IMPORT_NAME             19 (django.core.exceptions)
+               112 IMPORT_FROM             20 (ValidationError)
+               114 STORE_NAME              20 (ValidationError)
+               116 POP_TOP
+   
+    11         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               8 (('models', 'transaction'))
+               122 IMPORT_NAME             21 (django.db)
+               124 IMPORT_FROM             22 (models)
+               126 STORE_NAME              22 (models)
+               128 IMPORT_FROM             23 (transaction)
+               130 STORE_NAME              23 (transaction)
                132 POP_TOP
    
     12         134 LOAD_CONST               0 (0)
-               136 LOAD_CONST               9 (('Context', 'Template'))
-               138 IMPORT_NAME             23 (django.template)
-               140 IMPORT_FROM             24 (Context)
-               142 STORE_NAME              24 (Context)
-               144 IMPORT_FROM             25 (Template)
-               146 STORE_NAME              25 (Template)
-               148 POP_TOP
-   
-    13         150 LOAD_CONST               0 (0)
-               152 LOAD_CONST              10 (('reverse',))
-               154 IMPORT_NAME             26 (django.urls)
-               156 IMPORT_FROM             27 (reverse)
-               158 STORE_NAME              27 (reverse)
+               136 LOAD_CONST               9 (('JSONField',))
+               138 IMPORT_NAME             24 (django.db.models)
+               140 IMPORT_FROM             25 (JSONField)
+               142 STORE_NAME              25 (JSONField)
+               144 POP_TOP
+   
+    13         146 LOAD_CONST               0 (0)
+               148 LOAD_CONST              10 (('Context', 'Template'))
+               150 IMPORT_NAME             26 (django.template)
+               152 IMPORT_FROM             27 (Context)
+               154 STORE_NAME              27 (Context)
+               156 IMPORT_FROM             28 (Template)
+               158 STORE_NAME              28 (Template)
                160 POP_TOP
    
     14         162 LOAD_CONST               0 (0)
-               164 LOAD_CONST              11 (('timezone',))
-               166 IMPORT_NAME             28 (django.utils)
-               168 IMPORT_FROM             29 (timezone)
-               170 STORE_NAME              29 (timezone)
+               164 LOAD_CONST              11 (('reverse',))
+               166 IMPORT_NAME             29 (django.urls)
+               168 IMPORT_FROM             30 (reverse)
+               170 STORE_NAME              30 (reverse)
                172 POP_TOP
    
     15         174 LOAD_CONST               0 (0)
-               176 LOAD_CONST              12 (('strftime',))
-               178 IMPORT_NAME             30 (django.utils.datetime_safe)
-               180 IMPORT_FROM             31 (strftime)
-               182 STORE_NAME              31 (strftime)
+               176 LOAD_CONST              12 (('timezone',))
+               178 IMPORT_NAME             31 (django.utils)
+               180 IMPORT_FROM             32 (timezone)
+               182 STORE_NAME              32 (timezone)
                184 POP_TOP
    
     16         186 LOAD_CONST               0 (0)
-               188 LOAD_CONST              13 (('cached_property',))
-               190 IMPORT_NAME             32 (django.utils.functional)
-               192 IMPORT_FROM             33 (cached_property)
-               194 STORE_NAME              33 (cached_property)
+               188 LOAD_CONST              13 (('strftime',))
+               190 IMPORT_NAME             33 (django.utils.datetime_safe)
+               192 IMPORT_FROM             34 (strftime)
+               194 STORE_NAME              34 (strftime)
                196 POP_TOP
    
     17         198 LOAD_CONST               0 (0)
-               200 LOAD_CONST              14 (('slugify',))
-               202 IMPORT_NAME             34 (django.utils.text)
-               204 IMPORT_FROM             35 (slugify)
-               206 STORE_NAME              35 (slugify)
+               200 LOAD_CONST              14 (('cached_property',))
+               202 IMPORT_NAME             35 (django.utils.functional)
+               204 IMPORT_FROM             36 (cached_property)
+               206 STORE_NAME              36 (cached_property)
                208 POP_TOP
    
-    19         210 LOAD_CONST               0 (0)
-               212 LOAD_CONST               1 (None)
-               214 IMPORT_NAME             36 (celery)
-               216 STORE_NAME              36 (celery)
-   
-    20         218 LOAD_CONST               0 (0)
-               220 LOAD_CONST              15 (('states',))
-               222 IMPORT_NAME             36 (celery)
-               224 IMPORT_FROM             37 (states)
-               226 STORE_NAME              37 (states)
-               228 POP_TOP
+    18         210 LOAD_CONST               0 (0)
+               212 LOAD_CONST              15 (('slugify',))
+               214 IMPORT_NAME             37 (django.utils.text)
+               216 IMPORT_FROM             38 (slugify)
+               218 STORE_NAME              38 (slugify)
+               220 POP_TOP
+   
+    20         222 LOAD_CONST               0 (0)
+               224 LOAD_CONST               1 (None)
+               226 IMPORT_NAME             39 (celery)
+               228 STORE_NAME              39 (celery)
    
     21         230 LOAD_CONST               0 (0)
-               232 LOAD_CONST              16 (('AsyncResult',))
-               234 IMPORT_NAME             38 (celery.result)
-               236 IMPORT_FROM             39 (AsyncResult)
-               238 STORE_NAME              39 (AsyncResult)
+               232 LOAD_CONST              16 (('states',))
+               234 IMPORT_NAME             39 (celery)
+               236 IMPORT_FROM             40 (states)
+               238 STORE_NAME              40 (states)
                240 POP_TOP
    
     22         242 LOAD_CONST               0 (0)
-               244 LOAD_CONST              17 (('NaturalKeyModel',))
-               246 IMPORT_NAME             40 (natural_keys)
-               248 IMPORT_FROM             41 (NaturalKeyModel)
-               250 STORE_NAME              41 (NaturalKeyModel)
+               244 LOAD_CONST              17 (('AsyncResult',))
+               246 IMPORT_NAME             41 (celery.result)
+               248 IMPORT_FROM             42 (AsyncResult)
+               250 STORE_NAME              42 (AsyncResult)
                252 POP_TOP
    
     23         254 LOAD_CONST               0 (0)
-               256 LOAD_CONST              18 (('capture_exception', 'configure_scope'))
-               258 IMPORT_NAME             42 (sentry_sdk)
-               260 IMPORT_FROM             43 (capture_exception)
-               262 STORE_NAME              43 (capture_exception)
-               264 IMPORT_FROM             44 (configure_scope)
-               266 STORE_NAME              44 (configure_scope)
-               268 POP_TOP
-   
-    25         270 LOAD_CONST               0 (0)
-               272 LOAD_CONST              19 (('QueryRunError',))
-               274 IMPORT_NAME             45 (power_query.exceptions)
-               276 IMPORT_FROM             46 (QueryRunError)
-               278 STORE_NAME              46 (QueryRunError)
+               256 LOAD_CONST              18 (('NaturalKeyModel',))
+               258 IMPORT_NAME             43 (natural_keys)
+               260 IMPORT_FROM             44 (NaturalKeyModel)
+               262 STORE_NAME              44 (NaturalKeyModel)
+               264 POP_TOP
+   
+    24         266 LOAD_CONST               0 (0)
+               268 LOAD_CONST              19 (('capture_exception', 'configure_scope'))
+               270 IMPORT_NAME             45 (sentry_sdk)
+               272 IMPORT_FROM             46 (capture_exception)
+               274 STORE_NAME              46 (capture_exception)
+               276 IMPORT_FROM             47 (configure_scope)
+               278 STORE_NAME              47 (configure_scope)
                280 POP_TOP
    
     26         282 LOAD_CONST               0 (0)
-               284 LOAD_CONST              20 (('PQJSONEncoder',))
-               286 IMPORT_NAME             47 (power_query.json)
-               288 IMPORT_FROM             48 (PQJSONEncoder)
-               290 STORE_NAME              48 (PQJSONEncoder)
+               284 LOAD_CONST              20 (('QueryRunError',))
+               286 IMPORT_NAME             48 (power_query.exceptions)
+               288 IMPORT_FROM             49 (QueryRunError)
+               290 STORE_NAME              49 (QueryRunError)
                292 POP_TOP
    
     27         294 LOAD_CONST               0 (0)
-               296 LOAD_CONST              21 (('dict_hash', 'to_dataset'))
-               298 IMPORT_NAME             49 (power_query.utils)
-               300 IMPORT_FROM             50 (dict_hash)
-               302 STORE_NAME              50 (dict_hash)
-               304 IMPORT_FROM             51 (to_dataset)
-               306 STORE_NAME              51 (to_dataset)
-               308 POP_TOP
-   
-    28         310 LOAD_CONST               0 (0)
-               312 LOAD_CONST              22 (('FrequencyValidator',))
-               314 IMPORT_NAME             52 (power_query.validators)
-               316 IMPORT_FROM             53 (FrequencyValidator)
-               318 STORE_NAME              53 (FrequencyValidator)
+               296 LOAD_CONST              21 (('PQJSONEncoder',))
+               298 IMPORT_NAME             50 (power_query.json)
+               300 IMPORT_FROM             51 (PQJSONEncoder)
+               302 STORE_NAME              51 (PQJSONEncoder)
+               304 POP_TOP
+   
+    28         306 LOAD_CONST               0 (0)
+               308 LOAD_CONST              22 (('dict_hash', 'to_dataset'))
+               310 IMPORT_NAME             52 (power_query.utils)
+               312 IMPORT_FROM             53 (dict_hash)
+               314 STORE_NAME              53 (dict_hash)
+               316 IMPORT_FROM             54 (to_dataset)
+               318 STORE_NAME              54 (to_dataset)
                320 POP_TOP
    
-    30         322 PUSH_NULL
-               324 LOAD_NAME                1 (logging)
-               326 LOAD_ATTR               54 (getLogger)
-               336 LOAD_NAME               55 (__name__)
-               338 PRECALL                  1
-               342 CALL                     1
-               352 STORE_NAME              56 (logger)
-   
-    33         354 LOAD_CONST              23 ('text/csv')
-   
-    34         356 LOAD_CONST              24 ('text/html')
-   
-    35         358 LOAD_CONST              25 ('application/json')
-   
-    36         360 LOAD_CONST              26 ('text/plain')
-   
-    37         362 LOAD_CONST              27 ('application/vnd.ms-excel')
-   
-    38         364 LOAD_CONST              28 ('application/xml')
-   
-    39         366 LOAD_CONST              29 ('text/yaml')
-   
-    32         368 LOAD_CONST              30 (('csv', 'html', 'json', 'txt', 'xls', 'xml', 'yaml'))
-               370 BUILD_CONST_KEY_MAP      7
-               372 STORE_NAME              57 (mimetype_map)
-   
-    42         374 LOAD_CONST              31 (<code object <genexpr>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 42>)
-               376 MAKE_FUNCTION            0
-               378 LOAD_NAME               57 (mimetype_map)
-               380 LOAD_METHOD             58 (items)
-               402 PRECALL                  0
-               406 CALL                     0
-               416 GET_ITER
-               418 PRECALL                  0
-               422 CALL                     0
-               432 STORE_NAME              59 (MIMETYPES)
-   
-    44         434 LOAD_NAME                8 (Tuple)
-               436 LOAD_NAME               60 (int)
-               438 LOAD_NAME                9 (Union)
-               440 LOAD_NAME               61 (str)
-               442 LOAD_NAME               60 (int)
-               444 BUILD_TUPLE              2
-               446 BINARY_SUBSCR
+    29         322 LOAD_CONST               0 (0)
+               324 LOAD_CONST              23 (('FrequencyValidator',))
+               326 IMPORT_NAME             55 (power_query.validators)
+               328 IMPORT_FROM             56 (FrequencyValidator)
+               330 STORE_NAME              56 (FrequencyValidator)
+               332 POP_TOP
+   
+    31         334 PUSH_NULL
+               336 LOAD_NAME                1 (logging)
+               338 LOAD_ATTR               57 (getLogger)
+               348 LOAD_NAME               58 (__name__)
+               350 PRECALL                  1
+               354 CALL                     1
+               364 STORE_NAME              59 (logger)
+   
+    34         366 LOAD_CONST              24 ('text/csv')
+   
+    35         368 LOAD_CONST              25 ('text/html')
+   
+    36         370 LOAD_CONST              26 ('application/json')
+   
+    37         372 LOAD_CONST              27 ('text/plain')
+   
+    38         374 LOAD_CONST              28 ('application/vnd.ms-excel')
+   
+    39         376 LOAD_CONST              29 ('application/xml')
+   
+    40         378 LOAD_CONST              30 ('text/yaml')
+   
+    33         380 LOAD_CONST              31 (('csv', 'html', 'json', 'txt', 'xls', 'xml', 'yaml'))
+               382 BUILD_CONST_KEY_MAP      7
+               384 STORE_NAME              60 (mimetype_map)
+   
+    43         386 LOAD_CONST              32 (<code object <genexpr>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 43>)
+               388 MAKE_FUNCTION            0
+               390 LOAD_NAME               60 (mimetype_map)
+               392 LOAD_METHOD             61 (items)
+               414 PRECALL                  0
+               418 CALL                     0
+               428 GET_ITER
+               430 PRECALL                  0
+               434 CALL                     0
+               444 STORE_NAME              62 (MIMETYPES)
+   
+    45         446 LOAD_NAME                8 (Tuple)
+               448 LOAD_NAME               63 (int)
+               450 LOAD_NAME                9 (Union)
+               452 LOAD_NAME               64 (str)
+               454 LOAD_NAME               63 (int)
                456 BUILD_TUPLE              2
                458 BINARY_SUBSCR
-               468 STORE_NAME              62 (DocumentResult)
-   
-    45         470 LOAD_NAME                6 (List)
-               472 LOAD_NAME                9 (Union)
-               474 LOAD_NAME               62 (DocumentResult)
-               476 LOAD_NAME                4 (Any)
-               478 LOAD_NAME               61 (str)
-               480 BUILD_TUPLE              3
-               482 BINARY_SUBSCR
-               492 BINARY_SUBSCR
-               502 STORE_NAME              63 (ReportResult)
-   
-    46         504 LOAD_NAME                8 (Tuple)
-               506 LOAD_NAME                4 (Any)
-               508 LOAD_NAME                4 (Any)
-               510 BUILD_TUPLE              2
-               512 BINARY_SUBSCR
-               522 STORE_NAME              64 (QueryResult)
-   
-    47         524 LOAD_NAME                5 (Dict)
-               526 LOAD_NAME               61 (str)
-               528 LOAD_NAME                9 (Union)
-               530 LOAD_NAME               60 (int)
-               532 LOAD_NAME               61 (str)
-               534 BUILD_TUPLE              2
-               536 BINARY_SUBSCR
+               468 BUILD_TUPLE              2
+               470 BINARY_SUBSCR
+               480 STORE_NAME              65 (DocumentResult)
+   
+    46         482 LOAD_NAME                6 (List)
+               484 LOAD_NAME                9 (Union)
+               486 LOAD_NAME               65 (DocumentResult)
+               488 LOAD_NAME                4 (Any)
+               490 LOAD_NAME               64 (str)
+               492 BUILD_TUPLE              3
+               494 BINARY_SUBSCR
+               504 BINARY_SUBSCR
+               514 STORE_NAME              66 (ReportResult)
+   
+    47         516 LOAD_NAME                8 (Tuple)
+               518 LOAD_NAME                4 (Any)
+               520 LOAD_NAME                4 (Any)
+               522 BUILD_TUPLE              2
+               524 BINARY_SUBSCR
+               534 STORE_NAME              67 (QueryResult)
+   
+    48         536 LOAD_NAME                5 (Dict)
+               538 LOAD_NAME               64 (str)
+               540 LOAD_NAME                9 (Union)
+               542 LOAD_NAME               63 (int)
+               544 LOAD_NAME               64 (str)
                546 BUILD_TUPLE              2
                548 BINARY_SUBSCR
-               558 STORE_NAME              65 (QueryMatrixResult)
-   
-    50         560 LOAD_CONST              32 ('value')
-               562 LOAD_NAME                4 (Any)
-               564 LOAD_CONST              33 ('return')
-               566 LOAD_CONST               1 (None)
-               568 BUILD_TUPLE              4
-               570 LOAD_CONST              34 (<code object validate_queryargs, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 50>)
-               572 MAKE_FUNCTION            4 (annotations)
-               574 STORE_NAME              66 (validate_queryargs)
-   
-    65         576 PUSH_NULL
-               578 LOAD_BUILD_CLASS
-               580 LOAD_CONST              35 (<code object CeleryEnabled, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 65>)
-               582 MAKE_FUNCTION            0
-               584 LOAD_CONST              36 ('CeleryEnabled')
-               586 LOAD_NAME               19 (models)
-               588 LOAD_ATTR               67 (Model)
-               598 PRECALL                  3
-               602 CALL                     3
-               612 STORE_NAME              68 (CeleryEnabled)
-   
-   104         614 PUSH_NULL
-               616 LOAD_BUILD_CLASS
-               618 LOAD_CONST              37 (<code object Parametrizer, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 104>)
-               620 MAKE_FUNCTION            0
-               622 LOAD_CONST              38 ('Parametrizer')
-               624 LOAD_NAME               41 (NaturalKeyModel)
-               626 LOAD_NAME               19 (models)
-               628 LOAD_ATTR               67 (Model)
-               638 PRECALL                  4
-               642 CALL                     4
-               652 STORE_NAME              69 (Parametrizer)
-   
-   150         654 PUSH_NULL
-               656 LOAD_BUILD_CLASS
-               658 LOAD_CONST              39 (<code object Query, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 150>)
-               660 MAKE_FUNCTION            0
-               662 LOAD_CONST              40 ('Query')
-               664 LOAD_NAME               41 (NaturalKeyModel)
-               666 LOAD_NAME               68 (CeleryEnabled)
-               668 LOAD_NAME               19 (models)
-               670 LOAD_ATTR               67 (Model)
-               680 PRECALL                  5
-               684 CALL                     5
-               694 STORE_NAME              70 (Query)
-   
-   310         696 PUSH_NULL
-               698 LOAD_BUILD_CLASS
-               700 LOAD_CONST              41 (<code object Dataset, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 310>)
-               702 MAKE_FUNCTION            0
-               704 LOAD_CONST              42 ('Dataset')
-               706 LOAD_NAME               41 (NaturalKeyModel)
-               708 LOAD_NAME               19 (models)
-               710 LOAD_ATTR               67 (Model)
-               720 PRECALL                  4
-               724 CALL                     4
-               734 STORE_NAME              71 (Dataset)
-   
-   337         736 PUSH_NULL
-               738 LOAD_BUILD_CLASS
-               740 LOAD_CONST              43 (<code object Formatter, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 337>)
-               742 MAKE_FUNCTION            0
-               744 LOAD_CONST              44 ('Formatter')
-               746 LOAD_NAME               41 (NaturalKeyModel)
-               748 LOAD_NAME               19 (models)
-               750 LOAD_ATTR               67 (Model)
-               760 PRECALL                  4
-               764 CALL                     4
-               774 STORE_NAME              72 (Formatter)
-   
-   364         776 PUSH_NULL
-               778 LOAD_BUILD_CLASS
-               780 LOAD_CONST              45 (<code object Report, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 364>)
-               782 MAKE_FUNCTION            0
-               784 LOAD_CONST              46 ('Report')
-               786 LOAD_NAME               41 (NaturalKeyModel)
-               788 LOAD_NAME               68 (CeleryEnabled)
-               790 LOAD_NAME               19 (models)
-               792 LOAD_ATTR               67 (Model)
-               802 PRECALL                  5
-               806 CALL                     5
-               816 STORE_NAME              73 (Report)
-   
-   463         818 PUSH_NULL
-               820 LOAD_BUILD_CLASS
-               822 LOAD_CONST              47 (<code object ReportDocumentManager, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 463>)
-               824 MAKE_FUNCTION            0
-               826 LOAD_CONST              48 ('ReportDocumentManager')
-               828 LOAD_NAME               19 (models)
-               830 LOAD_ATTR               74 (Manager)
-               840 PRECALL                  3
-               844 CALL                     3
-               854 STORE_NAME              75 (ReportDocumentManager)
-   
-   468         856 PUSH_NULL
-               858 LOAD_BUILD_CLASS
-               860 LOAD_CONST              49 (<code object ReportDocument, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 468>)
-               862 MAKE_FUNCTION            0
-               864 LOAD_CONST              50 ('ReportDocument')
-               866 LOAD_NAME               19 (models)
-               868 LOAD_ATTR               67 (Model)
-               878 PRECALL                  3
-               882 CALL                     3
-               892 STORE_NAME              76 (ReportDocument)
-               894 LOAD_CONST               1 (None)
-               896 RETURN_VALUE
+               558 BUILD_TUPLE              2
+               560 BINARY_SUBSCR
+               570 STORE_NAME              68 (QueryMatrixResult)
+   
+    51         572 LOAD_CONST              33 ('value')
+               574 LOAD_NAME                4 (Any)
+               576 LOAD_CONST              34 ('return')
+               578 LOAD_CONST               1 (None)
+               580 BUILD_TUPLE              4
+               582 LOAD_CONST              35 (<code object validate_queryargs, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 51>)
+               584 MAKE_FUNCTION            4 (annotations)
+               586 STORE_NAME              69 (validate_queryargs)
+   
+    66         588 PUSH_NULL
+               590 LOAD_BUILD_CLASS
+               592 LOAD_CONST              36 (<code object CeleryEnabled, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 66>)
+               594 MAKE_FUNCTION            0
+               596 LOAD_CONST              37 ('CeleryEnabled')
+               598 LOAD_NAME               22 (models)
+               600 LOAD_ATTR               70 (Model)
+               610 PRECALL                  3
+               614 CALL                     3
+               624 STORE_NAME              71 (CeleryEnabled)
+   
+   105         626 PUSH_NULL
+               628 LOAD_BUILD_CLASS
+               630 LOAD_CONST              38 (<code object Parametrizer, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 105>)
+               632 MAKE_FUNCTION            0
+               634 LOAD_CONST              39 ('Parametrizer')
+               636 LOAD_NAME               44 (NaturalKeyModel)
+               638 LOAD_NAME               22 (models)
+               640 LOAD_ATTR               70 (Model)
+               650 PRECALL                  4
+               654 CALL                     4
+               664 STORE_NAME              72 (Parametrizer)
+   
+   152         666 PUSH_NULL
+               668 LOAD_BUILD_CLASS
+               670 LOAD_CONST              40 (<code object Query, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 152>)
+               672 MAKE_FUNCTION            0
+               674 LOAD_CONST              41 ('Query')
+               676 LOAD_NAME               44 (NaturalKeyModel)
+               678 LOAD_NAME               71 (CeleryEnabled)
+               680 LOAD_NAME               22 (models)
+               682 LOAD_ATTR               70 (Model)
+               692 PRECALL                  5
+               696 CALL                     5
+               706 STORE_NAME              73 (Query)
+   
+   319         708 PUSH_NULL
+               710 LOAD_BUILD_CLASS
+               712 LOAD_CONST              42 (<code object Dataset, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 319>)
+               714 MAKE_FUNCTION            0
+               716 LOAD_CONST              43 ('Dataset')
+               718 LOAD_NAME               44 (NaturalKeyModel)
+               720 LOAD_NAME               22 (models)
+               722 LOAD_ATTR               70 (Model)
+               732 PRECALL                  4
+               736 CALL                     4
+               746 STORE_NAME              74 (Dataset)
+   
+   346         748 PUSH_NULL
+               750 LOAD_BUILD_CLASS
+               752 LOAD_CONST              44 (<code object Formatter, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 346>)
+               754 MAKE_FUNCTION            0
+               756 LOAD_CONST              45 ('Formatter')
+               758 LOAD_NAME               44 (NaturalKeyModel)
+               760 LOAD_NAME               22 (models)
+               762 LOAD_ATTR               70 (Model)
+               772 PRECALL                  4
+               776 CALL                     4
+               786 STORE_NAME              75 (Formatter)
+   
+   373         788 PUSH_NULL
+               790 LOAD_BUILD_CLASS
+               792 LOAD_CONST              46 (<code object Report, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 373>)
+               794 MAKE_FUNCTION            0
+               796 LOAD_CONST              47 ('Report')
+               798 LOAD_NAME               44 (NaturalKeyModel)
+               800 LOAD_NAME               71 (CeleryEnabled)
+               802 LOAD_NAME               22 (models)
+               804 LOAD_ATTR               70 (Model)
+               814 PRECALL                  5
+               818 CALL                     5
+               828 STORE_NAME              76 (Report)
+   
+   472         830 PUSH_NULL
+               832 LOAD_BUILD_CLASS
+               834 LOAD_CONST              48 (<code object ReportDocumentManager, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 472>)
+               836 MAKE_FUNCTION            0
+               838 LOAD_CONST              49 ('ReportDocumentManager')
+               840 LOAD_NAME               22 (models)
+               842 LOAD_ATTR               77 (Manager)
+               852 PRECALL                  3
+               856 CALL                     3
+               866 STORE_NAME              78 (ReportDocumentManager)
+   
+   477         868 PUSH_NULL
+               870 LOAD_BUILD_CLASS
+               872 LOAD_CONST              50 (<code object ReportDocument, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 477>)
+               874 MAKE_FUNCTION            0
+               876 LOAD_CONST              51 ('ReportDocument')
+               878 LOAD_NAME               22 (models)
+               880 LOAD_ATTR               70 (Model)
+               890 PRECALL                  3
+               894 CALL                     3
+               904 STORE_NAME              79 (ReportDocument)
+               906 LOAD_CONST               1 (None)
+               908 RETURN_VALUE
    consts
       0
       None
       ('Any', 'Dict', 'List', 'Optional', 'Tuple', 'Union')
+      ('apps',)
       ('settings',)
       ('get_user_model',)
       ('ContentType',)
       ('ValidationError',)
       ('models', 'transaction')
       ('JSONField',)
       ('Context', 'Template')
@@ -441,15 +450,15 @@
          argcount  : 1
          nlocals   : 3
          stacksize : 3
          flags     : 35
          code
             0x4b00010097007c005d0b5c0200007d017d027c017c0266025600970101
             008c0c64005300
-          42           0 RETURN_GENERATOR
+          43           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
                        6 LOAD_FAST                0 (.0)
                  >>    8 FOR_ITER                11 (to 32)
                       10 UNPACK_SEQUENCE          2
                       14 STORE_FAST               1 (k)
                       16 STORE_FAST               2 (v)
@@ -466,15 +475,15 @@
             None
          names      ()
          varnames   ('.0', 'k', 'v')
          freevars   ()
          cellvars   ()
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       '<genexpr>'
-         firstlineno 42
+         firstlineno 43
          lnotab 0x
       'value'
       'return'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
@@ -488,87 +497,87 @@
             008e00a6010000ab0100000000000000007d0188006601640284087c0144
             00a6000000ab000000000000000000010064005300230074040000000000
             00000000002400720201008200740e00000000000000000000240072197d
             02740500000000000000000000640389007c0264049c02ac05a6020000ab
             020000000000000000820164007d027e0277017700780359007701
                        0 MAKE_CELL                0 (value)
          
-          50           2 RESUME                   0
+          51           2 RESUME                   0
          
-          51           4 NOP
+          52           4 NOP
          
-          52           6 LOAD_GLOBAL              1 (NULL + isinstance)
+          53           6 LOAD_GLOBAL              1 (NULL + isinstance)
                       18 LOAD_DEREF               0 (value)
                       20 LOAD_GLOBAL              2 (dict)
                       32 PRECALL                  2
                       36 CALL                     2
                       46 POP_JUMP_FORWARD_IF_TRUE    15 (to 78)
          
-          53          48 LOAD_GLOBAL              5 (NULL + ValidationError)
+          54          48 LOAD_GLOBAL              5 (NULL + ValidationError)
                       60 LOAD_CONST               1 ('QueryArgs must be a dict')
                       62 PRECALL                  1
                       66 CALL                     1
                       76 RAISE_VARARGS            1
          
-          54     >>   78 LOAD_GLOBAL              7 (NULL + list)
+          55     >>   78 LOAD_GLOBAL              7 (NULL + list)
                       90 LOAD_GLOBAL              9 (NULL + itertools)
                      102 LOAD_ATTR                5 (product)
                      112 LOAD_DEREF               0 (value)
                      114 LOAD_METHOD              6 (values)
                      136 PRECALL                  0
                      140 CALL                     0
                      150 CALL_FUNCTION_EX         0
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_FAST               1 (product)
          
-          55         168 LOAD_CLOSURE             0 (value)
+          56         168 LOAD_CLOSURE             0 (value)
                      170 BUILD_TUPLE              1
-                     172 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 55>)
+                     172 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 56>)
                      174 MAKE_FUNCTION            8 (closure)
                      176 LOAD_FAST                1 (product)
                      178 GET_ITER
                      180 PRECALL                  0
                      184 CALL                     0
                      194 POP_TOP
                      196 LOAD_CONST               0 (None)
                      198 RETURN_VALUE
                  >>  200 PUSH_EXC_INFO
          
-          56         202 LOAD_GLOBAL              4 (ValidationError)
+          57         202 LOAD_GLOBAL              4 (ValidationError)
                      214 CHECK_EXC_MATCH
                      216 POP_JUMP_FORWARD_IF_FALSE     2 (to 222)
                      218 POP_TOP
          
-          57         220 RAISE_VARARGS            0
+          58         220 RAISE_VARARGS            0
          
-          58     >>  222 LOAD_GLOBAL             14 (Exception)
+          59     >>  222 LOAD_GLOBAL             14 (Exception)
                      234 CHECK_EXC_MATCH
                      236 POP_JUMP_FORWARD_IF_FALSE    25 (to 288)
                      238 STORE_FAST               2 (e)
          
-          59         240 LOAD_GLOBAL              5 (NULL + ValidationError)
+          60         240 LOAD_GLOBAL              5 (NULL + ValidationError)
          
-          60         252 LOAD_CONST               3 ('%(exc)s: %(value)s is not a valid QueryArgs')
+          61         252 LOAD_CONST               3 ('%(exc)s: %(value)s is not a valid QueryArgs')
          
-          61         254 LOAD_DEREF               0 (value)
+          62         254 LOAD_DEREF               0 (value)
                      256 LOAD_FAST                2 (e)
                      258 LOAD_CONST               4 (('value', 'exc'))
                      260 BUILD_CONST_KEY_MAP      2
          
-          59         262 KW_NAMES                 5
+          60         262 KW_NAMES                 5
                      264 PRECALL                  2
                      268 CALL                     2
                      278 RAISE_VARARGS            1
                  >>  280 LOAD_CONST               0 (None)
                      282 STORE_FAST               2 (e)
                      284 DELETE_FAST              2 (e)
                      286 RERAISE                  1
          
-          58     >>  288 RERAISE                  0
+          59     >>  288 RERAISE                  0
                  >>  290 COPY                     3
                      292 POP_EXCEPT
                      294 RERAISE                  1
          ExceptionTable:
            6 to 194 -> 200 [0]
            200 to 238 -> 290 [1] lasti
            240 to 278 -> 280 [1] lasti
@@ -584,15 +593,15 @@
                code
                   0x9501970067007c005d317d017401000000000000000000007403000000
                   000000000000008902a00200000000000000000000000000000000000000
                   00a6000000ab0000000000000000007c01a6020000ab0200000000000000
                   00a6010000ab01000000000000000091028c325300
                              0 COPY_FREE_VARS           1
                
-                55           2 RESUME                   0
+                56           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                49 (to 108)
                             10 STORE_FAST               1 (e)
                             12 LOAD_GLOBAL              1 (NULL + dict)
                             24 LOAD_GLOBAL              3 (NULL + zip)
                             36 LOAD_DEREF               2 (value)
@@ -610,26 +619,26 @@
                consts
                names      ('dict', 'zip', 'keys')
                varnames   ('.0', 'e')
                freevars   ('value',)
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '<listcomp>'
-               firstlineno 55
+               firstlineno 56
                lnotab 0x
             '%(exc)s: %(value)s is not a valid QueryArgs'
             ('value', 'exc')
             ('params',)
          names      ('isinstance', 'dict', 'ValidationError', 'list', 'itertools', 'product', 'values', 'Exception')
          varnames   ('value', 'product', 'e')
          freevars   ()
          cellvars   ('value',)
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'validate_queryargs'
-         firstlineno 50
+         firstlineno 51
          lnotab 0x040102012a011e015a0122011201020112010c01020108fe1aff
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
@@ -637,92 +646,92 @@
             06000000000000000065046a07000000000000000065046a080000000000
             0000006804a6010000ab0100000000000000005a090200650a6a0b000000
             0000000000640164026402ac03a6030000ab0300000000000000005a0c02
             004700640484006405a6020000ab0200000000000000005a0d6406650e66
             02640784045a0f6510640665116512190000000000000000006602640884
             04a6000000ab0000000000000000005a1364066511650e19000000000000
             0000006602640984045a146406650e6602640a84045a15640b5300
-          65           0 RESUME                   0
+          66           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CeleryEnabled')
                        8 STORE_NAME               2 (__qualname__)
          
-          66          10 PUSH_NULL
+          67          10 PUSH_NULL
                       12 LOAD_NAME                3 (frozenset)
          
-          67          14 LOAD_NAME                4 (states)
+          68          14 LOAD_NAME                4 (states)
                       16 LOAD_ATTR                5 (PENDING)
                       26 LOAD_NAME                4 (states)
                       28 LOAD_ATTR                6 (RECEIVED)
                       38 LOAD_NAME                4 (states)
                       40 LOAD_ATTR                7 (STARTED)
                       50 LOAD_NAME                4 (states)
                       52 LOAD_ATTR                8 (RETRY)
                       62 BUILD_SET                4
          
-          66          64 PRECALL                  1
+          67          64 PRECALL                  1
                       68 CALL                     1
                       78 STORE_NAME               9 (SCHEDULED)
          
-          70          80 PUSH_NULL
+          71          80 PUSH_NULL
                       82 LOAD_NAME               10 (models)
                       84 LOAD_ATTR               11 (CharField)
                       94 LOAD_CONST               1 (36)
                       96 LOAD_CONST               2 (True)
                       98 LOAD_CONST               2 (True)
                      100 KW_NAMES                 3
                      102 PRECALL                  3
                      106 CALL                     3
                      116 STORE_NAME              12 (celery_task)
          
-          72         118 PUSH_NULL
+          73         118 PUSH_NULL
                      120 LOAD_BUILD_CLASS
-                     122 LOAD_CONST               4 (<code object Meta, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 72>)
+                     122 LOAD_CONST               4 (<code object Meta, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 73>)
                      124 MAKE_FUNCTION            0
                      126 LOAD_CONST               5 ('Meta')
                      128 PRECALL                  2
                      132 CALL                     2
                      142 STORE_NAME              13 (Meta)
          
-          75         144 LOAD_CONST               6 ('return')
+          76         144 LOAD_CONST               6 ('return')
                      146 LOAD_NAME               14 (str)
                      148 BUILD_TUPLE              2
-                     150 LOAD_CONST               7 (<code object status, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 75>)
+                     150 LOAD_CONST               7 (<code object status, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 76>)
                      152 MAKE_FUNCTION            4 (annotations)
                      154 STORE_NAME              15 (status)
          
-          85         156 LOAD_NAME               16 (property)
+          86         156 LOAD_NAME               16 (property)
          
-          86         158 LOAD_CONST               6 ('return')
+          87         158 LOAD_CONST               6 ('return')
                      160 LOAD_NAME               17 (Optional)
                      162 LOAD_NAME               18 (AsyncResult)
                      164 BINARY_SUBSCR
                      174 BUILD_TUPLE              2
-                     176 LOAD_CONST               8 (<code object async_result, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 85>)
+                     176 LOAD_CONST               8 (<code object async_result, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 86>)
                      178 MAKE_FUNCTION            4 (annotations)
          
-          85         180 PRECALL                  0
+          86         180 PRECALL                  0
                      184 CALL                     0
          
-          86         194 STORE_NAME              19 (async_result)
+          87         194 STORE_NAME              19 (async_result)
          
-          92         196 LOAD_CONST               6 ('return')
+          93         196 LOAD_CONST               6 ('return')
                      198 LOAD_NAME               17 (Optional)
                      200 LOAD_NAME               14 (str)
                      202 BINARY_SUBSCR
                      212 BUILD_TUPLE              2
-                     214 LOAD_CONST               9 (<code object queue, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 92>)
+                     214 LOAD_CONST               9 (<code object queue, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 93>)
                      216 MAKE_FUNCTION            4 (annotations)
                      218 STORE_NAME              20 (queue)
          
-         100         220 LOAD_CONST               6 ('return')
+         101         220 LOAD_CONST               6 ('return')
                      222 LOAD_NAME               14 (str)
                      224 BUILD_TUPLE              2
-                     226 LOAD_CONST              10 (<code object _queue, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 100>)
+                     226 LOAD_CONST              10 (<code object _queue, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 101>)
                      228 MAKE_FUNCTION            4 (annotations)
                      230 STORE_NAME              21 (_queue)
                      232 LOAD_CONST              11 (None)
                      234 RETURN_VALUE
          consts
             'CeleryEnabled'
             36
@@ -730,93 +739,93 @@
             ('max_length', 'blank', 'null')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-                72           0 RESUME                   0
+                73           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('CeleryEnabled.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                73          10 LOAD_CONST               1 (True)
+                74          10 LOAD_CONST               1 (True)
                             12 STORE_NAME               3 (abstract)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'CeleryEnabled.Meta'
                   True
                   None
                names      ('__name__', '__module__', '__qualname__', 'abstract')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'Meta'
-               firstlineno 72
+               firstlineno 73
                lnotab 0x0a01
             'Meta'
             'return'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000723409007c006a0100000000000000
                   006a0200000000000000007d016e28230074060000000000000000000024
                   0072197d027409000000000000000000007c02a6010000ab010000000000
                   0000007d01590064007d027e026e0a64007d027e02770177007803590077
                   0164017d017c015300
-                75           0 RESUME                   0
+                76           0 RESUME                   0
                
-                76           2 LOAD_FAST                0 (self)
+                77           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (celery_task)
                             14 POP_JUMP_FORWARD_IF_FALSE    52 (to 120)
                
-                77          16 NOP
+                78          16 NOP
                
-                78          18 LOAD_FAST                0 (self)
+                79          18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (async_result)
                             30 LOAD_ATTR                2 (state)
                             40 STORE_FAST               1 (result)
                             42 JUMP_FORWARD            40 (to 124)
                        >>   44 PUSH_EXC_INFO
                
-                79          46 LOAD_GLOBAL              6 (Exception)
+                80          46 LOAD_GLOBAL              6 (Exception)
                             58 CHECK_EXC_MATCH
                             60 POP_JUMP_FORWARD_IF_FALSE    25 (to 112)
                             62 STORE_FAST               2 (e)
                
-                80          64 LOAD_GLOBAL              9 (NULL + str)
+                81          64 LOAD_GLOBAL              9 (NULL + str)
                             76 LOAD_FAST                2 (e)
                             78 PRECALL                  1
                             82 CALL                     1
                             92 STORE_FAST               1 (result)
                             94 POP_EXCEPT
                             96 LOAD_CONST               0 (None)
                             98 STORE_FAST               2 (e)
                            100 DELETE_FAST              2 (e)
                            102 JUMP_FORWARD            10 (to 124)
                        >>  104 LOAD_CONST               0 (None)
                            106 STORE_FAST               2 (e)
                            108 DELETE_FAST              2 (e)
                            110 RERAISE                  1
                
-                79     >>  112 RERAISE                  0
+                80     >>  112 RERAISE                  0
                        >>  114 COPY                     3
                            116 POP_EXCEPT
                            118 RERAISE                  1
                
-                82     >>  120 LOAD_CONST               1 ('Not scheduled')
+                83     >>  120 LOAD_CONST               1 ('Not scheduled')
                            122 STORE_FAST               1 (result)
                
-                83     >>  124 LOAD_FAST                1 (result)
+                84     >>  124 LOAD_FAST                1 (result)
                            126 RETURN_VALUE
                ExceptionTable:
                  18 to 40 -> 44 [0]
                  44 to 62 -> 114 [1] lasti
                  64 to 92 -> 104 [1] lasti
                  104 to 112 -> 114 [1] lasti
                consts
@@ -824,140 +833,140 @@
                   'Not scheduled'
                names      ('celery_task', 'async_result', 'state', 'Exception', 'str')
                varnames   ('self', 'result', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'status'
-               firstlineno 75
+               firstlineno 76
                lnotab 0x02010e0102011c01120130ff08030401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000722e7c006a0100000000000000007c
                   006a020000000000000000760172207407000000000000000000007c006a
                   0000000000000000007408000000000000000000006a0500000000000000
                   00ac01a6020000ab020000000000000000530064005300
-                85           0 RESUME                   0
+                86           0 RESUME                   0
                
-                87           2 LOAD_FAST                0 (self)
+                88           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (celery_task)
                             14 POP_JUMP_FORWARD_IF_FALSE    46 (to 108)
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (status)
                             28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                2 (SCHEDULED)
                             40 CONTAINS_OP              1
                             42 POP_JUMP_FORWARD_IF_FALSE    32 (to 108)
                
-                88          44 LOAD_GLOBAL              7 (NULL + AsyncResult)
+                89          44 LOAD_GLOBAL              7 (NULL + AsyncResult)
                             56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                0 (celery_task)
                             68 LOAD_GLOBAL              8 (celery)
                             80 LOAD_ATTR                5 (current_app)
                             90 KW_NAMES                 1
                             92 PRECALL                  2
                             96 CALL                     2
                            106 RETURN_VALUE
                
-                90     >>  108 LOAD_CONST               0 (None)
+                91     >>  108 LOAD_CONST               0 (None)
                            110 RETURN_VALUE
                consts
                   None
                   ('app',)
                names      ('celery_task', 'status', 'SCHEDULED', 'AsyncResult', 'celery', 'current_app')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'async_result'
-               firstlineno 85
+               firstlineno 86
                lnotab 0x02022a014002
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c006a010000000000000000760172
                   277c00a0020000000000000000000000000000000000000000a6000000ab
                   0000000000000000007d017c01730f7407000000000000000000006401a6
                   010000ab01000000000000000082017c01530064005300
-                92           0 RESUME                   0
+                93           0 RESUME                   0
                
-                93           2 LOAD_FAST                0 (self)
+                94           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (status)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (SCHEDULED)
                             26 CONTAINS_OP              1
                             28 POP_JUMP_FORWARD_IF_FALSE    39 (to 108)
                
-                94          30 LOAD_FAST                0 (self)
+                95          30 LOAD_FAST                0 (self)
                             32 LOAD_METHOD              2 (_queue)
                             54 PRECALL                  0
                             58 CALL                     0
                             68 STORE_FAST               1 (task_id)
                
-                95          70 LOAD_FAST                1 (task_id)
+                96          70 LOAD_FAST                1 (task_id)
                             72 POP_JUMP_FORWARD_IF_TRUE    15 (to 104)
                
-                96          74 LOAD_GLOBAL              7 (NULL + NotImplementedError)
+                97          74 LOAD_GLOBAL              7 (NULL + NotImplementedError)
                             86 LOAD_CONST               1 ('`_queue` not properly implemented')
                             88 PRECALL                  1
                             92 CALL                     1
                            102 RAISE_VARARGS            1
                
-                97     >>  104 LOAD_FAST                1 (task_id)
+                98     >>  104 LOAD_FAST                1 (task_id)
                            106 RETURN_VALUE
                
-                98     >>  108 LOAD_CONST               0 (None)
+                99     >>  108 LOAD_CONST               0 (None)
                            110 RETURN_VALUE
                consts
                   None
                   '`_queue` not properly implemented'
                names      ('status', 'SCHEDULED', '_queue', 'NotImplementedError')
                varnames   ('self', 'task_id')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'queue'
-               firstlineno 92
+               firstlineno 93
                lnotab 0x02011c01280104011e010401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064015300
-               100           0 RESUME                   0
+               101           0 RESUME                   0
                
-               101           2 LOAD_CONST               1 ('')
+               102           2 LOAD_CONST               1 ('')
                              4 RETURN_VALUE
                consts
                   None
                   ''
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '_queue'
-               firstlineno 100
+               firstlineno 101
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'frozenset', 'states', 'PENDING', 'RECEIVED', 'STARTED', 'RETRY', 'SCHEDULED', 'models', 'CharField', 'celery_task', 'Meta', 'str', 'status', 'property', 'Optional', 'AsyncResult', 'async_result', 'queue', '_queue')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'CeleryEnabled'
-         firstlineno 65
+         firstlineno 66
          lnotab 0x0a01040132ff100426021a030c0a020116ff0e0102061808
       'CeleryEnabled'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
@@ -974,167 +983,167 @@
             0200000000000000005a136419641084045a14640e651565161900000000
             00000000006602641184045a170900090009000900641a64126518641365
             1864146519651a1900000000000000000064156519651a19000000000000
             000000640e640f660a880066016416840d5a1b6419641784045a1c640e65
             1d6602641884045a1e880078015a1f5300
                        0 MAKE_CELL                0 (__class__)
          
-         104           2 RESUME                   0
+         105           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Parametrizer')
                       10 STORE_NAME               2 (__qualname__)
          
-         105          12 PUSH_NULL
+         106          12 PUSH_NULL
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (SlugField)
                       26 LOAD_CONST               1 (255)
                       28 LOAD_CONST               2 (True)
                       30 LOAD_CONST               3 (False)
                       32 KW_NAMES                 4
                       34 PRECALL                  3
                       38 CALL                     3
                       48 STORE_NAME               5 (code)
          
-         106          50 PUSH_NULL
+         107          50 PUSH_NULL
                       52 LOAD_NAME                3 (models)
                       54 LOAD_ATTR                6 (CharField)
                       64 LOAD_CONST               1 (255)
                       66 LOAD_CONST               2 (True)
                       68 KW_NAMES                 5
                       70 PRECALL                  2
                       74 CALL                     2
                       84 STORE_NAME               7 (name)
          
-         107          86 PUSH_NULL
+         108          86 PUSH_NULL
                       88 LOAD_NAME                3 (models)
                       90 LOAD_ATTR                8 (TextField)
          
-         108         100 LOAD_CONST               1 (255)
+         109         100 LOAD_CONST               1 (255)
          
-         109         102 LOAD_CONST               2 (True)
+         110         102 LOAD_CONST               2 (True)
          
-         110         104 LOAD_CONST               2 (True)
+         111         104 LOAD_CONST               2 (True)
          
-         107         106 KW_NAMES                 6
+         108         106 KW_NAMES                 6
                      108 PRECALL                  3
                      112 CALL                     3
                      122 STORE_NAME               9 (description)
          
-         112         124 PUSH_NULL
+         113         124 PUSH_NULL
                      126 LOAD_NAME                3 (models)
                      128 LOAD_ATTR               10 (JSONField)
                      138 LOAD_NAME               11 (dict)
                      140 LOAD_CONST               3 (False)
                      142 LOAD_NAME               12 (validate_queryargs)
                      144 BUILD_LIST               1
                      146 KW_NAMES                 7
                      148 PRECALL                  3
                      152 CALL                     3
                      162 STORE_NAME              13 (value)
          
-         113         164 PUSH_NULL
+         114         164 PUSH_NULL
                      166 LOAD_NAME                3 (models)
                      168 LOAD_ATTR               14 (BooleanField)
                      178 LOAD_CONST               2 (True)
                      180 LOAD_CONST               3 (False)
                      182 LOAD_CONST               3 (False)
                      184 KW_NAMES                 8
                      186 PRECALL                  3
                      190 CALL                     3
                      200 STORE_NAME              15 (system)
          
-         114         202 PUSH_NULL
+         115         202 PUSH_NULL
                      204 LOAD_NAME                3 (models)
                      206 LOAD_ATTR               16 (ForeignKey)
          
-         115         216 LOAD_CONST               9 ('Query')
+         116         216 LOAD_CONST               9 ('Query')
                      218 LOAD_CONST               2 (True)
                      220 LOAD_CONST               2 (True)
                      222 LOAD_NAME                3 (models)
                      224 LOAD_ATTR               17 (CASCADE)
                      234 LOAD_CONST              10 ('+')
          
-         114         236 KW_NAMES                11
+         115         236 KW_NAMES                11
                      238 PRECALL                  5
                      242 CALL                     5
                      252 STORE_NAME              18 (source)
          
-         118         254 PUSH_NULL
+         119         254 PUSH_NULL
                      256 LOAD_BUILD_CLASS
-                     258 LOAD_CONST              12 (<code object Meta, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 118>)
+                     258 LOAD_CONST              12 (<code object Meta, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 119>)
                      260 MAKE_FUNCTION            0
                      262 LOAD_CONST              13 ('Meta')
                      264 PRECALL                  2
                      268 CALL                     2
                      278 STORE_NAME              19 (Meta)
          
-         122         280 LOAD_CONST              25 (('return', None))
-                     282 LOAD_CONST              16 (<code object clean, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 122>)
+         123         280 LOAD_CONST              25 (('return', None))
+                     282 LOAD_CONST              16 (<code object clean, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 123>)
                      284 MAKE_FUNCTION            4 (annotations)
                      286 STORE_NAME              20 (clean)
          
-         125         288 LOAD_CONST              14 ('return')
+         126         288 LOAD_CONST              14 ('return')
                      290 LOAD_NAME               21 (List)
                      292 LOAD_NAME               22 (Dict)
                      294 BINARY_SUBSCR
                      304 BUILD_TUPLE              2
-                     306 LOAD_CONST              17 (<code object get_matrix, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 125>)
+                     306 LOAD_CONST              17 (<code object get_matrix, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 126>)
                      308 MAKE_FUNCTION            4 (annotations)
                      310 STORE_NAME              23 (get_matrix)
          
-         131         312 NOP
+         132         312 NOP
          
-         132         314 NOP
+         133         314 NOP
          
-         133         316 NOP
+         134         316 NOP
          
-         134         318 NOP
+         135         318 NOP
          
-         129         320 LOAD_CONST              26 ((False, False, None, None))
+         130         320 LOAD_CONST              26 ((False, False, None, None))
                      322 LOAD_CONST              18 ('force_insert')
          
-         131         324 LOAD_NAME               24 (bool)
+         132         324 LOAD_NAME               24 (bool)
          
-         129         326 LOAD_CONST              19 ('force_update')
+         130         326 LOAD_CONST              19 ('force_update')
          
-         132         328 LOAD_NAME               24 (bool)
+         133         328 LOAD_NAME               24 (bool)
          
-         129         330 LOAD_CONST              20 ('using')
+         130         330 LOAD_CONST              20 ('using')
          
-         133         332 LOAD_NAME               25 (Optional)
+         134         332 LOAD_NAME               25 (Optional)
                      334 LOAD_NAME               26 (Any)
                      336 BINARY_SUBSCR
          
-         129         346 LOAD_CONST              21 ('update_fields')
+         130         346 LOAD_CONST              21 ('update_fields')
          
-         134         348 LOAD_NAME               25 (Optional)
+         135         348 LOAD_NAME               25 (Optional)
                      350 LOAD_NAME               26 (Any)
                      352 BINARY_SUBSCR
          
-         129         362 LOAD_CONST              14 ('return')
+         130         362 LOAD_CONST              14 ('return')
          
-         135         364 LOAD_CONST              15 (None)
+         136         364 LOAD_CONST              15 (None)
          
-         129         366 BUILD_TUPLE             10
+         130         366 BUILD_TUPLE             10
                      368 LOAD_CLOSURE             0 (__class__)
                      370 BUILD_TUPLE              1
-                     372 LOAD_CONST              22 (<code object save, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 129>)
+                     372 LOAD_CONST              22 (<code object save, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 130>)
                      374 MAKE_FUNCTION           13 (defaults, annotations, closure)
                      376 STORE_NAME              27 (save)
          
-         140         378 LOAD_CONST              25 (('return', None))
-                     380 LOAD_CONST              23 (<code object refresh, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 140>)
+         141         378 LOAD_CONST              25 (('return', None))
+                     380 LOAD_CONST              23 (<code object refresh, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 141>)
                      382 MAKE_FUNCTION            4 (annotations)
                      384 STORE_NAME              28 (refresh)
          
-         146         386 LOAD_CONST              14 ('return')
+         148         386 LOAD_CONST              14 ('return')
                      388 LOAD_NAME               29 (str)
                      390 BUILD_TUPLE              2
-                     392 LOAD_CONST              24 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 146>)
+                     392 LOAD_CONST              24 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 148>)
                      394 MAKE_FUNCTION            4 (annotations)
                      396 STORE_NAME              30 (__str__)
                      398 LOAD_CLOSURE             0 (__class__)
                      400 COPY                     1
                      402 STORE_NAME              31 (__classcell__)
                      404 RETURN_VALUE
          consts
@@ -1152,53 +1161,53 @@
             ('blank', 'null', 'on_delete', 'related_name')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364015a0464025300
-               118           0 RESUME                   0
+               119           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Parametrizer.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               119          10 LOAD_CONST               1 ('Arguments')
+               120          10 LOAD_CONST               1 ('Arguments')
                             12 STORE_NAME               3 (verbose_name_plural)
                
-               120          14 LOAD_CONST               1 ('Arguments')
+               121          14 LOAD_CONST               1 ('Arguments')
                             16 STORE_NAME               4 (verbose_name)
                             18 LOAD_CONST               2 (None)
                             20 RETURN_VALUE
                consts
                   'Parametrizer.Meta'
                   'Arguments'
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name_plural', 'verbose_name')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'Meta'
-               firstlineno 118
+               firstlineno 119
                lnotab 0x0a010401
             'Meta'
             'return'
             None
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab010000000000000000010064005300
-               122           0 RESUME                   0
+               123           0 RESUME                   0
                
-               123           2 LOAD_GLOBAL              1 (NULL + validate_queryargs)
+               124           2 LOAD_GLOBAL              1 (NULL + validate_queryargs)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (value)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
@@ -1206,47 +1215,47 @@
                   None
                names      ('validate_queryargs', 'value')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'clean'
-               firstlineno 122
+               firstlineno 123
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x870097007401000000000000000000007403000000000000000000006a
                   02000000000000000089006a030000000000000000a00400000000000000
                   00000000000000000000000000a6000000ab0000000000000000008e00a6
                   010000ab0100000000000000007d0188006601640184087c014400a60000
                   00ab0000000000000000005300
                              0 MAKE_CELL                0 (self)
                
-               125           2 RESUME                   0
+               126           2 RESUME                   0
                
-               126           4 LOAD_GLOBAL              1 (NULL + list)
+               127           4 LOAD_GLOBAL              1 (NULL + list)
                             16 LOAD_GLOBAL              3 (NULL + itertools)
                             28 LOAD_ATTR                2 (product)
                             38 LOAD_DEREF               0 (self)
                             40 LOAD_ATTR                3 (value)
                             50 LOAD_METHOD              4 (values)
                             72 PRECALL                  0
                             76 CALL                     0
                             86 CALL_FUNCTION_EX         0
                             88 PRECALL                  1
                             92 CALL                     1
                            102 STORE_FAST               1 (product)
                
-               127         104 LOAD_CLOSURE             0 (self)
+               128         104 LOAD_CLOSURE             0 (self)
                            106 BUILD_TUPLE              1
-                           108 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 127>)
+                           108 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 128>)
                            110 MAKE_FUNCTION            8 (closure)
                            112 LOAD_FAST                1 (product)
                            114 GET_ITER
                            116 PRECALL                  0
                            120 CALL                     0
                            130 RETURN_VALUE
                consts
@@ -1260,15 +1269,15 @@
                         0x9501970067007c005d367d017401000000000000000000007403000000
                         0000000000000089026a020000000000000000a003000000000000000000
                         0000000000000000000000a6000000ab0000000000000000007c01a60200
                         00ab020000000000000000a6010000ab01000000000000000091028c3753
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     127           2 RESUME                   0
+                     128           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                54 (to 118)
                                   10 STORE_FAST               1 (e)
                                   12 LOAD_GLOBAL              1 (NULL + dict)
                                   24 LOAD_GLOBAL              3 (NULL + zip)
                                   36 LOAD_DEREF               2 (self)
@@ -1287,23 +1296,23 @@
                      consts
                      names      ('dict', 'zip', 'value', 'keys')
                      varnames   ('.0', 'e')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                      name       '<listcomp>'
-                     firstlineno 127
+                     firstlineno 128
                      lnotab 0x
                names      ('list', 'itertools', 'product', 'value', 'values')
                varnames   ('self', 'product')
                freevars   ()
                cellvars   ('self',)
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'get_matrix'
-               firstlineno 125
+               firstlineno 126
                lnotab 0x04016401
             'force_insert'
             'force_update'
             'using'
             'update_fields'
             code
                argcount  : 5
@@ -1314,29 +1323,29 @@
                   0x950197007c006a00000000000000000073197403000000000000000000
                   007c006a020000000000000000a6010000ab0100000000000000007c005f
                   000000000000000000740700000000000000000000a6000000ab00000000
                   0000000000a00400000000000000000000000000000000000000007c017c
                   027c037c04a6040000ab040000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-               129           2 RESUME                   0
+               130           2 RESUME                   0
                
-               136           4 LOAD_FAST                0 (self)
+               137           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (code)
                             16 POP_JUMP_FORWARD_IF_TRUE    25 (to 68)
                
-               137          18 LOAD_GLOBAL              3 (NULL + slugify)
+               138          18 LOAD_GLOBAL              3 (NULL + slugify)
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (name)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 LOAD_FAST                0 (self)
                             58 STORE_ATTR               0 (code)
                
-               138     >>   68 LOAD_GLOBAL              7 (NULL + super)
+               139     >>   68 LOAD_GLOBAL              7 (NULL + super)
                             80 PRECALL                  0
                             84 CALL                     0
                             94 LOAD_METHOD              4 (save)
                            116 LOAD_FAST                1 (force_insert)
                            118 LOAD_FAST                2 (force_update)
                            120 LOAD_FAST                3 (using)
                            122 LOAD_FAST                4 (update_fields)
@@ -1349,104 +1358,110 @@
                   None
                names      ('code', 'slugify', 'name', 'super', 'save')
                varnames   ('self', 'force_insert', 'force_update', 'using', 'update_fields')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'save'
-               firstlineno 129
+               firstlineno 130
                lnotab 0x04070e013201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
-                  0x97007c006a000000000000000000723b7c006a000000000000000000a0
+                  0x97007c006a00000000000000000072497c006a000000000000000000a0
                   0100000000000000000000000000000000000000006401ac02a6010000ab
                   0100000000000000005c0200007d017d027c017c005f0200000000000000
-                  007c00a0030000000000000000000000000000000000000000a6000000ab
-                  00000000000000000001006400530064005300
-               140           0 RESUME                   0
+                  00740700000000000000000000a6000000ab00000000000000000001007c
+                  00a0040000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000001006400530064005300
+               141           0 RESUME                   0
                
-               141           2 LOAD_FAST                0 (self)
+               142           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (source)
-                            14 POP_JUMP_FORWARD_IF_FALSE    59 (to 134)
+                            14 POP_JUMP_FORWARD_IF_FALSE    73 (to 162)
                
-               142          16 LOAD_FAST                0 (self)
+               143          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                0 (source)
                             28 LOAD_METHOD              1 (run)
                             50 LOAD_CONST               1 (True)
                             52 KW_NAMES                 2
                             54 PRECALL                  1
                             58 CALL                     1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               1 (out)
                             74 STORE_FAST               2 (__)
                
-               143          76 LOAD_FAST                1 (out)
+               144          76 LOAD_FAST                1 (out)
                             78 LOAD_FAST                0 (self)
                             80 STORE_ATTR               2 (value)
                
-               144          90 LOAD_FAST                0 (self)
-                            92 LOAD_METHOD              3 (save)
-                           114 PRECALL                  0
-                           118 CALL                     0
-                           128 POP_TOP
-                           130 LOAD_CONST               0 (None)
-                           132 RETURN_VALUE
+               145          90 LOAD_GLOBAL              7 (NULL + breakpoint)
+                           102 PRECALL                  0
+                           106 CALL                     0
+                           116 POP_TOP
+               
+               146         118 LOAD_FAST                0 (self)
+                           120 LOAD_METHOD              4 (save)
+                           142 PRECALL                  0
+                           146 CALL                     0
+                           156 POP_TOP
+                           158 LOAD_CONST               0 (None)
+                           160 RETURN_VALUE
                
-               141     >>  134 LOAD_CONST               0 (None)
-                           136 RETURN_VALUE
+               142     >>  162 LOAD_CONST               0 (None)
+                           164 RETURN_VALUE
                consts
                   None
                   True
                   ('use_existing',)
-               names      ('source', 'run', 'value', 'save')
+               names      ('source', 'run', 'value', 'breakpoint', 'save')
                varnames   ('self', 'out', '__')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'refresh'
-               firstlineno 140
-               lnotab 0x02010e013c010e012cfd
+               firstlineno 141
+               lnotab 0x02010e013c010e011c012cfc
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               146           0 RESUME                   0
+               148           0 RESUME                   0
                
-               147           2 LOAD_FAST                0 (self)
+               149           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (name)
                             14 RETURN_VALUE
                consts
                   None
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '__str__'
-               firstlineno 146
+               firstlineno 148
                lnotab 0x0201
             ('return', None)
             (False, False, None, None)
          names      ('__name__', '__module__', '__qualname__', 'models', 'SlugField', 'code', 'CharField', 'name', 'TextField', 'description', 'JSONField', 'dict', 'validate_queryargs', 'value', 'BooleanField', 'system', 'ForeignKey', 'CASCADE', 'source', 'Meta', 'clean', 'List', 'Dict', 'get_matrix', 'bool', 'Optional', 'Any', 'save', 'refresh', 'str', '__str__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'Parametrizer'
-         firstlineno 104
+         firstlineno 105
          lnotab
             0x0c01260124010e010201020102fd1205280126010e0114ff12041a0408
             03180602010201020102fb040202fe020302fd02040efc02050efb020602
-            fa0c0b0806
+            fa0c0b0807
       'Parametrizer'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
@@ -1471,266 +1486,266 @@
             00000064106415660a88006601641a840d5a21641b6522641c6523641065
             246606641d84045a25641e6526641064156604641f84045a276427642065
             1e64216520641065266606642284055a2809000900090064286420651e64
             1c651f6524190000000000000000006423651e641065296608642484055a
             2a6410651b6602642584045a2b880078015a2c5300
                        0 MAKE_CELL                0 (__class__)
          
-         150           2 RESUME                   0
+         152           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Query')
                       10 STORE_NAME               2 (__qualname__)
          
-         151          12 PUSH_NULL
+         153          12 PUSH_NULL
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (CharField)
                       26 LOAD_CONST               1 (255)
                       28 LOAD_CONST               2 (True)
                       30 KW_NAMES                 3
                       32 PRECALL                  2
                       36 CALL                     2
                       46 STORE_NAME               5 (name)
          
-         152          48 PUSH_NULL
+         154          48 PUSH_NULL
                       50 LOAD_NAME                3 (models)
                       52 LOAD_ATTR                6 (TextField)
                       62 LOAD_CONST               2 (True)
                       64 LOAD_CONST               2 (True)
                       66 KW_NAMES                 4
                       68 PRECALL                  2
                       72 CALL                     2
                       82 STORE_NAME               7 (description)
          
-         153          84 PUSH_NULL
+         155          84 PUSH_NULL
                       86 LOAD_NAME                3 (models)
                       88 LOAD_ATTR                8 (ForeignKey)
          
-         154          98 PUSH_NULL
+         156          98 PUSH_NULL
                      100 LOAD_NAME                9 (get_user_model)
                      102 PRECALL                  0
                      106 CALL                     0
                      116 LOAD_NAME                3 (models)
                      118 LOAD_ATTR               10 (CASCADE)
                      128 LOAD_CONST               5 ('power_queries')
          
-         153         130 KW_NAMES                 6
+         155         130 KW_NAMES                 6
                      132 PRECALL                  3
                      136 CALL                     3
                      146 STORE_NAME              11 (owner)
          
-         156         148 PUSH_NULL
+         158         148 PUSH_NULL
                      150 LOAD_NAME                3 (models)
                      152 LOAD_ATTR                8 (ForeignKey)
                      162 LOAD_NAME               12 (ContentType)
                      164 LOAD_NAME                3 (models)
                      166 LOAD_ATTR               10 (CASCADE)
                      176 KW_NAMES                 7
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_NAME              13 (target)
          
-         157         194 PUSH_NULL
+         159         194 PUSH_NULL
                      196 LOAD_NAME                3 (models)
                      198 LOAD_ATTR                6 (TextField)
                      208 LOAD_CONST               8 ('qs=conn.all()')
                      210 LOAD_CONST               2 (True)
                      212 KW_NAMES                 9
                      214 PRECALL                  2
                      218 CALL                     2
                      228 STORE_NAME              14 (code)
          
-         158         230 PUSH_NULL
+         160         230 PUSH_NULL
                      232 LOAD_NAME               15 (JSONField)
                      234 LOAD_NAME               16 (dict)
                      236 LOAD_CONST               2 (True)
                      238 LOAD_NAME               17 (PQJSONEncoder)
                      240 KW_NAMES                10
                      242 PRECALL                  3
                      246 CALL                     3
                      256 STORE_NAME              18 (info)
          
-         159         258 PUSH_NULL
+         161         258 PUSH_NULL
                      260 LOAD_NAME                3 (models)
                      262 LOAD_ATTR                8 (ForeignKey)
          
-         160         272 LOAD_NAME               19 (Parametrizer)
+         162         272 LOAD_NAME               19 (Parametrizer)
                      274 LOAD_NAME                3 (models)
                      276 LOAD_ATTR               10 (CASCADE)
                      286 LOAD_CONST               2 (True)
                      288 LOAD_CONST               2 (True)
          
-         159         290 KW_NAMES                11
+         161         290 KW_NAMES                11
                      292 PRECALL                  4
                      296 CALL                     4
                      306 STORE_NAME              20 (parametrizer)
          
-         162         308 PUSH_NULL
+         164         308 PUSH_NULL
                      310 LOAD_NAME                3 (models)
                      312 LOAD_ATTR                4 (CharField)
                      322 LOAD_CONST              12 (400)
                      324 LOAD_CONST               2 (True)
                      326 LOAD_CONST               2 (True)
                      328 KW_NAMES                13
                      330 PRECALL                  3
                      334 CALL                     3
                      344 STORE_NAME              21 (sentry_error_id)
          
-         163         346 PUSH_NULL
+         165         346 PUSH_NULL
                      348 LOAD_NAME                3 (models)
                      350 LOAD_ATTR                4 (CharField)
                      360 LOAD_CONST              12 (400)
                      362 LOAD_CONST               2 (True)
                      364 LOAD_CONST               2 (True)
                      366 KW_NAMES                13
                      368 PRECALL                  3
                      372 CALL                     3
                      382 STORE_NAME              22 (error_message)
          
-         165         384 PUSH_NULL
+         167         384 PUSH_NULL
                      386 LOAD_NAME                3 (models)
                      388 LOAD_ATTR               23 (DateTimeField)
                      398 LOAD_CONST               2 (True)
                      400 LOAD_CONST               2 (True)
                      402 KW_NAMES                14
                      404 PRECALL                  2
                      408 CALL                     2
                      418 STORE_NAME              24 (last_run)
          
-         167         420 PUSH_NULL
+         169         420 PUSH_NULL
                      422 LOAD_NAME                3 (models)
                      424 LOAD_ATTR               25 (BooleanField)
                      434 LOAD_CONST               2 (True)
                      436 KW_NAMES                15
                      438 PRECALL                  1
                      442 CALL                     1
                      452 STORE_NAME              26 (active)
          
-         169         454 LOAD_CONST              16 ('return')
+         171         454 LOAD_CONST              16 ('return')
                      456 LOAD_NAME               27 (str)
                      458 BUILD_TUPLE              2
-                     460 LOAD_CONST              17 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 169>)
+                     460 LOAD_CONST              17 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 171>)
                      462 MAKE_FUNCTION            4 (annotations)
                      464 STORE_NAME              28 (__str__)
          
-         172         466 PUSH_NULL
+         174         466 PUSH_NULL
                      468 LOAD_BUILD_CLASS
-                     470 LOAD_CONST              18 (<code object Meta, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 172>)
+                     470 LOAD_CONST              18 (<code object Meta, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 174>)
                      472 MAKE_FUNCTION            0
                      474 LOAD_CONST              19 ('Meta')
                      476 PRECALL                  2
                      480 CALL                     2
                      490 STORE_NAME              29 (Meta)
          
-         178         492 NOP
+         180         492 NOP
          
-         179         494 NOP
+         181         494 NOP
          
-         180         496 NOP
+         182         496 NOP
          
-         181         498 NOP
+         183         498 NOP
          
-         176         500 LOAD_CONST              38 ((False, False, None, None))
+         178         500 LOAD_CONST              38 ((False, False, None, None))
                      502 LOAD_CONST              22 ('force_insert')
          
-         178         504 LOAD_NAME               30 (bool)
+         180         504 LOAD_NAME               30 (bool)
          
-         176         506 LOAD_CONST              23 ('force_update')
+         178         506 LOAD_CONST              23 ('force_update')
          
-         179         508 LOAD_NAME               30 (bool)
+         181         508 LOAD_NAME               30 (bool)
          
-         176         510 LOAD_CONST              24 ('using')
+         178         510 LOAD_CONST              24 ('using')
          
-         180         512 LOAD_NAME               31 (Optional)
+         182         512 LOAD_NAME               31 (Optional)
                      514 LOAD_NAME               32 (Any)
                      516 BINARY_SUBSCR
          
-         176         526 LOAD_CONST              25 ('update_fields')
+         178         526 LOAD_CONST              25 ('update_fields')
          
-         181         528 LOAD_NAME               31 (Optional)
+         183         528 LOAD_NAME               31 (Optional)
                      530 LOAD_NAME               32 (Any)
                      532 BINARY_SUBSCR
          
-         176         542 LOAD_CONST              16 ('return')
+         178         542 LOAD_CONST              16 ('return')
          
-         182         544 LOAD_CONST              21 (None)
+         184         544 LOAD_CONST              21 (None)
          
-         176         546 BUILD_TUPLE             10
+         178         546 BUILD_TUPLE             10
                      548 LOAD_CLOSURE             0 (__class__)
                      550 BUILD_TUPLE              1
-                     552 LOAD_CONST              26 (<code object save, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 176>)
+                     552 LOAD_CONST              26 (<code object save, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 178>)
                      554 MAKE_FUNCTION           13 (defaults, annotations, closure)
                      556 STORE_NAME              33 (save)
          
-         187         558 LOAD_CONST              27 ('query_id')
+         189         558 LOAD_CONST              27 ('query_id')
                      560 LOAD_NAME               34 (int)
                      562 LOAD_CONST              28 ('arguments')
                      564 LOAD_NAME               35 (List)
                      566 LOAD_CONST              16 ('return')
                      568 LOAD_NAME               36 (Dict)
                      570 BUILD_TUPLE              6
-                     572 LOAD_CONST              29 (<code object _invoke, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 187>)
+                     572 LOAD_CONST              29 (<code object _invoke, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 189>)
                      574 MAKE_FUNCTION            4 (annotations)
                      576 STORE_NAME              37 (_invoke)
          
-         192         578 LOAD_CONST              30 ('results')
+         194         578 LOAD_CONST              30 ('results')
                      580 LOAD_NAME               38 (QueryMatrixResult)
                      582 LOAD_CONST              16 ('return')
                      584 LOAD_CONST              21 (None)
                      586 BUILD_TUPLE              4
-                     588 LOAD_CONST              31 (<code object update_results, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 192>)
+                     588 LOAD_CONST              31 (<code object update_results, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 194>)
                      590 MAKE_FUNCTION            4 (annotations)
                      592 STORE_NAME              39 (update_results)
          
-         199         594 LOAD_CONST              39 ((True,))
+         201         594 LOAD_CONST              39 ((True,))
                      596 LOAD_CONST              32 ('persist')
                      598 LOAD_NAME               30 (bool)
                      600 LOAD_CONST              33 ('kwargs')
                      602 LOAD_NAME               32 (Any)
                      604 LOAD_CONST              16 ('return')
                      606 LOAD_NAME               38 (QueryMatrixResult)
                      608 BUILD_TUPLE              6
-                     610 LOAD_CONST              34 (<code object execute_matrix, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 199>)
+                     610 LOAD_CONST              34 (<code object execute_matrix, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 201>)
                      612 MAKE_FUNCTION            5 (defaults, annotations)
                      614 STORE_NAME              40 (execute_matrix)
          
-         239         616 NOP
+         241         616 NOP
          
-         240         618 NOP
+         242         618 NOP
          
-         241         620 NOP
+         243         620 NOP
          
-         237         622 LOAD_CONST              40 ((False, None, False))
+         239         622 LOAD_CONST              40 ((False, None, False))
                      624 LOAD_CONST              32 ('persist')
          
-         239         626 LOAD_NAME               30 (bool)
+         241         626 LOAD_NAME               30 (bool)
          
-         237         628 LOAD_CONST              28 ('arguments')
+         239         628 LOAD_CONST              28 ('arguments')
          
-         240         630 LOAD_NAME               31 (Optional)
+         242         630 LOAD_NAME               31 (Optional)
                      632 LOAD_NAME               36 (Dict)
                      634 BINARY_SUBSCR
          
-         237         644 LOAD_CONST              35 ('use_existing')
+         239         644 LOAD_CONST              35 ('use_existing')
          
-         241         646 LOAD_NAME               30 (bool)
+         243         646 LOAD_NAME               30 (bool)
          
-         237         648 LOAD_CONST              16 ('return')
+         239         648 LOAD_CONST              16 ('return')
          
-         242         650 LOAD_NAME               41 (QueryResult)
+         244         650 LOAD_NAME               41 (QueryResult)
          
-         237         652 BUILD_TUPLE              8
-                     654 LOAD_CONST              36 (<code object run, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 237>)
+         239         652 BUILD_TUPLE              8
+                     654 LOAD_CONST              36 (<code object run, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 239>)
                      656 MAKE_FUNCTION            5 (defaults, annotations)
                      658 STORE_NAME              42 (run)
          
-         301         660 LOAD_CONST              16 ('return')
+         310         660 LOAD_CONST              16 ('return')
                      662 LOAD_NAME               27 (str)
                      664 BUILD_TUPLE              2
-                     666 LOAD_CONST              37 (<code object _queue, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 301>)
+                     666 LOAD_CONST              37 (<code object _queue, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 310>)
                      668 MAKE_FUNCTION            4 (annotations)
                      670 STORE_NAME              43 (_queue)
                      672 LOAD_CLOSURE             0 (__class__)
                      674 COPY                     1
                      676 STORE_NAME              44 (__classcell__)
                      678 RETURN_VALUE
          consts
@@ -1753,63 +1768,63 @@
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a000000000000000000700164015300
-               169           0 RESUME                   0
+               171           0 RESUME                   0
                
-               170           2 LOAD_FAST                0 (self)
+               172           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (name)
                             14 JUMP_IF_TRUE_OR_POP      1 (to 18)
                             16 LOAD_CONST               1 ('')
                        >>   18 RETURN_VALUE
                consts
                   None
                   ''
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '__str__'
-               firstlineno 169
+               firstlineno 171
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035300
-               172           0 RESUME                   0
+               174           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Query.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               173          10 LOAD_CONST               1 ('Power Queries')
+               175          10 LOAD_CONST               1 ('Power Queries')
                             12 STORE_NAME               3 (verbose_name_plural)
                
-               174          14 LOAD_CONST               2 (('name',))
+               176          14 LOAD_CONST               2 (('name',))
                             16 STORE_NAME               4 (ordering)
                             18 LOAD_CONST               3 (None)
                             20 RETURN_VALUE
                consts
                   'Query.Meta'
                   'Power Queries'
                   ('name',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'Meta'
-               firstlineno 172
+               firstlineno 174
                lnotab 0x0a010401
             'Meta'
             False
             None
             'force_insert'
             'force_update'
             'using'
@@ -1822,25 +1837,25 @@
                code
                   0x950197007c006a000000000000000000730764017c005f000000000000
                   000000740300000000000000000000a6000000ab000000000000000000a0
                   0200000000000000000000000000000000000000007c017c027c037c04a6
                   040000ab040000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-               176           2 RESUME                   0
+               178           2 RESUME                   0
                
-               183           4 LOAD_FAST                0 (self)
+               185           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (code)
                             16 POP_JUMP_FORWARD_IF_TRUE     7 (to 32)
                
-               184          18 LOAD_CONST               1 ("qs=conn.all().order_by('id')")
+               186          18 LOAD_CONST               1 ("qs=conn.all().order_by('id')")
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (code)
                
-               185     >>   32 LOAD_GLOBAL              3 (NULL + super)
+               187     >>   32 LOAD_GLOBAL              3 (NULL + super)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 LOAD_METHOD              2 (save)
                             80 LOAD_FAST                1 (force_insert)
                             82 LOAD_FAST                2 (force_update)
                             84 LOAD_FAST                3 (using)
                             86 LOAD_FAST                4 (update_fields)
@@ -1854,64 +1869,64 @@
                   "qs=conn.all().order_by('id')"
                names      ('code', 'super', 'save')
                varnames   ('self', 'force_insert', 'force_update', 'using', 'update_fields')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'save'
-               firstlineno 176
+               firstlineno 178
                lnotab 0x04070e010e01
             'query_id'
             'arguments'
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c01ac01a6010000ab01000000
                   00000000007d037c03a00300000000000000000000000000000000000000
                   0064027c026403ac04a6030000ab0300000000000000007d047c045300
-               187           0 RESUME                   0
+               189           0 RESUME                   0
                
-               188           2 LOAD_GLOBAL              0 (Query)
+               190           2 LOAD_GLOBAL              0 (Query)
                             14 LOAD_ATTR                1 (objects)
                             24 LOAD_METHOD              2 (get)
                             46 LOAD_FAST                1 (query_id)
                             48 KW_NAMES                 1
                             50 PRECALL                  1
                             54 CALL                     1
                             64 STORE_FAST               3 (query)
                
-               189          66 LOAD_FAST                3 (query)
+               191          66 LOAD_FAST                3 (query)
                             68 LOAD_METHOD              3 (run)
                             90 LOAD_CONST               2 (False)
                             92 LOAD_FAST                2 (arguments)
                             94 LOAD_CONST               3 (True)
                             96 KW_NAMES                 4
                             98 PRECALL                  3
                            102 CALL                     3
                            112 STORE_FAST               4 (result)
                
-               190         114 LOAD_FAST                4 (result)
+               192         114 LOAD_FAST                4 (result)
                            116 RETURN_VALUE
                consts
                   None
                   ('id',)
                   False
                   True
                   ('persist', 'arguments', 'use_existing')
                names      ('Query', 'objects', 'get', 'run')
                varnames   ('self', 'query_id', 'arguments', 'query', 'result')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '_invoke'
-               firstlineno 187
+               firstlineno 189
                lnotab 0x020140013001
             'results'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
@@ -1920,48 +1935,48 @@
                   000000000000000000000000000000000064026403a6020000ab02000000
                   00000000007c005f0200000000000000007c01a001000000000000000000
                   000000000000000000000064046403a6020000ab0200000000000000007c
                   005f0300000000000000007409000000000000000000006a050000000000
                   000000a6000000ab0000000000000000007c005f0600000000000000007c
                   00a0070000000000000000000000000000000000000000a6000000ab0000
                   00000000000000010064005300
-               192           0 RESUME                   0
+               194           0 RESUME                   0
                
-               193           2 LOAD_FAST                1 (results)
+               195           2 LOAD_FAST                1 (results)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (info)
                             16 LOAD_CONST               1 ('last_run_results')
                             18 STORE_SUBSCR
                
-               194          22 LOAD_FAST                1 (results)
+               196          22 LOAD_FAST                1 (results)
                             24 LOAD_METHOD              1 (get)
                             46 LOAD_CONST               2 ('error_message')
                             48 LOAD_CONST               3 ('')
                             50 PRECALL                  2
                             54 CALL                     2
                             64 LOAD_FAST                0 (self)
                             66 STORE_ATTR               2 (error_message)
                
-               195          76 LOAD_FAST                1 (results)
+               197          76 LOAD_FAST                1 (results)
                             78 LOAD_METHOD              1 (get)
                            100 LOAD_CONST               4 ('sentry_error_id')
                            102 LOAD_CONST               3 ('')
                            104 PRECALL                  2
                            108 CALL                     2
                            118 LOAD_FAST                0 (self)
                            120 STORE_ATTR               3 (sentry_error_id)
                
-               196         130 LOAD_GLOBAL              9 (NULL + timezone)
+               198         130 LOAD_GLOBAL              9 (NULL + timezone)
                            142 LOAD_ATTR                5 (now)
                            152 PRECALL                  0
                            156 CALL                     0
                            166 LOAD_FAST                0 (self)
                            168 STORE_ATTR               6 (last_run)
                
-               197         178 LOAD_FAST                0 (self)
+               199         178 LOAD_FAST                0 (self)
                            180 LOAD_METHOD              7 (save)
                            202 PRECALL                  0
                            206 CALL                     0
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                consts
@@ -1972,15 +1987,15 @@
                   'sentry_error_id'
                names      ('info', 'get', 'error_message', 'sentry_error_id', 'timezone', 'now', 'last_run', 'save')
                varnames   ('self', 'results')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'update_results'
-               firstlineno 192
+               firstlineno 194
                lnotab 0x02011401360136013001
             'persist'
             'kwargs'
             code
                argcount  : 2
                nlocals   : 10
                stacksize : 8
@@ -2023,147 +2038,147 @@
                   0000000000a6000000ab0000000000000000000100640064006400a60200
                   00ab02000000000000000001006e0b230031007304770278035900770101
                   00590001000100640064006400a6020000ab02000000000000000001006e
                   0b23003100730477027803590077010100590001000100890a5300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL               10 (results)
                
-               199           4 RESUME                   0
+               201           4 RESUME                   0
                
-               200           6 LOAD_DEREF               0 (self)
+               202           6 LOAD_DEREF               0 (self)
                              8 LOAD_ATTR                0 (parametrizer)
                             18 POP_JUMP_FORWARD_IF_FALSE    43 (to 106)
                
-               201          20 LOAD_DEREF               0 (self)
+               203          20 LOAD_DEREF               0 (self)
                             22 LOAD_ATTR                0 (parametrizer)
                             32 LOAD_METHOD              1 (get_matrix)
                             54 PRECALL                  0
                             58 CALL                     0
                             68 STORE_FAST               3 (args)
                
-               202          70 LOAD_FAST                3 (args)
+               204          70 LOAD_FAST                3 (args)
                             72 POP_JUMP_FORWARD_IF_TRUE    15 (to 104)
                
-               203          74 LOAD_GLOBAL              5 (NULL + ValueError)
+               205          74 LOAD_GLOBAL              5 (NULL + ValueError)
                             86 LOAD_CONST               1 ('No valid arguments provided')
                             88 PRECALL                  1
                             92 CALL                     1
                            102 RAISE_VARARGS            1
                
-               202     >>  104 JUMP_FORWARD             3 (to 112)
+               204     >>  104 JUMP_FORWARD             3 (to 112)
                
-               205     >>  106 BUILD_MAP                0
+               207     >>  106 BUILD_MAP                0
                            108 BUILD_LIST               1
                            110 STORE_FAST               3 (args)
                
-               206     >>  112 LOAD_CONST               0 (None)
+               208     >>  112 LOAD_CONST               0 (None)
                            114 LOAD_DEREF               0 (self)
                            116 STORE_ATTR               3 (error_message)
                
-               207         126 LOAD_CONST               0 (None)
+               209         126 LOAD_CONST               0 (None)
                            128 LOAD_DEREF               0 (self)
                            130 STORE_ATTR               4 (sentry_error_id)
                
-               208         140 LOAD_CONST               0 (None)
+               210         140 LOAD_CONST               0 (None)
                            142 LOAD_DEREF               0 (self)
                            144 STORE_ATTR               5 (last_run)
                
-               209         154 BUILD_MAP                0
+               211         154 BUILD_MAP                0
                            156 LOAD_DEREF               0 (self)
                            158 STORE_ATTR               6 (info)
                
-               212         168 LOAD_CONST               2 ('timestamp')
+               214         168 LOAD_CONST               2 ('timestamp')
                            170 LOAD_GLOBAL             15 (NULL + strftime)
                            182 LOAD_GLOBAL             17 (NULL + timezone)
                            194 LOAD_ATTR                9 (now)
                            204 PRECALL                  0
                            208 CALL                     0
                            218 LOAD_CONST               3 ('%Y-%m-%d %H:%M')
                            220 PRECALL                  2
                            224 CALL                     2
                
-               211         234 BUILD_MAP                1
+               213         234 BUILD_MAP                1
                            236 STORE_DEREF             10 (results)
                
-               214         238 LOAD_GLOBAL             21 (NULL + configure_scope)
+               216         238 LOAD_GLOBAL             21 (NULL + configure_scope)
                            250 PRECALL                  0
                            254 CALL                     0
                            264 BEFORE_WITH
                            266 STORE_FAST               4 (scope)
                
-               215         268 LOAD_FAST                4 (scope)
+               217         268 LOAD_FAST                4 (scope)
                            270 LOAD_METHOD             11 (set_tag)
                            292 LOAD_CONST               4 ('power_query')
                            294 LOAD_CONST               5 (True)
                            296 PRECALL                  2
                            300 CALL                     2
                            310 POP_TOP
                
-               216         312 LOAD_FAST                4 (scope)
+               218         312 LOAD_FAST                4 (scope)
                            314 LOAD_METHOD             11 (set_tag)
                            336 LOAD_CONST               6 ('power_query.name')
                            338 LOAD_DEREF               0 (self)
                            340 LOAD_ATTR               12 (name)
                            350 PRECALL                  2
                            354 CALL                     2
                            364 POP_TOP
                
-               217         366 LOAD_GLOBAL             27 (NULL + transaction)
+               219         366 LOAD_GLOBAL             27 (NULL + transaction)
                            378 LOAD_ATTR               14 (atomic)
                            388 PRECALL                  0
                            392 CALL                     0
                            402 BEFORE_WITH
                            404 POP_TOP
                
-               218         406 LOAD_GLOBAL             27 (NULL + transaction)
+               220         406 LOAD_GLOBAL             27 (NULL + transaction)
                            418 LOAD_ATTR               15 (on_commit)
                            428 LOAD_CLOSURE            10 (results)
                            430 LOAD_CLOSURE             0 (self)
                            432 BUILD_TUPLE              2
-                           434 LOAD_CONST               7 (<code object <lambda>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 218>)
+                           434 LOAD_CONST               7 (<code object <lambda>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 220>)
                            436 MAKE_FUNCTION            8 (closure)
                            438 PRECALL                  1
                            442 CALL                     1
                            452 POP_TOP
                
-               219         454 LOAD_FAST                3 (args)
+               221         454 LOAD_FAST                3 (args)
                            456 GET_ITER
                        >>  458 FOR_ITER               217 (to 894)
                            460 STORE_FAST               5 (a)
                
-               220         462 NOP
+               222         462 NOP
                
-               221         464 LOAD_DEREF               0 (self)
+               223         464 LOAD_DEREF               0 (self)
                            466 LOAD_METHOD             16 (run)
                            488 LOAD_FAST                1 (persist)
                            490 LOAD_FAST                5 (a)
                            492 PRECALL                  2
                            496 CALL                     2
                            506 UNPACK_SEQUENCE          2
                            510 STORE_FAST               6 (dataset)
                            512 STORE_FAST               7 (__)
                
-               222         514 LOAD_GLOBAL             35 (NULL + isinstance)
+               224         514 LOAD_GLOBAL             35 (NULL + isinstance)
                            526 LOAD_FAST                6 (dataset)
                            528 LOAD_GLOBAL             36 (Dataset)
                            540 PRECALL                  2
                            544 CALL                     2
                            554 POP_JUMP_FORWARD_IF_FALSE    24 (to 604)
                
-               223         556 LOAD_FAST                6 (dataset)
+               225         556 LOAD_FAST                6 (dataset)
                            558 LOAD_ATTR               19 (pk)
                            568 LOAD_DEREF              10 (results)
                            570 LOAD_GLOBAL             41 (NULL + str)
                            582 LOAD_FAST                5 (a)
                            584 PRECALL                  1
                            588 CALL                     1
                            598 STORE_SUBSCR
                            602 JUMP_FORWARD            44 (to 692)
                
-               225     >>  604 LOAD_GLOBAL             41 (NULL + str)
+               227     >>  604 LOAD_GLOBAL             41 (NULL + str)
                            616 LOAD_GLOBAL             43 (NULL + len)
                            628 LOAD_FAST                6 (dataset)
                            630 PRECALL                  1
                            634 CALL                     1
                            644 PRECALL                  1
                            648 CALL                     1
                            658 LOAD_DEREF              10 (results)
@@ -2171,41 +2186,41 @@
                            672 LOAD_FAST                5 (a)
                            674 PRECALL                  1
                            678 CALL                     1
                            688 STORE_SUBSCR
                        >>  692 JUMP_BACKWARD          118 (to 458)
                        >>  694 PUSH_EXC_INFO
                
-               227         696 LOAD_GLOBAL             44 (QueryRunError)
+               229         696 LOAD_GLOBAL             44 (QueryRunError)
                            708 CHECK_EXC_MATCH
                            710 POP_JUMP_FORWARD_IF_FALSE    87 (to 886)
                            712 STORE_FAST               8 (e)
                
-               228         714 LOAD_GLOBAL             46 (logger)
+               230         714 LOAD_GLOBAL             46 (logger)
                            726 LOAD_METHOD             24 (exception)
                            748 LOAD_FAST                8 (e)
                            750 PRECALL                  1
                            754 CALL                     1
                            764 POP_TOP
                
-               229         766 LOAD_GLOBAL             51 (NULL + capture_exception)
+               231         766 LOAD_GLOBAL             51 (NULL + capture_exception)
                            778 LOAD_FAST                8 (e)
                            780 PRECALL                  1
                            784 CALL                     1
                            794 STORE_FAST               9 (err)
                
-               230         796 LOAD_GLOBAL             41 (NULL + str)
+               232         796 LOAD_GLOBAL             41 (NULL + str)
                            808 LOAD_FAST                9 (err)
                            810 PRECALL                  1
                            814 CALL                     1
                            824 LOAD_DEREF              10 (results)
                            826 LOAD_CONST               8 ('sentry_error_id')
                            828 STORE_SUBSCR
                
-               231         832 LOAD_GLOBAL             41 (NULL + str)
+               233         832 LOAD_GLOBAL             41 (NULL + str)
                            844 LOAD_FAST                8 (e)
                            846 PRECALL                  1
                            850 CALL                     1
                            860 LOAD_DEREF              10 (results)
                            862 LOAD_CONST               9 ('error_message')
                            864 STORE_SUBSCR
                            868 POP_EXCEPT
@@ -2214,43 +2229,43 @@
                            874 DELETE_FAST              8 (e)
                            876 JUMP_BACKWARD          210 (to 458)
                        >>  878 LOAD_CONST               0 (None)
                            880 STORE_FAST               8 (e)
                            882 DELETE_FAST              8 (e)
                            884 RERAISE                  1
                
-               227     >>  886 RERAISE                  0
+               229     >>  886 RERAISE                  0
                        >>  888 COPY                     3
                            890 POP_EXCEPT
                            892 RERAISE                  1
                
-               232     >>  894 LOAD_DEREF               0 (self)
+               234     >>  894 LOAD_DEREF               0 (self)
                            896 LOAD_ATTR               26 (datasets)
                            906 LOAD_METHOD             27 (exclude)
                
-               233         928 LOAD_CONST              10 (<code object <listcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 233>)
+               235         928 LOAD_CONST              10 (<code object <listcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 235>)
                            930 MAKE_FUNCTION            0
                            932 LOAD_DEREF              10 (results)
                            934 LOAD_METHOD             28 (values)
                            956 PRECALL                  0
                            960 CALL                     0
                            970 GET_ITER
                            972 PRECALL                  0
                            976 CALL                     0
                
-               232         986 KW_NAMES                11
+               234         986 KW_NAMES                11
                            988 PRECALL                  1
                            992 CALL                     1
                
-               234        1002 LOAD_METHOD             29 (delete)
+               236        1002 LOAD_METHOD             29 (delete)
                           1024 PRECALL                  0
                           1028 CALL                     0
                           1038 POP_TOP
                
-               217        1040 LOAD_CONST               0 (None)
+               219        1040 LOAD_CONST               0 (None)
                           1042 LOAD_CONST               0 (None)
                           1044 LOAD_CONST               0 (None)
                           1046 PRECALL                  2
                           1050 CALL                     2
                           1060 POP_TOP
                           1062 JUMP_FORWARD            11 (to 1086)
                        >> 1064 PUSH_EXC_INFO
@@ -2261,15 +2276,15 @@
                           1074 POP_EXCEPT
                           1076 RERAISE                  1
                        >> 1078 POP_TOP
                           1080 POP_EXCEPT
                           1082 POP_TOP
                           1084 POP_TOP
                
-               214     >> 1086 LOAD_CONST               0 (None)
+               216     >> 1086 LOAD_CONST               0 (None)
                           1088 LOAD_CONST               0 (None)
                           1090 LOAD_CONST               0 (None)
                           1092 PRECALL                  2
                           1096 CALL                     2
                           1106 POP_TOP
                           1108 JUMP_FORWARD            11 (to 1132)
                        >> 1110 PUSH_EXC_INFO
@@ -2280,15 +2295,15 @@
                           1120 POP_EXCEPT
                           1122 RERAISE                  1
                        >> 1124 POP_TOP
                           1126 POP_EXCEPT
                           1128 POP_TOP
                           1130 POP_TOP
                
-               235     >> 1132 LOAD_DEREF              10 (results)
+               237     >> 1132 LOAD_DEREF              10 (results)
                           1134 RETURN_VALUE
                ExceptionTable:
                  266 to 402 -> 1110 [1] lasti
                  404 to 460 -> 1064 [2] lasti
                  464 to 690 -> 694 [3]
                  692 to 692 -> 1064 [2] lasti
                  694 to 712 -> 888 [4] lasti
@@ -2317,43 +2332,43 @@
                      stacksize : 3
                      flags     : 19
                      code
                         0x950297008901a000000000000000000000000000000000000000000089
                         00a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           2
                      
-                     218           2 RESUME                   0
+                     220           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (update_results)
                                   28 LOAD_DEREF               0 (results)
                                   30 PRECALL                  1
                                   34 CALL                     1
                                   44 RETURN_VALUE
                      consts
                         None
                      names      ('update_results',)
                      varnames   ()
                      freevars   ('results', 'self')
                      cellvars   ()
                      filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                      name       '<lambda>'
-                     firstlineno 218
+                     firstlineno 220
                      lnotab 0x
                   'sentry_error_id'
                   'error_message'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x970067007c005d197d017401000000000000000000007c017402000000
                         00000000000000a6020000ab020000000000000000af177c0191028c1a53
                         00
-                     233           0 RESUME                   0
+                     235           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                25 (to 58)
                                    8 STORE_FAST               1 (dpk)
                                   10 LOAD_GLOBAL              1 (NULL + isinstance)
                                   22 LOAD_FAST                1 (dpk)
                                   24 LOAD_GLOBAL              2 (int)
@@ -2367,449 +2382,509 @@
                      consts
                      names      ('isinstance', 'int')
                      varnames   ('.0', 'dpk')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                      name       '<listcomp>'
-                     firstlineno 233
+                     firstlineno 235
                      lnotab 0x
                   ('pk__in',)
                names      ('parametrizer', 'get_matrix', 'ValueError', 'error_message', 'sentry_error_id', 'last_run', 'info', 'strftime', 'timezone', 'now', 'configure_scope', 'set_tag', 'name', 'transaction', 'atomic', 'on_commit', 'run', 'isinstance', 'Dataset', 'pk', 'str', 'len', 'QueryRunError', 'logger', 'exception', 'capture_exception', 'datasets', 'exclude', 'values', 'delete')
                varnames   ('self', 'persist', 'kwargs', 'args', 'scope', 'a', 'dataset', '__', 'e', 'err')
                freevars   ()
                cellvars   ('self', 'results')
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'execute_matrix'
-               firstlineno 199
+               firstlineno 201
                lnotab
                   0x06010e01320104011eff020306010e010e010e010e0342ff04031e012c
                   013601280130010801020132012a0130025c02120134011e01240136fc08
                   0522013aff100226ef2efd2e15
             'use_existing'
             code
                argcount  : 4
-               nlocals   : 16
+               nlocals   : 17
                stacksize : 10
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
-                  00000000000000a6000000ab0000000000000000007d0464018400740500
-                  000000000000000000a6000000ab00000000000000000066014400a60000
-                  00ab0000000000000000007d057c006a0300000000000000006a04000000
-                  00000000007222740a000000000000000000006a060000000000000000a0
-                  070000000000000000000000000000000000000000a6000000ab00000000
-                  00000000007c0564023c0000006e28740a000000000000000000006a0600
-                  00000000000000a00700000000000000000000000000000000000000007c
-                  006a030000000000000000ac03a6010000ab0100000000000000007c0564
-                  023c00000009007c046a080000000000000000a009000000000000000000
-                  00000000000000000000007414000000000000000000006a0b0000000000
-                  000000a6010000ab0100000000000000007c007c027c027c006a0c000000
-                  000000000064049c057c05a5017d06741b0000000000000000000064057c
-                  006a0e000000000000000069017c0272027c026e016900a501a6010000ab
-                  0100000000000000007d077c03723f741e000000000000000000006a0600
-                  00000000000000a00700000000000000000000000000000000000000007c
-                  007c07ac06a6020000ab020000000000000000a010000000000000000000
-                  0000000000000000000000a6000000ab00000000000000000078017d0872
-                  0a7c087c086a11000000000000000066027d096ecf742500000000000000
-                  0000007c006a130000000000000000742900000000000000000000a60000
-                  00ab0000000000000000007c06a6030000ab03000000000000000001007c
-                  06a015000000000000000000000000000000000000000064076400a60200
-                  00ab0200000000000000007d0a7c06a01500000000000000000000000000
-                  0000000000000064086400a6020000ab0200000000000000007d0b7c0172
-                  7b742d000000000000000000007c0aa6010000ab0100000000000000006a
-                  1700000000000000007c0264099c027d0c741e000000000000000000006a
-                  060000000000000000a01800000000000000000000000000000000000000
-                  007c007c077c0c7433000000000000000000006a1a0000000000000000a6
-                  000000ab0000000000000000007437000000000000000000006a1c000000
-                  00000000007c0aa6010000ab010000000000000000743700000000000000
-                  0000006a1c00000000000000007c0ba6010000ab01000000000000000064
-                  0a9c04ac0ba6030000ab0300000000000000005c0200007d0d7d0e7c0d7c
-                  0b66027d096e047c0a7c0b66027d096e222300743a000000000000000000
-                  00240072157d0f743d000000000000000000007c0fa6010000ab01000000
-                  00000000007c0f820264007d0f7e0f770177007803590077017c095300
-               237           0 RESUME                   0
+                  00000000000000a6000000ab0000000000000000007d0474050000000000
+                  0000000000a6000000ab00000000000000000067017d0574060000000000
+                  00000000006a04000000000000000072297c05a005000000000000000000
+                  0000000000000000000000640184007406000000000000000000006a0400
+                  000000000000004400a6000000ab000000000000000000a6010000ab0100
+                  000000000000000100640284007c054400a6000000ab0000000000000000
+                  007d067c006a0600000000000000006a0700000000000000007222741000
+                  0000000000000000006a090000000000000000a00a000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000007c0664033c
+                  0000006e287410000000000000000000006a090000000000000000a00a00
+                  000000000000000000000000000000000000007c006a0600000000000000
+                  00ac04a6010000ab0100000000000000007c0664033c00000009007c046a
+                  0b0000000000000000a00c00000000000000000000000000000000000000
+                  007406000000000000000000006a0d0000000000000000a6010000ab0100
+                  000000000000007c007c027c027c006a0e000000000000000064059c057c
+                  06a5017d07741f0000000000000000000064067c006a1000000000000000
+                  0069017c0272027c026e016900a501a6010000ab0100000000000000007d
+                  087c03723f7422000000000000000000006a090000000000000000a00a00
+                  000000000000000000000000000000000000007c007c08ac07a6020000ab
+                  020000000000000000a01200000000000000000000000000000000000000
+                  00a6000000ab00000000000000000078017d09720a7c097c096a13000000
+                  000000000066027d0a6ecf7429000000000000000000007c006a15000000
+                  0000000000742d00000000000000000000a6000000ab0000000000000000
+                  007c07a6030000ab03000000000000000001007c07a01700000000000000
+                  0000000000000000000000000064086400a6020000ab0200000000000000
+                  007d0b7c07a0170000000000000000000000000000000000000000640964
+                  00a6020000ab0200000000000000007d0c7c01727b743100000000000000
+                  0000007c0ba6010000ab0100000000000000006a1900000000000000007c
+                  02640a9c027d0d7422000000000000000000006a090000000000000000a0
+                  1a00000000000000000000000000000000000000007c007c087c0d743700
+                  0000000000000000006a1c0000000000000000a6000000ab000000000000
+                  000000743b000000000000000000006a1e00000000000000007c0ba60100
+                  00ab010000000000000000743b000000000000000000006a1e0000000000
+                  0000007c0ca6010000ab010000000000000000640b9c04ac0ca6030000ab
+                  0300000000000000005c0200007d0e7d0f7c0e7c0c66027d0a6e047c0b7c
+                  0c66027d0a6e222300743e00000000000000000000240072157d10744100
+                  0000000000000000007c10a6010000ab0100000000000000007c10820264
+                  007d107e10770177007803590077017c0a5300
+               239           0 RESUME                   0
                
-               243           2 LOAD_FAST                0 (self)
+               245           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (target)
                             14 LOAD_METHOD              1 (model_class)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 STORE_FAST               4 (model)
                
-               244          52 LOAD_CONST               1 (<code object <dictcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 244>)
-                            54 MAKE_FUNCTION            0
-               
-               249          56 LOAD_GLOBAL              5 (NULL + get_user_model)
-                            68 PRECALL                  0
-                            72 CALL                     0
-               
-               248          82 BUILD_TUPLE              1
-               
-               244          84 GET_ITER
-                            86 PRECALL                  0
-                            90 CALL                     0
-                           100 STORE_FAST               5 (connections)
-               
-               253         102 LOAD_FAST                0 (self)
-                           104 LOAD_ATTR                3 (owner)
-                           114 LOAD_ATTR                4 (is_superuser)
-                           124 POP_JUMP_FORWARD_IF_FALSE    34 (to 194)
-               
-               254         126 LOAD_GLOBAL             10 (Query)
-                           138 LOAD_ATTR                6 (objects)
-                           148 LOAD_METHOD              7 (filter)
-                           170 PRECALL                  0
-                           174 CALL                     0
-                           184 LOAD_FAST                5 (connections)
-                           186 LOAD_CONST               2 ('QueryManager')
-                           188 STORE_SUBSCR
-                           192 JUMP_FORWARD            40 (to 274)
-               
-               256     >>  194 LOAD_GLOBAL             10 (Query)
-                           206 LOAD_ATTR                6 (objects)
-                           216 LOAD_METHOD              7 (filter)
-                           238 LOAD_FAST                0 (self)
-                           240 LOAD_ATTR                3 (owner)
-                           250 KW_NAMES                 3
-                           252 PRECALL                  1
-                           256 CALL                     1
-                           266 LOAD_FAST                5 (connections)
-                           268 LOAD_CONST               2 ('QueryManager')
-                           270 STORE_SUBSCR
-               
-               258     >>  274 NOP
-               
-               260         276 LOAD_FAST                4 (model)
-                           278 LOAD_ATTR                8 (_default_manager)
-                           288 LOAD_METHOD              9 (using)
-                           310 LOAD_GLOBAL             20 (settings)
-                           322 LOAD_ATTR               11 (POWER_QUERY_DB_ALIAS)
-                           332 PRECALL                  1
-                           336 CALL                     1
-               
-               261         346 LOAD_FAST                0 (self)
-               
-               262         348 LOAD_FAST                2 (arguments)
-               
-               263         350 LOAD_FAST                2 (arguments)
-               
-               264         352 LOAD_FAST                0 (self)
-                           354 LOAD_ATTR               12 (_invoke)
-               
-               259         364 LOAD_CONST               4 (('conn', 'query', 'args', 'arguments', 'invoke'))
-                           366 BUILD_CONST_KEY_MAP      5
-               
-               265         368 LOAD_FAST                5 (connections)
-               
-               259         370 DICT_UPDATE              1
-                           372 STORE_FAST               6 (locals_)
-               
-               267         374 LOAD_GLOBAL             27 (NULL + dict_hash)
-               
-               268         386 LOAD_CONST               5 ('query')
-                           388 LOAD_FAST                0 (self)
-                           390 LOAD_ATTR               14 (pk)
-                           400 BUILD_MAP                1
-                           402 LOAD_FAST                2 (arguments)
-                           404 POP_JUMP_FORWARD_IF_FALSE     2 (to 410)
-                           406 LOAD_FAST                2 (arguments)
-                           408 JUMP_FORWARD             1 (to 412)
-                       >>  410 BUILD_MAP                0
-                       >>  412 DICT_UPDATE              1
-               
-               267         414 PRECALL                  1
-                           418 CALL                     1
-                           428 STORE_FAST               7 (signature)
-               
-               270         430 LOAD_FAST                3 (use_existing)
-                           432 POP_JUMP_FORWARD_IF_FALSE    63 (to 560)
-               
-               271         434 LOAD_GLOBAL             30 (Dataset)
-                           446 LOAD_ATTR                6 (objects)
-                           456 LOAD_METHOD              7 (filter)
-                           478 LOAD_FAST                0 (self)
-                           480 LOAD_FAST                7 (signature)
-                           482 KW_NAMES                 6
-                           484 PRECALL                  2
-                           488 CALL                     2
-                           498 LOAD_METHOD             16 (first)
-                           520 PRECALL                  0
-                           524 CALL                     0
-                           534 COPY                     1
-                           536 STORE_FAST               8 (ds)
-               
-               270         538 POP_JUMP_FORWARD_IF_FALSE    10 (to 560)
-               
-               273         540 LOAD_FAST                8 (ds)
-                           542 LOAD_FAST                8 (ds)
-                           544 LOAD_ATTR               17 (extra)
-                           554 BUILD_TUPLE              2
-                           556 STORE_FAST               9 (return_value)
-                           558 JUMP_FORWARD           207 (to 974)
-               
-               275     >>  560 LOAD_GLOBAL             37 (NULL + exec)
-                           572 LOAD_FAST                0 (self)
-                           574 LOAD_ATTR               19 (code)
-                           584 LOAD_GLOBAL             41 (NULL + globals)
-                           596 PRECALL                  0
-                           600 CALL                     0
-                           610 LOAD_FAST                6 (locals_)
-                           612 PRECALL                  3
-                           616 CALL                     3
-                           626 POP_TOP
-               
-               276         628 LOAD_FAST                6 (locals_)
-                           630 LOAD_METHOD             21 (get)
-                           652 LOAD_CONST               7 ('result')
-                           654 LOAD_CONST               0 (None)
-                           656 PRECALL                  2
-                           660 CALL                     2
-                           670 STORE_FAST              10 (result)
-               
-               277         672 LOAD_FAST                6 (locals_)
-                           674 LOAD_METHOD             21 (get)
-                           696 LOAD_CONST               8 ('extra')
-                           698 LOAD_CONST               0 (None)
-                           700 PRECALL                  2
-                           704 CALL                     2
-                           714 STORE_FAST              11 (extra)
+               247          52 LOAD_GLOBAL              5 (NULL + get_user_model)
+                            64 PRECALL                  0
+                            68 CALL                     0
+                            78 BUILD_LIST               1
+                            80 STORE_FAST               5 (connections_model)
+               
+               248          82 LOAD_GLOBAL              6 (settings)
+                            94 LOAD_ATTR                4 (POWER_QUERY_EXTRA_CONNECTIONS)
+                           104 POP_JUMP_FORWARD_IF_FALSE    41 (to 188)
+               
+               249         106 LOAD_FAST                5 (connections_model)
+                           108 LOAD_METHOD              5 (extend)
+               
+               250         130 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 250>)
+                           132 MAKE_FUNCTION            0
+               
+               252         134 LOAD_GLOBAL              6 (settings)
+                           146 LOAD_ATTR                4 (POWER_QUERY_EXTRA_CONNECTIONS)
+               
+               250         156 GET_ITER
+                           158 PRECALL                  0
+                           162 CALL                     0
+               
+               249         172 PRECALL                  1
+                           176 CALL                     1
+                           186 POP_TOP
+               
+               255     >>  188 LOAD_CONST               2 (<code object <dictcomp>, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 255>)
+                           190 MAKE_FUNCTION            0
+               
+               259         192 LOAD_FAST                5 (connections_model)
+               
+               255         194 GET_ITER
+                           196 PRECALL                  0
+                           200 CALL                     0
+                           210 STORE_FAST               6 (connections)
+               
+               262         212 LOAD_FAST                0 (self)
+                           214 LOAD_ATTR                6 (owner)
+                           224 LOAD_ATTR                7 (is_superuser)
+                           234 POP_JUMP_FORWARD_IF_FALSE    34 (to 304)
+               
+               263         236 LOAD_GLOBAL             16 (Query)
+                           248 LOAD_ATTR                9 (objects)
+                           258 LOAD_METHOD             10 (filter)
+                           280 PRECALL                  0
+                           284 CALL                     0
+                           294 LOAD_FAST                6 (connections)
+                           296 LOAD_CONST               3 ('QueryManager')
+                           298 STORE_SUBSCR
+                           302 JUMP_FORWARD            40 (to 384)
+               
+               265     >>  304 LOAD_GLOBAL             16 (Query)
+                           316 LOAD_ATTR                9 (objects)
+                           326 LOAD_METHOD             10 (filter)
+                           348 LOAD_FAST                0 (self)
+                           350 LOAD_ATTR                6 (owner)
+                           360 KW_NAMES                 4
+                           362 PRECALL                  1
+                           366 CALL                     1
+                           376 LOAD_FAST                6 (connections)
+                           378 LOAD_CONST               3 ('QueryManager')
+                           380 STORE_SUBSCR
+               
+               267     >>  384 NOP
+               
+               269         386 LOAD_FAST                4 (model)
+                           388 LOAD_ATTR               11 (_default_manager)
+                           398 LOAD_METHOD             12 (using)
+                           420 LOAD_GLOBAL              6 (settings)
+                           432 LOAD_ATTR               13 (POWER_QUERY_DB_ALIAS)
+                           442 PRECALL                  1
+                           446 CALL                     1
+               
+               270         456 LOAD_FAST                0 (self)
+               
+               271         458 LOAD_FAST                2 (arguments)
+               
+               272         460 LOAD_FAST                2 (arguments)
+               
+               273         462 LOAD_FAST                0 (self)
+                           464 LOAD_ATTR               14 (_invoke)
+               
+               268         474 LOAD_CONST               5 (('conn', 'query', 'args', 'arguments', 'invoke'))
+                           476 BUILD_CONST_KEY_MAP      5
+               
+               274         478 LOAD_FAST                6 (connections)
+               
+               268         480 DICT_UPDATE              1
+                           482 STORE_FAST               7 (locals_)
+               
+               276         484 LOAD_GLOBAL             31 (NULL + dict_hash)
+               
+               277         496 LOAD_CONST               6 ('query')
+                           498 LOAD_FAST                0 (self)
+                           500 LOAD_ATTR               16 (pk)
+                           510 BUILD_MAP                1
+                           512 LOAD_FAST                2 (arguments)
+                           514 POP_JUMP_FORWARD_IF_FALSE     2 (to 520)
+                           516 LOAD_FAST                2 (arguments)
+                           518 JUMP_FORWARD             1 (to 522)
+                       >>  520 BUILD_MAP                0
+                       >>  522 DICT_UPDATE              1
+               
+               276         524 PRECALL                  1
+                           528 CALL                     1
+                           538 STORE_FAST               8 (signature)
+               
+               279         540 LOAD_FAST                3 (use_existing)
+                           542 POP_JUMP_FORWARD_IF_FALSE    63 (to 670)
+               
+               280         544 LOAD_GLOBAL             34 (Dataset)
+                           556 LOAD_ATTR                9 (objects)
+                           566 LOAD_METHOD             10 (filter)
+                           588 LOAD_FAST                0 (self)
+                           590 LOAD_FAST                8 (signature)
+                           592 KW_NAMES                 7
+                           594 PRECALL                  2
+                           598 CALL                     2
+                           608 LOAD_METHOD             18 (first)
+                           630 PRECALL                  0
+                           634 CALL                     0
+                           644 COPY                     1
+                           646 STORE_FAST               9 (ds)
+               
+               279         648 POP_JUMP_FORWARD_IF_FALSE    10 (to 670)
+               
+               282         650 LOAD_FAST                9 (ds)
+                           652 LOAD_FAST                9 (ds)
+                           654 LOAD_ATTR               19 (extra)
+                           664 BUILD_TUPLE              2
+                           666 STORE_FAST              10 (return_value)
+                           668 JUMP_FORWARD           207 (to 1084)
+               
+               284     >>  670 LOAD_GLOBAL             41 (NULL + exec)
+                           682 LOAD_FAST                0 (self)
+                           684 LOAD_ATTR               21 (code)
+                           694 LOAD_GLOBAL             45 (NULL + globals)
+                           706 PRECALL                  0
+                           710 CALL                     0
+                           720 LOAD_FAST                7 (locals_)
+                           722 PRECALL                  3
+                           726 CALL                     3
+                           736 POP_TOP
+               
+               285         738 LOAD_FAST                7 (locals_)
+                           740 LOAD_METHOD             23 (get)
+                           762 LOAD_CONST               8 ('result')
+                           764 LOAD_CONST               0 (None)
+                           766 PRECALL                  2
+                           770 CALL                     2
+                           780 STORE_FAST              11 (result)
+               
+               286         782 LOAD_FAST                7 (locals_)
+                           784 LOAD_METHOD             23 (get)
+                           806 LOAD_CONST               9 ('extra')
+                           808 LOAD_CONST               0 (None)
+                           810 PRECALL                  2
+                           814 CALL                     2
+                           824 STORE_FAST              12 (extra)
+               
+               288         826 LOAD_FAST                1 (persist)
+                           828 POP_JUMP_FORWARD_IF_FALSE   123 (to 1076)
+               
+               290         830 LOAD_GLOBAL             49 (NULL + type)
+                           842 LOAD_FAST               11 (result)
+                           844 PRECALL                  1
+                           848 CALL                     1
+                           858 LOAD_ATTR               25 (__name__)
+               
+               291         868 LOAD_FAST                2 (arguments)
+               
+               289         870 LOAD_CONST              10 (('type', 'arguments'))
+                           872 BUILD_CONST_KEY_MAP      2
+                           874 STORE_FAST              13 (info)
+               
+               293         876 LOAD_GLOBAL             34 (Dataset)
+                           888 LOAD_ATTR                9 (objects)
+                           898 LOAD_METHOD             26 (update_or_create)
+               
+               294         920 LOAD_FAST                0 (self)
+               
+               295         922 LOAD_FAST                8 (signature)
+               
+               297         924 LOAD_FAST               13 (info)
+               
+               298         926 LOAD_GLOBAL             55 (NULL + timezone)
+                           938 LOAD_ATTR               28 (now)
+                           948 PRECALL                  0
+                           952 CALL                     0
+               
+               299         962 LOAD_GLOBAL             59 (NULL + pickle)
+                           974 LOAD_ATTR               30 (dumps)
+                           984 LOAD_FAST               11 (result)
+                           986 PRECALL                  1
+                           990 CALL                     1
+               
+               300        1000 LOAD_GLOBAL             59 (NULL + pickle)
+                          1012 LOAD_ATTR               30 (dumps)
+                          1022 LOAD_FAST               12 (extra)
+                          1024 PRECALL                  1
+                          1028 CALL                     1
+               
+               296        1038 LOAD_CONST              11 (('info', 'last_run', 'value', 'extra'))
+                          1040 BUILD_CONST_KEY_MAP      4
+               
+               293        1042 KW_NAMES                12
+                          1044 PRECALL                  3
+                          1048 CALL                     3
+                          1058 UNPACK_SEQUENCE          2
+                          1062 STORE_FAST              14 (dataset)
+                          1064 STORE_FAST              15 (__)
+               
+               303        1066 LOAD_FAST               14 (dataset)
+                          1068 LOAD_FAST               12 (extra)
+                          1070 BUILD_TUPLE              2
+                          1072 STORE_FAST              10 (return_value)
+                          1074 JUMP_FORWARD             4 (to 1084)
+               
+               305     >> 1076 LOAD_FAST               11 (result)
+                          1078 LOAD_FAST               12 (extra)
+                          1080 BUILD_TUPLE              2
+                          1082 STORE_FAST              10 (return_value)
+                       >> 1084 JUMP_FORWARD            34 (to 1154)
+                       >> 1086 PUSH_EXC_INFO
+               
+               306        1088 LOAD_GLOBAL             62 (Exception)
+                          1100 CHECK_EXC_MATCH
+                          1102 POP_JUMP_FORWARD_IF_FALSE    21 (to 1146)
+                          1104 STORE_FAST              16 (e)
+               
+               307        1106 LOAD_GLOBAL             65 (NULL + QueryRunError)
+                          1118 LOAD_FAST               16 (e)
+                          1120 PRECALL                  1
+                          1124 CALL                     1
+                          1134 LOAD_FAST               16 (e)
+                          1136 RAISE_VARARGS            2
+                       >> 1138 LOAD_CONST               0 (None)
+                          1140 STORE_FAST              16 (e)
+                          1142 DELETE_FAST             16 (e)
+                          1144 RERAISE                  1
+               
+               306     >> 1146 RERAISE                  0
+                       >> 1148 COPY                     3
+                          1150 POP_EXCEPT
+                          1152 RERAISE                  1
                
-               279         716 LOAD_FAST                1 (persist)
-                           718 POP_JUMP_FORWARD_IF_FALSE   123 (to 966)
-               
-               281         720 LOAD_GLOBAL             45 (NULL + type)
-                           732 LOAD_FAST               10 (result)
-                           734 PRECALL                  1
-                           738 CALL                     1
-                           748 LOAD_ATTR               23 (__name__)
-               
-               282         758 LOAD_FAST                2 (arguments)
-               
-               280         760 LOAD_CONST               9 (('type', 'arguments'))
-                           762 BUILD_CONST_KEY_MAP      2
-                           764 STORE_FAST              12 (info)
-               
-               284         766 LOAD_GLOBAL             30 (Dataset)
-                           778 LOAD_ATTR                6 (objects)
-                           788 LOAD_METHOD             24 (update_or_create)
-               
-               285         810 LOAD_FAST                0 (self)
-               
-               286         812 LOAD_FAST                7 (signature)
-               
-               288         814 LOAD_FAST               12 (info)
-               
-               289         816 LOAD_GLOBAL             51 (NULL + timezone)
-                           828 LOAD_ATTR               26 (now)
-                           838 PRECALL                  0
-                           842 CALL                     0
-               
-               290         852 LOAD_GLOBAL             55 (NULL + pickle)
-                           864 LOAD_ATTR               28 (dumps)
-                           874 LOAD_FAST               10 (result)
-                           876 PRECALL                  1
-                           880 CALL                     1
-               
-               291         890 LOAD_GLOBAL             55 (NULL + pickle)
-                           902 LOAD_ATTR               28 (dumps)
-                           912 LOAD_FAST               11 (extra)
-                           914 PRECALL                  1
-                           918 CALL                     1
-               
-               287         928 LOAD_CONST              10 (('info', 'last_run', 'value', 'extra'))
-                           930 BUILD_CONST_KEY_MAP      4
-               
-               284         932 KW_NAMES                11
-                           934 PRECALL                  3
-                           938 CALL                     3
-                           948 UNPACK_SEQUENCE          2
-                           952 STORE_FAST              13 (dataset)
-                           954 STORE_FAST              14 (__)
-               
-               294         956 LOAD_FAST               13 (dataset)
-                           958 LOAD_FAST               11 (extra)
-                           960 BUILD_TUPLE              2
-                           962 STORE_FAST               9 (return_value)
-                           964 JUMP_FORWARD             4 (to 974)
-               
-               296     >>  966 LOAD_FAST               10 (result)
-                           968 LOAD_FAST               11 (extra)
-                           970 BUILD_TUPLE              2
-                           972 STORE_FAST               9 (return_value)
-                       >>  974 JUMP_FORWARD            34 (to 1044)
-                       >>  976 PUSH_EXC_INFO
-               
-               297         978 LOAD_GLOBAL             58 (Exception)
-                           990 CHECK_EXC_MATCH
-                           992 POP_JUMP_FORWARD_IF_FALSE    21 (to 1036)
-                           994 STORE_FAST              15 (e)
-               
-               298         996 LOAD_GLOBAL             61 (NULL + QueryRunError)
-                          1008 LOAD_FAST               15 (e)
-                          1010 PRECALL                  1
-                          1014 CALL                     1
-                          1024 LOAD_FAST               15 (e)
-                          1026 RAISE_VARARGS            2
-                       >> 1028 LOAD_CONST               0 (None)
-                          1030 STORE_FAST              15 (e)
-                          1032 DELETE_FAST             15 (e)
-                          1034 RERAISE                  1
-               
-               297     >> 1036 RERAISE                  0
-                       >> 1038 COPY                     3
-                          1040 POP_EXCEPT
-                          1042 RERAISE                  1
-               
-               299     >> 1044 LOAD_FAST                9 (return_value)
-                          1046 RETURN_VALUE
+               308     >> 1154 LOAD_FAST               10 (return_value)
+                          1156 RETURN_VALUE
                ExceptionTable:
-                 276 to 972 -> 976 [0]
-                 976 to 994 -> 1038 [1] lasti
-                 996 to 1026 -> 1028 [1] lasti
-                 1028 to 1036 -> 1038 [1] lasti
+                 386 to 1082 -> 1086 [0]
+                 1086 to 1104 -> 1148 [1] lasti
+                 1106 to 1136 -> 1138 [1] lasti
+                 1138 to 1146 -> 1148 [1] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
+                     stacksize : 5
+                     flags     : 19
+                     code
+                        0x970067007c005d167d017401000000000000000000006a010000000000
+                        0000007c01a6010000ab01000000000000000091028c175300
+                     250           0 RESUME                   0
+                                   2 BUILD_LIST               0
+                                   4 LOAD_FAST                0 (.0)
+                             >>    6 FOR_ITER                22 (to 52)
+                     
+                     252           8 STORE_FAST               1 (label2model)
+                     
+                     251          10 LOAD_GLOBAL              1 (NULL + django_apps)
+                                  22 LOAD_ATTR                1 (get_model)
+                                  32 LOAD_FAST                1 (label2model)
+                                  34 PRECALL                  1
+                                  38 CALL                     1
+                     
+                     250          48 LIST_APPEND              2
+                                  50 JUMP_BACKWARD           23 (to 6)
+                             >>   52 RETURN_VALUE
+                     consts
+                     names      ('django_apps', 'get_model')
+                     varnames   ('.0', 'label2model')
+                     freevars   ()
+                     cellvars   ()
+                     filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
+                     name       '<listcomp>'
+                     firstlineno 250
+                     lnotab 0x080202ff26ff
+                  code
+                     argcount  : 1
+                     nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x970069007c005d347d017c016a0000000000000000006a010000000000
                         0000009b0064009d027c016a020000000000000000a00300000000000000
                         000000000000000000000000007408000000000000000000006a05000000
                         0000000000a6010000ab01000000000000000093028c355300
-                     244           0 RESUME                   0
+                     255           0 RESUME                   0
                                    2 BUILD_MAP                0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                52 (to 112)
                      
-                     248           8 STORE_FAST               1 (model)
+                     259           8 STORE_FAST               1 (model)
                      
-                     245          10 LOAD_FAST                1 (model)
+                     256          10 LOAD_FAST                1 (model)
                                   12 LOAD_ATTR                0 (_meta)
                                   22 LOAD_ATTR                1 (object_name)
                                   32 FORMAT_VALUE             0
                                   34 LOAD_CONST               0 ('Manager')
                                   36 BUILD_STRING             2
                                   38 LOAD_FAST                1 (model)
                                   40 LOAD_ATTR                2 (_default_manager)
                                   50 LOAD_METHOD              3 (using)
                      
-                     246          72 LOAD_GLOBAL              8 (settings)
+                     257          72 LOAD_GLOBAL              8 (settings)
                                   84 LOAD_ATTR                5 (POWER_QUERY_DB_ALIAS)
                      
-                     245          94 PRECALL                  1
+                     256          94 PRECALL                  1
                                   98 CALL                     1
                      
-                     244         108 MAP_ADD                  2
+                     255         108 MAP_ADD                  2
                                  110 JUMP_BACKWARD           53 (to 6)
                              >>  112 RETURN_VALUE
                      consts
                         'Manager'
                      names      ('_meta', 'object_name', '_default_manager', 'using', 'settings', 'POWER_QUERY_DB_ALIAS')
                      varnames   ('.0', 'model')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                      name       '<dictcomp>'
-                     firstlineno 244
+                     firstlineno 255
                      lnotab 0x080402fd3e0116ff0eff
                   'QueryManager'
                   ('owner',)
                   ('conn', 'query', 'args', 'arguments', 'invoke')
                   'query'
                   ('query', 'hash')
                   'result'
                   'extra'
                   ('type', 'arguments')
                   ('info', 'last_run', 'value', 'extra')
                   ('query', 'hash', 'defaults')
-               names      ('target', 'model_class', 'get_user_model', 'owner', 'is_superuser', 'Query', 'objects', 'filter', '_default_manager', 'using', 'settings', 'POWER_QUERY_DB_ALIAS', '_invoke', 'dict_hash', 'pk', 'Dataset', 'first', 'extra', 'exec', 'code', 'globals', 'get', 'type', '__name__', 'update_or_create', 'timezone', 'now', 'pickle', 'dumps', 'Exception', 'QueryRunError')
-               varnames   ('self', 'persist', 'arguments', 'use_existing', 'model', 'connections', 'locals_', 'signature', 'ds', 'return_value', 'result', 'extra', 'info', 'dataset', '__', 'e')
+               names      ('target', 'model_class', 'get_user_model', 'settings', 'POWER_QUERY_EXTRA_CONNECTIONS', 'extend', 'owner', 'is_superuser', 'Query', 'objects', 'filter', '_default_manager', 'using', 'POWER_QUERY_DB_ALIAS', '_invoke', 'dict_hash', 'pk', 'Dataset', 'first', 'extra', 'exec', 'code', 'globals', 'get', 'type', '__name__', 'update_or_create', 'timezone', 'now', 'pickle', 'dumps', 'Exception', 'QueryRunError')
+               varnames   ('self', 'persist', 'arguments', 'use_existing', 'model', 'connections_model', 'connections', 'locals_', 'signature', 'ds', 'return_value', 'result', 'extra', 'info', 'dataset', '__', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'run'
-               firstlineno 237
+               firstlineno 239
                lnotab
-                  0x0206320104051aff02fc1209180144025002020246010201020102010c
-                  fb040602fa04080c011cff1003040168ff0203140244012c012c02040226
-                  0102fe06042c010201020202012401260126fc04fd180a0a020c01120128
-                  ff0802
+                  0x020632021e0118011801040216fe10ff1006040402fc12071801440250
+                  02020246010201020102010cfb040602fa04080c011cff1003040168ff02
+                  03140244012c012c020402260102fe06042c010201020202012401260126
+                  fc04fd180a0a020c01120128ff0802
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x9700640164026c006d017d0101007c01a0020000000000000000000000
                   0000000000000000007c006a030000000000000000a6010000ab01000000
                   00000000007d027c026a0300000000000000007c005f0400000000000000
                   007c00a0050000000000000000000000000000000000000000a6000000ab
                   00000000000000000001007c026a0300000000000000005300
-               301           0 RESUME                   0
+               310           0 RESUME                   0
                
-               302           2 LOAD_CONST               1 (0)
+               311           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('run_background_query',))
                              6 IMPORT_NAME              0 (power_query.celery_tasks)
                              8 IMPORT_FROM              1 (run_background_query)
                             10 STORE_FAST               1 (run_background_query)
                             12 POP_TOP
                
-               304          14 LOAD_FAST                1 (run_background_query)
+               313          14 LOAD_FAST                1 (run_background_query)
                             16 LOAD_METHOD              2 (delay)
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                3 (id)
                             50 PRECALL                  1
                             54 CALL                     1
                             64 STORE_FAST               2 (res)
                
-               305          66 LOAD_FAST                2 (res)
+               314          66 LOAD_FAST                2 (res)
                             68 LOAD_ATTR                3 (id)
                             78 LOAD_FAST                0 (self)
                             80 STORE_ATTR               4 (celery_task)
                
-               306          90 LOAD_FAST                0 (self)
+               315          90 LOAD_FAST                0 (self)
                             92 LOAD_METHOD              5 (save)
                            114 PRECALL                  0
                            118 CALL                     0
                            128 POP_TOP
                
-               307         130 LOAD_FAST                2 (res)
+               316         130 LOAD_FAST                2 (res)
                            132 LOAD_ATTR                3 (id)
                            142 RETURN_VALUE
                consts
                   None
                   0
                   ('run_background_query',)
                names      ('power_query.celery_tasks', 'run_background_query', 'delay', 'id', 'celery_task', 'save')
                varnames   ('self', 'run_background_query', 'res')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '_queue'
-               firstlineno 301
+               firstlineno 310
                lnotab 0x02010c02340118012801
             (False, False, None, None)
             (True,)
             (False, None, False)
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'name', 'TextField', 'description', 'ForeignKey', 'get_user_model', 'CASCADE', 'owner', 'ContentType', 'target', 'code', 'JSONField', 'dict', 'PQJSONEncoder', 'info', 'Parametrizer', 'parametrizer', 'sentry_error_id', 'error_message', 'DateTimeField', 'last_run', 'BooleanField', 'active', 'str', '__str__', 'Meta', 'bool', 'Optional', 'Any', 'save', 'int', 'List', 'Dict', '_invoke', 'QueryMatrixResult', 'update_results', 'execute_matrix', 'QueryResult', 'run', '_queue', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'Query'
-         firstlineno 150
+         firstlineno 152
          lnotab
             0x0c01240124010e0120ff12032e0124011c010e0112ff12032601260224
             0222020c031a0602010201020102fb040202fe020302fd02040efc02050e
             fb020602fa0c0b1405100716280201020102fc040202fe02030efd020402
-            fc020502fb0840
+            fc020502fb0847
       'Query'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
@@ -2822,139 +2897,139 @@
             0064016401ac05a6020000ab0200000000000000005a0e0200650f651064
             01ac0aa6020000ab0200000000000000005a11020065036a0d0000000000
             00000064016401640bac0ca6030000ab0300000000000000005a12640d65
             136602640e84045a146515640d65166602640f8404a6000000ab00000000
             00000000005a176515640d6518660264108404a6000000ab000000000000
             0000005a196515640d651a660264118404a6000000ab0000000000000000
             005a1b64125300
-         310           0 RESUME                   0
+         319           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Dataset')
                        8 STORE_NAME               2 (__qualname__)
          
-         311          10 PUSH_NULL
+         320          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (CharField)
                       24 LOAD_CONST               1 (True)
                       26 LOAD_CONST               2 (200)
                       28 LOAD_CONST               3 (False)
                       30 KW_NAMES                 4
                       32 PRECALL                  3
                       36 CALL                     3
                       46 STORE_NAME               5 (hash)
          
-         312          48 PUSH_NULL
+         321          48 PUSH_NULL
                       50 LOAD_NAME                3 (models)
                       52 LOAD_ATTR                6 (DateTimeField)
                       62 LOAD_CONST               1 (True)
                       64 LOAD_CONST               1 (True)
                       66 KW_NAMES                 5
                       68 PRECALL                  2
                       72 CALL                     2
                       82 STORE_NAME               7 (last_run)
          
-         313          84 PUSH_NULL
+         322          84 PUSH_NULL
                       86 LOAD_NAME                3 (models)
                       88 LOAD_ATTR                4 (CharField)
                       98 LOAD_CONST               6 (100)
                      100 KW_NAMES                 7
                      102 PRECALL                  1
                      106 CALL                     1
                      116 STORE_NAME               8 (description)
          
-         314         118 PUSH_NULL
+         323         118 PUSH_NULL
                      120 LOAD_NAME                3 (models)
                      122 LOAD_ATTR                9 (ForeignKey)
                      132 LOAD_NAME               10 (Query)
                      134 LOAD_NAME                3 (models)
                      136 LOAD_ATTR               11 (CASCADE)
                      146 LOAD_CONST               8 ('datasets')
                      148 KW_NAMES                 9
                      150 PRECALL                  3
                      154 CALL                     3
                      164 STORE_NAME              12 (query)
          
-         315         166 PUSH_NULL
+         324         166 PUSH_NULL
                      168 LOAD_NAME                3 (models)
                      170 LOAD_ATTR               13 (BinaryField)
                      180 LOAD_CONST               1 (True)
                      182 LOAD_CONST               1 (True)
                      184 KW_NAMES                 5
                      186 PRECALL                  2
                      190 CALL                     2
                      200 STORE_NAME              14 (value)
          
-         316         202 PUSH_NULL
+         325         202 PUSH_NULL
                      204 LOAD_NAME               15 (JSONField)
                      206 LOAD_NAME               16 (dict)
                      208 LOAD_CONST               1 (True)
                      210 KW_NAMES                10
                      212 PRECALL                  2
                      216 CALL                     2
                      226 STORE_NAME              17 (info)
          
-         317         228 PUSH_NULL
+         326         228 PUSH_NULL
                      230 LOAD_NAME                3 (models)
                      232 LOAD_ATTR               13 (BinaryField)
          
-         318         242 LOAD_CONST               1 (True)
+         327         242 LOAD_CONST               1 (True)
                      244 LOAD_CONST               1 (True)
                      246 LOAD_CONST              11 ('Any other attribute to pass to the formatter')
          
-         317         248 KW_NAMES                12
+         326         248 KW_NAMES                12
                      250 PRECALL                  3
                      254 CALL                     3
                      264 STORE_NAME              18 (extra)
          
-         321         266 LOAD_CONST              13 ('return')
+         330         266 LOAD_CONST              13 ('return')
                      268 LOAD_NAME               19 (str)
                      270 BUILD_TUPLE              2
-                     272 LOAD_CONST              14 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 321>)
+                     272 LOAD_CONST              14 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 330>)
                      274 MAKE_FUNCTION            4 (annotations)
                      276 STORE_NAME              20 (__str__)
          
-         324         278 LOAD_NAME               21 (property)
+         333         278 LOAD_NAME               21 (property)
          
-         325         280 LOAD_CONST              13 ('return')
+         334         280 LOAD_CONST              13 ('return')
                      282 LOAD_NAME               22 (Any)
                      284 BUILD_TUPLE              2
-                     286 LOAD_CONST              15 (<code object data, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 324>)
+                     286 LOAD_CONST              15 (<code object data, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 333>)
                      288 MAKE_FUNCTION            4 (annotations)
          
-         324         290 PRECALL                  0
+         333         290 PRECALL                  0
                      294 CALL                     0
          
-         325         304 STORE_NAME              23 (data)
+         334         304 STORE_NAME              23 (data)
          
-         328         306 LOAD_NAME               21 (property)
+         337         306 LOAD_NAME               21 (property)
          
-         329         308 LOAD_CONST              13 ('return')
+         338         308 LOAD_CONST              13 ('return')
                      310 LOAD_NAME               24 (int)
                      312 BUILD_TUPLE              2
-                     314 LOAD_CONST              16 (<code object size, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 328>)
+                     314 LOAD_CONST              16 (<code object size, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 337>)
                      316 MAKE_FUNCTION            4 (annotations)
          
-         328         318 PRECALL                  0
+         337         318 PRECALL                  0
                      322 CALL                     0
          
-         329         332 STORE_NAME              25 (size)
+         338         332 STORE_NAME              25 (size)
          
-         332         334 LOAD_NAME               21 (property)
+         341         334 LOAD_NAME               21 (property)
          
-         333         336 LOAD_CONST              13 ('return')
+         342         336 LOAD_CONST              13 ('return')
                      338 LOAD_NAME               26 (Dict)
                      340 BUILD_TUPLE              2
-                     342 LOAD_CONST              17 (<code object arguments, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 332>)
+                     342 LOAD_CONST              17 (<code object arguments, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 341>)
                      344 MAKE_FUNCTION            4 (annotations)
          
-         332         346 PRECALL                  0
+         341         346 PRECALL                  0
                      350 CALL                     0
          
-         333         360 STORE_NAME              27 (arguments)
+         342         360 STORE_NAME              27 (arguments)
                      362 LOAD_CONST              18 (None)
                      364 RETURN_VALUE
          consts
             'Dataset'
             True
             200
             False
@@ -2972,17 +3047,17 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970064017c006a0000000000000000006a0100000000000000009b0064
                   027c006a0200000000000000009b009d045300
-               321           0 RESUME                   0
+               330           0 RESUME                   0
                
-               322           2 LOAD_CONST               1 ('Result of ')
+               331           2 LOAD_CONST               1 ('Result of ')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (query)
                             16 LOAD_ATTR                1 (name)
                             26 FORMAT_VALUE             0
                             28 LOAD_CONST               2 (' ')
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (arguments)
@@ -2995,80 +3070,80 @@
                   ' '
                names      ('query', 'name', 'arguments')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '__str__'
-               firstlineno 321
+               firstlineno 330
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   00000000000000a6010000ab0100000000000000005300
-               324           0 RESUME                   0
+               333           0 RESUME                   0
                
-               326           2 LOAD_GLOBAL              1 (NULL + pickle)
+               335           2 LOAD_GLOBAL              1 (NULL + pickle)
                             14 LOAD_ATTR                1 (loads)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (value)
                             36 PRECALL                  1
                             40 CALL                     1
                             50 RETURN_VALUE
                consts
                   None
                names      ('pickle', 'loads', 'value')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'data'
-               firstlineno 324
+               firstlineno 333
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-               328           0 RESUME                   0
+               337           0 RESUME                   0
                
-               330           2 LOAD_GLOBAL              1 (NULL + len)
+               339           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (value)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('len', 'value')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'size'
-               firstlineno 328
+               firstlineno 337
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016900a6020000ab0200000000000000005300
-               332           0 RESUME                   0
+               341           0 RESUME                   0
                
-               334           2 LOAD_FAST                0 (self)
+               343           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (info)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('arguments')
                             38 BUILD_MAP                0
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -3077,24 +3152,24 @@
                   'arguments'
                names      ('info', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'arguments'
-               firstlineno 332
+               firstlineno 341
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'hash', 'DateTimeField', 'last_run', 'description', 'ForeignKey', 'Query', 'CASCADE', 'query', 'BinaryField', 'value', 'JSONField', 'dict', 'info', 'extra', 'str', '__str__', 'property', 'Any', 'data', 'int', 'size', 'Dict', 'arguments')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'Dataset'
-         firstlineno 310
+         firstlineno 319
          lnotab
             0x0a01260124012201300124011a010e0106ff12040c0302010aff0e0102
             0302010aff0e01020302010aff0e01
       'Dataset'
       code
          argcount  : 0
          nlocals   : 0
@@ -3103,65 +3178,65 @@
          code
             0x970065005a0164005a02020065036a0400000000000000006401640264
             026402ac03a6040000ab0400000000000000005a05020065036a04000000
             000000000064046506ac05a6020000ab0200000000000000005a07020065
             036a08000000000000000064026402ac06a6020000ab0200000000000000
             005a096407650a6602640884045a0b6409650c6407650a6604640a84045a
             0d640b5300
-         337           0 RESUME                   0
+         346           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Formatter')
                        8 STORE_NAME               2 (__qualname__)
          
-         338          10 PUSH_NULL
+         347          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (CharField)
                       24 LOAD_CONST               1 (255)
                       26 LOAD_CONST               2 (True)
                       28 LOAD_CONST               2 (True)
                       30 LOAD_CONST               2 (True)
                       32 KW_NAMES                 3
                       34 PRECALL                  4
                       38 CALL                     4
                       48 STORE_NAME               5 (name)
          
-         339          50 PUSH_NULL
+         348          50 PUSH_NULL
                       52 LOAD_NAME                3 (models)
                       54 LOAD_ATTR                4 (CharField)
                       64 LOAD_CONST               4 (5)
                       66 LOAD_NAME                6 (MIMETYPES)
                       68 KW_NAMES                 5
                       70 PRECALL                  2
                       74 CALL                     2
                       84 STORE_NAME               7 (content_type)
          
-         340          86 PUSH_NULL
+         349          86 PUSH_NULL
                       88 LOAD_NAME                3 (models)
                       90 LOAD_ATTR                8 (TextField)
                      100 LOAD_CONST               2 (True)
                      102 LOAD_CONST               2 (True)
                      104 KW_NAMES                 6
                      106 PRECALL                  2
                      110 CALL                     2
                      120 STORE_NAME               9 (code)
          
-         342         122 LOAD_CONST               7 ('return')
+         351         122 LOAD_CONST               7 ('return')
                      124 LOAD_NAME               10 (str)
                      126 BUILD_TUPLE              2
-                     128 LOAD_CONST               8 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 342>)
+                     128 LOAD_CONST               8 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 351>)
                      130 MAKE_FUNCTION            4 (annotations)
                      132 STORE_NAME              11 (__str__)
          
-         345         134 LOAD_CONST               9 ('context')
+         354         134 LOAD_CONST               9 ('context')
                      136 LOAD_NAME               12 (Dict)
                      138 LOAD_CONST               7 ('return')
                      140 LOAD_NAME               10 (str)
                      142 BUILD_TUPLE              4
-                     144 LOAD_CONST              10 (<code object render, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 345>)
+                     144 LOAD_CONST              10 (<code object render, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 354>)
                      146 MAKE_FUNCTION            4 (annotations)
                      148 STORE_NAME              13 (render)
                      150 LOAD_CONST              11 (None)
                      152 RETURN_VALUE
          consts
             'Formatter'
             255
@@ -3173,31 +3248,31 @@
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a000000000000000000700164015300
-               342           0 RESUME                   0
+               351           0 RESUME                   0
                
-               343           2 LOAD_FAST                0 (self)
+               352           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (name)
                             14 JUMP_IF_TRUE_OR_POP      1 (to 18)
                             16 LOAD_CONST               1 ('')
                        >>   18 RETURN_VALUE
                consts
                   None
                   ''
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '__str__'
-               firstlineno 342
+               firstlineno 351
                lnotab 0x0201
             'context'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 3
@@ -3215,101 +3290,101 @@
                   00000064046b0200000000722f7403000000000000000000007c01640219
                   0000000000000000006a020000000000000000a6010000ab010000000000
                   0000007d027c02a003000000000000000000000000000000000000000064
                   04a6010000ab0100000000000000005300740d0000000000000000000064
                   05a6010000ab01000000000000000082017c03a007000000000000000000
                   00000000000000000000007411000000000000000000007c01a6010000ab
                   010000000000000000a6010000ab0100000000000000005300
-               345           0 RESUME                   0
+               354           0 RESUME                   0
                
-               346           2 LOAD_FAST                0 (self)
+               355           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (content_type)
                             14 LOAD_CONST               1 ('xls')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE    47 (to 118)
                
-               347          24 LOAD_GLOBAL              3 (NULL + to_dataset)
+               356          24 LOAD_GLOBAL              3 (NULL + to_dataset)
                             36 LOAD_FAST                1 (context)
                             38 LOAD_CONST               2 ('dataset')
                             40 BINARY_SUBSCR
                             50 LOAD_ATTR                2 (data)
                             60 PRECALL                  1
                             64 CALL                     1
                             74 STORE_FAST               2 (dt)
                
-               348          76 LOAD_FAST                2 (dt)
+               357          76 LOAD_FAST                2 (dt)
                             78 LOAD_METHOD              3 (export)
                            100 LOAD_CONST               1 ('xls')
                            102 PRECALL                  1
                            106 CALL                     1
                            116 RETURN_VALUE
                
-               350     >>  118 LOAD_FAST                0 (self)
+               359     >>  118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                4 (code)
                            130 POP_JUMP_FORWARD_IF_FALSE    21 (to 174)
                
-               351         132 LOAD_GLOBAL             11 (NULL + Template)
+               360         132 LOAD_GLOBAL             11 (NULL + Template)
                            144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                4 (code)
                            156 PRECALL                  1
                            160 CALL                     1
                            170 STORE_FAST               3 (tpl)
                            172 JUMP_FORWARD           131 (to 436)
                
-               352     >>  174 LOAD_FAST                0 (self)
+               361     >>  174 LOAD_FAST                0 (self)
                            176 LOAD_ATTR                0 (content_type)
                            186 LOAD_CONST               3 ('json')
                            188 COMPARE_OP               2 (==)
                            194 POP_JUMP_FORWARD_IF_FALSE    47 (to 290)
                
-               353         196 LOAD_GLOBAL              3 (NULL + to_dataset)
+               362         196 LOAD_GLOBAL              3 (NULL + to_dataset)
                            208 LOAD_FAST                1 (context)
                            210 LOAD_CONST               2 ('dataset')
                            212 BINARY_SUBSCR
                            222 LOAD_ATTR                2 (data)
                            232 PRECALL                  1
                            236 CALL                     1
                            246 STORE_FAST               2 (dt)
                
-               354         248 LOAD_FAST                2 (dt)
+               363         248 LOAD_FAST                2 (dt)
                            250 LOAD_METHOD              3 (export)
                            272 LOAD_CONST               3 ('json')
                            274 PRECALL                  1
                            278 CALL                     1
                            288 RETURN_VALUE
                
-               355     >>  290 LOAD_FAST                0 (self)
+               364     >>  290 LOAD_FAST                0 (self)
                            292 LOAD_ATTR                0 (content_type)
                            302 LOAD_CONST               4 ('yaml')
                            304 COMPARE_OP               2 (==)
                            310 POP_JUMP_FORWARD_IF_FALSE    47 (to 406)
                
-               356         312 LOAD_GLOBAL              3 (NULL + to_dataset)
+               365         312 LOAD_GLOBAL              3 (NULL + to_dataset)
                            324 LOAD_FAST                1 (context)
                            326 LOAD_CONST               2 ('dataset')
                            328 BINARY_SUBSCR
                            338 LOAD_ATTR                2 (data)
                            348 PRECALL                  1
                            352 CALL                     1
                            362 STORE_FAST               2 (dt)
                
-               357         364 LOAD_FAST                2 (dt)
+               366         364 LOAD_FAST                2 (dt)
                            366 LOAD_METHOD              3 (export)
                            388 LOAD_CONST               4 ('yaml')
                            390 PRECALL                  1
                            394 CALL                     1
                            404 RETURN_VALUE
                
-               359     >>  406 LOAD_GLOBAL             13 (NULL + ValueError)
+               368     >>  406 LOAD_GLOBAL             13 (NULL + ValueError)
                            418 LOAD_CONST               5 ('Unable to render')
                            420 PRECALL                  1
                            424 CALL                     1
                            434 RAISE_VARARGS            1
                
-               361     >>  436 LOAD_FAST                3 (tpl)
+               370     >>  436 LOAD_FAST                3 (tpl)
                            438 LOAD_METHOD              7 (render)
                            460 LOAD_GLOBAL             17 (NULL + Context)
                            472 LOAD_FAST                1 (context)
                            474 PRECALL                  1
                            478 CALL                     1
                            488 PRECALL                  1
                            492 CALL                     1
@@ -3323,24 +3398,24 @@
                   'Unable to render'
                names      ('content_type', 'to_dataset', 'data', 'export', 'code', 'Template', 'ValueError', 'render', 'Context')
                varnames   ('self', 'context', 'dt', 'tpl')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'render'
-               firstlineno 345
+               firstlineno 354
                lnotab 0x0201160134012a020e012a01160134012a01160134012a021e02
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'name', 'MIMETYPES', 'content_type', 'TextField', 'code', 'str', '__str__', 'Dict', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'Formatter'
-         firstlineno 337
+         firstlineno 346
          lnotab 0x0a012801240124020c03
       'Formatter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
@@ -3363,225 +3438,225 @@
             00640fac06a6010000ab0100000000000000005a18090009000900090064
             1d64126519641365196414651a651b190000000000000000006415651a65
             1b1900000000000000000064166411660a880066016417840d5a1c641e64
             1865196416651d6604641984055a1e6416651f6602641a84045a20641665
             1f6602641b84045a216416651f6602641c84045a22880078015a235300
                        0 MAKE_CELL                0 (__class__)
          
-         364           2 RESUME                   0
+         373           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Report')
                       10 STORE_NAME               2 (__qualname__)
          
-         365          12 PUSH_NULL
+         374          12 PUSH_NULL
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (CharField)
                       26 LOAD_CONST               1 (255)
                       28 LOAD_CONST               2 (True)
                       30 LOAD_CONST               2 (True)
                       32 LOAD_CONST               2 (True)
                       34 KW_NAMES                 3
                       36 PRECALL                  4
                       40 CALL                     4
                       50 STORE_NAME               5 (name)
          
-         366          52 PUSH_NULL
+         375          52 PUSH_NULL
                       54 LOAD_NAME                3 (models)
                       56 LOAD_ATTR                4 (CharField)
                       66 LOAD_CONST               1 (255)
                       68 LOAD_CONST               2 (True)
                       70 LOAD_CONST               2 (True)
                       72 KW_NAMES                 4
                       74 PRECALL                  3
                       78 CALL                     3
                       88 STORE_NAME               6 (document_title)
          
-         367          90 PUSH_NULL
+         376          90 PUSH_NULL
                       92 LOAD_NAME                3 (models)
                       94 LOAD_ATTR                7 (ForeignKey)
                      104 LOAD_NAME                8 (Query)
                      106 LOAD_NAME                3 (models)
                      108 LOAD_ATTR                9 (CASCADE)
                      118 KW_NAMES                 5
                      120 PRECALL                  2
                      124 CALL                     2
                      134 STORE_NAME              10 (query)
          
-         368         136 PUSH_NULL
+         377         136 PUSH_NULL
                      138 LOAD_NAME                3 (models)
                      140 LOAD_ATTR                7 (ForeignKey)
                      150 LOAD_NAME               11 (Formatter)
                      152 LOAD_NAME                3 (models)
                      154 LOAD_ATTR                9 (CASCADE)
                      164 KW_NAMES                 5
                      166 PRECALL                  2
                      170 CALL                     2
                      180 STORE_NAME              12 (formatter)
          
-         369         182 PUSH_NULL
+         378         182 PUSH_NULL
                      184 LOAD_NAME                3 (models)
                      186 LOAD_ATTR               13 (BooleanField)
                      196 LOAD_CONST               2 (True)
                      198 KW_NAMES                 6
                      200 PRECALL                  1
                      204 CALL                     1
                      214 STORE_NAME              14 (active)
          
-         370         216 PUSH_NULL
+         379         216 PUSH_NULL
                      218 LOAD_NAME                3 (models)
                      220 LOAD_ATTR                7 (ForeignKey)
          
-         371         230 PUSH_NULL
+         380         230 PUSH_NULL
                      232 LOAD_NAME               15 (get_user_model)
                      234 PRECALL                  0
                      238 CALL                     0
          
-         372         248 LOAD_CONST               2 (True)
+         381         248 LOAD_CONST               2 (True)
          
-         373         250 LOAD_CONST               2 (True)
+         382         250 LOAD_CONST               2 (True)
          
-         374         252 LOAD_NAME                3 (models)
+         383         252 LOAD_NAME                3 (models)
                      254 LOAD_ATTR                9 (CASCADE)
          
-         375         264 LOAD_CONST               7 ('+')
+         384         264 LOAD_CONST               7 ('+')
          
-         370         266 KW_NAMES                 8
+         379         266 KW_NAMES                 8
                      268 PRECALL                  5
                      272 CALL                     5
                      282 STORE_NAME              16 (owner)
          
-         377         284 PUSH_NULL
+         386         284 PUSH_NULL
                      286 LOAD_NAME                3 (models)
                      288 LOAD_ATTR               17 (ManyToManyField)
          
-         378         298 PUSH_NULL
+         387         298 PUSH_NULL
                      300 LOAD_NAME               15 (get_user_model)
                      302 PRECALL                  0
                      306 CALL                     0
                      316 LOAD_CONST               2 (True)
                      318 LOAD_CONST               7 ('+')
          
-         377         320 KW_NAMES                 9
+         386         320 KW_NAMES                 9
                      322 PRECALL                  3
                      326 CALL                     3
                      336 STORE_NAME              18 (limit_access_to)
          
-         380         338 PUSH_NULL
+         389         338 PUSH_NULL
                      340 LOAD_NAME                3 (models)
                      342 LOAD_ATTR                4 (CharField)
          
-         381         352 LOAD_CONST              10 (30)
+         390         352 LOAD_CONST              10 (30)
          
-         382         354 LOAD_CONST               2 (True)
+         391         354 LOAD_CONST               2 (True)
          
-         383         356 LOAD_CONST               2 (True)
+         392         356 LOAD_CONST               2 (True)
          
-         384         358 LOAD_CONST              11 ('Refresh every (e.g. 3 - 1/3 - mon - 1/3,Mon)')
+         393         358 LOAD_CONST              11 ('Refresh every (e.g. 3 - 1/3 - mon - 1/3,Mon)')
          
-         385         360 LOAD_CONST              12 ('mon,tue,wed,thu,fri,sat,sun')
+         394         360 LOAD_CONST              12 ('mon,tue,wed,thu,fri,sat,sun')
          
-         386         362 PUSH_NULL
+         395         362 PUSH_NULL
                      364 LOAD_NAME               19 (FrequencyValidator)
                      366 PRECALL                  0
                      370 CALL                     0
                      380 BUILD_LIST               1
          
-         380         382 KW_NAMES                13
+         389         382 KW_NAMES                13
                      384 PRECALL                  6
                      388 CALL                     6
                      398 STORE_NAME              20 (frequence)
          
-         388         400 PUSH_NULL
+         397         400 PUSH_NULL
                      402 LOAD_NAME                3 (models)
                      404 LOAD_ATTR               21 (DateTimeField)
                      414 LOAD_CONST               2 (True)
                      416 LOAD_CONST               2 (True)
                      418 KW_NAMES                14
                      420 PRECALL                  2
                      424 CALL                     2
                      434 STORE_NAME              22 (last_run)
          
-         389         436 PUSH_NULL
+         398         436 PUSH_NULL
                      438 LOAD_NAME                3 (models)
                      440 LOAD_ATTR               23 (IntegerField)
                      450 LOAD_CONST              15 (365)
                      452 KW_NAMES                 6
                      454 PRECALL                  1
                      458 CALL                     1
                      468 STORE_NAME              24 (validity_days)
          
-         393         470 NOP
+         402         470 NOP
          
-         394         472 NOP
+         403         472 NOP
          
-         395         474 NOP
+         404         474 NOP
          
-         396         476 NOP
+         405         476 NOP
          
-         391         478 LOAD_CONST              29 ((False, False, None, None))
+         400         478 LOAD_CONST              29 ((False, False, None, None))
                      480 LOAD_CONST              18 ('force_insert')
          
-         393         482 LOAD_NAME               25 (bool)
+         402         482 LOAD_NAME               25 (bool)
          
-         391         484 LOAD_CONST              19 ('force_update')
+         400         484 LOAD_CONST              19 ('force_update')
          
-         394         486 LOAD_NAME               25 (bool)
+         403         486 LOAD_NAME               25 (bool)
          
-         391         488 LOAD_CONST              20 ('using')
+         400         488 LOAD_CONST              20 ('using')
          
-         395         490 LOAD_NAME               26 (Optional)
+         404         490 LOAD_NAME               26 (Optional)
                      492 LOAD_NAME               27 (Any)
                      494 BINARY_SUBSCR
          
-         391         504 LOAD_CONST              21 ('update_fields')
+         400         504 LOAD_CONST              21 ('update_fields')
          
-         396         506 LOAD_NAME               26 (Optional)
+         405         506 LOAD_NAME               26 (Optional)
                      508 LOAD_NAME               27 (Any)
                      510 BINARY_SUBSCR
          
-         391         520 LOAD_CONST              22 ('return')
+         400         520 LOAD_CONST              22 ('return')
          
-         397         522 LOAD_CONST              17 (None)
+         406         522 LOAD_CONST              17 (None)
          
-         391         524 BUILD_TUPLE             10
+         400         524 BUILD_TUPLE             10
                      526 LOAD_CLOSURE             0 (__class__)
                      528 BUILD_TUPLE              1
-                     530 LOAD_CONST              23 (<code object save, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 391>)
+                     530 LOAD_CONST              23 (<code object save, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 400>)
                      532 MAKE_FUNCTION           13 (defaults, annotations, closure)
                      534 STORE_NAME              28 (save)
          
-         402         536 LOAD_CONST              30 ((False,))
+         411         536 LOAD_CONST              30 ((False,))
                      538 LOAD_CONST              24 ('run_query')
                      540 LOAD_NAME               25 (bool)
                      542 LOAD_CONST              22 ('return')
                      544 LOAD_NAME               29 (ReportResult)
                      546 BUILD_TUPLE              4
-                     548 LOAD_CONST              25 (<code object execute, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 402>)
+                     548 LOAD_CONST              25 (<code object execute, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 411>)
                      550 MAKE_FUNCTION            5 (defaults, annotations)
                      552 STORE_NAME              30 (execute)
          
-         448         554 LOAD_CONST              22 ('return')
+         457         554 LOAD_CONST              22 ('return')
                      556 LOAD_NAME               31 (str)
                      558 BUILD_TUPLE              2
-                     560 LOAD_CONST              26 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 448>)
+                     560 LOAD_CONST              26 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 457>)
                      562 MAKE_FUNCTION            4 (annotations)
                      564 STORE_NAME              32 (__str__)
          
-         451         566 LOAD_CONST              22 ('return')
+         460         566 LOAD_CONST              22 ('return')
                      568 LOAD_NAME               31 (str)
                      570 BUILD_TUPLE              2
-                     572 LOAD_CONST              27 (<code object get_absolute_url, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 451>)
+                     572 LOAD_CONST              27 (<code object get_absolute_url, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 460>)
                      574 MAKE_FUNCTION            4 (annotations)
                      576 STORE_NAME              33 (get_absolute_url)
          
-         454         578 LOAD_CONST              22 ('return')
+         463         578 LOAD_CONST              22 ('return')
                      580 LOAD_NAME               31 (str)
                      582 BUILD_TUPLE              2
-                     584 LOAD_CONST              28 (<code object _queue, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 454>)
+                     584 LOAD_CONST              28 (<code object _queue, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 463>)
                      586 MAKE_FUNCTION            4 (annotations)
                      588 STORE_NAME              34 (_queue)
                      590 LOAD_CLOSURE             0 (__class__)
                      592 COPY                     1
                      594 STORE_NAME              35 (__classcell__)
                      596 RETURN_VALUE
          consts
@@ -3616,26 +3691,26 @@
                code
                   0x950197007c006a000000000000000000730c7c006a0100000000000000
                   007c005f000000000000000000740500000000000000000000a6000000ab
                   000000000000000000a00300000000000000000000000000000000000000
                   007c017c027c037c04a6040000ab040000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-               391           2 RESUME                   0
+               400           2 RESUME                   0
                
-               398           4 LOAD_FAST                0 (self)
+               407           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (document_title)
                             16 POP_JUMP_FORWARD_IF_TRUE    12 (to 42)
                
-               399          18 LOAD_FAST                0 (self)
+               408          18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (name)
                             30 LOAD_FAST                0 (self)
                             32 STORE_ATTR               0 (document_title)
                
-               400     >>   42 LOAD_GLOBAL              5 (NULL + super)
+               409     >>   42 LOAD_GLOBAL              5 (NULL + super)
                             54 PRECALL                  0
                             58 CALL                     0
                             68 LOAD_METHOD              3 (save)
                             90 LOAD_FAST                1 (force_insert)
                             92 LOAD_FAST                2 (force_update)
                             94 LOAD_FAST                3 (using)
                             96 LOAD_FAST                4 (update_fields)
@@ -3648,15 +3723,15 @@
                   None
                names      ('document_title', 'name', 'super', 'save')
                varnames   ('self', 'force_insert', 'force_update', 'using', 'update_fields')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'save'
-               firstlineno 391
+               firstlineno 400
                lnotab 0x04070e011801
             'run_query'
             code
                argcount  : 2
                nlocals   : 11
                stacksize : 10
                flags     : 3
@@ -3686,140 +3761,140 @@
                   000000000000007c0aa6010000ab01000000000000000001007c03a01200
                   000000000000000000000000000000000000007c046a1300000000000000
                   007433000000000000000000007c0aa6010000ab01000000000000000066
                   02a6010000ab0100000000000000000100590064007d0a7e0a90018c4c64
                   007d0a7e0a770177007803590077017435000000000000000000006a1b00
                   00000000000000a6000000ab0000000000000000007c005f1c0000000000
                   0000007c037303640467017d037c035300
-               402           0 RESUME                   0
+               411           0 RESUME                   0
                
-               404           2 LOAD_FAST                0 (self)
+               413           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (query)
                             14 STORE_FAST               2 (query)
                
-               405          16 BUILD_LIST               0
+               414          16 BUILD_LIST               0
                             18 STORE_FAST               3 (result)
                
-               406          20 LOAD_FAST                1 (run_query)
+               415          20 LOAD_FAST                1 (run_query)
                             22 POP_JUMP_FORWARD_IF_FALSE    20 (to 64)
                
-               407          24 LOAD_FAST                2 (query)
+               416          24 LOAD_FAST                2 (query)
                             26 LOAD_METHOD              1 (execute_matrix)
                             48 PRECALL                  0
                             52 CALL                     0
                             62 POP_TOP
                
-               408     >>   64 LOAD_FAST                2 (query)
+               417     >>   64 LOAD_FAST                2 (query)
                             66 LOAD_ATTR                2 (datasets)
                             76 LOAD_METHOD              3 (all)
                             98 PRECALL                  0
                            102 CALL                     0
                            112 GET_ITER
                        >>  114 EXTENDED_ARG             1
                            116 FOR_ITER               338 (to 794)
                            118 STORE_FAST               4 (dataset)
                
-               409         120 LOAD_FAST                4 (dataset)
+               418         120 LOAD_FAST                4 (dataset)
                            122 LOAD_ATTR                4 (size)
                            132 POP_JUMP_FORWARD_IF_TRUE     1 (to 136)
                
-               410         134 JUMP_BACKWARD           11 (to 114)
+               419         134 JUMP_BACKWARD           11 (to 114)
                
-               411     >>  136 NOP
+               420     >>  136 NOP
                
-               412         138 LOAD_FAST                4 (dataset)
+               421         138 LOAD_FAST                4 (dataset)
                            140 LOAD_ATTR                5 (arguments)
                            150 STORE_FAST               5 (context)
                
-               413         152 LOAD_FAST                4 (dataset)
+               422         152 LOAD_FAST                4 (dataset)
                            154 LOAD_ATTR                6 (extra)
                            164 POP_JUMP_FORWARD_IF_FALSE    46 (to 258)
                
-               414         166 LOAD_FAST                5 (context)
+               423         166 LOAD_FAST                5 (context)
                            168 LOAD_METHOD              7 (update)
                            190 LOAD_GLOBAL             17 (NULL + pickle)
                            202 LOAD_ATTR                9 (loads)
                            212 LOAD_FAST                4 (dataset)
                            214 LOAD_ATTR                6 (extra)
                            224 PRECALL                  1
                            228 CALL                     1
                            238 JUMP_IF_TRUE_OR_POP      1 (to 242)
                            240 BUILD_MAP                0
                        >>  242 PRECALL                  1
                            246 CALL                     1
                            256 POP_TOP
                
-               418     >>  258 LOAD_FAST                0 (self)
+               427     >>  258 LOAD_FAST                0 (self)
                            260 LOAD_ATTR               10 (document_title)
                
-               417         270 POP_JUMP_FORWARD_IF_FALSE    10 (to 292)
+               426         270 POP_JUMP_FORWARD_IF_FALSE    10 (to 292)
                            272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR               10 (document_title)
                            284 LOAD_FAST                5 (context)
                            286 BINARY_OP                6 (%)
                            290 JUMP_FORWARD             6 (to 304)
                
-               419     >>  292 LOAD_FAST                0 (self)
+               428     >>  292 LOAD_FAST                0 (self)
                            294 LOAD_ATTR               10 (document_title)
                
-               416     >>  304 STORE_FAST               6 (title)
+               425     >>  304 STORE_FAST               6 (title)
                
-               421         306 LOAD_FAST                0 (self)
+               430         306 LOAD_FAST                0 (self)
                            308 LOAD_ATTR               11 (formatter)
                            318 LOAD_METHOD             12 (render)
                
-               423         340 LOAD_FAST                4 (dataset)
+               432         340 LOAD_FAST                4 (dataset)
                
-               424         342 LOAD_FAST                0 (self)
+               433         342 LOAD_FAST                0 (self)
                
-               425         344 LOAD_FAST                6 (title)
+               434         344 LOAD_FAST                6 (title)
                
-               426         346 LOAD_FAST                5 (context)
+               435         346 LOAD_FAST                5 (context)
                
-               422         348 LOAD_CONST               1 (('dataset', 'report', 'title', 'context'))
+               431         348 LOAD_CONST               1 (('dataset', 'report', 'title', 'context'))
                            350 BUILD_CONST_KEY_MAP      4
                
-               421         352 PRECALL                  1
+               430         352 PRECALL                  1
                            356 CALL                     1
                            366 STORE_FAST               7 (output)
                
-               429         368 LOAD_GLOBAL             26 (ReportDocument)
+               438         368 LOAD_GLOBAL             26 (ReportDocument)
                            380 LOAD_ATTR               14 (objects)
                            390 LOAD_METHOD             15 (update_or_create)
                
-               430         412 LOAD_FAST                0 (self)
+               439         412 LOAD_FAST                0 (self)
                
-               431         414 LOAD_FAST                4 (dataset)
+               440         414 LOAD_FAST                4 (dataset)
                
-               433         416 LOAD_FAST                6 (title)
+               442         416 LOAD_FAST                6 (title)
                
-               434         418 LOAD_FAST                0 (self)
+               443         418 LOAD_FAST                0 (self)
                            420 LOAD_ATTR               11 (formatter)
                            430 LOAD_ATTR               16 (content_type)
                
-               435         440 LOAD_GLOBAL             17 (NULL + pickle)
+               444         440 LOAD_GLOBAL             17 (NULL + pickle)
                            452 LOAD_ATTR               17 (dumps)
                            462 LOAD_FAST                7 (output)
                            464 PRECALL                  1
                            468 CALL                     1
                
-               436         478 LOAD_FAST                4 (dataset)
+               445         478 LOAD_FAST                4 (dataset)
                            480 LOAD_ATTR                5 (arguments)
                
-               432         490 LOAD_CONST               2 (('title', 'content_type', 'output', 'arguments'))
+               441         490 LOAD_CONST               2 (('title', 'content_type', 'output', 'arguments'))
                            492 BUILD_CONST_KEY_MAP      4
                
-               429         494 KW_NAMES                 3
+               438         494 KW_NAMES                 3
                            496 PRECALL                  3
                            500 CALL                     3
                            510 UNPACK_SEQUENCE          2
                            514 STORE_FAST               8 (res)
                            516 STORE_FAST               9 (__)
                
-               439         518 LOAD_FAST                3 (result)
+               448         518 LOAD_FAST                3 (result)
                            520 LOAD_METHOD             18 (append)
                            542 LOAD_FAST                8 (res)
                            544 LOAD_ATTR               19 (pk)
                            554 LOAD_GLOBAL             41 (NULL + len)
                            566 LOAD_FAST                8 (res)
                            568 LOAD_ATTR               21 (output)
                            578 PRECALL                  1
@@ -3827,27 +3902,27 @@
                            592 BUILD_TUPLE              2
                            594 PRECALL                  1
                            598 CALL                     1
                            608 POP_TOP
                            610 JUMP_BACKWARD          249 (to 114)
                        >>  612 PUSH_EXC_INFO
                
-               440         614 LOAD_GLOBAL             44 (Exception)
+               449         614 LOAD_GLOBAL             44 (Exception)
                            626 CHECK_EXC_MATCH
                            628 POP_JUMP_FORWARD_IF_FALSE    78 (to 786)
                            630 STORE_FAST              10 (e)
                
-               441         632 LOAD_GLOBAL             46 (logger)
+               450         632 LOAD_GLOBAL             46 (logger)
                            644 LOAD_METHOD             24 (exception)
                            666 LOAD_FAST               10 (e)
                            668 PRECALL                  1
                            672 CALL                     1
                            682 POP_TOP
                
-               442         684 LOAD_FAST                3 (result)
+               451         684 LOAD_FAST                3 (result)
                            686 LOAD_METHOD             18 (append)
                            708 LOAD_FAST                4 (dataset)
                            710 LOAD_ATTR               19 (pk)
                            720 LOAD_GLOBAL             51 (NULL + str)
                            732 LOAD_FAST               10 (e)
                            734 PRECALL                  1
                            738 CALL                     1
@@ -3862,34 +3937,34 @@
                            774 EXTENDED_ARG             1
                            776 JUMP_BACKWARD          332 (to 114)
                        >>  778 LOAD_CONST               0 (None)
                            780 STORE_FAST              10 (e)
                            782 DELETE_FAST             10 (e)
                            784 RERAISE                  1
                
-               440     >>  786 RERAISE                  0
+               449     >>  786 RERAISE                  0
                        >>  788 COPY                     3
                            790 POP_EXCEPT
                            792 RERAISE                  1
                
-               443     >>  794 LOAD_GLOBAL             53 (NULL + timezone)
+               452     >>  794 LOAD_GLOBAL             53 (NULL + timezone)
                            806 LOAD_ATTR               27 (now)
                            816 PRECALL                  0
                            820 CALL                     0
                            830 LOAD_FAST                0 (self)
                            832 STORE_ATTR              28 (last_run)
                
-               444         842 LOAD_FAST                3 (result)
+               453         842 LOAD_FAST                3 (result)
                            844 POP_JUMP_FORWARD_IF_TRUE     3 (to 852)
                
-               445         846 LOAD_CONST               4 ('No Dataset available')
+               454         846 LOAD_CONST               4 ('No Dataset available')
                            848 BUILD_LIST               1
                            850 STORE_FAST               3 (result)
                
-               446     >>  852 LOAD_FAST                3 (result)
+               455     >>  852 LOAD_FAST                3 (result)
                            854 RETURN_VALUE
                ExceptionTable:
                  138 to 608 -> 612 [1]
                  612 to 630 -> 788 [2] lasti
                  632 to 764 -> 778 [2] lasti
                  778 to 786 -> 788 [2] lasti
                consts
@@ -3900,54 +3975,54 @@
                   'No Dataset available'
                names      ('query', 'execute_matrix', 'datasets', 'all', 'size', 'arguments', 'extra', 'update', 'pickle', 'loads', 'document_title', 'formatter', 'render', 'ReportDocument', 'objects', 'update_or_create', 'content_type', 'dumps', 'append', 'pk', 'len', 'output', 'Exception', 'logger', 'exception', 'str', 'timezone', 'now', 'last_run')
                varnames   ('self', 'run_query', 'query', 'result', 'dataset', 'context', 'title', 'output', 'res', '__', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'execute'
-               firstlineno 402
+               firstlineno 411
                lnotab
                   0x02020e0104010401280138010e01020102010e010e015c040cff16020c
                   fd0205220202010201020102fc04ff10082c01020102020201160126010c
                   fc04fd180a60011201340166fe0803300104010601
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a000000000000000000700164015300
-               448           0 RESUME                   0
+               457           0 RESUME                   0
                
-               449           2 LOAD_FAST                0 (self)
+               458           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (name)
                             14 JUMP_IF_TRUE_OR_POP      1 (to 18)
                             16 LOAD_CONST               1 ('')
                        >>   18 RETURN_VALUE
                consts
                   None
                   ''
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '__str__'
-               firstlineno 448
+               firstlineno 457
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               451           0 RESUME                   0
+               460           0 RESUME                   0
                
-               452           2 LOAD_GLOBAL              1 (NULL + reverse)
+               461           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('power_query:report')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (pk)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -3958,79 +4033,79 @@
                   ('args',)
                names      ('reverse', 'pk')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'get_absolute_url'
-               firstlineno 451
+               firstlineno 460
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x9700640164026c006d017d0101007c01a0020000000000000000000000
                   0000000000000000007c006a030000000000000000a6010000ab01000000
                   00000000007d027c026a0300000000000000007c005f0400000000000000
                   007c00a0050000000000000000000000000000000000000000a6000000ab
                   00000000000000000001007c026a0300000000000000005300
-               454           0 RESUME                   0
+               463           0 RESUME                   0
                
-               455           2 LOAD_CONST               1 (0)
+               464           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('refresh_report',))
                              6 IMPORT_NAME              0 (power_query.celery_tasks)
                              8 IMPORT_FROM              1 (refresh_report)
                             10 STORE_FAST               1 (refresh_report)
                             12 POP_TOP
                
-               457          14 LOAD_FAST                1 (refresh_report)
+               466          14 LOAD_FAST                1 (refresh_report)
                             16 LOAD_METHOD              2 (delay)
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                3 (id)
                             50 PRECALL                  1
                             54 CALL                     1
                             64 STORE_FAST               2 (res)
                
-               458          66 LOAD_FAST                2 (res)
+               467          66 LOAD_FAST                2 (res)
                             68 LOAD_ATTR                3 (id)
                             78 LOAD_FAST                0 (self)
                             80 STORE_ATTR               4 (celery_task)
                
-               459          90 LOAD_FAST                0 (self)
+               468          90 LOAD_FAST                0 (self)
                             92 LOAD_METHOD              5 (save)
                            114 PRECALL                  0
                            118 CALL                     0
                            128 POP_TOP
                
-               460         130 LOAD_FAST                2 (res)
+               469         130 LOAD_FAST                2 (res)
                            132 LOAD_ATTR                3 (id)
                            142 RETURN_VALUE
                consts
                   None
                   0
                   ('refresh_report',)
                names      ('power_query.celery_tasks', 'refresh_report', 'delay', 'id', 'celery_task', 'save')
                varnames   ('self', 'refresh_report', 'res')
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '_queue'
-               firstlineno 454
+               firstlineno 463
                lnotab 0x02010c02340118012801
             (False, False, None, None)
             (False,)
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'name', 'document_title', 'ForeignKey', 'Query', 'CASCADE', 'query', 'Formatter', 'formatter', 'BooleanField', 'active', 'get_user_model', 'owner', 'ManyToManyField', 'limit_access_to', 'FrequencyValidator', 'frequence', 'DateTimeField', 'last_run', 'IntegerField', 'validity_days', 'bool', 'Optional', 'Any', 'save', 'ReportResult', 'execute', 'str', '__str__', 'get_absolute_url', '_queue', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'Report'
-         firstlineno 364
+         firstlineno 373
          lnotab
             0x0c01280126012e012e0122010e011201020102010c0102fb12070e0116
             ff12030e010201020102010201020114fa12082401220402010201020102
             fb040202fe020302fd02040efc02050efb020602fa0c0b122e0c030c03
       'Report'
       code
          argcount  : 0
@@ -4038,27 +4113,27 @@
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a02640165036a040000000000000000660288
             0066016402840c5a05880078015a065300
                        0 MAKE_CELL                0 (__class__)
          
-         463           2 RESUME                   0
+         472           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ReportDocumentManager')
                       10 STORE_NAME               2 (__qualname__)
          
-         464          12 LOAD_CONST               1 ('return')
+         473          12 LOAD_CONST               1 ('return')
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (QuerySet)
                       26 BUILD_TUPLE              2
                       28 LOAD_CLOSURE             0 (__class__)
                       30 BUILD_TUPLE              1
-                      32 LOAD_CONST               2 (<code object get_queryset, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 464>)
+                      32 LOAD_CONST               2 (<code object get_queryset, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 473>)
                       34 MAKE_FUNCTION           12 (annotations, closure)
                       36 STORE_NAME               5 (get_queryset)
                       38 LOAD_CLOSURE             0 (__class__)
                       40 COPY                     1
                       42 STORE_NAME               6 (__classcell__)
                       44 RETURN_VALUE
          consts
@@ -4072,17 +4147,17 @@
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a0010000000000000000000000000000000000000000a6000000ab0000
                   00000000000000a002000000000000000000000000000000000000000064
                   01a6010000ab0100000000000000005300
                              0 COPY_FREE_VARS           1
                
-               464           2 RESUME                   0
+               473           2 RESUME                   0
                
-               465           4 LOAD_GLOBAL              1 (NULL + super)
+               474           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (get_queryset)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 LOAD_METHOD              2 (select_related)
                             88 LOAD_CONST               1 ('report')
@@ -4094,23 +4169,23 @@
                   'report'
                names      ('super', 'get_queryset', 'select_related')
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'get_queryset'
-               firstlineno 464
+               firstlineno 473
                lnotab 0x0401
          names      ('__name__', '__module__', '__qualname__', 'models', 'QuerySet', 'get_queryset', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'ReportDocumentManager'
-         firstlineno 463
+         firstlineno 472
          lnotab 0x0c01
       'ReportDocumentManager'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
@@ -4127,161 +4202,161 @@
             000000000000006401640aac0ba6030000ab0300000000000000005a1602
             0065036a060000000000000000640c6517ac0da6020000ab020000000000
             0000005a1802006519a6000000ab0000000000000000005a1a0200470064
             0e8400640fa6020000ab0200000000000000005a1b6410651c6602641184
             045a1d651e6410651f660264128404a6000000ab0000000000000000005a
             20651e64106521660264138404a6000000ab0000000000000000005a2264
             10651c6602641484045a2364155300
-         468           0 RESUME                   0
+         477           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ReportDocument')
                        8 STORE_NAME               2 (__qualname__)
          
-         469          10 PUSH_NULL
+         478          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (DateTimeField)
                       24 LOAD_CONST               1 (True)
                       26 KW_NAMES                 2
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_NAME               5 (timestamp)
          
-         470          44 PUSH_NULL
+         479          44 PUSH_NULL
                       46 LOAD_NAME                3 (models)
                       48 LOAD_ATTR                6 (CharField)
                       58 LOAD_CONST               3 (300)
                       60 KW_NAMES                 4
                       62 PRECALL                  1
                       66 CALL                     1
                       76 STORE_NAME               7 (title)
          
-         471          78 PUSH_NULL
+         480          78 PUSH_NULL
                       80 LOAD_NAME                3 (models)
                       82 LOAD_ATTR                8 (ForeignKey)
          
-         472          92 LOAD_NAME                9 (Report)
+         481          92 LOAD_NAME                9 (Report)
                       94 LOAD_NAME                3 (models)
                       96 LOAD_ATTR               10 (CASCADE)
                      106 LOAD_CONST               5 ('documents')
          
-         471         108 KW_NAMES                 6
+         480         108 KW_NAMES                 6
                      110 PRECALL                  3
                      114 CALL                     3
                      124 STORE_NAME              11 (report)
          
-         474         126 PUSH_NULL
+         483         126 PUSH_NULL
                      128 LOAD_NAME                3 (models)
                      130 LOAD_ATTR                8 (ForeignKey)
                      140 LOAD_NAME               12 (Dataset)
                      142 LOAD_NAME                3 (models)
                      144 LOAD_ATTR               10 (CASCADE)
                      154 KW_NAMES                 7
                      156 PRECALL                  2
                      160 CALL                     2
                      170 STORE_NAME              13 (dataset)
          
-         475         172 PUSH_NULL
+         484         172 PUSH_NULL
                      174 LOAD_NAME                3 (models)
                      176 LOAD_ATTR               14 (BinaryField)
                      186 LOAD_CONST               1 (True)
                      188 LOAD_CONST               1 (True)
                      190 KW_NAMES                 8
                      192 PRECALL                  2
                      196 CALL                     2
                      206 STORE_NAME              15 (output)
          
-         476         208 PUSH_NULL
+         485         208 PUSH_NULL
                      210 LOAD_NAME                3 (models)
                      212 LOAD_ATTR               16 (JSONField)
                      222 LOAD_NAME               17 (dict)
                      224 LOAD_NAME               18 (PQJSONEncoder)
                      226 KW_NAMES                 9
                      228 PRECALL                  2
                      232 CALL                     2
                      242 STORE_NAME              19 (arguments)
          
-         477         244 PUSH_NULL
+         486         244 PUSH_NULL
                      246 LOAD_NAME                3 (models)
                      248 LOAD_ATTR               20 (ManyToManyField)
          
-         478         258 PUSH_NULL
+         487         258 PUSH_NULL
                      260 LOAD_NAME               21 (get_user_model)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_CONST               1 (True)
                      278 LOAD_CONST              10 ('+')
          
-         477         280 KW_NAMES                11
+         486         280 KW_NAMES                11
                      282 PRECALL                  3
                      286 CALL                     3
                      296 STORE_NAME              22 (limit_access_to)
          
-         480         298 PUSH_NULL
+         489         298 PUSH_NULL
                      300 LOAD_NAME                3 (models)
                      302 LOAD_ATTR                6 (CharField)
                      312 LOAD_CONST              12 (5)
                      314 LOAD_NAME               23 (MIMETYPES)
                      316 KW_NAMES                13
                      318 PRECALL                  2
                      322 CALL                     2
                      332 STORE_NAME              24 (content_type)
          
-         482         334 PUSH_NULL
+         491         334 PUSH_NULL
                      336 LOAD_NAME               25 (ReportDocumentManager)
                      338 PRECALL                  0
                      342 CALL                     0
                      352 STORE_NAME              26 (objects)
          
-         484         354 PUSH_NULL
+         493         354 PUSH_NULL
                      356 LOAD_BUILD_CLASS
-                     358 LOAD_CONST              14 (<code object Meta, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 484>)
+                     358 LOAD_CONST              14 (<code object Meta, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 493>)
                      360 MAKE_FUNCTION            0
                      362 LOAD_CONST              15 ('Meta')
                      364 PRECALL                  2
                      368 CALL                     2
                      378 STORE_NAME              27 (Meta)
          
-         487         380 LOAD_CONST              16 ('return')
+         496         380 LOAD_CONST              16 ('return')
                      382 LOAD_NAME               28 (str)
                      384 BUILD_TUPLE              2
-                     386 LOAD_CONST              17 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 487>)
+                     386 LOAD_CONST              17 (<code object __str__, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 496>)
                      388 MAKE_FUNCTION            4 (annotations)
                      390 STORE_NAME              29 (__str__)
          
-         490         392 LOAD_NAME               30 (cached_property)
+         499         392 LOAD_NAME               30 (cached_property)
          
-         491         394 LOAD_CONST              16 ('return')
+         500         394 LOAD_CONST              16 ('return')
                      396 LOAD_NAME               31 (Any)
                      398 BUILD_TUPLE              2
-                     400 LOAD_CONST              18 (<code object data, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 490>)
+                     400 LOAD_CONST              18 (<code object data, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 499>)
                      402 MAKE_FUNCTION            4 (annotations)
          
-         490         404 PRECALL                  0
+         499         404 PRECALL                  0
                      408 CALL                     0
          
-         491         418 STORE_NAME              32 (data)
+         500         418 STORE_NAME              32 (data)
          
-         494         420 LOAD_NAME               30 (cached_property)
+         503         420 LOAD_NAME               30 (cached_property)
          
-         495         422 LOAD_CONST              16 ('return')
+         504         422 LOAD_CONST              16 ('return')
                      424 LOAD_NAME               33 (int)
                      426 BUILD_TUPLE              2
-                     428 LOAD_CONST              19 (<code object size, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 494>)
+                     428 LOAD_CONST              19 (<code object size, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 503>)
                      430 MAKE_FUNCTION            4 (annotations)
          
-         494         432 PRECALL                  0
+         503         432 PRECALL                  0
                      436 CALL                     0
          
-         495         446 STORE_NAME              34 (size)
+         504         446 STORE_NAME              34 (size)
          
-         498         448 LOAD_CONST              16 ('return')
+         507         448 LOAD_CONST              16 ('return')
                      450 LOAD_NAME               28 (str)
                      452 BUILD_TUPLE              2
-                     454 LOAD_CONST              20 (<code object get_absolute_url, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 498>)
+                     454 LOAD_CONST              20 (<code object get_absolute_url, file "/Users/jojo/workspace/unicef-power-query/src/power_query/models.py", line 507>)
                      456 MAKE_FUNCTION            4 (annotations)
                      458 STORE_NAME              35 (get_absolute_url)
                      460 LOAD_CONST              21 (None)
                      462 RETURN_VALUE
          consts
             'ReportDocument'
             True
@@ -4299,124 +4374,124 @@
             ('max_length', 'choices')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               484           0 RESUME                   0
+               493           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('ReportDocument.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               485          10 LOAD_CONST               1 (('report', 'dataset'))
+               494          10 LOAD_CONST               1 (('report', 'dataset'))
                             12 STORE_NAME               3 (unique_together)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'ReportDocument.Meta'
                   ('report', 'dataset')
                   None
                names      ('__name__', '__module__', '__qualname__', 'unique_together')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'Meta'
-               firstlineno 484
+               firstlineno 493
                lnotab 0x0a01
             'Meta'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               487           0 RESUME                   0
+               496           0 RESUME                   0
                
-               488           2 LOAD_FAST                0 (self)
+               497           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       '__str__'
-               firstlineno 487
+               firstlineno 496
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   00000000000000a6010000ab0100000000000000005300
-               490           0 RESUME                   0
+               499           0 RESUME                   0
                
-               492           2 LOAD_GLOBAL              1 (NULL + pickle)
+               501           2 LOAD_GLOBAL              1 (NULL + pickle)
                             14 LOAD_ATTR                1 (loads)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (output)
                             36 PRECALL                  1
                             40 CALL                     1
                             50 RETURN_VALUE
                consts
                   None
                names      ('pickle', 'loads', 'output')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'data'
-               firstlineno 490
+               firstlineno 499
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-               494           0 RESUME                   0
+               503           0 RESUME                   0
                
-               496           2 LOAD_GLOBAL              1 (NULL + len)
+               505           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (output)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('len', 'output')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'size'
-               firstlineno 494
+               firstlineno 503
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a0100000000000000006a
                   0200000000000000007c006a0200000000000000006702ac02a6020000ab
                   0200000000000000005300
-               498           0 RESUME                   0
+               507           0 RESUME                   0
                
-               499           2 LOAD_GLOBAL              1 (NULL + reverse)
+               508           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('power_query:document')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (report)
                             28 LOAD_ATTR                2 (pk)
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (pk)
                             50 BUILD_LIST               2
@@ -4430,33 +4505,33 @@
                   ('args',)
                names      ('reverse', 'report', 'pk')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
                name       'get_absolute_url'
-               firstlineno 498
+               firstlineno 507
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'DateTimeField', 'timestamp', 'CharField', 'title', 'ForeignKey', 'Report', 'CASCADE', 'report', 'Dataset', 'dataset', 'BinaryField', 'output', 'JSONField', 'dict', 'PQJSONEncoder', 'arguments', 'ManyToManyField', 'get_user_model', 'limit_access_to', 'MIMETYPES', 'content_type', 'ReportDocumentManager', 'objects', 'Meta', 'str', '__str__', 'cached_property', 'Any', 'data', 'int', 'size', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
          name       'ReportDocument'
-         firstlineno 468
+         firstlineno 477
          lnotab
             0x0a01220122010e0110ff12032e01240124010e0116ff1203240214021a
             030c0302010aff0e01020302010aff0e010203
       'ReportDocument'
-   names      ('itertools', 'logging', 'pickle', 'typing', 'Any', 'Dict', 'List', 'Optional', 'Tuple', 'Union', 'django.conf', 'settings', 'django.contrib.auth', 'get_user_model', 'django.contrib.contenttypes.models', 'ContentType', 'django.core.exceptions', 'ValidationError', 'django.db', 'models', 'transaction', 'django.db.models', 'JSONField', 'django.template', 'Context', 'Template', 'django.urls', 'reverse', 'django.utils', 'timezone', 'django.utils.datetime_safe', 'strftime', 'django.utils.functional', 'cached_property', 'django.utils.text', 'slugify', 'celery', 'states', 'celery.result', 'AsyncResult', 'natural_keys', 'NaturalKeyModel', 'sentry_sdk', 'capture_exception', 'configure_scope', 'power_query.exceptions', 'QueryRunError', 'power_query.json', 'PQJSONEncoder', 'power_query.utils', 'dict_hash', 'to_dataset', 'power_query.validators', 'FrequencyValidator', 'getLogger', '__name__', 'logger', 'mimetype_map', 'items', 'MIMETYPES', 'int', 'str', 'DocumentResult', 'ReportResult', 'QueryResult', 'QueryMatrixResult', 'validate_queryargs', 'Model', 'CeleryEnabled', 'Parametrizer', 'Query', 'Dataset', 'Formatter', 'Report', 'Manager', 'ReportDocumentManager', 'ReportDocument')
+   names      ('itertools', 'logging', 'pickle', 'typing', 'Any', 'Dict', 'List', 'Optional', 'Tuple', 'Union', 'django.apps', 'apps', 'django_apps', 'django.conf', 'settings', 'django.contrib.auth', 'get_user_model', 'django.contrib.contenttypes.models', 'ContentType', 'django.core.exceptions', 'ValidationError', 'django.db', 'models', 'transaction', 'django.db.models', 'JSONField', 'django.template', 'Context', 'Template', 'django.urls', 'reverse', 'django.utils', 'timezone', 'django.utils.datetime_safe', 'strftime', 'django.utils.functional', 'cached_property', 'django.utils.text', 'slugify', 'celery', 'states', 'celery.result', 'AsyncResult', 'natural_keys', 'NaturalKeyModel', 'sentry_sdk', 'capture_exception', 'configure_scope', 'power_query.exceptions', 'QueryRunError', 'power_query.json', 'PQJSONEncoder', 'power_query.utils', 'dict_hash', 'to_dataset', 'power_query.validators', 'FrequencyValidator', 'getLogger', '__name__', 'logger', 'mimetype_map', 'items', 'MIMETYPES', 'int', 'str', 'DocumentResult', 'ReportResult', 'QueryResult', 'QueryMatrixResult', 'validate_queryargs', 'Model', 'CeleryEnabled', 'Parametrizer', 'Query', 'Dataset', 'Formatter', 'Report', 'Manager', 'ReportDocumentManager', 'ReportDocument')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jojo/workspace/unicef-power-query/src/power_query/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010801080120020c010c010c010c0110010c0110010c010c
-      010c010c010c0208010c010c010c0110020c010c0110010c022003020102
-      01020102010201020102f9060a3c022401220114012403100f2627282e2a
-      7f0021281b281b2a632605
+      0x00ff020108010801080120020c010c010c010c010c0110010c0110010c
+      010c010c010c010c0208010c010c010c0110020c010c0110010c02200302
+      010201020102010201020102f9060a3c022401220114012403100f262728
+      2f2a7f0028281b281b2a632605
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/models.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:27:46 2023 UTC, .py size: 17115 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,1032 +1,1052 @@
-00000000: 610d 0d0a 0000 0000 72a7 af64 db42 0000  a.......r..d.B..
+00000000: 610d 0d0a 0000 0000 7db3 b764 2744 0000  a.......}..d'D..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 6802 0000 6400  .....@...sh...d.
+00000020: 0008 0000 0040 0000 0073 7402 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
-00000060: 6d09 5a09 0100 6400 6403 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6404 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6405 6c0e 6d0f 5a0f 0100 6400 6406 6c10  d.l.m.Z...d.d.l.
-00000090: 6d11 5a11 0100 6400 6407 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
-000000a0: 6d14 5a14 0100 6400 6408 6c15 6d16 5a16  m.Z...d.d.l.m.Z.
-000000b0: 0100 6400 6409 6c17 6d18 5a18 6d19 5a19  ..d.d.l.m.Z.m.Z.
-000000c0: 0100 6400 640a 6c1a 6d1b 5a1b 0100 6400  ..d.d.l.m.Z...d.
-000000d0: 640b 6c1c 6d1d 5a1d 0100 6400 640c 6c1e  d.l.m.Z...d.d.l.
-000000e0: 6d1f 5a1f 0100 6400 640d 6c20 6d21 5a21  m.Z...d.d.l m!Z!
-000000f0: 0100 6400 640e 6c22 6d23 5a23 0100 6400  ..d.d.l"m#Z#..d.
-00000100: 6401 6c24 5a24 6400 640f 6c24 6d25 5a25  d.l$Z$d.d.l$m%Z%
-00000110: 0100 6400 6410 6c26 6d27 5a27 0100 6400  ..d.d.l&m'Z'..d.
-00000120: 6411 6c28 6d29 5a29 0100 6400 6412 6c2a  d.l(m)Z)..d.d.l*
-00000130: 6d2b 5a2b 6d2c 5a2c 0100 6400 6413 6c2d  m+Z+m,Z,..d.d.l-
-00000140: 6d2e 5a2e 0100 6400 6414 6c2f 6d30 5a30  m.Z...d.d.l/m0Z0
-00000150: 0100 6400 6415 6c31 6d32 5a32 6d33 5a33  ..d.d.l1m2Z2m3Z3
-00000160: 0100 6400 6416 6c34 6d35 5a35 0100 6501  ..d.d.l4m5Z5..e.
-00000170: a036 6537 a101 5a38 6417 6418 6419 641a  .6e7..Z8d.d.d.d.
-00000180: 641b 641c 641d 641e 9c07 5a39 641f 6420  d.d.d.d...Z9d.d 
-00000190: 8400 6539 a03a a100 4400 8301 5a3b 6508  ..e9.:..D...Z;e.
-000001a0: 653c 6509 653d 653c 6602 1900 6602 1900  e<e.e=e<f...f...
-000001b0: 5a3e 6506 6509 653e 6504 653d 6603 1900  Z>e.e.e>e.e=f...
-000001c0: 1900 5a3f 6508 6504 6504 6602 1900 5a40  ..Z?e.e.e.f...Z@
-000001d0: 6505 653d 6509 653c 653d 6602 1900 6602  e.e=e.e<e=f...f.
-000001e0: 1900 5a41 6504 6401 6421 9c02 6422 6423  ..ZAe.d.d!..d"d#
-000001f0: 8404 5a42 4700 6424 6425 8400 6425 6513  ..ZBG.d$d%..d%e.
-00000200: 6a43 8303 5a44 4700 6426 6427 8400 6427  jC..ZDG.d&d'..d'
-00000210: 6529 6513 6a43 8304 5a45 4700 6428 6429  e)e.jC..ZEG.d(d)
-00000220: 8400 6429 6529 6544 6513 6a43 8305 5a46  ..d)e)eDe.jC..ZF
-00000230: 4700 642a 642b 8400 642b 6529 6513 6a43  G.d*d+..d+e)e.jC
-00000240: 8304 5a47 4700 642c 642d 8400 642d 6529  ..ZGG.d,d-..d-e)
-00000250: 6513 6a43 8304 5a48 4700 642e 642f 8400  e.jC..ZHG.d.d/..
-00000260: 642f 6529 6544 6513 6a43 8305 5a49 4700  d/e)eDe.jC..ZIG.
-00000270: 6430 6431 8400 6431 6513 6a4a 8303 5a4b  d0d1..d1e.jJ..ZK
-00000280: 4700 6432 6433 8400 6433 6513 6a43 8303  G.d2d3..d3e.jC..
-00000290: 5a4c 6401 5300 2934 e900 0000 004e 2906  ZLd.S.)4.....N).
-000002a0: da03 416e 79da 0444 6963 74da 044c 6973  ..Any..Dict..Lis
-000002b0: 74da 084f 7074 696f 6e61 6cda 0554 7570  t..Optional..Tup
-000002c0: 6c65 da05 556e 696f 6e29 01da 0873 6574  le..Union)...set
-000002d0: 7469 6e67 7329 01da 0e67 6574 5f75 7365  tings)...get_use
-000002e0: 725f 6d6f 6465 6c29 01da 0b43 6f6e 7465  r_model)...Conte
-000002f0: 6e74 5479 7065 2901 da0f 5661 6c69 6461  ntType)...Valida
-00000300: 7469 6f6e 4572 726f 7229 02da 066d 6f64  tionError)...mod
-00000310: 656c 73da 0b74 7261 6e73 6163 7469 6f6e  els..transaction
-00000320: 2901 da09 4a53 4f4e 4669 656c 6429 02da  )...JSONField)..
-00000330: 0743 6f6e 7465 7874 da08 5465 6d70 6c61  .Context..Templa
-00000340: 7465 2901 da07 7265 7665 7273 6529 01da  te)...reverse)..
-00000350: 0874 696d 657a 6f6e 6529 01da 0873 7472  .timezone)...str
-00000360: 6674 696d 6529 01da 0f63 6163 6865 645f  ftime)...cached_
-00000370: 7072 6f70 6572 7479 2901 da07 736c 7567  property)...slug
-00000380: 6966 7929 01da 0673 7461 7465 7329 01da  ify)...states)..
-00000390: 0b41 7379 6e63 5265 7375 6c74 2901 da0f  .AsyncResult)...
-000003a0: 4e61 7475 7261 6c4b 6579 4d6f 6465 6c29  NaturalKeyModel)
-000003b0: 02da 1163 6170 7475 7265 5f65 7863 6570  ...capture_excep
-000003c0: 7469 6f6e da0f 636f 6e66 6967 7572 655f  tion..configure_
-000003d0: 7363 6f70 6529 01da 0d51 7565 7279 5275  scope)...QueryRu
-000003e0: 6e45 7272 6f72 2901 da0d 5051 4a53 4f4e  nError)...PQJSON
-000003f0: 456e 636f 6465 7229 02da 0964 6963 745f  Encoder)...dict_
-00000400: 6861 7368 da0a 746f 5f64 6174 6173 6574  hash..to_dataset
-00000410: 2901 da12 4672 6571 7565 6e63 7956 616c  )...FrequencyVal
-00000420: 6964 6174 6f72 7a08 7465 7874 2f63 7376  idatorz.text/csv
-00000430: 7a09 7465 7874 2f68 746d 6c7a 1061 7070  z.text/htmlz.app
-00000440: 6c69 6361 7469 6f6e 2f6a 736f 6e7a 0a74  lication/jsonz.t
-00000450: 6578 742f 706c 6169 6e7a 1861 7070 6c69  ext/plainz.appli
-00000460: 6361 7469 6f6e 2f76 6e64 2e6d 732d 6578  cation/vnd.ms-ex
-00000470: 6365 6c7a 0f61 7070 6c69 6361 7469 6f6e  celz.application
-00000480: 2f78 6d6c 7a09 7465 7874 2f79 616d 6c29  /xmlz.text/yaml)
-00000490: 07da 0363 7376 da04 6874 6d6c da04 6a73  ...csv..html..js
-000004a0: 6f6e da03 7478 74da 0378 6c73 da03 786d  on..txt..xls..xm
-000004b0: 6cda 0479 616d 6c63 0100 0000 0000 0000  l..yamlc........
-000004c0: 0000 0000 0300 0000 0300 0000 6300 0000  ............c...
-000004d0: 731a 0000 007c 005d 125c 027d 017d 027c  s....|.].\.}.}.|
-000004e0: 017c 0266 0256 0001 0071 0264 0053 00a9  .|.f.V...q.d.S..
-000004f0: 014e a900 2903 da02 2e30 da01 6bda 0176  .N..)....0..k..v
-00000500: 7228 0000 0072 2800 0000 fa42 2f55 7365  r(...r(....B/Use
-00000510: 7273 2f6a 6f6a 6f2f 776f 726b 7370 6163  rs/jojo/workspac
-00000520: 652f 756e 6963 6566 2d70 6f77 6572 2d71  e/unicef-power-q
-00000530: 7565 7279 2f73 7263 2f70 6f77 6572 5f71  uery/src/power_q
-00000540: 7565 7279 2f6d 6f64 656c 732e 7079 da09  uery/models.py..
-00000550: 3c67 656e 6578 7072 3e2a 0000 00f3 0000  <genexpr>*......
-00000560: 0000 722d 0000 0029 02da 0576 616c 7565  ..r-...)...value
-00000570: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-00000580: 0000 0000 0003 0000 000a 0000 0003 0000  ................
-00000590: 0073 8800 0000 7a3a 7400 8800 7401 8302  .s....z:t...t...
-000005a0: 7314 7402 6401 8301 8201 7403 7404 6a05  s.t.d.....t.t.j.
-000005b0: 8800 a006 a100 8e00 8301 7d01 8700 6601  ..........}...f.
-000005c0: 6402 6403 8408 7c01 4400 8301 0100 5700  d.d...|.D.....W.
-000005d0: 6e48 0400 7402 794e 0100 0100 0100 8200  nH..t.yN........
-000005e0: 5900 6e36 0400 7407 7982 0100 7d02 0100  Y.n6..t.y...}...
-000005f0: 7a1e 7402 6404 8800 7c02 6405 9c02 6406  z.t.d...|.d...d.
-00000600: 8d02 8201 5700 5900 6400 7d02 7e02 6e0a  ....W.Y.d.}.~.n.
-00000610: 6400 7d02 7e02 3000 3000 6400 5300 2907  d.}.~.0.0.d.S.).
-00000620: 4e7a 1851 7565 7279 4172 6773 206d 7573  Nz.QueryArgs mus
-00000630: 7420 6265 2061 2064 6963 7463 0100 0000  t be a dictc....
-00000640: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00000650: 1300 0000 731e 0000 0067 007c 005d 167d  ....s....g.|.].}
-00000660: 0174 0074 0188 00a0 02a1 007c 0183 0283  .t.t.......|....
-00000670: 0191 0271 0453 0072 2800 0000 2903 da04  ...q.S.r(...)...
-00000680: 6469 6374 da03 7a69 70da 046b 6579 73a9  dict..zip..keys.
-00000690: 0272 2900 0000 da01 65a9 0172 2f00 0000  .r).....e..r/...
-000006a0: 7228 0000 0072 2c00 0000 da0a 3c6c 6973  r(...r,.....<lis
-000006b0: 7463 6f6d 703e 3700 0000 722e 0000 007a  tcomp>7...r....z
-000006c0: 2676 616c 6964 6174 655f 7175 6572 7961  &validate_querya
-000006d0: 7267 732e 3c6c 6f63 616c 733e 2e3c 6c69  rgs.<locals>.<li
-000006e0: 7374 636f 6d70 3e7a 2b25 2865 7863 2973  stcomp>z+%(exc)s
-000006f0: 3a20 2528 7661 6c75 6529 7320 6973 206e  : %(value)s is n
-00000700: 6f74 2061 2076 616c 6964 2051 7565 7279  ot a valid Query
-00000710: 4172 6773 2902 722f 0000 00da 0365 7863  Args).r/.....exc
-00000720: 2901 da06 7061 7261 6d73 2908 da0a 6973  )...params)...is
-00000730: 696e 7374 616e 6365 7231 0000 0072 0b00  instancer1...r..
-00000740: 0000 da04 6c69 7374 da09 6974 6572 746f  ....list..iterto
-00000750: 6f6c 73da 0770 726f 6475 6374 da06 7661  ols..product..va
-00000760: 6c75 6573 da09 4578 6365 7074 696f 6e29  lues..Exception)
-00000770: 0372 2f00 0000 723d 0000 0072 3500 0000  .r/...r=...r5...
-00000780: 7228 0000 0072 3600 0000 722c 0000 00da  r(...r6...r,....
-00000790: 1276 616c 6964 6174 655f 7175 6572 7961  .validate_querya
-000007a0: 7267 7332 0000 0073 1800 0000 0001 0201  rgs2...s........
-000007b0: 0a01 0801 1201 1601 0c01 0601 0e01 0201  ................
-000007c0: 0201 08fe 7240 0000 0063 0000 0000 0000  ....r@...c......
-000007d0: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
-000007e0: 0000 7386 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
-000007f0: 0365 046a 0565 046a 0665 046a 0765 046a  .e.j.e.j.e.j.e.j
-00000800: 0868 0483 015a 0965 0a6a 0b64 0164 0264  .h...Z.e.j.d.d.d
-00000810: 0264 038d 035a 0c47 0064 0464 0584 0064  .d...Z.G.d.d...d
-00000820: 0583 025a 0d65 0e64 069c 0164 0764 0884  ...Z.e.d...d.d..
-00000830: 045a 0f65 1065 1165 1219 0064 069c 0164  .Z.e.e.e...d...d
-00000840: 0964 0a84 0483 015a 1365 1165 0e19 0064  .d.....Z.e.e...d
-00000850: 069c 0164 0b64 0c84 045a 1465 0e64 069c  ...d.d...Z.e.d..
-00000860: 0164 0d64 0e84 045a 1564 0f53 0029 10da  .d.d...Z.d.S.)..
-00000870: 0d43 656c 6572 7945 6e61 626c 6564 e924  .CeleryEnabled.$
-00000880: 0000 0054 a903 da0a 6d61 785f 6c65 6e67  ...T....max_leng
-00000890: 7468 da05 626c 616e 6bda 046e 756c 6c63  th..blank..nullc
-000008a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000008b0: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
-000008c0: 0164 005a 0264 015a 0364 0253 0029 037a  .d.Z.d.Z.d.S.).z
-000008d0: 1243 656c 6572 7945 6e61 626c 6564 2e4d  .CeleryEnabled.M
-000008e0: 6574 6154 4e29 04da 085f 5f6e 616d 655f  etaTN)...__name_
-000008f0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000900: 5f71 7561 6c6e 616d 655f 5fda 0861 6273  _qualname__..abs
-00000910: 7472 6163 7472 2800 0000 7228 0000 0072  tractr(...r(...r
-00000920: 2800 0000 722c 0000 00da 044d 6574 6148  (...r,.....MetaH
-00000930: 0000 0073 0200 0000 0801 724b 0000 00a9  ...s......rK....
-00000940: 0172 3000 0000 6301 0000 0000 0000 0000  .r0...c.........
-00000950: 0000 0003 0000 000a 0000 0043 0000 0073  ...........C...s
-00000960: 4a00 0000 7c00 6a00 7242 7a0c 7c00 6a01  J...|.j.rBz.|.j.
-00000970: 6a02 7d01 5700 7146 0400 7403 793e 0100  j.}.W.qF..t.y>..
-00000980: 7d02 0100 7a14 7404 7c02 8301 7d01 5700  }...z.t.|...}.W.
-00000990: 5900 6400 7d02 7e02 7146 6400 7d02 7e02  Y.d.}.~.qFd.}.~.
-000009a0: 3000 3000 6e04 6401 7d01 7c01 5300 2902  0.0.n.d.}.|.S.).
-000009b0: 4e7a 0d4e 6f74 2073 6368 6564 756c 6564  Nz.Not scheduled
-000009c0: 2905 da0b 6365 6c65 7279 5f74 6173 6bda  )...celery_task.
-000009d0: 0c61 7379 6e63 5f72 6573 756c 74da 0573  .async_result..s
-000009e0: 7461 7465 723f 0000 00da 0373 7472 2903  tater?.....str).
-000009f0: da04 7365 6c66 da06 7265 7375 6c74 7235  ..self..resultr5
-00000a00: 0000 0072 2800 0000 7228 0000 0072 2c00  ...r(...r(...r,.
-00000a10: 0000 da06 7374 6174 7573 4b00 0000 730e  ....statusK...s.
-00000a20: 0000 0000 0106 0102 010c 010e 0120 0204  ............. ..
-00000a30: 017a 1443 656c 6572 7945 6e61 626c 6564  .z.CeleryEnabled
-00000a40: 2e73 7461 7475 7363 0100 0000 0000 0000  .statusc........
-00000a50: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000a60: 732a 0000 007c 006a 0072 227c 006a 017c  s*...|.j.r"|.j.|
-00000a70: 006a 0276 0172 2274 037c 006a 0074 046a  .j.v.r"t.|.j.t.j
-00000a80: 0564 018d 0253 0064 0053 0064 0053 0029  .d...S.d.S.d.S.)
-00000a90: 024e 2901 da03 6170 7029 0672 4d00 0000  .N)...app).rM...
-00000aa0: 7253 0000 00da 0953 4348 4544 554c 4544  rS.....SCHEDULED
-00000ab0: 7217 0000 00da 0663 656c 6572 79da 0b63  r......celery..c
-00000ac0: 7572 7265 6e74 5f61 7070 a901 7251 0000  urrent_app..rQ..
-00000ad0: 0072 2800 0000 7228 0000 0072 2c00 0000  .r(...r(...r,...
-00000ae0: 724e 0000 0055 0000 0073 0600 0000 0002  rN...U...s......
-00000af0: 1201 1002 7a1a 4365 6c65 7279 456e 6162  ....z.CeleryEnab
-00000b00: 6c65 642e 6173 796e 635f 7265 7375 6c74  led.async_result
-00000b10: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000b20: 0002 0000 0043 0000 0073 2800 0000 7c00  .....C...s(...|.
-00000b30: 6a00 7c00 6a01 7601 7224 7c00 a002 a100  j.|.j.v.r$|.....
-00000b40: 7d01 7c01 7320 7403 6401 8301 8201 7c01  }.|.s t.d.....|.
-00000b50: 5300 6400 5300 2902 4e7a 2160 5f71 7565  S.d.S.).Nz!`_que
-00000b60: 7565 6020 6e6f 7420 7072 6f70 6572 6c79  ue` not properly
-00000b70: 2069 6d70 6c65 6d65 6e74 6564 2904 7253   implemented).rS
-00000b80: 0000 0072 5500 0000 da06 5f71 7565 7565  ...rU....._queue
-00000b90: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
-00000ba0: 4572 726f 7229 0272 5100 0000 da07 7461  Error).rQ.....ta
-00000bb0: 736b 5f69 6472 2800 0000 7228 0000 0072  sk_idr(...r(...r
-00000bc0: 2c00 0000 da05 7175 6575 655c 0000 0073  ,.....queue\...s
-00000bd0: 0c00 0000 0001 0c01 0801 0401 0801 0401  ................
-00000be0: 7a13 4365 6c65 7279 456e 6162 6c65 642e  z.CeleryEnabled.
-00000bf0: 7175 6575 6563 0100 0000 0000 0000 0000  queuec..........
-00000c00: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000c10: 0000 0064 0153 00a9 024e da00 7228 0000  ...d.S...N..r(..
-00000c20: 0072 5800 0000 7228 0000 0072 2800 0000  .rX...r(...r(...
-00000c30: 722c 0000 0072 5900 0000 6400 0000 7302  r,...rY...d...s.
-00000c40: 0000 0000 017a 1443 656c 6572 7945 6e61  .....z.CeleryEna
-00000c50: 626c 6564 2e5f 7175 6575 654e 2916 7247  bled._queueN).rG
-00000c60: 0000 0072 4800 0000 7249 0000 00da 0966  ...rH...rI.....f
-00000c70: 726f 7a65 6e73 6574 7216 0000 00da 0750  rozensetr......P
-00000c80: 454e 4449 4e47 da08 5245 4345 4956 4544  ENDING..RECEIVED
-00000c90: da07 5354 4152 5445 44da 0552 4554 5259  ..STARTED..RETRY
-00000ca0: 7255 0000 0072 0c00 0000 da09 4368 6172  rU...r......Char
-00000cb0: 4669 656c 6472 4d00 0000 724b 0000 0072  FieldrM...rK...r
-00000cc0: 5000 0000 7253 0000 00da 0870 726f 7065  P...rS.....prope
-00000cd0: 7274 7972 0500 0000 7217 0000 0072 4e00  rtyr....r....rN.
-00000ce0: 0000 725c 0000 0072 5900 0000 7228 0000  ..r\...rY...r(..
-00000cf0: 0072 2800 0000 7228 0000 0072 2c00 0000  .r(...r(...r,...
-00000d00: 7241 0000 0041 0000 0073 1400 0000 0801  rA...A...s......
-00000d10: 0201 12ff 0404 1002 0e03 0e0a 0201 1406  ................
-00000d20: 1208 7241 0000 0063 0000 0000 0000 0000  ..rA...c........
-00000d30: 0000 0000 0000 0000 0700 0000 0000 0000  ................
-00000d40: 73e4 0000 0065 005a 0164 005a 0265 036a  s....e.Z.d.Z.e.j
-00000d50: 0464 0164 0264 0364 048d 035a 0565 036a  .d.d.d.d...Z.e.j
-00000d60: 0664 0164 0264 058d 025a 0765 036a 0864  .d.d.d...Z.e.j.d
-00000d70: 0164 0264 0264 068d 035a 0965 036a 0a65  .d.d.d...Z.e.j.e
-00000d80: 0b64 0365 0c67 0164 078d 035a 0d65 036a  .d.e.g.d...Z.e.j
-00000d90: 0e64 0264 0364 0364 088d 035a 0f65 036a  .d.d.d.d...Z.e.j
-00000da0: 1064 0964 0264 0265 036a 1164 0a64 0b8d  .d.d.d.e.j.d.d..
-00000db0: 055a 1247 0064 0c64 0d84 0064 0d83 025a  .Z.G.d.d...d...Z
-00000dc0: 1364 0e64 0f9c 0164 1064 1184 045a 1465  .d.d...d.d...Z.e
-00000dd0: 1565 1619 0064 0f9c 0164 1264 1384 045a  .e...d...d.d...Z
-00000de0: 1764 1b65 1865 1865 1965 1a19 0065 1965  .d.e.e.e.e...e.e
-00000df0: 1a19 0064 0e64 149c 0587 0066 0164 1564  ...d.d.....f.d.d
-00000e00: 1684 0d5a 1b64 0e64 0f9c 0164 1764 1884  ...Z.d.d...d.d..
-00000e10: 045a 1c65 1d64 0f9c 0164 1964 1a84 045a  .Z.e.d...d.d...Z
-00000e20: 1e87 0004 005a 1f53 0029 1cda 0c50 6172  .....Z.S.)...Par
-00000e30: 616d 6574 7269 7a65 72e9 ff00 0000 5446  ametrizer.....TF
-00000e40: 2903 7244 0000 00da 0675 6e69 7175 65da  ).rD.....unique.
-00000e50: 0865 6469 7461 626c 65a9 0272 4400 0000  .editable..rD...
-00000e60: 7268 0000 0029 0372 4400 0000 7246 0000  rh...).rD...rF..
-00000e70: 0072 4500 0000 2903 da07 6465 6661 756c  .rE...)...defaul
-00000e80: 7472 4500 0000 da0a 7661 6c69 6461 746f  trE.....validato
-00000e90: 7273 2903 7245 0000 0072 6b00 0000 7269  rs).rE...rk...ri
-00000ea0: 0000 00da 0551 7565 7279 fa01 2ba9 0472  .....Query..+..r
-00000eb0: 4500 0000 7246 0000 00da 096f 6e5f 6465  E...rF.....on_de
-00000ec0: 6c65 7465 da0c 7265 6c61 7465 645f 6e61  lete..related_na
-00000ed0: 6d65 6300 0000 0000 0000 0000 0000 0000  mec.............
-00000ee0: 0000 0001 0000 0040 0000 0073 1400 0000  .......@...s....
-00000ef0: 6500 5a01 6400 5a02 6401 5a03 6401 5a04  e.Z.d.Z.d.Z.d.Z.
-00000f00: 6402 5300 2903 7a11 5061 7261 6d65 7472  d.S.).z.Parametr
-00000f10: 697a 6572 2e4d 6574 61da 0941 7267 756d  izer.Meta..Argum
-00000f20: 656e 7473 4e29 0572 4700 0000 7248 0000  entsN).rG...rH..
-00000f30: 0072 4900 0000 da13 7665 7262 6f73 655f  .rI.....verbose_
-00000f40: 6e61 6d65 5f70 6c75 7261 6cda 0c76 6572  name_plural..ver
-00000f50: 626f 7365 5f6e 616d 6572 2800 0000 7228  bose_namer(...r(
-00000f60: 0000 0072 2800 0000 722c 0000 0072 4b00  ...r(...r,...rK.
-00000f70: 0000 7600 0000 7304 0000 0008 0104 0172  ..v...s........r
-00000f80: 4b00 0000 4e72 4c00 0000 6301 0000 0000  K...NrL...c.....
-00000f90: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000fa0: 0000 0073 0e00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
-00000fb0: 0100 6400 5300 7227 0000 0029 0272 4000  ..d.S.r'...).r@.
-00000fc0: 0000 722f 0000 0072 5800 0000 7228 0000  ..r/...rX...r(..
-00000fd0: 0072 2800 0000 722c 0000 00da 0563 6c65  .r(...r,.....cle
-00000fe0: 616e 7a00 0000 7302 0000 0000 017a 1250  anz...s......z.P
-00000ff0: 6172 616d 6574 7269 7a65 722e 636c 6561  arametrizer.clea
-00001000: 6e63 0100 0000 0000 0000 0000 0000 0200  nc..............
-00001010: 0000 0400 0000 0300 0000 7326 0000 0074  ..........s&...t
-00001020: 0074 016a 0288 006a 03a0 04a1 008e 0083  .t.j...j........
-00001030: 017d 0187 0066 0164 0164 0284 087c 0144  .}...f.d.d...|.D
-00001040: 0083 0153 0029 034e 6301 0000 0000 0000  ...S.).Nc.......
-00001050: 0000 0000 0002 0000 0006 0000 0013 0000  ................
-00001060: 0073 2000 0000 6700 7c00 5d18 7d01 7400  .s ...g.|.].}.t.
-00001070: 7401 8800 6a02 a003 a100 7c01 8302 8301  t...j.....|.....
-00001080: 9102 7104 5300 7228 0000 0029 0472 3100  ..q.S.r(...).r1.
-00001090: 0000 7232 0000 0072 2f00 0000 7233 0000  ..r2...r/...r3..
-000010a0: 0072 3400 0000 7258 0000 0072 2800 0000  .r4...rX...r(...
-000010b0: 722c 0000 0072 3700 0000 7f00 0000 722e  r,...r7.......r.
-000010c0: 0000 007a 2b50 6172 616d 6574 7269 7a65  ...z+Parametrize
-000010d0: 722e 6765 745f 6d61 7472 6978 2e3c 6c6f  r.get_matrix.<lo
-000010e0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000010f0: 2905 723b 0000 0072 3c00 0000 723d 0000  ).r;...r<...r=..
-00001100: 0072 2f00 0000 723e 0000 0029 0272 5100  .r/...r>...).rQ.
-00001110: 0000 723d 0000 0072 2800 0000 7258 0000  ..r=...r(...rX..
-00001120: 0072 2c00 0000 da0a 6765 745f 6d61 7472  .r,.....get_matr
-00001130: 6978 7d00 0000 7304 0000 0000 0114 017a  ix}...s........z
-00001140: 1750 6172 616d 6574 7269 7a65 722e 6765  .Parametrizer.ge
-00001150: 745f 6d61 7472 6978 a905 da0c 666f 7263  t_matrix....forc
-00001160: 655f 696e 7365 7274 da0c 666f 7263 655f  e_insert..force_
-00001170: 7570 6461 7465 da05 7573 696e 67da 0d75  update..using..u
-00001180: 7064 6174 655f 6669 656c 6473 7230 0000  pdate_fieldsr0..
-00001190: 0063 0500 0000 0000 0000 0000 0000 0500  .c..............
-000011a0: 0000 0600 0000 0300 0000 7328 0000 007c  ..........s(...|
-000011b0: 006a 0073 1274 017c 006a 0283 017c 005f  .j.s.t.|.j...|._
-000011c0: 0074 0383 00a0 047c 017c 027c 037c 04a1  .t.....|.|.|.|..
-000011d0: 0401 0064 0053 0072 2700 0000 2905 da04  ...d.S.r'...)...
-000011e0: 636f 6465 7215 0000 00da 046e 616d 65da  coder......name.
-000011f0: 0573 7570 6572 da04 7361 7665 a905 7251  .super..save..rQ
-00001200: 0000 0072 7800 0000 7279 0000 0072 7a00  ...rx...ry...rz.
-00001210: 0000 727b 0000 00a9 01da 095f 5f63 6c61  ..r{.......__cla
-00001220: 7373 5f5f 7228 0000 0072 2c00 0000 727f  ss__r(...r,...r.
-00001230: 0000 0081 0000 0073 0600 0000 0007 0601  .......s........
-00001240: 0c01 7a11 5061 7261 6d65 7472 697a 6572  ..z.Parametrizer
-00001250: 2e73 6176 6563 0100 0000 0000 0000 0000  .savec..........
-00001260: 0000 0300 0000 0300 0000 4300 0000 732a  ..........C...s*
-00001270: 0000 007c 006a 0072 267c 006a 006a 0164  ...|.j.r&|.j.j.d
-00001280: 0164 028d 015c 027d 017d 027c 017c 005f  .d...\.}.}.|.|._
-00001290: 027c 00a0 03a1 0001 0064 0053 0029 034e  .|.......d.S.).N
-000012a0: 5429 01da 0c75 7365 5f65 7869 7374 696e  T)...use_existin
-000012b0: 6729 04da 0673 6f75 7263 65da 0372 756e  g)...source..run
-000012c0: 722f 0000 0072 7f00 0000 2903 7251 0000  r/...r....).rQ..
-000012d0: 00da 036f 7574 da02 5f5f 7228 0000 0072  ...out..__r(...r
-000012e0: 2800 0000 722c 0000 00da 0772 6566 7265  (...r,.....refre
-000012f0: 7368 8c00 0000 7308 0000 0000 0106 0112  sh....s.........
-00001300: 0106 017a 1450 6172 616d 6574 7269 7a65  ...z.Parametrize
-00001310: 722e 7265 6672 6573 6863 0100 0000 0000  r.refreshc......
-00001320: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00001330: 0000 7306 0000 007c 006a 0053 0072 2700  ..s....|.j.S.r'.
-00001340: 0000 a901 727d 0000 0072 5800 0000 7228  ....r}...rX...r(
-00001350: 0000 0072 2800 0000 722c 0000 00da 075f  ...r(...r,....._
-00001360: 5f73 7472 5f5f 9200 0000 7302 0000 0000  _str__....s.....
-00001370: 017a 1450 6172 616d 6574 7269 7a65 722e  .z.Parametrizer.
-00001380: 5f5f 7374 725f 5f29 0446 464e 4e29 2072  __str__).FFNN) r
-00001390: 4700 0000 7248 0000 0072 4900 0000 720c  G...rH...rI...r.
-000013a0: 0000 00da 0953 6c75 6746 6965 6c64 727c  .....SlugFieldr|
-000013b0: 0000 0072 6400 0000 727d 0000 00da 0954  ...rd...r}.....T
-000013c0: 6578 7446 6965 6c64 da0b 6465 7363 7269  extField..descri
-000013d0: 7074 696f 6e72 0e00 0000 7231 0000 0072  ptionr....r1...r
-000013e0: 4000 0000 722f 0000 00da 0c42 6f6f 6c65  @...r/.....Boole
-000013f0: 616e 4669 656c 64da 0673 7973 7465 6dda  anField..system.
-00001400: 0a46 6f72 6569 676e 4b65 79da 0743 4153  .ForeignKey..CAS
-00001410: 4341 4445 7284 0000 0072 4b00 0000 7275  CADEr....rK...ru
-00001420: 0000 0072 0400 0000 7203 0000 0072 7600  ...r....r....rv.
-00001430: 0000 da04 626f 6f6c 7205 0000 0072 0200  ....boolr....r..
-00001440: 0000 727f 0000 0072 8800 0000 7250 0000  ..r....r....rP..
-00001450: 0072 8a00 0000 da0d 5f5f 636c 6173 7363  .r......__classc
-00001460: 656c 6c5f 5f72 2800 0000 7228 0000 0072  ell__r(...r(...r
-00001470: 8100 0000 722c 0000 0072 6600 0000 6800  ....r,...rf...h.
-00001480: 0000 7338 0000 0008 0110 010e 0104 0102  ..s8............
-00001490: 0102 0102 fd06 0512 0110 0104 010c ff06  ................
-000014a0: 040e 040e 0312 0600 0100 0100 0100 fb02  ................
-000014b0: 0202 0102 0106 0106 0102 fa10 0b0e 0672  ...............r
-000014c0: 6600 0000 6300 0000 0000 0000 0000 0000  f...c...........
-000014d0: 0000 0000 0007 0000 0000 0000 0073 5801  .............sX.
-000014e0: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
-000014f0: 6402 6403 8d02 5a05 6503 6a06 6402 6402  d.d...Z.e.j.d.d.
-00001500: 6404 8d02 5a07 6503 6a08 6509 8300 6503  d...Z.e.j.e...e.
-00001510: 6a0a 6405 6406 8d03 5a0b 6503 6a08 650c  j.d.d...Z.e.j.e.
-00001520: 6503 6a0a 6407 8d02 5a0d 6503 6a06 6408  e.j.d...Z.e.j.d.
-00001530: 6402 6409 8d02 5a0e 650f 6510 6402 6511  d.d...Z.e.e.d.e.
-00001540: 640a 8d03 5a12 6503 6a08 6513 6503 6a0a  d...Z.e.j.e.e.j.
-00001550: 6402 6402 640b 8d04 5a14 6503 6a04 640c  d.d.d...Z.e.j.d.
-00001560: 6402 6402 640d 8d03 5a15 6503 6a04 640c  d.d.d...Z.e.j.d.
-00001570: 6402 6402 640d 8d03 5a16 6503 6a17 6402  d.d.d...Z.e.j.d.
-00001580: 6402 640e 8d02 5a18 6503 6a19 6402 640f  d.d...Z.e.j.d.d.
-00001590: 8d01 5a1a 651b 6410 9c01 6411 6412 8404  ..Z.e.d...d.d...
-000015a0: 5a1c 4700 6413 6414 8400 6414 8302 5a1d  Z.G.d.d...d...Z.
-000015b0: 6428 651e 651e 651f 6520 1900 651f 6520  d(e.e.e.e ..e.e 
-000015c0: 1900 6416 6417 9c05 8700 6601 6418 6419  ..d.d.....f.d.d.
-000015d0: 840d 5a21 6522 6523 6524 641a 9c03 641b  ..Z!e"e#e$d...d.
-000015e0: 641c 8404 5a25 6526 6416 641d 9c02 641e  d...Z%e&d.d...d.
-000015f0: 641f 8404 5a27 6429 651e 6520 6526 6420  d...Z'd)e.e e&d 
-00001600: 9c03 6421 6422 8405 5a28 642a 651e 651f  ..d!d"..Z(d*e.e.
-00001610: 6524 1900 651e 6529 6423 9c04 6424 6425  e$..e.e)d#..d$d%
-00001620: 8405 5a2a 651b 6410 9c01 6426 6427 8404  ..Z*e.d...d&d'..
-00001630: 5a2b 8700 0400 5a2c 5300 292b 726d 0000  Z+....Z,S.)+rm..
-00001640: 0072 6700 0000 5472 6a00 0000 a902 7245  .rg...Trj.....rE
-00001650: 0000 0072 4600 0000 5a0d 706f 7765 725f  ...rF...Z.power_
-00001660: 7175 6572 6965 73a9 0272 7000 0000 7271  queries..rp...rq
-00001670: 0000 00a9 0172 7000 0000 7a0d 7173 3d63  .....rp...z.qs=c
-00001680: 6f6e 6e2e 616c 6c28 29a9 0272 6b00 0000  onn.all()..rk...
-00001690: 7245 0000 0029 0372 6b00 0000 7245 0000  rE...).rk...rE..
-000016a0: 00da 0765 6e63 6f64 6572 2903 7270 0000  ...encoder).rp..
-000016b0: 0072 4500 0000 7246 0000 0069 9001 0000  .rE...rF...i....
-000016c0: 7243 0000 00a9 0272 4600 0000 7245 0000  rC.....rF...rE..
-000016d0: 00a9 0172 6b00 0000 724c 0000 0063 0100  ...rk...rL...c..
-000016e0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-000016f0: 0000 4300 0000 730a 0000 007c 006a 0070  ..C...s....|.j.p
-00001700: 0864 0153 0072 5d00 0000 7289 0000 0072  .d.S.r]...r....r
-00001710: 5800 0000 7228 0000 0072 2800 0000 722c  X...r(...r(...r,
-00001720: 0000 0072 8a00 0000 a900 0000 7302 0000  ...r........s...
-00001730: 0000 017a 0d51 7565 7279 2e5f 5f73 7472  ...z.Query.__str
-00001740: 5f5f 6300 0000 0000 0000 0000 0000 0000  __c.............
-00001750: 0000 0001 0000 0040 0000 0073 1400 0000  .......@...s....
-00001760: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-00001770: 6403 5300 2904 7a0a 5175 6572 792e 4d65  d.S.).z.Query.Me
-00001780: 7461 7a0d 506f 7765 7220 5175 6572 6965  taz.Power Querie
-00001790: 7372 8900 0000 4e29 0572 4700 0000 7248  sr....N).rG...rH
-000017a0: 0000 0072 4900 0000 7273 0000 00da 086f  ...rI...rs.....o
-000017b0: 7264 6572 696e 6772 2800 0000 7228 0000  rderingr(...r(..
-000017c0: 0072 2800 0000 722c 0000 0072 4b00 0000  .r(...r,...rK...
-000017d0: ac00 0000 7304 0000 0008 0104 0172 4b00  ....s........rK.
-000017e0: 0000 464e 7277 0000 0063 0500 0000 0000  ..FNrw...c......
-000017f0: 0000 0000 0000 0500 0000 0600 0000 0300  ................
-00001800: 0000 7322 0000 007c 006a 0073 0c64 017c  ..s"...|.j.s.d.|
-00001810: 005f 0074 0183 00a0 027c 017c 027c 037c  ._.t.....|.|.|.|
-00001820: 04a1 0401 0064 0053 0029 024e 7a1c 7173  .....d.S.).Nz.qs
-00001830: 3d63 6f6e 6e2e 616c 6c28 292e 6f72 6465  =conn.all().orde
-00001840: 725f 6279 2827 6964 2729 2903 727c 0000  r_by('id')).r|..
-00001850: 0072 7e00 0000 727f 0000 0072 8000 0000  .r~...r....r....
-00001860: 7281 0000 0072 2800 0000 722c 0000 0072  r....r(...r,...r
-00001870: 7f00 0000 b000 0000 7306 0000 0000 0706  ........s.......
-00001880: 0106 017a 0a51 7565 7279 2e73 6176 6529  ...z.Query.save)
-00001890: 03da 0871 7565 7279 5f69 64da 0961 7267  ...query_id..arg
-000018a0: 756d 656e 7473 7230 0000 0063 0300 0000  umentsr0...c....
-000018b0: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-000018c0: 4300 0000 7322 0000 0074 006a 016a 027c  C...s"...t.j.j.|
-000018d0: 0164 018d 017d 037c 036a 0364 027c 0264  .d...}.|.j.d.|.d
-000018e0: 0364 048d 037d 047c 0453 0029 054e 2901  .d...}.|.S.).N).
-000018f0: da02 6964 4654 2903 da07 7065 7273 6973  ..idFT)...persis
-00001900: 7472 9d00 0000 7283 0000 0029 0472 6d00  tr....r....).rm.
-00001910: 0000 da07 6f62 6a65 6374 73da 0367 6574  ....objects..get
-00001920: 7285 0000 0029 0572 5100 0000 729c 0000  r....).rQ...r...
-00001930: 0072 9d00 0000 da05 7175 6572 7972 5200  .r......queryrR.
-00001940: 0000 7228 0000 0072 2800 0000 722c 0000  ..r(...r(...r,..
-00001950: 00da 075f 696e 766f 6b65 bb00 0000 7306  ..._invoke....s.
-00001960: 0000 0000 010e 0110 017a 0d51 7565 7279  .........z.Query
-00001970: 2e5f 696e 766f 6b65 2902 da07 7265 7375  ._invoke)...resu
-00001980: 6c74 7372 3000 0000 6302 0000 0000 0000  ltsr0...c.......
-00001990: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000019a0: 0073 3c00 0000 7c01 7c00 6a00 6401 3c00  .s<...|.|.j.d.<.
-000019b0: 7c01 a001 6402 6403 a102 7c00 5f02 7c01  |...d.d...|._.|.
-000019c0: a001 6404 6403 a102 7c00 5f03 7404 a005  ..d.d...|._.t...
-000019d0: a100 7c00 5f06 7c00 a007 a100 0100 6400  ..|._.|.......d.
-000019e0: 5300 2905 4e5a 106c 6173 745f 7275 6e5f  S.).NZ.last_run_
-000019f0: 7265 7375 6c74 73da 0d65 7272 6f72 5f6d  results..error_m
-00001a00: 6573 7361 6765 725e 0000 00da 0f73 656e  essager^.....sen
-00001a10: 7472 795f 6572 726f 725f 6964 2908 da04  try_error_id)...
-00001a20: 696e 666f 72a1 0000 0072 a500 0000 72a6  infor....r....r.
-00001a30: 0000 0072 1200 0000 da03 6e6f 77da 086c  ...r......now..l
-00001a40: 6173 745f 7275 6e72 7f00 0000 2902 7251  ast_runr....).rQ
-00001a50: 0000 0072 a400 0000 7228 0000 0072 2800  ...r....r(...r(.
-00001a60: 0000 722c 0000 00da 0e75 7064 6174 655f  ..r,.....update_
-00001a70: 7265 7375 6c74 73c0 0000 0073 0a00 0000  results....s....
-00001a80: 0001 0a01 0e01 0e01 0a01 7a14 5175 6572  ..........z.Quer
-00001a90: 792e 7570 6461 7465 5f72 6573 756c 7473  y.update_results
-00001aa0: 2903 729f 0000 00da 066b 7761 7267 7372  ).r......kwargsr
-00001ab0: 3000 0000 6302 0000 0000 0000 0000 0000  0...c...........
-00001ac0: 000a 0000 000d 0000 000b 0000 0073 9201  .............s..
-00001ad0: 0000 8801 6a00 721e 8801 6a00 a001 a100  ....j.r...j.....
-00001ae0: 7d03 7c03 7324 7402 6401 8301 8201 6e06  }.|.s$t.d.....n.
-00001af0: 6900 6701 7d03 6400 8801 5f03 6400 8801  i.g.}.d..._.d...
-00001b00: 5f04 6400 8801 5f05 6900 8801 5f06 6402  _.d..._.i..._.d.
-00001b10: 7407 7408 a009 a100 6403 8302 6901 8900  t.t.....d...i...
-00001b20: 740a 8300 9001 8f26 7d04 7c04 a00b 6404  t......&}.|...d.
-00001b30: 6405 a102 0100 7c04 a00b 6406 8801 6a0c  d.....|...d...j.
-00001b40: a102 0100 740d a00e a100 8fe2 0100 740d  ....t.........t.
-00001b50: a00f 8700 8701 6602 6407 6408 8408 a101  ......f.d.d.....
-00001b60: 0100 7c03 4400 5d98 7d05 7a42 8801 a010  ..|.D.].}.zB....
-00001b70: 7c01 7c05 a102 5c02 7d06 7d07 7411 7c06  |.|...\.}.}.t.|.
-00001b80: 7412 8302 72c4 7c06 6a13 8800 7414 7c05  t...r.|.j...t.|.
-00001b90: 8301 3c00 6e14 7414 7415 7c06 8301 8301  ..<.n.t.t.|.....
-00001ba0: 8800 7414 7c05 8301 3c00 5700 7194 0400  ..t.|...<.W.q...
-00001bb0: 7416 9001 792a 0100 7d08 0100 7a36 7417  t...y*..}...z6t.
-00001bc0: a018 7c08 a101 0100 7419 7c08 8301 7d09  ..|.....t.|...}.
-00001bd0: 7414 7c09 8301 8800 6409 3c00 7414 7c08  t.|.....d.<.t.|.
-00001be0: 8301 8800 640a 3c00 5700 5900 6400 7d08  ....d.<.W.Y.d.}.
-00001bf0: 7e08 7194 6400 7d08 7e08 3000 3000 7194  ~.q.d.}.~.0.0.q.
-00001c00: 8801 6a1a 6a1b 640b 640c 8400 8800 a01c  ..j.j.d.d.......
-00001c10: a100 4400 8301 640d 8d01 a01d a100 0100  ..D...d.........
-00001c20: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
-00001c30: 9001 7364 3000 0100 0100 0100 5900 0100  ..sd0.......Y...
-00001c40: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
-00001c50: 9001 7384 3000 0100 0100 0100 5900 0100  ..s.0.......Y...
-00001c60: 8800 5300 290e 4e7a 1b4e 6f20 7661 6c69  ..S.).Nz.No vali
-00001c70: 6420 6172 6775 6d65 6e74 7320 7072 6f76  d arguments prov
-00001c80: 6964 6564 da09 7469 6d65 7374 616d 707a  ided..timestampz
-00001c90: 0e25 592d 256d 2d25 6420 2548 3a25 4dda  .%Y-%m-%d %H:%M.
-00001ca0: 0b70 6f77 6572 5f71 7565 7279 547a 1070  .power_queryTz.p
-00001cb0: 6f77 6572 5f71 7565 7279 2e6e 616d 6563  ower_query.namec
-00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cd0: 0300 0000 1300 0000 730a 0000 0088 01a0  ........s.......
-00001ce0: 0088 00a1 0153 0072 2700 0000 2901 72aa  .....S.r'...).r.
-00001cf0: 0000 0072 2800 0000 a902 72a4 0000 0072  ...r(.....r....r
-00001d00: 5100 0000 7228 0000 0072 2c00 0000 da08  Q...r(...r,.....
-00001d10: 3c6c 616d 6264 613e da00 0000 722e 0000  <lambda>....r...
-00001d20: 007a 2651 7565 7279 2e65 7865 6375 7465  .z&Query.execute
-00001d30: 5f6d 6174 7269 782e 3c6c 6f63 616c 733e  _matrix.<locals>
-00001d40: 2e3c 6c61 6d62 6461 3e72 a600 0000 72a5  .<lambda>r....r.
-00001d50: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001d60: 0200 0000 0500 0000 5300 0000 731a 0000  ........S...s...
-00001d70: 0067 007c 005d 127d 0174 007c 0174 0183  .g.|.].}.t.|.t..
-00001d80: 0272 047c 0191 0271 0453 0072 2800 0000  .r.|...q.S.r(...
-00001d90: 2902 723a 0000 00da 0369 6e74 2902 7229  ).r:.....int).r)
-00001da0: 0000 005a 0364 706b 7228 0000 0072 2800  ...Z.dpkr(...r(.
-00001db0: 0000 722c 0000 0072 3700 0000 e900 0000  ..r,...r7.......
-00001dc0: 722e 0000 007a 2851 7565 7279 2e65 7865  r....z(Query.exe
-00001dd0: 6375 7465 5f6d 6174 7269 782e 3c6c 6f63  cute_matrix.<loc
-00001de0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
-00001df0: 01da 0670 6b5f 5f69 6e29 1eda 0c70 6172  ...pk__in)...par
-00001e00: 616d 6574 7269 7a65 7272 7600 0000 da0a  ametrizerrv.....
-00001e10: 5661 6c75 6545 7272 6f72 72a5 0000 0072  ValueErrorr....r
-00001e20: a600 0000 72a9 0000 0072 a700 0000 7213  ....r....r....r.
-00001e30: 0000 0072 1200 0000 72a8 0000 0072 1a00  ...r....r....r..
-00001e40: 0000 da07 7365 745f 7461 6772 7d00 0000  ....set_tagr}...
-00001e50: 720d 0000 00da 0661 746f 6d69 63da 096f  r......atomic..o
-00001e60: 6e5f 636f 6d6d 6974 7285 0000 0072 3a00  n_commitr....r:.
-00001e70: 0000 da07 4461 7461 7365 74da 0270 6b72  ....Dataset..pkr
-00001e80: 5000 0000 da03 6c65 6e72 1b00 0000 da06  P.....lenr......
-00001e90: 6c6f 6767 6572 da09 6578 6365 7074 696f  logger..exceptio
-00001ea0: 6e72 1900 0000 da08 6461 7461 7365 7473  nr......datasets
-00001eb0: da07 6578 636c 7564 6572 3e00 0000 da06  ..excluder>.....
-00001ec0: 6465 6c65 7465 290a 7251 0000 0072 9f00  delete).rQ...r..
-00001ed0: 0000 72ab 0000 00da 0461 7267 73da 0573  ..r......args..s
-00001ee0: 636f 7065 da01 61da 0764 6174 6173 6574  cope..a..dataset
-00001ef0: 7287 0000 0072 3500 0000 da03 6572 7272  r....r5.....errr
-00001f00: 2800 0000 72ae 0000 0072 2c00 0000 da0e  (...r....r,.....
-00001f10: 6578 6563 7574 655f 6d61 7472 6978 c700  execute_matrix..
-00001f20: 0000 733e 0000 0000 0106 010a 0104 010a  ..s>............
-00001f30: 0206 0106 0106 0106 0106 030e ff04 030a  ................
-00001f40: 010c 010e 010a 0114 0108 0102 0110 010a  ................
-00001f50: 0110 0218 0210 010a 0108 010c 0124 0106  .............$..
-00001f60: 0110 ff4a 037a 1451 7565 7279 2e65 7865  ...J.z.Query.exe
-00001f70: 6375 7465 5f6d 6174 7269 7829 0472 9f00  cute_matrix).r..
-00001f80: 0000 729d 0000 0072 8300 0000 7230 0000  ..r....r....r0..
-00001f90: 0063 0400 0000 0000 0000 0000 0000 1000  .c..............
-00001fa0: 0000 0a00 0000 4300 0000 7364 0100 007c  ......C...sd...|
-00001fb0: 006a 00a0 01a1 007d 0464 0164 0284 0074  .j.....}.d.d...t
-00001fc0: 0283 0066 0144 0083 017d 057c 006a 036a  ...f.D...}.|.j.j
-00001fd0: 0472 3474 056a 06a0 07a1 007c 0564 033c  .r4t.j.....|.d.<
-00001fe0: 006e 1474 056a 066a 077c 006a 0364 048d  .n.t.j.j.|.j.d..
-00001ff0: 017c 0564 033c 007a e67c 046a 08a0 0974  .|.d.<.z.|.j...t
-00002000: 0a6a 0ba1 017c 007c 027c 027c 006a 0c64  .j...|.|.|.|.j.d
-00002010: 059c 057c 05a5 017d 0674 0d64 067c 006a  ...|...}.t.d.|.j
-00002020: 0e69 017c 0272 7c7c 026e 0269 00a5 0183  .i.|.r||.n.i....
-00002030: 017d 077c 0372 ac74 0f6a 066a 077c 007c  .}.|.r.t.j.j.|.|
-00002040: 0764 078d 02a0 10a1 0004 007d 0872 ac7c  .d.........}.r.|
-00002050: 087c 086a 1166 027d 096e 8074 127c 006a  .|.j.f.}.n.t.|.j
-00002060: 1374 1483 007c 0683 0301 007c 06a0 1564  .t...|.....|...d
-00002070: 0864 00a1 027d 0a7c 06a0 1564 0964 00a1  .d...}.|...d.d..
-00002080: 027d 0b7c 0190 0172 2474 167c 0a83 016a  .}.|...r$t.|...j
-00002090: 177c 0264 0a9c 027d 0c74 0f6a 066a 187c  .|.d...}.t.j.j.|
-000020a0: 007c 077c 0c74 19a0 1aa1 0074 1ba0 1c7c  .|.|.t.....t...|
-000020b0: 0aa1 0174 1ba0 1c7c 0ba1 0164 0b9c 0464  ...t...|...d...d
-000020c0: 0c8d 035c 027d 0d7d 0e7c 0d7c 0b66 027d  ...\.}.}.|.|.f.}
-000020d0: 096e 087c 0a7c 0b66 027d 0957 006e 3004  .n.|.|.f.}.W.n0.
-000020e0: 0074 1d90 0179 5e01 007d 0f01 007a 1674  .t...y^..}...z.t
-000020f0: 1e7c 0f83 017c 0f82 0257 0059 0064 007d  .|...|...W.Y.d.}
-00002100: 0f7e 0f6e 0a64 007d 0f7e 0f30 0030 007c  .~.n.d.}.~.0.0.|
-00002110: 0953 0029 0d4e 6301 0000 0000 0000 0000  .S.).Nc.........
-00002120: 0000 0002 0000 0006 0000 0053 0000 0073  ...........S...s
-00002130: 2600 0000 6900 7c00 5d1e 7d01 7c01 6a00  &...i.|.].}.|.j.
-00002140: 6a01 9b00 6400 9d02 7c01 6a02 a003 7404  j...d...|.j...t.
-00002150: 6a05 a101 9302 7104 5300 2901 da07 4d61  j.....q.S.)...Ma
-00002160: 6e61 6765 7229 06da 055f 6d65 7461 da0b  nager)..._meta..
-00002170: 6f62 6a65 6374 5f6e 616d 65da 105f 6465  object_name.._de
-00002180: 6661 756c 745f 6d61 6e61 6765 7272 7a00  fault_managerrz.
-00002190: 0000 7208 0000 00da 1450 4f57 4552 5f51  ..r......POWER_Q
-000021a0: 5545 5259 5f44 425f 414c 4941 5329 0272  UERY_DB_ALIAS).r
-000021b0: 2900 0000 da05 6d6f 6465 6c72 2800 0000  ).....modelr(...
-000021c0: 7228 0000 0072 2c00 0000 da0a 3c64 6963  r(...r,.....<dic
-000021d0: 7463 6f6d 703e f400 0000 7308 0000 0006  tcomp>....s.....
-000021e0: 0402 fd12 0104 ff7a 1d51 7565 7279 2e72  .......z.Query.r
-000021f0: 756e 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  un.<locals>.<dic
-00002200: 7463 6f6d 703e da0c 5175 6572 794d 616e  tcomp>..QueryMan
-00002210: 6167 6572 2901 da05 6f77 6e65 7229 05da  ager)...owner)..
-00002220: 0463 6f6e 6e72 a200 0000 72bf 0000 0072  .connr....r....r
-00002230: 9d00 0000 da06 696e 766f 6b65 72a2 0000  ......invoker...
-00002240: 0029 0272 a200 0000 da04 6861 7368 7252  .).r......hashrR
-00002250: 0000 00da 0565 7874 7261 2902 da04 7479  .....extra)...ty
-00002260: 7065 729d 0000 0029 0472 a700 0000 72a9  per....).r....r.
-00002270: 0000 0072 2f00 0000 72d1 0000 0029 0372  ...r/...r....).r
-00002280: a200 0000 72d0 0000 00da 0864 6566 6175  ....r......defau
-00002290: 6c74 7329 1fda 0674 6172 6765 74da 0b6d  lts)...target..m
-000022a0: 6f64 656c 5f63 6c61 7373 7209 0000 0072  odel_classr....r
-000022b0: cd00 0000 da0c 6973 5f73 7570 6572 7573  ......is_superus
-000022c0: 6572 726d 0000 0072 a000 0000 da06 6669  errm...r......fi
-000022d0: 6c74 6572 72c8 0000 0072 7a00 0000 7208  lterr....rz...r.
-000022e0: 0000 0072 c900 0000 72a3 0000 0072 1d00  ...r....r....r..
-000022f0: 0000 72b8 0000 0072 b700 0000 da05 6669  ..r....r......fi
-00002300: 7273 7472 d100 0000 da04 6578 6563 727c  rstr......execr|
-00002310: 0000 00da 0767 6c6f 6261 6c73 72a1 0000  .....globalsr...
-00002320: 0072 d200 0000 7247 0000 00da 1075 7064  .r....rG.....upd
-00002330: 6174 655f 6f72 5f63 7265 6174 6572 1200  ate_or_creater..
-00002340: 0000 72a8 0000 00da 0670 6963 6b6c 65da  ..r......pickle.
-00002350: 0564 756d 7073 723f 0000 0072 1b00 0000  .dumpsr?...r....
-00002360: 2910 7251 0000 0072 9f00 0000 729d 0000  ).rQ...r....r...
-00002370: 0072 8300 0000 72ca 0000 00da 0b63 6f6e  .r....r......con
-00002380: 6e65 6374 696f 6e73 da07 6c6f 6361 6c73  nections..locals
-00002390: 5fda 0973 6967 6e61 7475 7265 da02 6473  _..signature..ds
-000023a0: da0c 7265 7475 726e 5f76 616c 7565 7252  ..return_valuerR
-000023b0: 0000 0072 d100 0000 72a7 0000 0072 c200  ...r....r....r..
-000023c0: 0000 7287 0000 0072 3500 0000 7228 0000  ..r....r5...r(..
-000023d0: 0072 2800 0000 722c 0000 0072 8500 0000  .r(...r,...r....
-000023e0: ed00 0000 735a 0000 0000 060a 0106 0504  ....sZ..........
-000023f0: ff02 fc06 0908 0110 0214 0202 020c 0102  ................
-00002400: 0102 0102 0104 fb04 0602 fa04 0802 0114  ................
-00002410: ff04 0304 0116 ff02 030c 0210 010c 010c  ................
-00002420: 0206 0208 0102 fe06 0406 0102 0102 0202  ................
-00002430: 0106 0108 0108 fc04 fd0a 0a0a 020c 0110  ................
-00002440: 0120 017a 0951 7565 7279 2e72 756e 6301  . .z.Query.runc.
-00002450: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00002460: 0000 0043 0000 0073 2e00 0000 6401 6402  ...C...s....d.d.
-00002470: 6c00 6d01 7d01 0100 7c01 a002 7c00 6a03  l.m.}...|...|.j.
-00002480: a101 7d02 7c02 6a03 7c00 5f04 7c00 a005  ..}.|.j.|._.|...
-00002490: a100 0100 7c02 6a03 5300 2903 4e72 0100  ....|.j.S.).Nr..
-000024a0: 0000 2901 da14 7275 6e5f 6261 636b 6772  ..)...run_backgr
-000024b0: 6f75 6e64 5f71 7565 7279 2906 da18 706f  ound_query)...po
-000024c0: 7765 725f 7175 6572 792e 6365 6c65 7279  wer_query.celery
-000024d0: 5f74 6173 6b73 72e3 0000 00da 0564 656c  _tasksr......del
-000024e0: 6179 729e 0000 0072 4d00 0000 727f 0000  ayr....rM...r...
-000024f0: 0029 0372 5100 0000 72e3 0000 00da 0372  .).rQ...r......r
-00002500: 6573 7228 0000 0072 2800 0000 722c 0000  esr(...r(...r,..
-00002510: 0072 5900 0000 2d01 0000 730a 0000 0000  .rY...-...s.....
-00002520: 010c 020c 0108 0108 017a 0c51 7565 7279  .........z.Query
-00002530: 2e5f 7175 6575 6529 0446 464e 4e29 0154  ._queue).FFNN).T
-00002540: 2903 464e 4629 2d72 4700 0000 7248 0000  ).FNF)-rG...rH..
-00002550: 0072 4900 0000 720c 0000 0072 6400 0000  .rI...r....rd...
-00002560: 727d 0000 0072 8c00 0000 728d 0000 0072  r}...r....r....r
-00002570: 9000 0000 7209 0000 0072 9100 0000 72cd  ....r....r....r.
-00002580: 0000 0072 0a00 0000 72d4 0000 0072 7c00  ...r....r....r|.
-00002590: 0000 720e 0000 0072 3100 0000 721c 0000  ..r....r1...r...
-000025a0: 0072 a700 0000 7266 0000 0072 b200 0000  .r....rf...r....
-000025b0: 72a6 0000 0072 a500 0000 da0d 4461 7465  r....r......Date
-000025c0: 5469 6d65 4669 656c 6472 a900 0000 728e  TimeFieldr....r.
-000025d0: 0000 00da 0661 6374 6976 6572 5000 0000  .....activerP...
-000025e0: 728a 0000 0072 4b00 0000 7292 0000 0072  r....rK...r....r
-000025f0: 0500 0000 7202 0000 0072 7f00 0000 72b0  ....r....r....r.
-00002600: 0000 0072 0400 0000 7203 0000 0072 a300  ...r....r....r..
-00002610: 0000 da11 5175 6572 794d 6174 7269 7852  ....QueryMatrixR
-00002620: 6573 756c 7472 aa00 0000 72c4 0000 00da  esultr....r.....
-00002630: 0b51 7565 7279 5265 7375 6c74 7285 0000  .QueryResultr...
-00002640: 0072 5900 0000 7293 0000 0072 2800 0000  .rY...r....r(...
-00002650: 7228 0000 0072 8100 0000 722c 0000 0072  r(...r....r,...r
-00002660: 6d00 0000 9600 0000 7352 0000 0008 010e  m.......sR......
-00002670: 010e 0104 010a ff06 0310 010e 010e 0104  ................
-00002680: 010a ff06 0310 0110 020e 020c 020e 030e  ................
-00002690: 0600 0100 0100 0100 fb02 0202 0102 0106  ................
-000026a0: 0106 0102 fa10 0b12 0510 0714 2800 0100  ............(...
-000026b0: 0100 fc02 0202 0106 0102 0102 fb0c 4072  ..............@r
-000026c0: 6d00 0000 6300 0000 0000 0000 0000 0000  m...c...........
-000026d0: 0000 0000 0005 0000 0040 0000 0073 b600  .........@...s..
-000026e0: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
-000026f0: 6402 6403 6404 8d03 5a05 6503 6a06 6401  d.d.d...Z.e.j.d.
-00002700: 6401 6405 8d02 5a07 6503 6a04 6406 6407  d.d...Z.e.j.d.d.
-00002710: 8d01 5a08 6503 6a09 650a 6503 6a0b 6408  ..Z.e.j.e.e.j.d.
-00002720: 6409 8d03 5a0c 6503 6a0d 6401 6401 6405  d...Z.e.j.d.d.d.
-00002730: 8d02 5a0e 650f 6510 6401 640a 8d02 5a11  ..Z.e.e.d.d...Z.
-00002740: 6503 6a0d 6401 6401 640b 640c 8d03 5a12  e.j.d.d.d.d...Z.
-00002750: 6513 640d 9c01 640e 640f 8404 5a14 6515  e.d...d.d...Z.e.
-00002760: 6516 640d 9c01 6410 6411 8404 8301 5a17  e.d...d.d.....Z.
-00002770: 6515 6518 640d 9c01 6412 6413 8404 8301  e.e.d...d.d.....
-00002780: 5a19 6515 651a 640d 9c01 6414 6415 8404  Z.e.e.d...d.d...
-00002790: 8301 5a1b 6416 5300 2917 72b7 0000 0054  ..Z.d.S.).r....T
-000027a0: e9c8 0000 0046 2903 7268 0000 0072 4400  .....F).rh...rD.
-000027b0: 0000 7269 0000 0072 9900 0000 e964 0000  ..ri...r.....d..
-000027c0: 00a9 0172 4400 0000 72bc 0000 0072 9500  ...rD...r....r..
-000027d0: 0000 7297 0000 007a 2c41 6e79 206f 7468  ..r....z,Any oth
-000027e0: 6572 2061 7474 7269 6275 7465 2074 6f20  er attribute to 
-000027f0: 7061 7373 2074 6f20 7468 6520 666f 726d  pass to the form
-00002800: 6174 7465 7229 0372 4600 0000 7245 0000  atter).rF...rE..
-00002810: 00da 0968 656c 705f 7465 7874 724c 0000  ...help_textrL..
-00002820: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00002830: 0000 0400 0000 4300 0000 7316 0000 0064  ......C...s....d
-00002840: 017c 006a 006a 019b 0064 027c 006a 029b  .|.j.j...d.|.j..
-00002850: 009d 0453 0029 034e 7a0a 5265 7375 6c74  ...S.).Nz.Result
-00002860: 206f 6620 da01 2029 0372 a200 0000 727d   of .. ).r....r}
-00002870: 0000 0072 9d00 0000 7258 0000 0072 2800  ...r....rX...r(.
-00002880: 0000 7228 0000 0072 2c00 0000 728a 0000  ..r(...r,...r...
-00002890: 0041 0100 0073 0200 0000 0001 7a0f 4461  .A...s......z.Da
-000028a0: 7461 7365 742e 5f5f 7374 725f 5f63 0100  taset.__str__c..
-000028b0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000028c0: 0000 4300 0000 730c 0000 0074 00a0 017c  ..C...s....t...|
-000028d0: 006a 02a1 0153 0072 2700 0000 2903 72dc  .j...S.r'...).r.
-000028e0: 0000 00da 056c 6f61 6473 722f 0000 0072  .....loadsr/...r
-000028f0: 5800 0000 7228 0000 0072 2800 0000 722c  X...r(...r(...r,
-00002900: 0000 00da 0464 6174 6144 0100 0073 0200  .....dataD...s..
-00002910: 0000 0002 7a0c 4461 7461 7365 742e 6461  ....z.Dataset.da
-00002920: 7461 6301 0000 0000 0000 0000 0000 0001  tac.............
-00002930: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00002940: 7400 7c00 6a01 8301 5300 7227 0000 0029  t.|.j...S.r'...)
-00002950: 0272 b900 0000 722f 0000 0072 5800 0000  .r....r/...rX...
-00002960: 7228 0000 0072 2800 0000 722c 0000 00da  r(...r(...r,....
-00002970: 0473 697a 6548 0100 0073 0200 0000 0002  .sizeH...s......
-00002980: 7a0c 4461 7461 7365 742e 7369 7a65 6301  z.Dataset.sizec.
-00002990: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000029a0: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
-000029b0: a001 6401 6900 a102 5300 2902 4e72 9d00  ..d.i...S.).Nr..
-000029c0: 0000 2902 72a7 0000 0072 a100 0000 7258  ..).r....r....rX
-000029d0: 0000 0072 2800 0000 7228 0000 0072 2c00  ...r(...r(...r,.
-000029e0: 0000 729d 0000 004c 0100 0073 0200 0000  ..r....L...s....
-000029f0: 0002 7a11 4461 7461 7365 742e 6172 6775  ..z.Dataset.argu
-00002a00: 6d65 6e74 734e 291c 7247 0000 0072 4800  mentsN).rG...rH.
-00002a10: 0000 7249 0000 0072 0c00 0000 7264 0000  ..rI...r....rd..
-00002a20: 0072 d000 0000 72e7 0000 0072 a900 0000  .r....r....r....
-00002a30: 728d 0000 0072 9000 0000 726d 0000 0072  r....r....rm...r
-00002a40: 9100 0000 72a2 0000 00da 0b42 696e 6172  ....r......Binar
-00002a50: 7946 6965 6c64 722f 0000 0072 0e00 0000  yFieldr/...r....
-00002a60: 7231 0000 0072 a700 0000 72d1 0000 0072  r1...r....r....r
-00002a70: 5000 0000 728a 0000 0072 6500 0000 7202  P...r....re...r.
-00002a80: 0000 0072 f100 0000 72b0 0000 0072 f200  ...r....r....r..
-00002a90: 0000 7203 0000 0072 9d00 0000 7228 0000  ..r....r....r(..
-00002aa0: 0072 2800 0000 7228 0000 0072 2c00 0000  .r(...r(...r,...
-00002ab0: 72b7 0000 0036 0100 0073 2000 0000 0801  r....6...s .....
-00002ac0: 1001 0e01 0c01 1201 0e01 0c01 0401 06ff  ................
-00002ad0: 0604 0e03 0201 1003 0201 1003 0201 72b7  ..............r.
-00002ae0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00002af0: 0000 0000 0600 0000 4000 0000 7358 0000  ........@...sX..
-00002b00: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
-00002b10: 0264 0264 0264 038d 045a 0565 036a 0464  .d.d.d...Z.e.j.d
-00002b20: 0465 0664 058d 025a 0765 036a 0864 0264  .e.d...Z.e.j.d.d
-00002b30: 0264 068d 025a 0965 0a64 079c 0164 0864  .d...Z.e.d...d.d
-00002b40: 0984 045a 0b65 0c65 0a64 0a9c 0264 0b64  ...Z.e.e.d...d.d
-00002b50: 0c84 045a 0d64 0d53 0029 0eda 0946 6f72  ...Z.d.S.)...For
-00002b60: 6d61 7474 6572 7267 0000 0054 a904 7244  matterrg...T..rD
-00002b70: 0000 0072 4500 0000 7246 0000 0072 6800  ...rE...rF...rh.
-00002b80: 0000 e905 0000 00a9 0272 4400 0000 da07  .........rD.....
-00002b90: 6368 6f69 6365 7372 9400 0000 724c 0000  choicesr....rL..
-00002ba0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00002bb0: 0000 0100 0000 4300 0000 730a 0000 007c  ......C...s....|
-00002bc0: 006a 0070 0864 0153 0072 5d00 0000 7289  .j.p.d.S.r]...r.
-00002bd0: 0000 0072 5800 0000 7228 0000 0072 2800  ...rX...r(...r(.
-00002be0: 0000 722c 0000 0072 8a00 0000 5601 0000  ..r,...r....V...
-00002bf0: 7302 0000 0000 017a 1146 6f72 6d61 7474  s......z.Formatt
-00002c00: 6572 2e5f 5f73 7472 5f5f 2902 da07 636f  er.__str__)...co
-00002c10: 6e74 6578 7472 3000 0000 6302 0000 0000  ntextr0...c.....
-00002c20: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00002c30: 0000 0073 8e00 0000 7c00 6a00 6401 6b02  ...s....|.j.d.k.
-00002c40: 7222 7401 7c01 6402 1900 6a02 8301 7d02  r"t.|.d...j...}.
-00002c50: 7c02 a003 6401 a101 5300 7c00 6a04 7234  |...d...S.|.j.r4
-00002c60: 7405 7c00 6a04 8301 7d03 6e4c 7c00 6a00  t.|.j...}.nL|.j.
-00002c70: 6403 6b02 7256 7401 7c01 6402 1900 6a02  d.k.rVt.|.d...j.
-00002c80: 8301 7d02 7c02 a003 6403 a101 5300 7c00  ..}.|...d...S.|.
-00002c90: 6a00 6404 6b02 7278 7401 7c01 6402 1900  j.d.k.rxt.|.d...
-00002ca0: 6a02 8301 7d02 7c02 a003 6404 a101 5300  j...}.|...d...S.
-00002cb0: 7406 6405 8301 8201 7c03 a007 7408 7c01  t.d.....|...t.|.
-00002cc0: 8301 a101 5300 2906 4e72 2400 0000 72c2  ....S.).Nr$...r.
-00002cd0: 0000 0072 2200 0000 7226 0000 007a 1055  ...r"...r&...z.U
-00002ce0: 6e61 626c 6520 746f 2072 656e 6465 7229  nable to render)
-00002cf0: 09da 0c63 6f6e 7465 6e74 5f74 7970 6572  ...content_typer
-00002d00: 1e00 0000 72f1 0000 00da 0665 7870 6f72  ....r......expor
-00002d10: 7472 7c00 0000 7210 0000 0072 b300 0000  tr|...r....r....
-00002d20: da06 7265 6e64 6572 720f 0000 0029 0472  ..renderr....).r
-00002d30: 5100 0000 72f9 0000 00da 0264 74da 0374  Q...r......dt..t
-00002d40: 706c 7228 0000 0072 2800 0000 722c 0000  plr(...r(...r,..
-00002d50: 0072 fc00 0000 5901 0000 731a 0000 0000  .r....Y...s.....
-00002d60: 010a 010e 010a 0206 010c 010a 010e 010a  ................
-00002d70: 010a 010e 010a 0208 027a 1046 6f72 6d61  .........z.Forma
-00002d80: 7474 6572 2e72 656e 6465 724e 290e 7247  tter.renderN).rG
-00002d90: 0000 0072 4800 0000 7249 0000 0072 0c00  ...rH...rI...r..
-00002da0: 0000 7264 0000 0072 7d00 0000 da09 4d49  ..rd...r}.....MI
-00002db0: 4d45 5459 5045 5372 fa00 0000 728c 0000  METYPESr....r...
-00002dc0: 0072 7c00 0000 7250 0000 0072 8a00 0000  .r|...rP...r....
-00002dd0: 7203 0000 0072 fc00 0000 7228 0000 0072  r....r....r(...r
-00002de0: 2800 0000 7228 0000 0072 2c00 0000 72f4  (...r(...r,...r.
-00002df0: 0000 0051 0100 0073 0a00 0000 0801 1201  ...Q...s........
-00002e00: 0e01 0e02 0e03 72f4 0000 0063 0000 0000  ......r....c....
-00002e10: 0000 0000 0000 0000 0000 0000 0800 0000  ................
-00002e20: 0000 0000 731c 0100 0065 005a 0164 005a  ....s....e.Z.d.Z
-00002e30: 0265 036a 0464 0164 0264 0264 0264 038d  .e.j.d.d.d.d.d..
-00002e40: 045a 0565 036a 0464 0164 0264 0264 048d  .Z.e.j.d.d.d.d..
-00002e50: 035a 0665 036a 0765 0865 036a 0964 058d  .Z.e.j.e.e.j.d..
-00002e60: 025a 0a65 036a 0765 0b65 036a 0964 058d  .Z.e.j.e.e.j.d..
-00002e70: 025a 0c65 036a 0d64 0264 068d 015a 0e65  .Z.e.j.d.d...Z.e
-00002e80: 036a 0765 0f83 0064 0264 0265 036a 0964  .j.e...d.d.e.j.d
-00002e90: 0764 088d 055a 1065 036a 1165 0f83 0064  .d...Z.e.j.e...d
-00002ea0: 0264 0764 098d 035a 1265 036a 0464 0a64  .d.d...Z.e.j.d.d
-00002eb0: 0264 0264 0b64 0c65 1383 0067 0164 0d8d  .d.d.d.e...g.d..
-00002ec0: 065a 1465 036a 1564 0264 0264 0e8d 025a  .Z.e.j.d.d.d...Z
-00002ed0: 1665 036a 1764 0f64 068d 015a 1864 1f65  .e.j.d.d...Z.d.e
-00002ee0: 1965 1965 1a65 1b19 0065 1a65 1b19 0064  .e.e.e...e.e...d
-00002ef0: 1164 129c 0587 0066 0164 1364 1484 0d5a  .d.....f.d.d...Z
-00002f00: 1c64 2065 1965 1d64 159c 0264 1664 1784  .d e.e.d...d.d..
-00002f10: 055a 1e65 1f64 189c 0164 1964 1a84 045a  .Z.e.d...d.d...Z
-00002f20: 2065 1f64 189c 0164 1b64 1c84 045a 2165   e.d...d.d...Z!e
-00002f30: 1f64 189c 0164 1d64 1e84 045a 2287 0004  .d...d.d...Z"...
-00002f40: 005a 2353 0029 21da 0652 6570 6f72 7472  .Z#S.)!..Reportr
-00002f50: 6700 0000 5472 f500 0000 7243 0000 0072  g...Tr....rC...r
-00002f60: 9600 0000 729a 0000 0072 6e00 0000 726f  ....r....rn...ro
-00002f70: 0000 00a9 0272 4500 0000 7271 0000 00e9  .....rE...rq....
-00002f80: 1e00 0000 7a2c 5265 6672 6573 6820 6576  ....z,Refresh ev
-00002f90: 6572 7920 2865 2e67 2e20 3320 2d20 312f  ery (e.g. 3 - 1/
-00002fa0: 3320 2d20 6d6f 6e20 2d20 312f 332c 4d6f  3 - mon - 1/3,Mo
-00002fb0: 6e29 7a1b 6d6f 6e2c 7475 652c 7765 642c  n)z.mon,tue,wed,
-00002fc0: 7468 752c 6672 692c 7361 742c 7375 6e29  thu,fri,sat,sun)
-00002fd0: 0672 4400 0000 7246 0000 0072 4500 0000  .rD...rF...rE...
-00002fe0: 72ee 0000 0072 6b00 0000 726c 0000 0072  r....rk...rl...r
-00002ff0: 9900 0000 696d 0100 0046 4e72 7700 0000  ....im...FNrw...
-00003000: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
-00003010: 0006 0000 0003 0000 0073 2400 0000 7c00  .........s$...|.
-00003020: 6a00 730e 7c00 6a01 7c00 5f00 7402 8300  j.s.|.j.|._.t...
-00003030: a003 7c01 7c02 7c03 7c04 a104 0100 6400  ..|.|.|.|.....d.
-00003040: 5300 7227 0000 0029 04da 0e64 6f63 756d  S.r'...)...docum
-00003050: 656e 745f 7469 746c 6572 7d00 0000 727e  ent_titler}...r~
-00003060: 0000 0072 7f00 0000 7280 0000 0072 8100  ...r....r....r..
-00003070: 0000 7228 0000 0072 2c00 0000 727f 0000  ..r(...r,...r...
-00003080: 0087 0100 0073 0600 0000 0007 0601 0801  .....s..........
-00003090: 7a0b 5265 706f 7274 2e73 6176 6529 02da  z.Report.save)..
-000030a0: 0972 756e 5f71 7565 7279 7230 0000 0063  .run_queryr0...c
-000030b0: 0200 0000 0000 0000 0000 0000 0b00 0000  ................
-000030c0: 0b00 0000 4300 0000 7322 0100 007c 006a  ....C...s"...|.j
-000030d0: 007d 0267 007d 037c 0172 167c 02a0 01a1  .}.g.}.|.r.|....
-000030e0: 0001 007c 026a 02a0 03a1 0044 005d e67d  ...|.j.....D.].}
-000030f0: 047c 046a 0473 2c71 207a 947c 046a 057d  .|.j.s,q z.|.j.}
-00003100: 057c 046a 0672 507c 05a0 0774 08a0 097c  .|.j.rP|...t...|
-00003110: 046a 06a1 0170 4c69 00a1 0101 007c 006a  .j...pLi.....|.j
-00003120: 0a72 607c 006a 0a7c 0516 006e 047c 006a  .r`|.j.|...n.|.j
-00003130: 0a7d 067c 006a 0ba0 0c7c 047c 007c 067c  .}.|.j...|.|.|.|
-00003140: 0564 019c 04a1 017d 0774 0d6a 0e6a 0f7c  .d.....}.t.j.j.|
-00003150: 007c 047c 067c 006a 0b6a 1074 08a0 117c  .|.|.|.j.j.t...|
-00003160: 07a1 017c 046a 0564 029c 0464 038d 035c  ...|.j.d...d...\
-00003170: 027d 087d 097c 03a0 127c 086a 1374 147c  .}.}.|...|.j.t.|
-00003180: 086a 1583 0166 02a1 0101 0057 0071 2004  .j...f.....W.q .
-00003190: 0074 1690 0179 0401 007d 0a01 007a 2a74  .t...y...}...z*t
-000031a0: 17a0 187c 0aa1 0101 007c 03a0 127c 046a  ...|.....|...|.j
-000031b0: 1374 197c 0a83 0166 02a1 0101 0057 0059  .t.|...f.....W.Y
-000031c0: 0064 007d 0a7e 0a71 2064 007d 0a7e 0a30  .d.}.~.q d.}.~.0
-000031d0: 0030 0071 2074 1aa0 1ba1 007c 005f 1c7c  .0.q t.....|._.|
-000031e0: 0390 0173 1e64 0467 017d 037c 0353 0029  ...s.d.g.}.|.S.)
-000031f0: 054e 2904 72c2 0000 00da 0672 6570 6f72  .N).r......repor
-00003200: 74da 0574 6974 6c65 72f9 0000 0029 0472  t..titler....).r
-00003210: 0601 0000 72fa 0000 00da 066f 7574 7075  ....r......outpu
-00003220: 7472 9d00 0000 2903 7205 0100 0072 c200  tr....).r....r..
-00003230: 0000 72d3 0000 007a 144e 6f20 4461 7461  ..r....z.No Data
-00003240: 7365 7420 6176 6169 6c61 626c 6529 1d72  set available).r
-00003250: a200 0000 72c4 0000 0072 bc00 0000 da03  ....r....r......
-00003260: 616c 6c72 f200 0000 729d 0000 0072 d100  allr....r....r..
-00003270: 0000 da06 7570 6461 7465 72dc 0000 0072  ....updater....r
-00003280: f000 0000 7203 0100 00da 0966 6f72 6d61  ....r......forma
-00003290: 7474 6572 72fc 0000 00da 0e52 6570 6f72  tterr......Repor
-000032a0: 7444 6f63 756d 656e 7472 a000 0000 72db  tDocumentr....r.
-000032b0: 0000 0072 fa00 0000 72dd 0000 00da 0661  ...r....r......a
-000032c0: 7070 656e 6472 b800 0000 72b9 0000 0072  ppendr....r....r
-000032d0: 0701 0000 723f 0000 0072 ba00 0000 72bb  ....r?...r....r.
-000032e0: 0000 0072 5000 0000 7212 0000 0072 a800  ...rP...r....r..
-000032f0: 0000 72a9 0000 0029 0b72 5100 0000 7204  ..r....).rQ...r.
-00003300: 0100 0072 a200 0000 7252 0000 0072 c200  ...r....rR...r..
-00003310: 0000 72f9 0000 0072 0601 0000 7207 0100  ..r....r....r...
-00003320: 0072 e600 0000 7287 0000 0072 3500 0000  .r....r....r5...
-00003330: 7228 0000 0072 2800 0000 722c 0000 00da  r(...r(...r,....
-00003340: 0765 7865 6375 7465 9201 0000 734e 0000  .execute....sN..
-00003350: 0000 0206 0104 0104 0108 010e 0106 0102  ................
-00003360: 0102 0106 0106 0116 0404 ff0c 0204 fd02  ................
-00003370: 0506 0202 0102 0102 0102 fc04 ff04 0806  ................
-00003380: 0102 0102 0202 0106 0108 0104 fc04 fd0a  ................
-00003390: 0a1a 0110 010a 012c 010a 0106 0106 017a  .......,.......z
-000033a0: 0e52 6570 6f72 742e 6578 6563 7574 6572  .Report.executer
-000033b0: 4c00 0000 6301 0000 0000 0000 0000 0000  L...c...........
-000033c0: 0001 0000 0001 0000 0043 0000 0073 0a00  .........C...s..
-000033d0: 0000 7c00 6a00 7008 6401 5300 725d 0000  ..|.j.p.d.S.r]..
-000033e0: 0072 8900 0000 7258 0000 0072 2800 0000  .r....rX...r(...
-000033f0: 7228 0000 0072 2c00 0000 728a 0000 00c0  r(...r,...r.....
-00003400: 0100 0073 0200 0000 0001 7a0e 5265 706f  ...s......z.Repo
-00003410: 7274 2e5f 5f73 7472 5f5f 6301 0000 0000  rt.__str__c.....
-00003420: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00003430: 0000 0073 1000 0000 7400 6401 7c00 6a01  ...s....t.d.|.j.
-00003440: 6701 6402 8d02 5300 2903 4e7a 1270 6f77  g.d...S.).Nz.pow
-00003450: 6572 5f71 7565 7279 3a72 6570 6f72 74a9  er_query:report.
-00003460: 0172 bf00 0000 2902 7211 0000 0072 b800  .r....).r....r..
-00003470: 0000 7258 0000 0072 2800 0000 7228 0000  ..rX...r(...r(..
-00003480: 0072 2c00 0000 da10 6765 745f 6162 736f  .r,.....get_abso
-00003490: 6c75 7465 5f75 726c c301 0000 7302 0000  lute_url....s...
-000034a0: 0000 017a 1752 6570 6f72 742e 6765 745f  ...z.Report.get_
-000034b0: 6162 736f 6c75 7465 5f75 726c 6301 0000  absolute_urlc...
-000034c0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-000034d0: 0043 0000 0073 2e00 0000 6401 6402 6c00  .C...s....d.d.l.
-000034e0: 6d01 7d01 0100 7c01 a002 7c00 6a03 a101  m.}...|...|.j...
-000034f0: 7d02 7c02 6a03 7c00 5f04 7c00 a005 a100  }.|.j.|._.|.....
-00003500: 0100 7c02 6a03 5300 2903 4e72 0100 0000  ..|.j.S.).Nr....
-00003510: 2901 da0e 7265 6672 6573 685f 7265 706f  )...refresh_repo
-00003520: 7274 2906 72e4 0000 0072 1001 0000 72e5  rt).r....r....r.
-00003530: 0000 0072 9e00 0000 724d 0000 0072 7f00  ...r....rM...r..
-00003540: 0000 2903 7251 0000 0072 1001 0000 72e6  ..).rQ...r....r.
-00003550: 0000 0072 2800 0000 7228 0000 0072 2c00  ...r(...r(...r,.
-00003560: 0000 7259 0000 00c6 0100 0073 0a00 0000  ..rY.......s....
-00003570: 0001 0c02 0c01 0801 0801 7a0d 5265 706f  ..........z.Repo
-00003580: 7274 2e5f 7175 6575 6529 0446 464e 4e29  rt._queue).FFNN)
-00003590: 0146 2924 7247 0000 0072 4800 0000 7249  .F)$rG...rH...rI
-000035a0: 0000 0072 0c00 0000 7264 0000 0072 7d00  ...r....rd...r}.
-000035b0: 0000 7203 0100 0072 9000 0000 726d 0000  ..r....r....rm..
-000035c0: 0072 9100 0000 72a2 0000 0072 f400 0000  .r....r....r....
-000035d0: 720a 0100 0072 8e00 0000 72e8 0000 0072  r....r....r....r
-000035e0: 0900 0000 72cd 0000 00da 0f4d 616e 7954  ....r......ManyT
-000035f0: 6f4d 616e 7946 6965 6c64 da0f 6c69 6d69  oManyField..limi
-00003600: 745f 6163 6365 7373 5f74 6f72 1f00 0000  t_access_tor....
-00003610: 5a09 6672 6571 7565 6e63 6572 e700 0000  Z.frequencer....
-00003620: 72a9 0000 00da 0c49 6e74 6567 6572 4669  r......IntegerFi
-00003630: 656c 645a 0d76 616c 6964 6974 795f 6461  eldZ.validity_da
-00003640: 7973 7292 0000 0072 0500 0000 7202 0000  ysr....r....r...
-00003650: 0072 7f00 0000 da0c 5265 706f 7274 5265  .r......ReportRe
-00003660: 7375 6c74 720d 0100 0072 5000 0000 728a  sultr....rP...r.
-00003670: 0000 0072 0f01 0000 7259 0000 0072 9300  ...r....rY...r..
-00003680: 0000 7228 0000 0072 2800 0000 7281 0000  ..r(...r(...r...
-00003690: 0072 2c00 0000 7200 0100 006c 0100 0073  .r,...r....l...s
-000036a0: 5000 0000 0801 1201 1001 1001 1001 0c01  P...............
-000036b0: 0401 0401 0201 0201 0401 02fb 0607 0401  ................
-000036c0: 08ff 0603 0401 0201 0201 0201 0201 0201  ................
-000036d0: 06fa 0608 0e01 0c04 0001 0001 0001 00fb  ................
-000036e0: 0202 0201 0201 0601 0601 02fa 100b 122e  ................
-000036f0: 0e03 0e03 7200 0100 0063 0000 0000 0000  ....r....c......
-00003700: 0000 0000 0000 0000 0000 0400 0000 0000  ................
-00003710: 0000 7324 0000 0065 005a 0164 005a 0265  ..s$...e.Z.d.Z.e
-00003720: 036a 0464 019c 0187 0066 0164 0264 0384  .j.d.....f.d.d..
-00003730: 0c5a 0587 0004 005a 0653 0029 04da 1552  .Z.....Z.S.)...R
-00003740: 6570 6f72 7444 6f63 756d 656e 744d 616e  eportDocumentMan
-00003750: 6167 6572 724c 0000 0063 0100 0000 0000  agerrL...c......
-00003760: 0000 0000 0000 0100 0000 0300 0000 0300  ................
-00003770: 0000 7310 0000 0074 0083 00a0 01a1 00a0  ..s....t........
-00003780: 0264 01a1 0153 0029 024e 7205 0100 0029  .d...S.).Nr....)
-00003790: 0372 7e00 0000 da0c 6765 745f 7175 6572  .r~.....get_quer
-000037a0: 7973 6574 da0e 7365 6c65 6374 5f72 656c  yset..select_rel
-000037b0: 6174 6564 7258 0000 0072 8100 0000 7228  atedrX...r....r(
-000037c0: 0000 0072 2c00 0000 7216 0100 00d0 0100  ...r,...r.......
-000037d0: 0073 0200 0000 0001 7a22 5265 706f 7274  .s......z"Report
-000037e0: 446f 6375 6d65 6e74 4d61 6e61 6765 722e  DocumentManager.
-000037f0: 6765 745f 7175 6572 7973 6574 2907 7247  get_queryset).rG
-00003800: 0000 0072 4800 0000 7249 0000 0072 0c00  ...rH...rI...r..
-00003810: 0000 da08 5175 6572 7953 6574 7216 0100  ....QuerySetr...
-00003820: 0072 9300 0000 7228 0000 0072 2800 0000  .r....r(...r(...
-00003830: 7281 0000 0072 2c00 0000 7215 0100 00cf  r....r,...r.....
-00003840: 0100 0073 0200 0000 0801 7215 0100 0063  ...s......r....c
-00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003860: 0500 0000 4000 0000 73d6 0000 0065 005a  ....@...s....e.Z
-00003870: 0164 005a 0265 036a 0464 0164 028d 015a  .d.Z.e.j.d.d...Z
-00003880: 0565 036a 0664 0364 048d 015a 0765 036a  .e.j.d.d...Z.e.j
-00003890: 0865 0965 036a 0a64 0564 068d 035a 0b65  .e.e.j.d.d...Z.e
-000038a0: 036a 0865 0c65 036a 0a64 078d 025a 0d65  .j.e.e.j.d...Z.e
-000038b0: 036a 0e64 0164 0164 088d 025a 0f65 036a  .j.d.d.d...Z.e.j
-000038c0: 1065 1165 1264 098d 025a 1365 036a 1465  .e.e.d...Z.e.j.e
-000038d0: 1583 0064 0164 0a64 0b8d 035a 1665 036a  ...d.d.d...Z.e.j
-000038e0: 0664 0c65 1764 0d8d 025a 1865 1983 005a  .d.e.d...Z.e...Z
-000038f0: 1a47 0064 0e64 0f84 0064 0f83 025a 1b65  .G.d.d...d...Z.e
-00003900: 1c64 109c 0164 1164 1284 045a 1d65 1e65  .d...d.d...Z.e.e
-00003910: 1f64 109c 0164 1364 1484 0483 015a 2065  .d...d.d.....Z e
-00003920: 1e65 2164 109c 0164 1564 1684 0483 015a  .e!d...d.d.....Z
-00003930: 2265 1c64 109c 0164 1764 1884 045a 2364  "e.d...d.d...Z#d
-00003940: 1953 0029 1a72 0b01 0000 5429 01da 0861  .S.).r....T)...a
-00003950: 7574 6f5f 6e6f 7769 2c01 0000 72ed 0000  uto_nowi,...r...
-00003960: 00da 0964 6f63 756d 656e 7473 7295 0000  ...documentsr...
-00003970: 0072 9600 0000 7299 0000 0029 0272 6b00  .r....r....).rk.
-00003980: 0000 7298 0000 0072 6e00 0000 7201 0100  ..r....rn...r...
-00003990: 0072 f600 0000 72f7 0000 0063 0000 0000  .r....r....c....
-000039a0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-000039b0: 4000 0000 7310 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-000039c0: 0264 015a 0364 0253 0029 037a 1352 6570  .d.Z.d.S.).z.Rep
-000039d0: 6f72 7444 6f63 756d 656e 742e 4d65 7461  ortDocument.Meta
-000039e0: 2902 7205 0100 0072 c200 0000 4e29 0472  ).r....r....N).r
-000039f0: 4700 0000 7248 0000 0072 4900 0000 da0f  G...rH...rI.....
-00003a00: 756e 6971 7565 5f74 6f67 6574 6865 7272  unique_togetherr
-00003a10: 2800 0000 7228 0000 0072 2800 0000 722c  (...r(...r(...r,
-00003a20: 0000 0072 4b00 0000 e401 0000 7302 0000  ...rK.......s...
-00003a30: 0008 0172 4b00 0000 724c 0000 0063 0100  ...rK...rL...c..
-00003a40: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00003a50: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
-00003a60: 0072 2700 0000 2901 7206 0100 0072 5800  .r'...).r....rX.
-00003a70: 0000 7228 0000 0072 2800 0000 722c 0000  ..r(...r(...r,..
-00003a80: 0072 8a00 0000 e701 0000 7302 0000 0000  .r........s.....
-00003a90: 017a 1652 6570 6f72 7444 6f63 756d 656e  .z.ReportDocumen
-00003aa0: 742e 5f5f 7374 725f 5f63 0100 0000 0000  t.__str__c......
-00003ab0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00003ac0: 0000 730c 0000 0074 00a0 017c 006a 02a1  ..s....t...|.j..
-00003ad0: 0153 0072 2700 0000 2903 72dc 0000 0072  .S.r'...).r....r
-00003ae0: f000 0000 7207 0100 0072 5800 0000 7228  ....r....rX...r(
-00003af0: 0000 0072 2800 0000 722c 0000 0072 f100  ...r(...r,...r..
-00003b00: 0000 ea01 0000 7302 0000 0000 027a 1352  ......s......z.R
-00003b10: 6570 6f72 7444 6f63 756d 656e 742e 6461  eportDocument.da
-00003b20: 7461 6301 0000 0000 0000 0000 0000 0001  tac.............
-00003b30: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00003b40: 7400 7c00 6a01 8301 5300 7227 0000 0029  t.|.j...S.r'...)
-00003b50: 0272 b900 0000 7207 0100 0072 5800 0000  .r....r....rX...
-00003b60: 7228 0000 0072 2800 0000 722c 0000 0072  r(...r(...r,...r
-00003b70: f200 0000 ee01 0000 7302 0000 0000 027a  ........s......z
-00003b80: 1352 6570 6f72 7444 6f63 756d 656e 742e  .ReportDocument.
-00003b90: 7369 7a65 6301 0000 0000 0000 0000 0000  sizec...........
-00003ba0: 0001 0000 0004 0000 0043 0000 0073 1600  .........C...s..
-00003bb0: 0000 7400 6401 7c00 6a01 6a02 7c00 6a02  ..t.d.|.j.j.|.j.
-00003bc0: 6702 6402 8d02 5300 2903 4e7a 1470 6f77  g.d...S.).Nz.pow
-00003bd0: 6572 5f71 7565 7279 3a64 6f63 756d 656e  er_query:documen
-00003be0: 7472 0e01 0000 2903 7211 0000 0072 0501  tr....).r....r..
-00003bf0: 0000 72b8 0000 0072 5800 0000 7228 0000  ..r....rX...r(..
-00003c00: 0072 2800 0000 722c 0000 0072 0f01 0000  .r(...r,...r....
-00003c10: f201 0000 7302 0000 0000 017a 1f52 6570  ....s......z.Rep
-00003c20: 6f72 7444 6f63 756d 656e 742e 6765 745f  ortDocument.get_
-00003c30: 6162 736f 6c75 7465 5f75 726c 4e29 2472  absolute_urlN)$r
-00003c40: 4700 0000 7248 0000 0072 4900 0000 720c  G...rH...rI...r.
-00003c50: 0000 0072 e700 0000 72ac 0000 0072 6400  ...r....r....rd.
-00003c60: 0000 7206 0100 0072 9000 0000 7200 0100  ..r....r....r...
-00003c70: 0072 9100 0000 7205 0100 0072 b700 0000  .r....r....r....
-00003c80: 72c2 0000 0072 f300 0000 7207 0100 0072  r....r....r....r
-00003c90: 0e00 0000 7231 0000 0072 1c00 0000 729d  ....r1...r....r.
-00003ca0: 0000 0072 1101 0000 7209 0000 0072 1201  ...r....r....r..
-00003cb0: 0000 72ff 0000 0072 fa00 0000 7215 0100  ..r....r....r...
-00003cc0: 0072 a000 0000 724b 0000 0072 5000 0000  .r....rK...rP...
-00003cd0: 728a 0000 0072 1400 0000 7202 0000 0072  r....r....r....r
-00003ce0: f100 0000 72b0 0000 0072 f200 0000 720f  ....r....r....r.
-00003cf0: 0100 0072 2800 0000 7228 0000 0072 2800  ...r(...r(...r(.
-00003d00: 0000 722c 0000 0072 0b01 0000 d401 0000  ..r,...r........
-00003d10: 7328 0000 0008 010c 010c 0104 0108 ff06  s(..............
-00003d20: 0310 010e 010e 0104 0108 ff06 030e 0206  ................
-00003d30: 020e 030e 0302 0110 0302 0110 0372 0b01  .............r..
-00003d40: 0000 294d 723c 0000 00da 076c 6f67 6769  ..)Mr<.....loggi
-00003d50: 6e67 72dc 0000 00da 0674 7970 696e 6772  ngr......typingr
-00003d60: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
-00003d70: 0000 0072 0600 0000 7207 0000 00da 0b64  ...r....r......d
-00003d80: 6a61 6e67 6f2e 636f 6e66 7208 0000 00da  jango.confr.....
-00003d90: 1364 6a61 6e67 6f2e 636f 6e74 7269 622e  .django.contrib.
-00003da0: 6175 7468 7209 0000 00da 2264 6a61 6e67  authr....."djang
-00003db0: 6f2e 636f 6e74 7269 622e 636f 6e74 656e  o.contrib.conten
-00003dc0: 7474 7970 6573 2e6d 6f64 656c 7372 0a00  ttypes.modelsr..
-00003dd0: 0000 da16 646a 616e 676f 2e63 6f72 652e  ....django.core.
-00003de0: 6578 6365 7074 696f 6e73 720b 0000 00da  exceptionsr.....
-00003df0: 0964 6a61 6e67 6f2e 6462 720c 0000 0072  .django.dbr....r
-00003e00: 0d00 0000 da10 646a 616e 676f 2e64 622e  ......django.db.
-00003e10: 6d6f 6465 6c73 720e 0000 00da 0f64 6a61  modelsr......dja
-00003e20: 6e67 6f2e 7465 6d70 6c61 7465 720f 0000  ngo.templater...
-00003e30: 0072 1000 0000 da0b 646a 616e 676f 2e75  .r......django.u
-00003e40: 726c 7372 1100 0000 da0c 646a 616e 676f  rlsr......django
-00003e50: 2e75 7469 6c73 7212 0000 005a 1a64 6a61  .utilsr....Z.dja
-00003e60: 6e67 6f2e 7574 696c 732e 6461 7465 7469  ngo.utils.dateti
-00003e70: 6d65 5f73 6166 6572 1300 0000 da17 646a  me_safer......dj
-00003e80: 616e 676f 2e75 7469 6c73 2e66 756e 6374  ango.utils.funct
-00003e90: 696f 6e61 6c72 1400 0000 da11 646a 616e  ionalr......djan
-00003ea0: 676f 2e75 7469 6c73 2e74 6578 7472 1500  go.utils.textr..
-00003eb0: 0000 7256 0000 0072 1600 0000 da0d 6365  ..rV...r......ce
-00003ec0: 6c65 7279 2e72 6573 756c 7472 1700 0000  lery.resultr....
-00003ed0: da0c 6e61 7475 7261 6c5f 6b65 7973 7218  ..natural_keysr.
-00003ee0: 0000 00da 0a73 656e 7472 795f 7364 6b72  .....sentry_sdkr
-00003ef0: 1900 0000 721a 0000 005a 1670 6f77 6572  ....r....Z.power
-00003f00: 5f71 7565 7279 2e65 7863 6570 7469 6f6e  _query.exception
-00003f10: 7372 1b00 0000 5a10 706f 7765 725f 7175  sr....Z.power_qu
-00003f20: 6572 792e 6a73 6f6e 721c 0000 005a 1170  ery.jsonr....Z.p
-00003f30: 6f77 6572 5f71 7565 7279 2e75 7469 6c73  ower_query.utils
-00003f40: 721d 0000 0072 1e00 0000 5a16 706f 7765  r....r....Z.powe
-00003f50: 725f 7175 6572 792e 7661 6c69 6461 746f  r_query.validato
-00003f60: 7273 721f 0000 00da 0967 6574 4c6f 6767  rsr......getLogg
-00003f70: 6572 7247 0000 0072 ba00 0000 5a0c 6d69  errG...r....Z.mi
-00003f80: 6d65 7479 7065 5f6d 6170 da05 6974 656d  metype_map..item
-00003f90: 7372 ff00 0000 72b0 0000 0072 5000 0000  sr....r....rP...
-00003fa0: 5a0e 446f 6375 6d65 6e74 5265 7375 6c74  Z.DocumentResult
-00003fb0: 7214 0100 0072 ea00 0000 72e9 0000 0072  r....r....r....r
-00003fc0: 4000 0000 da05 4d6f 6465 6c72 4100 0000  @.....ModelrA...
-00003fd0: 7266 0000 0072 6d00 0000 72b7 0000 0072  rf...rm...r....r
-00003fe0: f400 0000 7200 0100 0072 c500 0000 7215  ....r....r....r.
-00003ff0: 0100 0072 0b01 0000 7228 0000 0072 2800  ...r....r(...r(.
-00004000: 0000 7228 0000 0072 2c00 0000 da08 3c6d  ..r(...r,.....<m
-00004010: 6f64 756c 653e 0100 0000 7360 0000 0008  odule>....s`....
-00004020: 0108 0108 0120 020c 010c 010c 010c 0110  ..... ..........
-00004030: 010c 0110 010c 010c 010c 010c 010c 0208  ................
-00004040: 010c 010c 010c 0110 020c 010c 0110 010c  ................
-00004050: 020a 0302 0102 0102 0102 0102 0102 0102  ................
-00004060: f906 0a12 0214 0112 010c 0114 0310 0f12  ................
-00004070: 2714 2e16 7f00 2114 1b14 1b16 6312 05    '.....!.....c..
+00000060: 6d09 5a09 0100 6400 6403 6c0a 6d0b 5a0c  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6404 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6405 6c0f 6d10 5a10 0100 6400 6406 6c11  d.l.m.Z...d.d.l.
+00000090: 6d12 5a12 0100 6400 6407 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
+000000a0: 0100 6400 6408 6c15 6d16 5a16 6d17 5a17  ..d.d.l.m.Z.m.Z.
+000000b0: 0100 6400 6409 6c18 6d19 5a19 0100 6400  ..d.d.l.m.Z...d.
+000000c0: 640a 6c1a 6d1b 5a1b 6d1c 5a1c 0100 6400  d.l.m.Z.m.Z...d.
+000000d0: 640b 6c1d 6d1e 5a1e 0100 6400 640c 6c1f  d.l.m.Z...d.d.l.
+000000e0: 6d20 5a20 0100 6400 640d 6c21 6d22 5a22  m Z ..d.d.l!m"Z"
+000000f0: 0100 6400 640e 6c23 6d24 5a24 0100 6400  ..d.d.l#m$Z$..d.
+00000100: 640f 6c25 6d26 5a26 0100 6400 6401 6c27  d.l%m&Z&..d.d.l'
+00000110: 5a27 6400 6410 6c27 6d28 5a28 0100 6400  Z'd.d.l'm(Z(..d.
+00000120: 6411 6c29 6d2a 5a2a 0100 6400 6412 6c2b  d.l)m*Z*..d.d.l+
+00000130: 6d2c 5a2c 0100 6400 6413 6c2d 6d2e 5a2e  m,Z,..d.d.l-m.Z.
+00000140: 6d2f 5a2f 0100 6400 6414 6c30 6d31 5a31  m/Z/..d.d.l0m1Z1
+00000150: 0100 6400 6415 6c32 6d33 5a33 0100 6400  ..d.d.l2m3Z3..d.
+00000160: 6416 6c34 6d35 5a35 6d36 5a36 0100 6400  d.l4m5Z5m6Z6..d.
+00000170: 6417 6c37 6d38 5a38 0100 6501 a039 653a  d.l7m8Z8..e..9e:
+00000180: a101 5a3b 6418 6419 641a 641b 641c 641d  ..Z;d.d.d.d.d.d.
+00000190: 641e 641f 9c07 5a3c 6420 6421 8400 653c  d.d...Z<d d!..e<
+000001a0: a03d a100 4400 8301 5a3e 6508 653f 6509  .=..D...Z>e.e?e.
+000001b0: 6540 653f 6602 1900 6602 1900 5a41 6506  e@e?f...f...ZAe.
+000001c0: 6509 6541 6504 6540 6603 1900 1900 5a42  e.eAe.e@f.....ZB
+000001d0: 6508 6504 6504 6602 1900 5a43 6505 6540  e.e.e.f...ZCe.e@
+000001e0: 6509 653f 6540 6602 1900 6602 1900 5a44  e.e?e@f...f...ZD
+000001f0: 6504 6401 6422 9c02 6423 6424 8404 5a45  e.d.d"..d#d$..ZE
+00000200: 4700 6425 6426 8400 6426 6516 6a46 8303  G.d%d&..d&e.jF..
+00000210: 5a47 4700 6427 6428 8400 6428 652c 6516  ZGG.d'd(..d(e,e.
+00000220: 6a46 8304 5a48 4700 6429 642a 8400 642a  jF..ZHG.d)d*..d*
+00000230: 652c 6547 6516 6a46 8305 5a49 4700 642b  e,eGe.jF..ZIG.d+
+00000240: 642c 8400 642c 652c 6516 6a46 8304 5a4a  d,..d,e,e.jF..ZJ
+00000250: 4700 642d 642e 8400 642e 652c 6516 6a46  G.d-d...d.e,e.jF
+00000260: 8304 5a4b 4700 642f 6430 8400 6430 652c  ..ZKG.d/d0..d0e,
+00000270: 6547 6516 6a46 8305 5a4c 4700 6431 6432  eGe.jF..ZLG.d1d2
+00000280: 8400 6432 6516 6a4d 8303 5a4e 4700 6433  ..d2e.jM..ZNG.d3
+00000290: 6434 8400 6434 6516 6a46 8303 5a4f 6401  d4..d4e.jF..ZOd.
+000002a0: 5300 2935 e900 0000 004e 2906 da03 416e  S.)5.....N)...An
+000002b0: 79da 0444 6963 74da 044c 6973 74da 084f  y..Dict..List..O
+000002c0: 7074 696f 6e61 6cda 0554 7570 6c65 da05  ptional..Tuple..
+000002d0: 556e 696f 6e29 01da 0461 7070 7329 01da  Union)...apps)..
+000002e0: 0873 6574 7469 6e67 7329 01da 0e67 6574  .settings)...get
+000002f0: 5f75 7365 725f 6d6f 6465 6c29 01da 0b43  _user_model)...C
+00000300: 6f6e 7465 6e74 5479 7065 2901 da0f 5661  ontentType)...Va
+00000310: 6c69 6461 7469 6f6e 4572 726f 7229 02da  lidationError)..
+00000320: 066d 6f64 656c 73da 0b74 7261 6e73 6163  .models..transac
+00000330: 7469 6f6e 2901 da09 4a53 4f4e 4669 656c  tion)...JSONFiel
+00000340: 6429 02da 0743 6f6e 7465 7874 da08 5465  d)...Context..Te
+00000350: 6d70 6c61 7465 2901 da07 7265 7665 7273  mplate)...revers
+00000360: 6529 01da 0874 696d 657a 6f6e 6529 01da  e)...timezone)..
+00000370: 0873 7472 6674 696d 6529 01da 0f63 6163  .strftime)...cac
+00000380: 6865 645f 7072 6f70 6572 7479 2901 da07  hed_property)...
+00000390: 736c 7567 6966 7929 01da 0673 7461 7465  slugify)...state
+000003a0: 7329 01da 0b41 7379 6e63 5265 7375 6c74  s)...AsyncResult
+000003b0: 2901 da0f 4e61 7475 7261 6c4b 6579 4d6f  )...NaturalKeyMo
+000003c0: 6465 6c29 02da 1163 6170 7475 7265 5f65  del)...capture_e
+000003d0: 7863 6570 7469 6f6e da0f 636f 6e66 6967  xception..config
+000003e0: 7572 655f 7363 6f70 6529 01da 0d51 7565  ure_scope)...Que
+000003f0: 7279 5275 6e45 7272 6f72 2901 da0d 5051  ryRunError)...PQ
+00000400: 4a53 4f4e 456e 636f 6465 7229 02da 0964  JSONEncoder)...d
+00000410: 6963 745f 6861 7368 da0a 746f 5f64 6174  ict_hash..to_dat
+00000420: 6173 6574 2901 da12 4672 6571 7565 6e63  aset)...Frequenc
+00000430: 7956 616c 6964 6174 6f72 7a08 7465 7874  yValidatorz.text
+00000440: 2f63 7376 7a09 7465 7874 2f68 746d 6c7a  /csvz.text/htmlz
+00000450: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00000460: 6e7a 0a74 6578 742f 706c 6169 6e7a 1861  nz.text/plainz.a
+00000470: 7070 6c69 6361 7469 6f6e 2f76 6e64 2e6d  pplication/vnd.m
+00000480: 732d 6578 6365 6c7a 0f61 7070 6c69 6361  s-excelz.applica
+00000490: 7469 6f6e 2f78 6d6c 7a09 7465 7874 2f79  tion/xmlz.text/y
+000004a0: 616d 6c29 07da 0363 7376 da04 6874 6d6c  aml)...csv..html
+000004b0: da04 6a73 6f6e da03 7478 74da 0378 6c73  ..json..txt..xls
+000004c0: da03 786d 6cda 0479 616d 6c63 0100 0000  ..xml..yamlc....
+000004d0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000004e0: 6300 0000 731a 0000 007c 005d 125c 027d  c...s....|.].\.}
+000004f0: 017d 027c 017c 0266 0256 0001 0071 0264  .}.|.|.f.V...q.d
+00000500: 0053 00a9 014e a900 2903 da02 2e30 da01  .S...N..)....0..
+00000510: 6bda 0176 7229 0000 0072 2900 0000 fa42  k..vr)...r)....B
+00000520: 2f55 7365 7273 2f6a 6f6a 6f2f 776f 726b  /Users/jojo/work
+00000530: 7370 6163 652f 756e 6963 6566 2d70 6f77  space/unicef-pow
+00000540: 6572 2d71 7565 7279 2f73 7263 2f70 6f77  er-query/src/pow
+00000550: 6572 5f71 7565 7279 2f6d 6f64 656c 732e  er_query/models.
+00000560: 7079 da09 3c67 656e 6578 7072 3e2b 0000  py..<genexpr>+..
+00000570: 00f3 0000 0000 722e 0000 0029 02da 0576  ......r....)...v
+00000580: 616c 7565 da06 7265 7475 726e 6301 0000  alue..returnc...
+00000590: 0000 0000 0000 0000 0003 0000 000a 0000  ................
+000005a0: 0003 0000 0073 8800 0000 7a3a 7400 8800  .....s....z:t...
+000005b0: 7401 8302 7314 7402 6401 8301 8201 7403  t...s.t.d.....t.
+000005c0: 7404 6a05 8800 a006 a100 8e00 8301 7d01  t.j...........}.
+000005d0: 8700 6601 6402 6403 8408 7c01 4400 8301  ..f.d.d...|.D...
+000005e0: 0100 5700 6e48 0400 7402 794e 0100 0100  ..W.nH..t.yN....
+000005f0: 0100 8200 5900 6e36 0400 7407 7982 0100  ....Y.n6..t.y...
+00000600: 7d02 0100 7a1e 7402 6404 8800 7c02 6405  }...z.t.d...|.d.
+00000610: 9c02 6406 8d02 8201 5700 5900 6400 7d02  ..d.....W.Y.d.}.
+00000620: 7e02 6e0a 6400 7d02 7e02 3000 3000 6400  ~.n.d.}.~.0.0.d.
+00000630: 5300 2907 4e7a 1851 7565 7279 4172 6773  S.).Nz.QueryArgs
+00000640: 206d 7573 7420 6265 2061 2064 6963 7463   must be a dictc
+00000650: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000660: 0600 0000 1300 0000 731e 0000 0067 007c  ........s....g.|
+00000670: 005d 167d 0174 0074 0188 00a0 02a1 007c  .].}.t.t.......|
+00000680: 0183 0283 0191 0271 0453 0072 2900 0000  .......q.S.r)...
+00000690: 2903 da04 6469 6374 da03 7a69 70da 046b  )...dict..zip..k
+000006a0: 6579 73a9 0272 2a00 0000 da01 65a9 0172  eys..r*.....e..r
+000006b0: 3000 0000 7229 0000 0072 2d00 0000 da0a  0...r)...r-.....
+000006c0: 3c6c 6973 7463 6f6d 703e 3800 0000 722f  <listcomp>8...r/
+000006d0: 0000 007a 2676 616c 6964 6174 655f 7175  ...z&validate_qu
+000006e0: 6572 7961 7267 732e 3c6c 6f63 616c 733e  eryargs.<locals>
+000006f0: 2e3c 6c69 7374 636f 6d70 3e7a 2b25 2865  .<listcomp>z+%(e
+00000700: 7863 2973 3a20 2528 7661 6c75 6529 7320  xc)s: %(value)s 
+00000710: 6973 206e 6f74 2061 2076 616c 6964 2051  is not a valid Q
+00000720: 7565 7279 4172 6773 2902 7230 0000 00da  ueryArgs).r0....
+00000730: 0365 7863 2901 da06 7061 7261 6d73 2908  .exc)...params).
+00000740: da0a 6973 696e 7374 616e 6365 7232 0000  ..isinstancer2..
+00000750: 0072 0c00 0000 da04 6c69 7374 da09 6974  .r......list..it
+00000760: 6572 746f 6f6c 73da 0770 726f 6475 6374  ertools..product
+00000770: da06 7661 6c75 6573 da09 4578 6365 7074  ..values..Except
+00000780: 696f 6e29 0372 3000 0000 723e 0000 0072  ion).r0...r>...r
+00000790: 3600 0000 7229 0000 0072 3700 0000 722d  6...r)...r7...r-
+000007a0: 0000 00da 1276 616c 6964 6174 655f 7175  .....validate_qu
+000007b0: 6572 7961 7267 7333 0000 0073 1800 0000  eryargs3...s....
+000007c0: 0001 0201 0a01 0801 1201 1601 0c01 0601  ................
+000007d0: 0e01 0201 0201 08fe 7241 0000 0063 0000  ........rA...c..
+000007e0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+000007f0: 0000 4000 0000 7386 0000 0065 005a 0164  ..@...s....e.Z.d
+00000800: 005a 0265 0365 046a 0565 046a 0665 046a  .Z.e.e.j.e.j.e.j
+00000810: 0765 046a 0868 0483 015a 0965 0a6a 0b64  .e.j.h...Z.e.j.d
+00000820: 0164 0264 0264 038d 035a 0c47 0064 0464  .d.d.d...Z.G.d.d
+00000830: 0584 0064 0583 025a 0d65 0e64 069c 0164  ...d...Z.e.d...d
+00000840: 0764 0884 045a 0f65 1065 1165 1219 0064  .d...Z.e.e.e...d
+00000850: 069c 0164 0964 0a84 0483 015a 1365 1165  ...d.d.....Z.e.e
+00000860: 0e19 0064 069c 0164 0b64 0c84 045a 1465  ...d...d.d...Z.e
+00000870: 0e64 069c 0164 0d64 0e84 045a 1564 0f53  .d...d.d...Z.d.S
+00000880: 0029 10da 0d43 656c 6572 7945 6e61 626c  .)...CeleryEnabl
+00000890: 6564 e924 0000 0054 a903 da0a 6d61 785f  ed.$...T....max_
+000008a0: 6c65 6e67 7468 da05 626c 616e 6bda 046e  length..blank..n
+000008b0: 756c 6c63 0000 0000 0000 0000 0000 0000  ullc............
+000008c0: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
+000008d0: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
+000008e0: 0029 037a 1243 656c 6572 7945 6e61 626c  .).z.CeleryEnabl
+000008f0: 6564 2e4d 6574 6154 4e29 04da 085f 5f6e  ed.MetaTN)...__n
+00000900: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000910: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000920: 0861 6273 7472 6163 7472 2900 0000 7229  .abstractr)...r)
+00000930: 0000 0072 2900 0000 722d 0000 00da 044d  ...r)...r-.....M
+00000940: 6574 6149 0000 0073 0200 0000 0801 724c  etaI...s......rL
+00000950: 0000 00a9 0172 3100 0000 6301 0000 0000  .....r1...c.....
+00000960: 0000 0000 0000 0003 0000 000a 0000 0043  ...............C
+00000970: 0000 0073 4a00 0000 7c00 6a00 7242 7a0c  ...sJ...|.j.rBz.
+00000980: 7c00 6a01 6a02 7d01 5700 7146 0400 7403  |.j.j.}.W.qF..t.
+00000990: 793e 0100 7d02 0100 7a14 7404 7c02 8301  y>..}...z.t.|...
+000009a0: 7d01 5700 5900 6400 7d02 7e02 7146 6400  }.W.Y.d.}.~.qFd.
+000009b0: 7d02 7e02 3000 3000 6e04 6401 7d01 7c01  }.~.0.0.n.d.}.|.
+000009c0: 5300 2902 4e7a 0d4e 6f74 2073 6368 6564  S.).Nz.Not sched
+000009d0: 756c 6564 2905 da0b 6365 6c65 7279 5f74  uled)...celery_t
+000009e0: 6173 6bda 0c61 7379 6e63 5f72 6573 756c  ask..async_resul
+000009f0: 74da 0573 7461 7465 7240 0000 00da 0373  t..stater@.....s
+00000a00: 7472 2903 da04 7365 6c66 da06 7265 7375  tr)...self..resu
+00000a10: 6c74 7236 0000 0072 2900 0000 7229 0000  ltr6...r)...r)..
+00000a20: 0072 2d00 0000 da06 7374 6174 7573 4c00  .r-.....statusL.
+00000a30: 0000 730e 0000 0000 0106 0102 010c 010e  ..s.............
+00000a40: 0120 0204 017a 1443 656c 6572 7945 6e61  . ...z.CeleryEna
+00000a50: 626c 6564 2e73 7461 7475 7363 0100 0000  bled.statusc....
+00000a60: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000a70: 4300 0000 732a 0000 007c 006a 0072 227c  C...s*...|.j.r"|
+00000a80: 006a 017c 006a 0276 0172 2274 037c 006a  .j.|.j.v.r"t.|.j
+00000a90: 0074 046a 0564 018d 0253 0064 0053 0064  .t.j.d...S.d.S.d
+00000aa0: 0053 0029 024e 2901 da03 6170 7029 0672  .S.).N)...app).r
+00000ab0: 4e00 0000 7254 0000 00da 0953 4348 4544  N...rT.....SCHED
+00000ac0: 554c 4544 7218 0000 00da 0663 656c 6572  ULEDr......celer
+00000ad0: 79da 0b63 7572 7265 6e74 5f61 7070 a901  y..current_app..
+00000ae0: 7252 0000 0072 2900 0000 7229 0000 0072  rR...r)...r)...r
+00000af0: 2d00 0000 724f 0000 0056 0000 0073 0600  -...rO...V...s..
+00000b00: 0000 0002 1201 1002 7a1a 4365 6c65 7279  ........z.Celery
+00000b10: 456e 6162 6c65 642e 6173 796e 635f 7265  Enabled.async_re
+00000b20: 7375 6c74 6301 0000 0000 0000 0000 0000  sultc...........
+00000b30: 0002 0000 0002 0000 0043 0000 0073 2800  .........C...s(.
+00000b40: 0000 7c00 6a00 7c00 6a01 7601 7224 7c00  ..|.j.|.j.v.r$|.
+00000b50: a002 a100 7d01 7c01 7320 7403 6401 8301  ....}.|.s t.d...
+00000b60: 8201 7c01 5300 6400 5300 2902 4e7a 2160  ..|.S.d.S.).Nz!`
+00000b70: 5f71 7565 7565 6020 6e6f 7420 7072 6f70  _queue` not prop
+00000b80: 6572 6c79 2069 6d70 6c65 6d65 6e74 6564  erly implemented
+00000b90: 2904 7254 0000 0072 5600 0000 da06 5f71  ).rT...rV....._q
+00000ba0: 7565 7565 da13 4e6f 7449 6d70 6c65 6d65  ueue..NotImpleme
+00000bb0: 6e74 6564 4572 726f 7229 0272 5200 0000  ntedError).rR...
+00000bc0: da07 7461 736b 5f69 6472 2900 0000 7229  ..task_idr)...r)
+00000bd0: 0000 0072 2d00 0000 da05 7175 6575 655d  ...r-.....queue]
+00000be0: 0000 0073 0c00 0000 0001 0c01 0801 0401  ...s............
+00000bf0: 0801 0401 7a13 4365 6c65 7279 456e 6162  ....z.CeleryEnab
+00000c00: 6c65 642e 7175 6575 6563 0100 0000 0000  led.queuec......
+00000c10: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000c20: 0000 7304 0000 0064 0153 00a9 024e da00  ..s....d.S...N..
+00000c30: 7229 0000 0072 5900 0000 7229 0000 0072  r)...rY...r)...r
+00000c40: 2900 0000 722d 0000 0072 5a00 0000 6500  )...r-...rZ...e.
+00000c50: 0000 7302 0000 0000 017a 1443 656c 6572  ..s......z.Celer
+00000c60: 7945 6e61 626c 6564 2e5f 7175 6575 654e  yEnabled._queueN
+00000c70: 2916 7248 0000 0072 4900 0000 724a 0000  ).rH...rI...rJ..
+00000c80: 00da 0966 726f 7a65 6e73 6574 7217 0000  ...frozensetr...
+00000c90: 00da 0750 454e 4449 4e47 da08 5245 4345  ...PENDING..RECE
+00000ca0: 4956 4544 da07 5354 4152 5445 44da 0552  IVED..STARTED..R
+00000cb0: 4554 5259 7256 0000 0072 0d00 0000 da09  ETRYrV...r......
+00000cc0: 4368 6172 4669 656c 6472 4e00 0000 724c  CharFieldrN...rL
+00000cd0: 0000 0072 5100 0000 7254 0000 00da 0870  ...rQ...rT.....p
+00000ce0: 726f 7065 7274 7972 0500 0000 7218 0000  ropertyr....r...
+00000cf0: 0072 4f00 0000 725d 0000 0072 5a00 0000  .rO...r]...rZ...
+00000d00: 7229 0000 0072 2900 0000 7229 0000 0072  r)...r)...r)...r
+00000d10: 2d00 0000 7242 0000 0042 0000 0073 1400  -...rB...B...s..
+00000d20: 0000 0801 0201 12ff 0404 1002 0e03 0e0a  ................
+00000d30: 0201 1406 1208 7242 0000 0063 0000 0000  ......rB...c....
+00000d40: 0000 0000 0000 0000 0000 0000 0700 0000  ................
+00000d50: 0000 0000 73e4 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00000d60: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
+00000d70: 0565 036a 0664 0164 0264 058d 025a 0765  .e.j.d.d.d...Z.e
+00000d80: 036a 0864 0164 0264 0264 068d 035a 0965  .j.d.d.d.d...Z.e
+00000d90: 036a 0a65 0b64 0365 0c67 0164 078d 035a  .j.e.d.e.g.d...Z
+00000da0: 0d65 036a 0e64 0264 0364 0364 088d 035a  .e.j.d.d.d.d...Z
+00000db0: 0f65 036a 1064 0964 0264 0265 036a 1164  .e.j.d.d.d.e.j.d
+00000dc0: 0a64 0b8d 055a 1247 0064 0c64 0d84 0064  .d...Z.G.d.d...d
+00000dd0: 0d83 025a 1364 0e64 0f9c 0164 1064 1184  ...Z.d.d...d.d..
+00000de0: 045a 1465 1565 1619 0064 0f9c 0164 1264  .Z.e.e...d...d.d
+00000df0: 1384 045a 1764 1b65 1865 1865 1965 1a19  ...Z.d.e.e.e.e..
+00000e00: 0065 1965 1a19 0064 0e64 149c 0587 0066  .e.e...d.d.....f
+00000e10: 0164 1564 1684 0d5a 1b64 0e64 0f9c 0164  .d.d...Z.d.d...d
+00000e20: 1764 1884 045a 1c65 1d64 0f9c 0164 1964  .d...Z.e.d...d.d
+00000e30: 1a84 045a 1e87 0004 005a 1f53 0029 1cda  ...Z.....Z.S.)..
+00000e40: 0c50 6172 616d 6574 7269 7a65 72e9 ff00  .Parametrizer...
+00000e50: 0000 5446 2903 7245 0000 00da 0675 6e69  ..TF).rE.....uni
+00000e60: 7175 65da 0865 6469 7461 626c 65a9 0272  que..editable..r
+00000e70: 4500 0000 7269 0000 0029 0372 4500 0000  E...ri...).rE...
+00000e80: 7247 0000 0072 4600 0000 2903 da07 6465  rG...rF...)...de
+00000e90: 6661 756c 7472 4600 0000 da0a 7661 6c69  faultrF.....vali
+00000ea0: 6461 746f 7273 2903 7246 0000 0072 6c00  dators).rF...rl.
+00000eb0: 0000 726a 0000 00da 0551 7565 7279 fa01  ..rj.....Query..
+00000ec0: 2ba9 0472 4600 0000 7247 0000 00da 096f  +..rF...rG.....o
+00000ed0: 6e5f 6465 6c65 7465 da0c 7265 6c61 7465  n_delete..relate
+00000ee0: 645f 6e61 6d65 6300 0000 0000 0000 0000  d_namec.........
+00000ef0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+00000f00: 1400 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00000f10: 6401 5a04 6402 5300 2903 7a11 5061 7261  d.Z.d.S.).z.Para
+00000f20: 6d65 7472 697a 6572 2e4d 6574 61da 0941  metrizer.Meta..A
+00000f30: 7267 756d 656e 7473 4e29 0572 4800 0000  rgumentsN).rH...
+00000f40: 7249 0000 0072 4a00 0000 da13 7665 7262  rI...rJ.....verb
+00000f50: 6f73 655f 6e61 6d65 5f70 6c75 7261 6cda  ose_name_plural.
+00000f60: 0c76 6572 626f 7365 5f6e 616d 6572 2900  .verbose_namer).
+00000f70: 0000 7229 0000 0072 2900 0000 722d 0000  ..r)...r)...r-..
+00000f80: 0072 4c00 0000 7700 0000 7304 0000 0008  .rL...w...s.....
+00000f90: 0104 0172 4c00 0000 4e72 4d00 0000 6301  ...rL...NrM...c.
+00000fa0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000fb0: 0000 0043 0000 0073 0e00 0000 7400 7c00  ...C...s....t.|.
+00000fc0: 6a01 8301 0100 6400 5300 7228 0000 0029  j.....d.S.r(...)
+00000fd0: 0272 4100 0000 7230 0000 0072 5900 0000  .rA...r0...rY...
+00000fe0: 7229 0000 0072 2900 0000 722d 0000 00da  r)...r)...r-....
+00000ff0: 0563 6c65 616e 7b00 0000 7302 0000 0000  .clean{...s.....
+00001000: 017a 1250 6172 616d 6574 7269 7a65 722e  .z.Parametrizer.
+00001010: 636c 6561 6e63 0100 0000 0000 0000 0000  cleanc..........
+00001020: 0000 0200 0000 0400 0000 0300 0000 7326  ..............s&
+00001030: 0000 0074 0074 016a 0288 006a 03a0 04a1  ...t.t.j...j....
+00001040: 008e 0083 017d 0187 0066 0164 0164 0284  .....}...f.d.d..
+00001050: 087c 0144 0083 0153 0029 034e 6301 0000  .|.D...S.).Nc...
+00001060: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00001070: 0013 0000 0073 2000 0000 6700 7c00 5d18  .....s ...g.|.].
+00001080: 7d01 7400 7401 8800 6a02 a003 a100 7c01  }.t.t...j.....|.
+00001090: 8302 8301 9102 7104 5300 7229 0000 0029  ......q.S.r)...)
+000010a0: 0472 3200 0000 7233 0000 0072 3000 0000  .r2...r3...r0...
+000010b0: 7234 0000 0072 3500 0000 7259 0000 0072  r4...r5...rY...r
+000010c0: 2900 0000 722d 0000 0072 3800 0000 8000  )...r-...r8.....
+000010d0: 0000 722f 0000 007a 2b50 6172 616d 6574  ..r/...z+Paramet
+000010e0: 7269 7a65 722e 6765 745f 6d61 7472 6978  rizer.get_matrix
+000010f0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00001100: 6f6d 703e 2905 723c 0000 0072 3d00 0000  omp>).r<...r=...
+00001110: 723e 0000 0072 3000 0000 723f 0000 0029  r>...r0...r?...)
+00001120: 0272 5200 0000 723e 0000 0072 2900 0000  .rR...r>...r)...
+00001130: 7259 0000 0072 2d00 0000 da0a 6765 745f  rY...r-.....get_
+00001140: 6d61 7472 6978 7e00 0000 7304 0000 0000  matrix~...s.....
+00001150: 0114 017a 1750 6172 616d 6574 7269 7a65  ...z.Parametrize
+00001160: 722e 6765 745f 6d61 7472 6978 a905 da0c  r.get_matrix....
+00001170: 666f 7263 655f 696e 7365 7274 da0c 666f  force_insert..fo
+00001180: 7263 655f 7570 6461 7465 da05 7573 696e  rce_update..usin
+00001190: 67da 0d75 7064 6174 655f 6669 656c 6473  g..update_fields
+000011a0: 7231 0000 0063 0500 0000 0000 0000 0000  r1...c..........
+000011b0: 0000 0500 0000 0600 0000 0300 0000 7328  ..............s(
+000011c0: 0000 007c 006a 0073 1274 017c 006a 0283  ...|.j.s.t.|.j..
+000011d0: 017c 005f 0074 0383 00a0 047c 017c 027c  .|._.t.....|.|.|
+000011e0: 037c 04a1 0401 0064 0053 0072 2800 0000  .|.....d.S.r(...
+000011f0: 2905 da04 636f 6465 7216 0000 00da 046e  )...coder......n
+00001200: 616d 65da 0573 7570 6572 da04 7361 7665  ame..super..save
+00001210: a905 7252 0000 0072 7900 0000 727a 0000  ..rR...ry...rz..
+00001220: 0072 7b00 0000 727c 0000 00a9 01da 095f  .r{...r|......._
+00001230: 5f63 6c61 7373 5f5f 7229 0000 0072 2d00  _class__r)...r-.
+00001240: 0000 7280 0000 0082 0000 0073 0600 0000  ..r........s....
+00001250: 0007 0601 0c01 7a11 5061 7261 6d65 7472  ......z.Parametr
+00001260: 697a 6572 2e73 6176 6563 0100 0000 0000  izer.savec......
+00001270: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00001280: 0000 732a 0000 007c 006a 0072 267c 006a  ..s*...|.j.r&|.j
+00001290: 006a 0164 0164 028d 015c 027d 017d 027c  .j.d.d...\.}.}.|
+000012a0: 017c 005f 027c 00a0 03a1 0001 0064 0053  .|._.|.......d.S
+000012b0: 0029 034e 5429 01da 0c75 7365 5f65 7869  .).NT)...use_exi
+000012c0: 7374 696e 6729 04da 0673 6f75 7263 65da  sting)...source.
+000012d0: 0372 756e 7230 0000 0072 8000 0000 2903  .runr0...r....).
+000012e0: 7252 0000 00da 036f 7574 da02 5f5f 7229  rR.....out..__r)
+000012f0: 0000 0072 2900 0000 722d 0000 00da 0772  ...r)...r-.....r
+00001300: 6566 7265 7368 8d00 0000 7308 0000 0000  efresh....s.....
+00001310: 0106 0112 0106 017a 1450 6172 616d 6574  .......z.Paramet
+00001320: 7269 7a65 722e 7265 6672 6573 6863 0100  rizer.refreshc..
+00001330: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00001340: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+00001350: 0072 2800 0000 a901 727e 0000 0072 5900  .r(.....r~...rY.
+00001360: 0000 7229 0000 0072 2900 0000 722d 0000  ..r)...r)...r-..
+00001370: 00da 075f 5f73 7472 5f5f 9300 0000 7302  ...__str__....s.
+00001380: 0000 0000 017a 1450 6172 616d 6574 7269  .....z.Parametri
+00001390: 7a65 722e 5f5f 7374 725f 5f29 0446 464e  zer.__str__).FFN
+000013a0: 4e29 2072 4800 0000 7249 0000 0072 4a00  N) rH...rI...rJ.
+000013b0: 0000 720d 0000 00da 0953 6c75 6746 6965  ..r......SlugFie
+000013c0: 6c64 727d 0000 0072 6500 0000 727e 0000  ldr}...re...r~..
+000013d0: 00da 0954 6578 7446 6965 6c64 da0b 6465  ...TextField..de
+000013e0: 7363 7269 7074 696f 6e72 0f00 0000 7232  scriptionr....r2
+000013f0: 0000 0072 4100 0000 7230 0000 00da 0c42  ...rA...r0.....B
+00001400: 6f6f 6c65 616e 4669 656c 64da 0673 7973  ooleanField..sys
+00001410: 7465 6dda 0a46 6f72 6569 676e 4b65 79da  tem..ForeignKey.
+00001420: 0743 4153 4341 4445 7285 0000 0072 4c00  .CASCADEr....rL.
+00001430: 0000 7276 0000 0072 0400 0000 7203 0000  ..rv...r....r...
+00001440: 0072 7700 0000 da04 626f 6f6c 7205 0000  .rw.....boolr...
+00001450: 0072 0200 0000 7280 0000 0072 8900 0000  .r....r....r....
+00001460: 7251 0000 0072 8b00 0000 da0d 5f5f 636c  rQ...r......__cl
+00001470: 6173 7363 656c 6c5f 5f72 2900 0000 7229  asscell__r)...r)
+00001480: 0000 0072 8200 0000 722d 0000 0072 6700  ...r....r-...rg.
+00001490: 0000 6900 0000 7338 0000 0008 0110 010e  ..i...s8........
+000014a0: 0104 0102 0102 0102 fd06 0512 0110 0104  ................
+000014b0: 010c ff06 040e 040e 0312 0600 0100 0100  ................
+000014c0: 0100 fb02 0202 0102 0106 0106 0102 fa10  ................
+000014d0: 0b0e 0672 6700 0000 6300 0000 0000 0000  ...rg...c.......
+000014e0: 0000 0000 0000 0000 0007 0000 0000 0000  ................
+000014f0: 0073 5801 0000 6500 5a01 6400 5a02 6503  .sX...e.Z.d.Z.e.
+00001500: 6a04 6401 6402 6403 8d02 5a05 6503 6a06  j.d.d.d...Z.e.j.
+00001510: 6402 6402 6404 8d02 5a07 6503 6a08 6509  d.d.d...Z.e.j.e.
+00001520: 8300 6503 6a0a 6405 6406 8d03 5a0b 6503  ..e.j.d.d...Z.e.
+00001530: 6a08 650c 6503 6a0a 6407 8d02 5a0d 6503  j.e.e.j.d...Z.e.
+00001540: 6a06 6408 6402 6409 8d02 5a0e 650f 6510  j.d.d.d...Z.e.e.
+00001550: 6402 6511 640a 8d03 5a12 6503 6a08 6513  d.e.d...Z.e.j.e.
+00001560: 6503 6a0a 6402 6402 640b 8d04 5a14 6503  e.j.d.d.d...Z.e.
+00001570: 6a04 640c 6402 6402 640d 8d03 5a15 6503  j.d.d.d.d...Z.e.
+00001580: 6a04 640c 6402 6402 640d 8d03 5a16 6503  j.d.d.d.d...Z.e.
+00001590: 6a17 6402 6402 640e 8d02 5a18 6503 6a19  j.d.d.d...Z.e.j.
+000015a0: 6402 640f 8d01 5a1a 651b 6410 9c01 6411  d.d...Z.e.d...d.
+000015b0: 6412 8404 5a1c 4700 6413 6414 8400 6414  d...Z.G.d.d...d.
+000015c0: 8302 5a1d 6428 651e 651e 651f 6520 1900  ..Z.d(e.e.e.e ..
+000015d0: 651f 6520 1900 6416 6417 9c05 8700 6601  e.e ..d.d.....f.
+000015e0: 6418 6419 840d 5a21 6522 6523 6524 641a  d.d...Z!e"e#e$d.
+000015f0: 9c03 641b 641c 8404 5a25 6526 6416 641d  ..d.d...Z%e&d.d.
+00001600: 9c02 641e 641f 8404 5a27 6429 651e 6520  ..d.d...Z'd)e.e 
+00001610: 6526 6420 9c03 6421 6422 8405 5a28 642a  e&d ..d!d"..Z(d*
+00001620: 651e 651f 6524 1900 651e 6529 6423 9c04  e.e.e$..e.e)d#..
+00001630: 6424 6425 8405 5a2a 651b 6410 9c01 6426  d$d%..Z*e.d...d&
+00001640: 6427 8404 5a2b 8700 0400 5a2c 5300 292b  d'..Z+....Z,S.)+
+00001650: 726e 0000 0072 6800 0000 5472 6b00 0000  rn...rh...Trk...
+00001660: a902 7246 0000 0072 4700 0000 5a0d 706f  ..rF...rG...Z.po
+00001670: 7765 725f 7175 6572 6965 73a9 0272 7100  wer_queries..rq.
+00001680: 0000 7272 0000 00a9 0172 7100 0000 7a0d  ..rr.....rq...z.
+00001690: 7173 3d63 6f6e 6e2e 616c 6c28 29a9 0272  qs=conn.all()..r
+000016a0: 6c00 0000 7246 0000 0029 0372 6c00 0000  l...rF...).rl...
+000016b0: 7246 0000 00da 0765 6e63 6f64 6572 2903  rF.....encoder).
+000016c0: 7271 0000 0072 4600 0000 7247 0000 0069  rq...rF...rG...i
+000016d0: 9001 0000 7244 0000 00a9 0272 4700 0000  ....rD.....rG...
+000016e0: 7246 0000 00a9 0172 6c00 0000 724d 0000  rF.....rl...rM..
+000016f0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001700: 0000 0100 0000 4300 0000 730a 0000 007c  ......C...s....|
+00001710: 006a 0070 0864 0153 0072 5e00 0000 728a  .j.p.d.S.r^...r.
+00001720: 0000 0072 5900 0000 7229 0000 0072 2900  ...rY...r)...r).
+00001730: 0000 722d 0000 0072 8b00 0000 aa00 0000  ..r-...r........
+00001740: 7302 0000 0000 017a 0d51 7565 7279 2e5f  s......z.Query._
+00001750: 5f73 7472 5f5f 6300 0000 0000 0000 0000  _str__c.........
+00001760: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+00001770: 1400 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00001780: 6402 5a04 6403 5300 2904 7a0a 5175 6572  d.Z.d.S.).z.Quer
+00001790: 792e 4d65 7461 7a0d 506f 7765 7220 5175  y.Metaz.Power Qu
+000017a0: 6572 6965 7372 8a00 0000 4e29 0572 4800  eriesr....N).rH.
+000017b0: 0000 7249 0000 0072 4a00 0000 7274 0000  ..rI...rJ...rt..
+000017c0: 00da 086f 7264 6572 696e 6772 2900 0000  ...orderingr)...
+000017d0: 7229 0000 0072 2900 0000 722d 0000 0072  r)...r)...r-...r
+000017e0: 4c00 0000 ad00 0000 7304 0000 0008 0104  L.......s.......
+000017f0: 0172 4c00 0000 464e 7278 0000 0063 0500  .rL...FNrx...c..
+00001800: 0000 0000 0000 0000 0000 0500 0000 0600  ................
+00001810: 0000 0300 0000 7322 0000 007c 006a 0073  ......s"...|.j.s
+00001820: 0c64 017c 005f 0074 0183 00a0 027c 017c  .d.|._.t.....|.|
+00001830: 027c 037c 04a1 0401 0064 0053 0029 024e  .|.|.....d.S.).N
+00001840: 7a1c 7173 3d63 6f6e 6e2e 616c 6c28 292e  z.qs=conn.all().
+00001850: 6f72 6465 725f 6279 2827 6964 2729 2903  order_by('id')).
+00001860: 727d 0000 0072 7f00 0000 7280 0000 0072  r}...r....r....r
+00001870: 8100 0000 7282 0000 0072 2900 0000 722d  ....r....r)...r-
+00001880: 0000 0072 8000 0000 b100 0000 7306 0000  ...r........s...
+00001890: 0000 0706 0106 017a 0a51 7565 7279 2e73  .......z.Query.s
+000018a0: 6176 6529 03da 0871 7565 7279 5f69 64da  ave)...query_id.
+000018b0: 0961 7267 756d 656e 7473 7231 0000 0063  .argumentsr1...c
+000018c0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+000018d0: 0500 0000 4300 0000 7322 0000 0074 006a  ....C...s"...t.j
+000018e0: 016a 027c 0164 018d 017d 037c 036a 0364  .j.|.d...}.|.j.d
+000018f0: 027c 0264 0364 048d 037d 047c 0453 0029  .|.d.d...}.|.S.)
+00001900: 054e 2901 da02 6964 4654 2903 da07 7065  .N)...idFT)...pe
+00001910: 7273 6973 7472 9e00 0000 7284 0000 0029  rsistr....r....)
+00001920: 0472 6e00 0000 da07 6f62 6a65 6374 73da  .rn.....objects.
+00001930: 0367 6574 7286 0000 0029 0572 5200 0000  .getr....).rR...
+00001940: 729d 0000 0072 9e00 0000 da05 7175 6572  r....r......quer
+00001950: 7972 5300 0000 7229 0000 0072 2900 0000  yrS...r)...r)...
+00001960: 722d 0000 00da 075f 696e 766f 6b65 bc00  r-....._invoke..
+00001970: 0000 7306 0000 0000 010e 0110 017a 0d51  ..s..........z.Q
+00001980: 7565 7279 2e5f 696e 766f 6b65 2902 da07  uery._invoke)...
+00001990: 7265 7375 6c74 7372 3100 0000 6302 0000  resultsr1...c...
+000019a0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000019b0: 0043 0000 0073 3c00 0000 7c01 7c00 6a00  .C...s<...|.|.j.
+000019c0: 6401 3c00 7c01 a001 6402 6403 a102 7c00  d.<.|...d.d...|.
+000019d0: 5f02 7c01 a001 6404 6403 a102 7c00 5f03  _.|...d.d...|._.
+000019e0: 7404 a005 a100 7c00 5f06 7c00 a007 a100  t.....|._.|.....
+000019f0: 0100 6400 5300 2905 4e5a 106c 6173 745f  ..d.S.).NZ.last_
+00001a00: 7275 6e5f 7265 7375 6c74 73da 0d65 7272  run_results..err
+00001a10: 6f72 5f6d 6573 7361 6765 725f 0000 00da  or_messager_....
+00001a20: 0f73 656e 7472 795f 6572 726f 725f 6964  .sentry_error_id
+00001a30: 2908 da04 696e 666f 72a2 0000 0072 a600  )...infor....r..
+00001a40: 0000 72a7 0000 0072 1300 0000 da03 6e6f  ..r....r......no
+00001a50: 77da 086c 6173 745f 7275 6e72 8000 0000  w..last_runr....
+00001a60: 2902 7252 0000 0072 a500 0000 7229 0000  ).rR...r....r)..
+00001a70: 0072 2900 0000 722d 0000 00da 0e75 7064  .r)...r-.....upd
+00001a80: 6174 655f 7265 7375 6c74 73c1 0000 0073  ate_results....s
+00001a90: 0a00 0000 0001 0a01 0e01 0e01 0a01 7a14  ..............z.
+00001aa0: 5175 6572 792e 7570 6461 7465 5f72 6573  Query.update_res
+00001ab0: 756c 7473 2903 72a0 0000 00da 066b 7761  ults).r......kwa
+00001ac0: 7267 7372 3100 0000 6302 0000 0000 0000  rgsr1...c.......
+00001ad0: 0000 0000 000a 0000 000d 0000 000b 0000  ................
+00001ae0: 0073 9201 0000 8801 6a00 721e 8801 6a00  .s......j.r...j.
+00001af0: a001 a100 7d03 7c03 7324 7402 6401 8301  ....}.|.s$t.d...
+00001b00: 8201 6e06 6900 6701 7d03 6400 8801 5f03  ..n.i.g.}.d..._.
+00001b10: 6400 8801 5f04 6400 8801 5f05 6900 8801  d..._.d..._.i...
+00001b20: 5f06 6402 7407 7408 a009 a100 6403 8302  _.d.t.t.....d...
+00001b30: 6901 8900 740a 8300 9001 8f26 7d04 7c04  i...t......&}.|.
+00001b40: a00b 6404 6405 a102 0100 7c04 a00b 6406  ..d.d.....|...d.
+00001b50: 8801 6a0c a102 0100 740d a00e a100 8fe2  ..j.....t.......
+00001b60: 0100 740d a00f 8700 8701 6602 6407 6408  ..t.......f.d.d.
+00001b70: 8408 a101 0100 7c03 4400 5d98 7d05 7a42  ......|.D.].}.zB
+00001b80: 8801 a010 7c01 7c05 a102 5c02 7d06 7d07  ....|.|...\.}.}.
+00001b90: 7411 7c06 7412 8302 72c4 7c06 6a13 8800  t.|.t...r.|.j...
+00001ba0: 7414 7c05 8301 3c00 6e14 7414 7415 7c06  t.|...<.n.t.t.|.
+00001bb0: 8301 8301 8800 7414 7c05 8301 3c00 5700  ......t.|...<.W.
+00001bc0: 7194 0400 7416 9001 792a 0100 7d08 0100  q...t...y*..}...
+00001bd0: 7a36 7417 a018 7c08 a101 0100 7419 7c08  z6t...|.....t.|.
+00001be0: 8301 7d09 7414 7c09 8301 8800 6409 3c00  ..}.t.|.....d.<.
+00001bf0: 7414 7c08 8301 8800 640a 3c00 5700 5900  t.|.....d.<.W.Y.
+00001c00: 6400 7d08 7e08 7194 6400 7d08 7e08 3000  d.}.~.q.d.}.~.0.
+00001c10: 3000 7194 8801 6a1a 6a1b 640b 640c 8400  0.q...j.j.d.d...
+00001c20: 8800 a01c a100 4400 8301 640d 8d01 a01d  ......D...d.....
+00001c30: a100 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00001c40: 6e12 3100 9001 7364 3000 0100 0100 0100  n.1...sd0.......
+00001c50: 5900 0100 5700 6400 0400 0400 8303 0100  Y...W.d.........
+00001c60: 6e12 3100 9001 7384 3000 0100 0100 0100  n.1...s.0.......
+00001c70: 5900 0100 8800 5300 290e 4e7a 1b4e 6f20  Y.....S.).Nz.No 
+00001c80: 7661 6c69 6420 6172 6775 6d65 6e74 7320  valid arguments 
+00001c90: 7072 6f76 6964 6564 da09 7469 6d65 7374  provided..timest
+00001ca0: 616d 707a 0e25 592d 256d 2d25 6420 2548  ampz.%Y-%m-%d %H
+00001cb0: 3a25 4dda 0b70 6f77 6572 5f71 7565 7279  :%M..power_query
+00001cc0: 547a 1070 6f77 6572 5f71 7565 7279 2e6e  Tz.power_query.n
+00001cd0: 616d 6563 0000 0000 0000 0000 0000 0000  amec............
+00001ce0: 0000 0000 0300 0000 1300 0000 730a 0000  ............s...
+00001cf0: 0088 01a0 0088 00a1 0153 0072 2800 0000  .........S.r(...
+00001d00: 2901 72ab 0000 0072 2900 0000 a902 72a5  ).r....r).....r.
+00001d10: 0000 0072 5200 0000 7229 0000 0072 2d00  ...rR...r)...r-.
+00001d20: 0000 da08 3c6c 616d 6264 613e db00 0000  ....<lambda>....
+00001d30: 722f 0000 007a 2651 7565 7279 2e65 7865  r/...z&Query.exe
+00001d40: 6375 7465 5f6d 6174 7269 782e 3c6c 6f63  cute_matrix.<loc
+00001d50: 616c 733e 2e3c 6c61 6d62 6461 3e72 a700  als>.<lambda>r..
+00001d60: 0000 72a6 0000 0063 0100 0000 0000 0000  ..r....c........
+00001d70: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00001d80: 731a 0000 0067 007c 005d 127d 0174 007c  s....g.|.].}.t.|
+00001d90: 0174 0183 0272 047c 0191 0271 0453 0072  .t...r.|...q.S.r
+00001da0: 2900 0000 2902 723b 0000 00da 0369 6e74  )...).r;.....int
+00001db0: 2902 722a 0000 005a 0364 706b 7229 0000  ).r*...Z.dpkr)..
+00001dc0: 0072 2900 0000 722d 0000 0072 3800 0000  .r)...r-...r8...
+00001dd0: ea00 0000 722f 0000 007a 2851 7565 7279  ....r/...z(Query
+00001de0: 2e65 7865 6375 7465 5f6d 6174 7269 782e  .execute_matrix.
+00001df0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001e00: 6d70 3e29 01da 0670 6b5f 5f69 6e29 1eda  mp>)...pk__in)..
+00001e10: 0c70 6172 616d 6574 7269 7a65 7272 7700  .parametrizerrw.
+00001e20: 0000 da0a 5661 6c75 6545 7272 6f72 72a6  ....ValueErrorr.
+00001e30: 0000 0072 a700 0000 72aa 0000 0072 a800  ...r....r....r..
+00001e40: 0000 7214 0000 0072 1300 0000 72a9 0000  ..r....r....r...
+00001e50: 0072 1b00 0000 da07 7365 745f 7461 6772  .r......set_tagr
+00001e60: 7e00 0000 720e 0000 00da 0661 746f 6d69  ~...r......atomi
+00001e70: 63da 096f 6e5f 636f 6d6d 6974 7286 0000  c..on_commitr...
+00001e80: 0072 3b00 0000 da07 4461 7461 7365 74da  .r;.....Dataset.
+00001e90: 0270 6b72 5100 0000 da03 6c65 6e72 1c00  .pkrQ.....lenr..
+00001ea0: 0000 da06 6c6f 6767 6572 da09 6578 6365  ....logger..exce
+00001eb0: 7074 696f 6e72 1a00 0000 da08 6461 7461  ptionr......data
+00001ec0: 7365 7473 da07 6578 636c 7564 6572 3f00  sets..excluder?.
+00001ed0: 0000 da06 6465 6c65 7465 290a 7252 0000  ....delete).rR..
+00001ee0: 0072 a000 0000 72ac 0000 00da 0461 7267  .r....r......arg
+00001ef0: 73da 0573 636f 7065 da01 61da 0764 6174  s..scope..a..dat
+00001f00: 6173 6574 7288 0000 0072 3600 0000 da03  asetr....r6.....
+00001f10: 6572 7272 2900 0000 72af 0000 0072 2d00  errr)...r....r-.
+00001f20: 0000 da0e 6578 6563 7574 655f 6d61 7472  ....execute_matr
+00001f30: 6978 c800 0000 733e 0000 0000 0106 010a  ix....s>........
+00001f40: 0104 010a 0206 0106 0106 0106 0106 030e  ................
+00001f50: ff04 030a 010c 010e 010a 0114 0108 0102  ................
+00001f60: 0110 010a 0110 0218 0210 010a 0108 010c  ................
+00001f70: 0124 0106 0110 ff4a 037a 1451 7565 7279  .$.....J.z.Query
+00001f80: 2e65 7865 6375 7465 5f6d 6174 7269 7829  .execute_matrix)
+00001f90: 0472 a000 0000 729e 0000 0072 8400 0000  .r....r....r....
+00001fa0: 7231 0000 0063 0400 0000 0000 0000 0000  r1...c..........
+00001fb0: 0000 1100 0000 0a00 0000 4300 0000 7384  ..........C...s.
+00001fc0: 0100 007c 006a 00a0 01a1 007d 0474 0283  ...|.j.....}.t..
+00001fd0: 0067 017d 0574 036a 0472 2e7c 05a0 0564  .g.}.t.j.r.|...d
+00001fe0: 0164 0284 0074 036a 0444 0083 01a1 0101  .d...t.j.D......
+00001ff0: 0064 0364 0484 007c 0544 0083 017d 067c  .d.d...|.D...}.|
+00002000: 006a 066a 0772 5474 086a 09a0 0aa1 007c  .j.j.rTt.j.....|
+00002010: 0664 053c 006e 1474 086a 096a 0a7c 006a  .d.<.n.t.j.j.|.j
+00002020: 0664 068d 017c 0664 053c 007a e67c 046a  .d...|.d.<.z.|.j
+00002030: 0ba0 0c74 036a 0da1 017c 007c 027c 027c  ...t.j...|.|.|.|
+00002040: 006a 0e64 079c 057c 06a5 017d 0774 0f64  .j.d...|...}.t.d
+00002050: 087c 006a 1069 017c 0272 9c7c 026e 0269  .|.j.i.|.r.|.n.i
+00002060: 00a5 0183 017d 087c 0372 cc74 116a 096a  .....}.|.r.t.j.j
+00002070: 0a7c 007c 0864 098d 02a0 12a1 0004 007d  .|.|.d.........}
+00002080: 0972 cc7c 097c 096a 1366 027d 0a6e 8074  .r.|.|.j.f.}.n.t
+00002090: 147c 006a 1574 1683 007c 0783 0301 007c  .|.j.t...|.....|
+000020a0: 07a0 1764 0a64 00a1 027d 0b7c 07a0 1764  ...d.d...}.|...d
+000020b0: 0b64 00a1 027d 0c7c 0190 0172 4474 187c  .d...}.|...rDt.|
+000020c0: 0b83 016a 197c 0264 0c9c 027d 0d74 116a  ...j.|.d...}.t.j
+000020d0: 096a 1a7c 007c 087c 0d74 1ba0 1ca1 0074  .j.|.|.|.t.....t
+000020e0: 1da0 1e7c 0ba1 0174 1da0 1e7c 0ca1 0164  ...|...t...|...d
+000020f0: 0d9c 0464 0e8d 035c 027d 0e7d 0f7c 0e7c  ...d...\.}.}.|.|
+00002100: 0c66 027d 0a6e 087c 0b7c 0c66 027d 0a57  .f.}.n.|.|.f.}.W
+00002110: 006e 3004 0074 1f90 0179 7e01 007d 1001  .n0..t...y~..}..
+00002120: 007a 1674 207c 1083 017c 1082 0257 0059  .z.t |...|...W.Y
+00002130: 0064 007d 107e 106e 0a64 007d 107e 1030  .d.}.~.n.d.}.~.0
+00002140: 0030 007c 0a53 0029 0f4e 6301 0000 0000  .0.|.S.).Nc.....
+00002150: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00002160: 0000 0073 1600 0000 6700 7c00 5d0e 7d01  ...s....g.|.].}.
+00002170: 7400 a001 7c01 a101 9102 7104 5300 7229  t...|.....q.S.r)
+00002180: 0000 0029 02da 0b64 6a61 6e67 6f5f 6170  ...)...django_ap
+00002190: 7073 da09 6765 745f 6d6f 6465 6c29 0272  ps..get_model).r
+000021a0: 2a00 0000 5a0b 6c61 6265 6c32 6d6f 6465  *...Z.label2mode
+000021b0: 6c72 2900 0000 7229 0000 0072 2d00 0000  lr)...r)...r-...
+000021c0: 7238 0000 00f9 0000 0073 0400 0000 0602  r8.......s......
+000021d0: 02ff 7a1d 5175 6572 792e 7275 6e2e 3c6c  ..z.Query.run.<l
+000021e0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+000021f0: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
+00002200: 0000 0600 0000 5300 0000 7326 0000 0069  ......S...s&...i
+00002210: 007c 005d 1e7d 017c 016a 006a 019b 0064  .|.].}.|.j.j...d
+00002220: 009d 027c 016a 02a0 0374 046a 05a1 0193  ...|.j...t.j....
+00002230: 0271 0453 0029 01da 074d 616e 6167 6572  .q.S.)...Manager
+00002240: 2906 da05 5f6d 6574 61da 0b6f 626a 6563  )..._meta..objec
+00002250: 745f 6e61 6d65 da10 5f64 6566 6175 6c74  t_name.._default
+00002260: 5f6d 616e 6167 6572 727b 0000 0072 0900  _managerr{...r..
+00002270: 0000 da14 504f 5745 525f 5155 4552 595f  ....POWER_QUERY_
+00002280: 4442 5f41 4c49 4153 2902 722a 0000 00da  DB_ALIAS).r*....
+00002290: 056d 6f64 656c 7229 0000 0072 2900 0000  .modelr)...r)...
+000022a0: 722d 0000 00da 0a3c 6469 6374 636f 6d70  r-.....<dictcomp
+000022b0: 3efe 0000 0073 0800 0000 0604 02fd 1201  >....s..........
+000022c0: 04ff 7a1d 5175 6572 792e 7275 6e2e 3c6c  ..z.Query.run.<l
+000022d0: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
+000022e0: 3eda 0c51 7565 7279 4d61 6e61 6765 7229  >..QueryManager)
+000022f0: 01da 056f 776e 6572 2905 da04 636f 6e6e  ...owner)...conn
+00002300: 72a3 0000 0072 c000 0000 729e 0000 00da  r....r....r.....
+00002310: 0669 6e76 6f6b 6572 a300 0000 2902 72a3  .invoker....).r.
+00002320: 0000 00da 0468 6173 6872 5300 0000 da05  .....hashrS.....
+00002330: 6578 7472 6129 02da 0474 7970 6572 9e00  extra)...typer..
+00002340: 0000 2904 72a8 0000 0072 aa00 0000 7230  ..).r....r....r0
+00002350: 0000 0072 d400 0000 2903 72a3 0000 0072  ...r....).r....r
+00002360: d300 0000 da08 6465 6661 756c 7473 2921  ......defaults)!
+00002370: da06 7461 7267 6574 da0b 6d6f 6465 6c5f  ..target..model_
+00002380: 636c 6173 7372 0a00 0000 7209 0000 00da  classr....r.....
+00002390: 1d50 4f57 4552 5f51 5545 5259 5f45 5854  .POWER_QUERY_EXT
+000023a0: 5241 5f43 4f4e 4e45 4354 494f 4e53 da06  RA_CONNECTIONS..
+000023b0: 6578 7465 6e64 72d0 0000 00da 0c69 735f  extendr......is_
+000023c0: 7375 7065 7275 7365 7272 6e00 0000 72a1  superuserrn...r.
+000023d0: 0000 00da 0666 696c 7465 7272 cb00 0000  .....filterr....
+000023e0: 727b 0000 0072 cc00 0000 72a4 0000 0072  r{...r....r....r
+000023f0: 1e00 0000 72b9 0000 0072 b800 0000 da05  ....r....r......
+00002400: 6669 7273 7472 d400 0000 da04 6578 6563  firstr......exec
+00002410: 727d 0000 00da 0767 6c6f 6261 6c73 72a2  r}.....globalsr.
+00002420: 0000 0072 d500 0000 7248 0000 00da 1075  ...r....rH.....u
+00002430: 7064 6174 655f 6f72 5f63 7265 6174 6572  pdate_or_creater
+00002440: 1300 0000 72a9 0000 00da 0670 6963 6b6c  ....r......pickl
+00002450: 65da 0564 756d 7073 7240 0000 0072 1c00  e..dumpsr@...r..
+00002460: 0000 2911 7252 0000 0072 a000 0000 729e  ..).rR...r....r.
+00002470: 0000 0072 8400 0000 72cd 0000 005a 1163  ...r....r....Z.c
+00002480: 6f6e 6e65 6374 696f 6e73 5f6d 6f64 656c  onnections_model
+00002490: da0b 636f 6e6e 6563 7469 6f6e 73da 076c  ..connections..l
+000024a0: 6f63 616c 735f da09 7369 676e 6174 7572  ocals_..signatur
+000024b0: 65da 0264 73da 0c72 6574 7572 6e5f 7661  e..ds..return_va
+000024c0: 6c75 6572 5300 0000 72d4 0000 0072 a800  luerS...r....r..
+000024d0: 0000 72c3 0000 0072 8800 0000 7236 0000  ..r....r....r6..
+000024e0: 0072 2900 0000 7229 0000 0072 2d00 0000  .r)...r)...r-...
+000024f0: 7286 0000 00ee 0000 0073 6600 0000 0006  r........sf.....
+00002500: 0a02 0801 0601 0401 0602 04fe 04ff 0406  ................
+00002510: 0604 02fc 0607 0801 1002 1402 0202 0c01  ................
+00002520: 0201 0201 0201 04fb 0406 02fa 0408 0201  ................
+00002530: 14ff 0403 0401 16ff 0203 0c02 1001 0c01  ................
+00002540: 0c02 0602 0801 02fe 0604 0601 0201 0202  ................
+00002550: 0201 0601 0801 08fc 04fd 0a0a 0a02 0c01  ................
+00002560: 1001 2001 7a09 5175 6572 792e 7275 6e63  .. .z.Query.runc
+00002570: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00002580: 0300 0000 4300 0000 732e 0000 0064 0164  ....C...s....d.d
+00002590: 026c 006d 017d 0101 007c 01a0 027c 006a  .l.m.}...|...|.j
+000025a0: 03a1 017d 027c 026a 037c 005f 047c 00a0  ...}.|.j.|._.|..
+000025b0: 05a1 0001 007c 026a 0353 0029 034e 7201  .....|.j.S.).Nr.
+000025c0: 0000 0029 01da 1472 756e 5f62 6163 6b67  ...)...run_backg
+000025d0: 726f 756e 645f 7175 6572 7929 06da 1870  round_query)...p
+000025e0: 6f77 6572 5f71 7565 7279 2e63 656c 6572  ower_query.celer
+000025f0: 795f 7461 736b 7372 e800 0000 da05 6465  y_tasksr......de
+00002600: 6c61 7972 9f00 0000 724e 0000 0072 8000  layr....rN...r..
+00002610: 0000 2903 7252 0000 0072 e800 0000 da03  ..).rR...r......
+00002620: 7265 7372 2900 0000 7229 0000 0072 2d00  resr)...r)...r-.
+00002630: 0000 725a 0000 0035 0100 0073 0a00 0000  ..rZ...5...s....
+00002640: 0001 0c02 0c01 0801 0801 7a0c 5175 6572  ..........z.Quer
+00002650: 792e 5f71 7565 7565 2904 4646 4e4e 2901  y._queue).FFNN).
+00002660: 5429 0346 4e46 292d 7248 0000 0072 4900  T).FNF)-rH...rI.
+00002670: 0000 724a 0000 0072 0d00 0000 7265 0000  ..rJ...r....re..
+00002680: 0072 7e00 0000 728d 0000 0072 8e00 0000  .r~...r....r....
+00002690: 7291 0000 0072 0a00 0000 7292 0000 0072  r....r....r....r
+000026a0: d000 0000 720b 0000 0072 d700 0000 727d  ....r....r....r}
+000026b0: 0000 0072 0f00 0000 7232 0000 0072 1d00  ...r....r2...r..
+000026c0: 0000 72a8 0000 0072 6700 0000 72b3 0000  ..r....rg...r...
+000026d0: 0072 a700 0000 72a6 0000 00da 0d44 6174  .r....r......Dat
+000026e0: 6554 696d 6546 6965 6c64 72aa 0000 0072  eTimeFieldr....r
+000026f0: 8f00 0000 da06 6163 7469 7665 7251 0000  ......activerQ..
+00002700: 0072 8b00 0000 724c 0000 0072 9300 0000  .r....rL...r....
+00002710: 7205 0000 0072 0200 0000 7280 0000 0072  r....r....r....r
+00002720: b100 0000 7204 0000 0072 0300 0000 72a4  ....r....r....r.
+00002730: 0000 00da 1151 7565 7279 4d61 7472 6978  .....QueryMatrix
+00002740: 5265 7375 6c74 72ab 0000 0072 c500 0000  Resultr....r....
+00002750: da0b 5175 6572 7952 6573 756c 7472 8600  ..QueryResultr..
+00002760: 0000 725a 0000 0072 9400 0000 7229 0000  ..rZ...r....r)..
+00002770: 0072 2900 0000 7282 0000 0072 2d00 0000  .r)...r....r-...
+00002780: 726e 0000 0097 0000 0073 5200 0000 0801  rn.......sR.....
+00002790: 0e01 0e01 0401 0aff 0603 1001 0e01 0e01  ................
+000027a0: 0401 0aff 0603 1001 1002 0e02 0c02 0e03  ................
+000027b0: 0e06 0001 0001 0001 00fb 0202 0201 0201  ................
+000027c0: 0601 0601 02fa 100b 1205 1007 1428 0001  .............(..
+000027d0: 0001 00fc 0202 0201 0601 0201 02fb 0c47  ...............G
+000027e0: 726e 0000 0063 0000 0000 0000 0000 0000  rn...c..........
+000027f0: 0000 0000 0000 0500 0000 4000 0000 73b6  ..........@...s.
+00002800: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
+00002810: 0164 0264 0364 048d 035a 0565 036a 0664  .d.d.d...Z.e.j.d
+00002820: 0164 0164 058d 025a 0765 036a 0464 0664  .d.d...Z.e.j.d.d
+00002830: 078d 015a 0865 036a 0965 0a65 036a 0b64  ...Z.e.j.e.e.j.d
+00002840: 0864 098d 035a 0c65 036a 0d64 0164 0164  .d...Z.e.j.d.d.d
+00002850: 058d 025a 0e65 0f65 1064 0164 0a8d 025a  ...Z.e.e.d.d...Z
+00002860: 1165 036a 0d64 0164 0164 0b64 0c8d 035a  .e.j.d.d.d.d...Z
+00002870: 1265 1364 0d9c 0164 0e64 0f84 045a 1465  .e.d...d.d...Z.e
+00002880: 1565 1664 0d9c 0164 1064 1184 0483 015a  .e.d...d.d.....Z
+00002890: 1765 1565 1864 0d9c 0164 1264 1384 0483  .e.e.d...d.d....
+000028a0: 015a 1965 1565 1a64 0d9c 0164 1464 1584  .Z.e.e.d...d.d..
+000028b0: 0483 015a 1b64 1653 0029 1772 b800 0000  ...Z.d.S.).r....
+000028c0: 54e9 c800 0000 4629 0372 6900 0000 7245  T.....F).ri...rE
+000028d0: 0000 0072 6a00 0000 729a 0000 00e9 6400  ...rj...r.....d.
+000028e0: 0000 a901 7245 0000 0072 bd00 0000 7296  ....rE...r....r.
+000028f0: 0000 0072 9800 0000 7a2c 416e 7920 6f74  ...r....z,Any ot
+00002900: 6865 7220 6174 7472 6962 7574 6520 746f  her attribute to
+00002910: 2070 6173 7320 746f 2074 6865 2066 6f72   pass to the for
+00002920: 6d61 7474 6572 2903 7247 0000 0072 4600  matter).rG...rF.
+00002930: 0000 da09 6865 6c70 5f74 6578 7472 4d00  ....help_textrM.
+00002940: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00002950: 0000 0004 0000 0043 0000 0073 1600 0000  .......C...s....
+00002960: 6401 7c00 6a00 6a01 9b00 6402 7c00 6a02  d.|.j.j...d.|.j.
+00002970: 9b00 9d04 5300 2903 4e7a 0a52 6573 756c  ....S.).Nz.Resul
+00002980: 7420 6f66 20da 0120 2903 72a3 0000 0072  t of .. ).r....r
+00002990: 7e00 0000 729e 0000 0072 5900 0000 7229  ~...r....rY...r)
+000029a0: 0000 0072 2900 0000 722d 0000 0072 8b00  ...r)...r-...r..
+000029b0: 0000 4901 0000 7302 0000 0000 017a 0f44  ..I...s......z.D
+000029c0: 6174 6173 6574 2e5f 5f73 7472 5f5f 6301  ataset.__str__c.
+000029d0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000029e0: 0000 0043 0000 0073 0c00 0000 7400 a001  ...C...s....t...
+000029f0: 7c00 6a02 a101 5300 7228 0000 0029 0372  |.j...S.r(...).r
+00002a00: e100 0000 da05 6c6f 6164 7372 3000 0000  ......loadsr0...
+00002a10: 7259 0000 0072 2900 0000 7229 0000 0072  rY...r)...r)...r
+00002a20: 2d00 0000 da04 6461 7461 4c01 0000 7302  -.....dataL...s.
+00002a30: 0000 0000 027a 0c44 6174 6173 6574 2e64  .....z.Dataset.d
+00002a40: 6174 6163 0100 0000 0000 0000 0000 0000  atac............
+00002a50: 0100 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+00002a60: 0074 007c 006a 0183 0153 0072 2800 0000  .t.|.j...S.r(...
+00002a70: 2902 72ba 0000 0072 3000 0000 7259 0000  ).r....r0...rY..
+00002a80: 0072 2900 0000 7229 0000 0072 2d00 0000  .r)...r)...r-...
+00002a90: da04 7369 7a65 5001 0000 7302 0000 0000  ..sizeP...s.....
+00002aa0: 027a 0c44 6174 6173 6574 2e73 697a 6563  .z.Dataset.sizec
+00002ab0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00002ac0: 0400 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
+00002ad0: 00a0 0164 0169 00a1 0253 0029 024e 729e  ...d.i...S.).Nr.
+00002ae0: 0000 0029 0272 a800 0000 72a2 0000 0072  ...).r....r....r
+00002af0: 5900 0000 7229 0000 0072 2900 0000 722d  Y...r)...r)...r-
+00002b00: 0000 0072 9e00 0000 5401 0000 7302 0000  ...r....T...s...
+00002b10: 0000 027a 1144 6174 6173 6574 2e61 7267  ...z.Dataset.arg
+00002b20: 756d 656e 7473 4e29 1c72 4800 0000 7249  umentsN).rH...rI
+00002b30: 0000 0072 4a00 0000 720d 0000 0072 6500  ...rJ...r....re.
+00002b40: 0000 72d3 0000 0072 ec00 0000 72aa 0000  ..r....r....r...
+00002b50: 0072 8e00 0000 7291 0000 0072 6e00 0000  .r....r....rn...
+00002b60: 7292 0000 0072 a300 0000 da0b 4269 6e61  r....r......Bina
+00002b70: 7279 4669 656c 6472 3000 0000 720f 0000  ryFieldr0...r...
+00002b80: 0072 3200 0000 72a8 0000 0072 d400 0000  .r2...r....r....
+00002b90: 7251 0000 0072 8b00 0000 7266 0000 0072  rQ...r....rf...r
+00002ba0: 0200 0000 72f6 0000 0072 b100 0000 72f7  ....r....r....r.
+00002bb0: 0000 0072 0300 0000 729e 0000 0072 2900  ...r....r....r).
+00002bc0: 0000 7229 0000 0072 2900 0000 722d 0000  ..r)...r)...r-..
+00002bd0: 0072 b800 0000 3e01 0000 7320 0000 0008  .r....>...s ....
+00002be0: 0110 010e 010c 0112 010e 010c 0104 0106  ................
+00002bf0: ff06 040e 0302 0110 0302 0110 0302 0172  ...............r
+00002c00: b800 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00002c10: 0000 0000 0006 0000 0040 0000 0073 5800  .........@...sX.
+00002c20: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
+00002c30: 6402 6402 6402 6403 8d04 5a05 6503 6a04  d.d.d.d...Z.e.j.
+00002c40: 6404 6506 6405 8d02 5a07 6503 6a08 6402  d.e.d...Z.e.j.d.
+00002c50: 6402 6406 8d02 5a09 650a 6407 9c01 6408  d.d...Z.e.d...d.
+00002c60: 6409 8404 5a0b 650c 650a 640a 9c02 640b  d...Z.e.e.d...d.
+00002c70: 640c 8404 5a0d 640d 5300 290e da09 466f  d...Z.d.S.)...Fo
+00002c80: 726d 6174 7465 7272 6800 0000 54a9 0472  rmatterrh...T..r
+00002c90: 4500 0000 7246 0000 0072 4700 0000 7269  E...rF...rG...ri
+00002ca0: 0000 00e9 0500 0000 a902 7245 0000 00da  ..........rE....
+00002cb0: 0763 686f 6963 6573 7295 0000 0072 4d00  .choicesr....rM.
+00002cc0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00002cd0: 0000 0001 0000 0043 0000 0073 0a00 0000  .......C...s....
+00002ce0: 7c00 6a00 7008 6401 5300 725e 0000 0072  |.j.p.d.S.r^...r
+00002cf0: 8a00 0000 7259 0000 0072 2900 0000 7229  ....rY...r)...r)
+00002d00: 0000 0072 2d00 0000 728b 0000 005e 0100  ...r-...r....^..
+00002d10: 0073 0200 0000 0001 7a11 466f 726d 6174  .s......z.Format
+00002d20: 7465 722e 5f5f 7374 725f 5f29 02da 0763  ter.__str__)...c
+00002d30: 6f6e 7465 7874 7231 0000 0063 0200 0000  ontextr1...c....
+00002d40: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00002d50: 4300 0000 738e 0000 007c 006a 0064 016b  C...s....|.j.d.k
+00002d60: 0272 2274 017c 0164 0219 006a 0283 017d  .r"t.|.d...j...}
+00002d70: 027c 02a0 0364 01a1 0153 007c 006a 0472  .|...d...S.|.j.r
+00002d80: 3474 057c 006a 0483 017d 036e 4c7c 006a  4t.|.j...}.nL|.j
+00002d90: 0064 036b 0272 5674 017c 0164 0219 006a  .d.k.rVt.|.d...j
+00002da0: 0283 017d 027c 02a0 0364 03a1 0153 007c  ...}.|...d...S.|
+00002db0: 006a 0064 046b 0272 7874 017c 0164 0219  .j.d.k.rxt.|.d..
+00002dc0: 006a 0283 017d 027c 02a0 0364 04a1 0153  .j...}.|...d...S
+00002dd0: 0074 0664 0583 0182 017c 03a0 0774 087c  .t.d.....|...t.|
+00002de0: 0183 01a1 0153 0029 064e 7225 0000 0072  .....S.).Nr%...r
+00002df0: c300 0000 7223 0000 0072 2700 0000 7a10  ....r#...r'...z.
+00002e00: 556e 6162 6c65 2074 6f20 7265 6e64 6572  Unable to render
+00002e10: 2909 da0c 636f 6e74 656e 745f 7479 7065  )...content_type
+00002e20: 721f 0000 0072 f600 0000 da06 6578 706f  r....r......expo
+00002e30: 7274 727d 0000 0072 1100 0000 72b4 0000  rtr}...r....r...
+00002e40: 00da 0672 656e 6465 7272 1000 0000 2904  ...renderr....).
+00002e50: 7252 0000 0072 fe00 0000 da02 6474 da03  rR...r......dt..
+00002e60: 7470 6c72 2900 0000 7229 0000 0072 2d00  tplr)...r)...r-.
+00002e70: 0000 7201 0100 0061 0100 0073 1a00 0000  ..r....a...s....
+00002e80: 0001 0a01 0e01 0a02 0601 0c01 0a01 0e01  ................
+00002e90: 0a01 0a01 0e01 0a02 0802 7a10 466f 726d  ..........z.Form
+00002ea0: 6174 7465 722e 7265 6e64 6572 4e29 0e72  atter.renderN).r
+00002eb0: 4800 0000 7249 0000 0072 4a00 0000 720d  H...rI...rJ...r.
+00002ec0: 0000 0072 6500 0000 727e 0000 00da 094d  ...re...r~.....M
+00002ed0: 494d 4554 5950 4553 72ff 0000 0072 8d00  IMETYPESr....r..
+00002ee0: 0000 727d 0000 0072 5100 0000 728b 0000  ..r}...rQ...r...
+00002ef0: 0072 0300 0000 7201 0100 0072 2900 0000  .r....r....r)...
+00002f00: 7229 0000 0072 2900 0000 722d 0000 0072  r)...r)...r-...r
+00002f10: f900 0000 5901 0000 730a 0000 0008 0112  ....Y...s.......
+00002f20: 010e 010e 020e 0372 f900 0000 6300 0000  .......r....c...
+00002f30: 0000 0000 0000 0000 0000 0000 0008 0000  ................
+00002f40: 0000 0000 0073 1c01 0000 6500 5a01 6400  .....s....e.Z.d.
+00002f50: 5a02 6503 6a04 6401 6402 6402 6402 6403  Z.e.j.d.d.d.d.d.
+00002f60: 8d04 5a05 6503 6a04 6401 6402 6402 6404  ..Z.e.j.d.d.d.d.
+00002f70: 8d03 5a06 6503 6a07 6508 6503 6a09 6405  ..Z.e.j.e.e.j.d.
+00002f80: 8d02 5a0a 6503 6a07 650b 6503 6a09 6405  ..Z.e.j.e.e.j.d.
+00002f90: 8d02 5a0c 6503 6a0d 6402 6406 8d01 5a0e  ..Z.e.j.d.d...Z.
+00002fa0: 6503 6a07 650f 8300 6402 6402 6503 6a09  e.j.e...d.d.e.j.
+00002fb0: 6407 6408 8d05 5a10 6503 6a11 650f 8300  d.d...Z.e.j.e...
+00002fc0: 6402 6407 6409 8d03 5a12 6503 6a04 640a  d.d.d...Z.e.j.d.
+00002fd0: 6402 6402 640b 640c 6513 8300 6701 640d  d.d.d.d.e...g.d.
+00002fe0: 8d06 5a14 6503 6a15 6402 6402 640e 8d02  ..Z.e.j.d.d.d...
+00002ff0: 5a16 6503 6a17 640f 6406 8d01 5a18 641f  Z.e.j.d.d...Z.d.
+00003000: 6519 6519 651a 651b 1900 651a 651b 1900  e.e.e.e...e.e...
+00003010: 6411 6412 9c05 8700 6601 6413 6414 840d  d.d.....f.d.d...
+00003020: 5a1c 6420 6519 651d 6415 9c02 6416 6417  Z.d e.e.d...d.d.
+00003030: 8405 5a1e 651f 6418 9c01 6419 641a 8404  ..Z.e.d...d.d...
+00003040: 5a20 651f 6418 9c01 641b 641c 8404 5a21  Z e.d...d.d...Z!
+00003050: 651f 6418 9c01 641d 641e 8404 5a22 8700  e.d...d.d...Z"..
+00003060: 0400 5a23 5300 2921 da06 5265 706f 7274  ..Z#S.)!..Report
+00003070: 7268 0000 0054 72fa 0000 0072 4400 0000  rh...Tr....rD...
+00003080: 7297 0000 0072 9b00 0000 726f 0000 0072  r....r....ro...r
+00003090: 7000 0000 a902 7246 0000 0072 7200 0000  p.....rF...rr...
+000030a0: e91e 0000 007a 2c52 6566 7265 7368 2065  .....z,Refresh e
+000030b0: 7665 7279 2028 652e 672e 2033 202d 2031  very (e.g. 3 - 1
+000030c0: 2f33 202d 206d 6f6e 202d 2031 2f33 2c4d  /3 - mon - 1/3,M
+000030d0: 6f6e 297a 1b6d 6f6e 2c74 7565 2c77 6564  on)z.mon,tue,wed
+000030e0: 2c74 6875 2c66 7269 2c73 6174 2c73 756e  ,thu,fri,sat,sun
+000030f0: 2906 7245 0000 0072 4700 0000 7246 0000  ).rE...rG...rF..
+00003100: 0072 f300 0000 726c 0000 0072 6d00 0000  .r....rl...rm...
+00003110: 729a 0000 0069 6d01 0000 464e 7278 0000  r....im...FNrx..
+00003120: 0063 0500 0000 0000 0000 0000 0000 0500  .c..............
+00003130: 0000 0600 0000 0300 0000 7324 0000 007c  ..........s$...|
+00003140: 006a 0073 0e7c 006a 017c 005f 0074 0283  .j.s.|.j.|._.t..
+00003150: 00a0 037c 017c 027c 037c 04a1 0401 0064  ...|.|.|.|.....d
+00003160: 0053 0072 2800 0000 2904 da0e 646f 6375  .S.r(...)...docu
+00003170: 6d65 6e74 5f74 6974 6c65 727e 0000 0072  ment_titler~...r
+00003180: 7f00 0000 7280 0000 0072 8100 0000 7282  ....r....r....r.
+00003190: 0000 0072 2900 0000 722d 0000 0072 8000  ...r)...r-...r..
+000031a0: 0000 8f01 0000 7306 0000 0000 0706 0108  ......s.........
+000031b0: 017a 0b52 6570 6f72 742e 7361 7665 2902  .z.Report.save).
+000031c0: da09 7275 6e5f 7175 6572 7972 3100 0000  ..run_queryr1...
+000031d0: 6302 0000 0000 0000 0000 0000 000b 0000  c...............
+000031e0: 000b 0000 0043 0000 0073 2201 0000 7c00  .....C...s"...|.
+000031f0: 6a00 7d02 6700 7d03 7c01 7216 7c02 a001  j.}.g.}.|.r.|...
+00003200: a100 0100 7c02 6a02 a003 a100 4400 5de6  ....|.j.....D.].
+00003210: 7d04 7c04 6a04 732c 7120 7a94 7c04 6a05  }.|.j.s,q z.|.j.
+00003220: 7d05 7c04 6a06 7250 7c05 a007 7408 a009  }.|.j.rP|...t...
+00003230: 7c04 6a06 a101 704c 6900 a101 0100 7c00  |.j...pLi.....|.
+00003240: 6a0a 7260 7c00 6a0a 7c05 1600 6e04 7c00  j.r`|.j.|...n.|.
+00003250: 6a0a 7d06 7c00 6a0b a00c 7c04 7c00 7c06  j.}.|.j...|.|.|.
+00003260: 7c05 6401 9c04 a101 7d07 740d 6a0e 6a0f  |.d.....}.t.j.j.
+00003270: 7c00 7c04 7c06 7c00 6a0b 6a10 7408 a011  |.|.|.|.j.j.t...
+00003280: 7c07 a101 7c04 6a05 6402 9c04 6403 8d03  |...|.j.d...d...
+00003290: 5c02 7d08 7d09 7c03 a012 7c08 6a13 7414  \.}.}.|...|.j.t.
+000032a0: 7c08 6a15 8301 6602 a101 0100 5700 7120  |.j...f.....W.q 
+000032b0: 0400 7416 9001 7904 0100 7d0a 0100 7a2a  ..t...y...}...z*
+000032c0: 7417 a018 7c0a a101 0100 7c03 a012 7c04  t...|.....|...|.
+000032d0: 6a13 7419 7c0a 8301 6602 a101 0100 5700  j.t.|...f.....W.
+000032e0: 5900 6400 7d0a 7e0a 7120 6400 7d0a 7e0a  Y.d.}.~.q d.}.~.
+000032f0: 3000 3000 7120 741a a01b a100 7c00 5f1c  0.0.q t.....|._.
+00003300: 7c03 9001 731e 6404 6701 7d03 7c03 5300  |...s.d.g.}.|.S.
+00003310: 2905 4e29 0472 c300 0000 da06 7265 706f  ).N).r......repo
+00003320: 7274 da05 7469 746c 6572 fe00 0000 2904  rt..titler....).
+00003330: 720b 0100 0072 ff00 0000 da06 6f75 7470  r....r......outp
+00003340: 7574 729e 0000 0029 0372 0a01 0000 72c3  utr....).r....r.
+00003350: 0000 0072 d600 0000 7a14 4e6f 2044 6174  ...r....z.No Dat
+00003360: 6173 6574 2061 7661 696c 6162 6c65 291d  aset available).
+00003370: 72a3 0000 0072 c500 0000 72bd 0000 00da  r....r....r.....
+00003380: 0361 6c6c 72f7 0000 0072 9e00 0000 72d4  .allr....r....r.
+00003390: 0000 00da 0675 7064 6174 6572 e100 0000  .....updater....
+000033a0: 72f5 0000 0072 0801 0000 da09 666f 726d  r....r......form
+000033b0: 6174 7465 7272 0101 0000 da0e 5265 706f  atterr......Repo
+000033c0: 7274 446f 6375 6d65 6e74 72a1 0000 0072  rtDocumentr....r
+000033d0: e000 0000 72ff 0000 0072 e200 0000 da06  ....r....r......
+000033e0: 6170 7065 6e64 72b9 0000 0072 ba00 0000  appendr....r....
+000033f0: 720c 0100 0072 4000 0000 72bb 0000 0072  r....r@...r....r
+00003400: bc00 0000 7251 0000 0072 1300 0000 72a9  ....rQ...r....r.
+00003410: 0000 0072 aa00 0000 290b 7252 0000 0072  ...r....).rR...r
+00003420: 0901 0000 72a3 0000 0072 5300 0000 72c3  ....r....rS...r.
+00003430: 0000 0072 fe00 0000 720b 0100 0072 0c01  ...r....r....r..
+00003440: 0000 72eb 0000 0072 8800 0000 7236 0000  ..r....r....r6..
+00003450: 0072 2900 0000 7229 0000 0072 2d00 0000  .r)...r)...r-...
+00003460: da07 6578 6563 7574 659a 0100 0073 4e00  ..execute....sN.
+00003470: 0000 0002 0601 0401 0401 0801 0e01 0601  ................
+00003480: 0201 0201 0601 0601 1604 04ff 0c02 04fd  ................
+00003490: 0205 0602 0201 0201 0201 02fc 04ff 0408  ................
+000034a0: 0601 0201 0202 0201 0601 0801 04fc 04fd  ................
+000034b0: 0a0a 1a01 1001 0a01 2c01 0a01 0601 0601  ........,.......
+000034c0: 7a0e 5265 706f 7274 2e65 7865 6375 7465  z.Report.execute
+000034d0: 724d 0000 0063 0100 0000 0000 0000 0000  rM...c..........
+000034e0: 0000 0100 0000 0100 0000 4300 0000 730a  ..........C...s.
+000034f0: 0000 007c 006a 0070 0864 0153 0072 5e00  ...|.j.p.d.S.r^.
+00003500: 0000 728a 0000 0072 5900 0000 7229 0000  ..r....rY...r)..
+00003510: 0072 2900 0000 722d 0000 0072 8b00 0000  .r)...r-...r....
+00003520: c801 0000 7302 0000 0000 017a 0e52 6570  ....s......z.Rep
+00003530: 6f72 742e 5f5f 7374 725f 5f63 0100 0000  ort.__str__c....
+00003540: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00003550: 4300 0000 7310 0000 0074 0064 017c 006a  C...s....t.d.|.j
+00003560: 0167 0164 028d 0253 0029 034e 7a12 706f  .g.d...S.).Nz.po
+00003570: 7765 725f 7175 6572 793a 7265 706f 7274  wer_query:report
+00003580: a901 72c0 0000 0029 0272 1200 0000 72b9  ..r....).r....r.
+00003590: 0000 0072 5900 0000 7229 0000 0072 2900  ...rY...r)...r).
+000035a0: 0000 722d 0000 00da 1067 6574 5f61 6273  ..r-.....get_abs
+000035b0: 6f6c 7574 655f 7572 6ccb 0100 0073 0200  olute_url....s..
+000035c0: 0000 0001 7a17 5265 706f 7274 2e67 6574  ....z.Report.get
+000035d0: 5f61 6273 6f6c 7574 655f 7572 6c63 0100  _absolute_urlc..
+000035e0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+000035f0: 0000 4300 0000 732e 0000 0064 0164 026c  ..C...s....d.d.l
+00003600: 006d 017d 0101 007c 01a0 027c 006a 03a1  .m.}...|...|.j..
+00003610: 017d 027c 026a 037c 005f 047c 00a0 05a1  .}.|.j.|._.|....
+00003620: 0001 007c 026a 0353 0029 034e 7201 0000  ...|.j.S.).Nr...
+00003630: 0029 01da 0e72 6566 7265 7368 5f72 6570  .)...refresh_rep
+00003640: 6f72 7429 0672 e900 0000 7215 0100 0072  ort).r....r....r
+00003650: ea00 0000 729f 0000 0072 4e00 0000 7280  ....r....rN...r.
+00003660: 0000 0029 0372 5200 0000 7215 0100 0072  ...).rR...r....r
+00003670: eb00 0000 7229 0000 0072 2900 0000 722d  ....r)...r)...r-
+00003680: 0000 0072 5a00 0000 ce01 0000 730a 0000  ...rZ.......s...
+00003690: 0000 010c 020c 0108 0108 017a 0d52 6570  ...........z.Rep
+000036a0: 6f72 742e 5f71 7565 7565 2904 4646 4e4e  ort._queue).FFNN
+000036b0: 2901 4629 2472 4800 0000 7249 0000 0072  ).F)$rH...rI...r
+000036c0: 4a00 0000 720d 0000 0072 6500 0000 727e  J...r....re...r~
+000036d0: 0000 0072 0801 0000 7291 0000 0072 6e00  ...r....r....rn.
+000036e0: 0000 7292 0000 0072 a300 0000 72f9 0000  ..r....r....r...
+000036f0: 0072 0f01 0000 728f 0000 0072 ed00 0000  .r....r....r....
+00003700: 720a 0000 0072 d000 0000 da0f 4d61 6e79  r....r......Many
+00003710: 546f 4d61 6e79 4669 656c 64da 0f6c 696d  ToManyField..lim
+00003720: 6974 5f61 6363 6573 735f 746f 7220 0000  it_access_tor ..
+00003730: 005a 0966 7265 7175 656e 6365 72ec 0000  .Z.frequencer...
+00003740: 0072 aa00 0000 da0c 496e 7465 6765 7246  .r......IntegerF
+00003750: 6965 6c64 5a0d 7661 6c69 6469 7479 5f64  ieldZ.validity_d
+00003760: 6179 7372 9300 0000 7205 0000 0072 0200  aysr....r....r..
+00003770: 0000 7280 0000 00da 0c52 6570 6f72 7452  ..r......ReportR
+00003780: 6573 756c 7472 1201 0000 7251 0000 0072  esultr....rQ...r
+00003790: 8b00 0000 7214 0100 0072 5a00 0000 7294  ....r....rZ...r.
+000037a0: 0000 0072 2900 0000 7229 0000 0072 8200  ...r)...r)...r..
+000037b0: 0000 722d 0000 0072 0501 0000 7401 0000  ..r-...r....t...
+000037c0: 7350 0000 0008 0112 0110 0110 0110 010c  sP..............
+000037d0: 0104 0104 0102 0102 0104 0102 fb06 0704  ................
+000037e0: 0108 ff06 0304 0102 0102 0102 0102 0102  ................
+000037f0: 0106 fa06 080e 010c 0400 0100 0100 0100  ................
+00003800: fb02 0202 0102 0106 0106 0102 fa10 0b12  ................
+00003810: 2e0e 030e 0372 0501 0000 6300 0000 0000  .....r....c.....
+00003820: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00003830: 0000 0073 2400 0000 6500 5a01 6400 5a02  ...s$...e.Z.d.Z.
+00003840: 6503 6a04 6401 9c01 8700 6601 6402 6403  e.j.d.....f.d.d.
+00003850: 840c 5a05 8700 0400 5a06 5300 2904 da15  ..Z.....Z.S.)...
+00003860: 5265 706f 7274 446f 6375 6d65 6e74 4d61  ReportDocumentMa
+00003870: 6e61 6765 7272 4d00 0000 6301 0000 0000  nagerrM...c.....
+00003880: 0000 0000 0000 0001 0000 0003 0000 0003  ................
+00003890: 0000 0073 1000 0000 7400 8300 a001 a100  ...s....t.......
+000038a0: a002 6401 a101 5300 2902 4e72 0a01 0000  ..d...S.).Nr....
+000038b0: 2903 727f 0000 00da 0c67 6574 5f71 7565  ).r......get_que
+000038c0: 7279 7365 74da 0e73 656c 6563 745f 7265  ryset..select_re
+000038d0: 6c61 7465 6472 5900 0000 7282 0000 0072  latedrY...r....r
+000038e0: 2900 0000 722d 0000 0072 1b01 0000 d801  )...r-...r......
+000038f0: 0000 7302 0000 0000 017a 2252 6570 6f72  ..s......z"Repor
+00003900: 7444 6f63 756d 656e 744d 616e 6167 6572  tDocumentManager
+00003910: 2e67 6574 5f71 7565 7279 7365 7429 0772  .get_queryset).r
+00003920: 4800 0000 7249 0000 0072 4a00 0000 720d  H...rI...rJ...r.
+00003930: 0000 00da 0851 7565 7279 5365 7472 1b01  .....QuerySetr..
+00003940: 0000 7294 0000 0072 2900 0000 7229 0000  ..r....r)...r)..
+00003950: 0072 8200 0000 722d 0000 0072 1a01 0000  .r....r-...r....
+00003960: d701 0000 7302 0000 0008 0172 1a01 0000  ....s......r....
+00003970: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00003980: 0005 0000 0040 0000 0073 d600 0000 6500  .....@...s....e.
+00003990: 5a01 6400 5a02 6503 6a04 6401 6402 8d01  Z.d.Z.e.j.d.d...
+000039a0: 5a05 6503 6a06 6403 6404 8d01 5a07 6503  Z.e.j.d.d...Z.e.
+000039b0: 6a08 6509 6503 6a0a 6405 6406 8d03 5a0b  j.e.e.j.d.d...Z.
+000039c0: 6503 6a08 650c 6503 6a0a 6407 8d02 5a0d  e.j.e.e.j.d...Z.
+000039d0: 6503 6a0e 6401 6401 6408 8d02 5a0f 6503  e.j.d.d.d...Z.e.
+000039e0: 6a10 6511 6512 6409 8d02 5a13 6503 6a14  j.e.e.d...Z.e.j.
+000039f0: 6515 8300 6401 640a 640b 8d03 5a16 6503  e...d.d.d...Z.e.
+00003a00: 6a06 640c 6517 640d 8d02 5a18 6519 8300  j.d.e.d...Z.e...
+00003a10: 5a1a 4700 640e 640f 8400 640f 8302 5a1b  Z.G.d.d...d...Z.
+00003a20: 651c 6410 9c01 6411 6412 8404 5a1d 651e  e.d...d.d...Z.e.
+00003a30: 651f 6410 9c01 6413 6414 8404 8301 5a20  e.d...d.d.....Z 
+00003a40: 651e 6521 6410 9c01 6415 6416 8404 8301  e.e!d...d.d.....
+00003a50: 5a22 651c 6410 9c01 6417 6418 8404 5a23  Z"e.d...d.d...Z#
+00003a60: 6419 5300 291a 7210 0100 0054 2901 da08  d.S.).r....T)...
+00003a70: 6175 746f 5f6e 6f77 692c 0100 0072 f200  auto_nowi,...r..
+00003a80: 0000 da09 646f 6375 6d65 6e74 7372 9600  ....documentsr..
+00003a90: 0000 7297 0000 0072 9a00 0000 2902 726c  ..r....r....).rl
+00003aa0: 0000 0072 9900 0000 726f 0000 0072 0601  ...r....ro...r..
+00003ab0: 0000 72fb 0000 0072 fc00 0000 6300 0000  ..r....r....c...
+00003ac0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00003ad0: 0040 0000 0073 1000 0000 6500 5a01 6400  .@...s....e.Z.d.
+00003ae0: 5a02 6401 5a03 6402 5300 2903 7a13 5265  Z.d.Z.d.S.).z.Re
+00003af0: 706f 7274 446f 6375 6d65 6e74 2e4d 6574  portDocument.Met
+00003b00: 6129 0272 0a01 0000 72c3 0000 004e 2904  a).r....r....N).
+00003b10: 7248 0000 0072 4900 0000 724a 0000 00da  rH...rI...rJ....
+00003b20: 0f75 6e69 7175 655f 746f 6765 7468 6572  .unique_together
+00003b30: 7229 0000 0072 2900 0000 7229 0000 0072  r)...r)...r)...r
+00003b40: 2d00 0000 724c 0000 00ec 0100 0073 0200  -...rL.......s..
+00003b50: 0000 0801 724c 0000 0072 4d00 0000 6301  ....rL...rM...c.
+00003b60: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00003b70: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+00003b80: 5300 7228 0000 0029 0172 0b01 0000 7259  S.r(...).r....rY
+00003b90: 0000 0072 2900 0000 7229 0000 0072 2d00  ...r)...r)...r-.
+00003ba0: 0000 728b 0000 00ef 0100 0073 0200 0000  ..r........s....
+00003bb0: 0001 7a16 5265 706f 7274 446f 6375 6d65  ..z.ReportDocume
+00003bc0: 6e74 2e5f 5f73 7472 5f5f 6301 0000 0000  nt.__str__c.....
+00003bd0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00003be0: 0000 0073 0c00 0000 7400 a001 7c00 6a02  ...s....t...|.j.
+00003bf0: a101 5300 7228 0000 0029 0372 e100 0000  ..S.r(...).r....
+00003c00: 72f5 0000 0072 0c01 0000 7259 0000 0072  r....r....rY...r
+00003c10: 2900 0000 7229 0000 0072 2d00 0000 72f6  )...r)...r-...r.
+00003c20: 0000 00f2 0100 0073 0200 0000 0002 7a13  .......s......z.
+00003c30: 5265 706f 7274 446f 6375 6d65 6e74 2e64  ReportDocument.d
+00003c40: 6174 6163 0100 0000 0000 0000 0000 0000  atac............
+00003c50: 0100 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+00003c60: 0074 007c 006a 0183 0153 0072 2800 0000  .t.|.j...S.r(...
+00003c70: 2902 72ba 0000 0072 0c01 0000 7259 0000  ).r....r....rY..
+00003c80: 0072 2900 0000 7229 0000 0072 2d00 0000  .r)...r)...r-...
+00003c90: 72f7 0000 00f6 0100 0073 0200 0000 0002  r........s......
+00003ca0: 7a13 5265 706f 7274 446f 6375 6d65 6e74  z.ReportDocument
+00003cb0: 2e73 697a 6563 0100 0000 0000 0000 0000  .sizec..........
+00003cc0: 0000 0100 0000 0400 0000 4300 0000 7316  ..........C...s.
+00003cd0: 0000 0074 0064 017c 006a 016a 027c 006a  ...t.d.|.j.j.|.j
+00003ce0: 0267 0264 028d 0253 0029 034e 7a14 706f  .g.d...S.).Nz.po
+00003cf0: 7765 725f 7175 6572 793a 646f 6375 6d65  wer_query:docume
+00003d00: 6e74 7213 0100 0029 0372 1200 0000 720a  ntr....).r....r.
+00003d10: 0100 0072 b900 0000 7259 0000 0072 2900  ...r....rY...r).
+00003d20: 0000 7229 0000 0072 2d00 0000 7214 0100  ..r)...r-...r...
+00003d30: 00fa 0100 0073 0200 0000 0001 7a1f 5265  .....s......z.Re
+00003d40: 706f 7274 446f 6375 6d65 6e74 2e67 6574  portDocument.get
+00003d50: 5f61 6273 6f6c 7574 655f 7572 6c4e 2924  _absolute_urlN)$
+00003d60: 7248 0000 0072 4900 0000 724a 0000 0072  rH...rI...rJ...r
+00003d70: 0d00 0000 72ec 0000 0072 ad00 0000 7265  ....r....r....re
+00003d80: 0000 0072 0b01 0000 7291 0000 0072 0501  ...r....r....r..
+00003d90: 0000 7292 0000 0072 0a01 0000 72b8 0000  ..r....r....r...
+00003da0: 0072 c300 0000 72f8 0000 0072 0c01 0000  .r....r....r....
+00003db0: 720f 0000 0072 3200 0000 721d 0000 0072  r....r2...r....r
+00003dc0: 9e00 0000 7216 0100 0072 0a00 0000 7217  ....r....r....r.
+00003dd0: 0100 0072 0401 0000 72ff 0000 0072 1a01  ...r....r....r..
+00003de0: 0000 72a1 0000 0072 4c00 0000 7251 0000  ..r....rL...rQ..
+00003df0: 0072 8b00 0000 7215 0000 0072 0200 0000  .r....r....r....
+00003e00: 72f6 0000 0072 b100 0000 72f7 0000 0072  r....r....r....r
+00003e10: 1401 0000 7229 0000 0072 2900 0000 7229  ....r)...r)...r)
+00003e20: 0000 0072 2d00 0000 7210 0100 00dc 0100  ...r-...r.......
+00003e30: 0073 2800 0000 0801 0c01 0c01 0401 08ff  .s(.............
+00003e40: 0603 1001 0e01 0e01 0401 08ff 0603 0e02  ................
+00003e50: 0602 0e03 0e03 0201 1003 0201 1003 7210  ..............r.
+00003e60: 0100 0029 5072 3d00 0000 da07 6c6f 6767  ...)Pr=.....logg
+00003e70: 696e 6772 e100 0000 da06 7479 7069 6e67  ingr......typing
+00003e80: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
+00003e90: 0500 0000 7206 0000 0072 0700 0000 da0b  ....r....r......
+00003ea0: 646a 616e 676f 2e61 7070 7372 0800 0000  django.appsr....
+00003eb0: 72c6 0000 00da 0b64 6a61 6e67 6f2e 636f  r......django.co
+00003ec0: 6e66 7209 0000 00da 1364 6a61 6e67 6f2e  nfr......django.
+00003ed0: 636f 6e74 7269 622e 6175 7468 720a 0000  contrib.authr...
+00003ee0: 00da 2264 6a61 6e67 6f2e 636f 6e74 7269  .."django.contri
+00003ef0: 622e 636f 6e74 656e 7474 7970 6573 2e6d  b.contenttypes.m
+00003f00: 6f64 656c 7372 0b00 0000 da16 646a 616e  odelsr......djan
+00003f10: 676f 2e63 6f72 652e 6578 6365 7074 696f  go.core.exceptio
+00003f20: 6e73 720c 0000 00da 0964 6a61 6e67 6f2e  nsr......django.
+00003f30: 6462 720d 0000 0072 0e00 0000 da10 646a  dbr....r......dj
+00003f40: 616e 676f 2e64 622e 6d6f 6465 6c73 720f  ango.db.modelsr.
+00003f50: 0000 00da 0f64 6a61 6e67 6f2e 7465 6d70  .....django.temp
+00003f60: 6c61 7465 7210 0000 0072 1100 0000 da0b  later....r......
+00003f70: 646a 616e 676f 2e75 726c 7372 1200 0000  django.urlsr....
+00003f80: da0c 646a 616e 676f 2e75 7469 6c73 7213  ..django.utilsr.
+00003f90: 0000 005a 1a64 6a61 6e67 6f2e 7574 696c  ...Z.django.util
+00003fa0: 732e 6461 7465 7469 6d65 5f73 6166 6572  s.datetime_safer
+00003fb0: 1400 0000 da17 646a 616e 676f 2e75 7469  ......django.uti
+00003fc0: 6c73 2e66 756e 6374 696f 6e61 6c72 1500  ls.functionalr..
+00003fd0: 0000 da11 646a 616e 676f 2e75 7469 6c73  ....django.utils
+00003fe0: 2e74 6578 7472 1600 0000 7257 0000 0072  .textr....rW...r
+00003ff0: 1700 0000 da0d 6365 6c65 7279 2e72 6573  ......celery.res
+00004000: 756c 7472 1800 0000 da0c 6e61 7475 7261  ultr......natura
+00004010: 6c5f 6b65 7973 7219 0000 00da 0a73 656e  l_keysr......sen
+00004020: 7472 795f 7364 6b72 1a00 0000 721b 0000  try_sdkr....r...
+00004030: 005a 1670 6f77 6572 5f71 7565 7279 2e65  .Z.power_query.e
+00004040: 7863 6570 7469 6f6e 7372 1c00 0000 5a10  xceptionsr....Z.
+00004050: 706f 7765 725f 7175 6572 792e 6a73 6f6e  power_query.json
+00004060: 721d 0000 005a 1170 6f77 6572 5f71 7565  r....Z.power_que
+00004070: 7279 2e75 7469 6c73 721e 0000 0072 1f00  ry.utilsr....r..
+00004080: 0000 5a16 706f 7765 725f 7175 6572 792e  ..Z.power_query.
+00004090: 7661 6c69 6461 746f 7273 7220 0000 00da  validatorsr ....
+000040a0: 0967 6574 4c6f 6767 6572 7248 0000 0072  .getLoggerrH...r
+000040b0: bb00 0000 5a0c 6d69 6d65 7479 7065 5f6d  ....Z.mimetype_m
+000040c0: 6170 da05 6974 656d 7372 0401 0000 72b1  ap..itemsr....r.
+000040d0: 0000 0072 5100 0000 5a0e 446f 6375 6d65  ...rQ...Z.Docume
+000040e0: 6e74 5265 7375 6c74 7219 0100 0072 ef00  ntResultr....r..
+000040f0: 0000 72ee 0000 0072 4100 0000 da05 4d6f  ..r....rA.....Mo
+00004100: 6465 6c72 4200 0000 7267 0000 0072 6e00  delrB...rg...rn.
+00004110: 0000 72b8 0000 0072 f900 0000 7205 0100  ..r....r....r...
+00004120: 0072 c800 0000 721a 0100 0072 1001 0000  .r....r....r....
+00004130: 7229 0000 0072 2900 0000 7229 0000 0072  r)...r)...r)...r
+00004140: 2d00 0000 da08 3c6d 6f64 756c 653e 0100  -.....<module>..
+00004150: 0000 7362 0000 0008 0108 0108 0120 020c  ..sb......... ..
+00004160: 010c 010c 010c 010c 0110 010c 0110 010c  ................
+00004170: 010c 010c 010c 010c 0208 010c 010c 010c  ................
+00004180: 0110 020c 010c 0110 010c 020a 0302 0102  ................
+00004190: 0102 0102 0102 0102 0102 f906 0a12 0214  ................
+000041a0: 0112 010c 0114 0310 0f12 2714 2e16 7f00  ..........'.....
+000041b0: 2814 1b14 1b16 6312 05                   (.....c..
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/urls.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/urls.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x7da5af64 (Thu Jul 13 07:19:25 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 368
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/utils.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x67a5af64 (Thu Jul 13 07:19:03 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 5041
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/utils.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:19:03 2023 UTC, .py size: 5041 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 67a5 af64 b113 0000  a.......g..d....
+00000000: 610d 0d0a 0000 0000 cd97 b764 b113 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4201 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000060: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000070: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/validators.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/validators.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xf5a4af64 (Thu Jul 13 07:17:09 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 453
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/validators.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/validators.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:17:09 2023 UTC, .py size: 453 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 f5a4 af64 c501 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 cd97 b764 c501 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6503 4700 6404 6405 8400 6405 8302  ..e.G.d.d...d...
 00000060: 8301 5a06 6406 5300 2907 e900 0000 0029  ..Z.d.S.)......)
 00000070: 01da 0f56 616c 6964 6174 696f 6e45 7272  ...ValidationErr
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/views.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/views.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x23c2af64 (Thu Jul 13 09:21:39 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 3360
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/views.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/views.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 09:21:39 2023 UTC, .py size: 3360 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 23c2 af64 200d 0000  a.......#..d ...
+00000000: 610d 0d0a 0000 0000 cd97 b764 200d 0000  a..........d ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 fe00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/widget.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/widget.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83a4af64 (Thu Jul 13 07:15:15 2023 UTC)
+moddate:  0xcd97b764 (Wed Jul 19 07:59:09 2023 UTC)
 files sz: 3111
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.3/src/power_query/__pycache__/widget.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/__pycache__/widget.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:15:15 2023 UTC, .py size: 3111 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 83a4 af64 270c 0000  a..........d'...
+00000000: 610d 0d0a 0000 0000 5002 b964 ab0b 0000  a.......P..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6504 725c 6400  d.l.m.Z...e.r\d.
@@ -44,185 +44,184 @@
 000002b0: 7370 6163 652f 756e 6963 6566 2d70 6f77  space/unicef-pow
 000002c0: 6572 2d71 7565 7279 2f73 7263 2f70 6f77  er-query/src/pow
 000002d0: 6572 5f71 7565 7279 2f77 6964 6765 742e  er_query/widget.
 000002e0: 7079 7216 0000 000f 0000 0073 0800 0000  pyr........s....
 000002f0: 0001 0c01 1201 0a01 7a18 466f 726d 6174  ........z.Format
 00000300: 7465 7245 6469 746f 722e 5f5f 696e 6974  terEditor.__init
 00000310: 5f5f 6300 0000 0000 0000 0000 0000 0000  __c.............
-00000320: 0000 000a 0000 0040 0000 0073 6c00 0000  .......@...sl...
+00000320: 0000 0008 0000 0040 0000 0073 6000 0000  .......@...s`...
 00000330: 6500 5a01 6400 5a02 6401 6503 6402 8301  e.Z.d.Z.d.e.d...
 00000340: 6503 6403 8301 6503 6404 8301 6503 6405  e.d...e.d...e.d.
 00000350: 8301 6503 6406 8301 6605 6901 5a04 6503  ..e.d...f.i.Z.e.
 00000360: 6407 8301 6503 6408 8301 6503 6409 8301  d...e.d...e.d...
 00000370: 6503 640a 8301 6503 640b 8301 6503 640c  e.d...e.d...e.d.
-00000380: 8301 6503 640d 8301 6503 640e 8301 6503  ..e.d...e.d...e.
-00000390: 640f 8301 6609 5a05 6410 5300 2911 7a15  d...f.Z.d.S.).z.
-000003a0: 466f 726d 6174 7465 7245 6469 746f 722e  FormatterEditor.
-000003b0: 4d65 6469 61da 0361 6c6c 7a2b 6164 6d69  Media..allz+admi
-000003c0: 6e2f 706f 7765 725f 7175 6572 792f 636f  n/power_query/co
-000003d0: 6465 6d69 7272 6f72 2f63 6f64 656d 6972  demirror/codemir
-000003e0: 726f 722e 6373 737a 2b61 646d 696e 2f70  ror.cssz+admin/p
-000003f0: 6f77 6572 5f71 7565 7279 2f63 6f64 656d  ower_query/codem
-00000400: 6972 726f 722f 6675 6c6c 7363 7265 656e  irror/fullscreen
-00000410: 2e63 7373 7a2b 6164 6d69 6e2f 706f 7765  .cssz+admin/powe
-00000420: 725f 7175 6572 792f 636f 6465 6d69 7272  r_query/codemirr
-00000430: 6f72 2f66 6f6c 6467 7574 7465 722e 6373  or/foldgutter.cs
-00000440: 737a 2961 646d 696e 2f70 6f77 6572 5f71  sz)admin/power_q
-00000450: 7565 7279 2f63 6f64 656d 6972 726f 722f  uery/codemirror/
-00000460: 6d69 646e 6967 6874 2e63 7373 7a27 6164  midnight.cssz'ad
-00000470: 6d69 6e2f 706f 7765 725f 7175 6572 792f  min/power_query/
-00000480: 636f 6465 6d69 7272 6f72 2f61 6263 6465  codemirror/abcde
-00000490: 662e 6373 737a 2a61 646d 696e 2f70 6f77  f.cssz*admin/pow
-000004a0: 6572 5f71 7565 7279 2f63 6f64 656d 6972  er_query/codemir
-000004b0: 726f 722f 636f 6465 6d69 7272 6f72 2e6a  ror/codemirror.j
-000004c0: 73fa 2661 646d 696e 2f70 6f77 6572 5f71  s.&admin/power_q
-000004d0: 7565 7279 2f63 6f64 656d 6972 726f 722f  uery/codemirror/
-000004e0: 7079 7468 6f6e 2e6a 737a 2a61 646d 696e  python.jsz*admin
-000004f0: 2f70 6f77 6572 5f71 7565 7279 2f63 6f64  /power_query/cod
-00000500: 656d 6972 726f 722f 6675 6c6c 7363 7265  emirror/fullscre
-00000510: 656e 2e6a 737a 2b61 646d 696e 2f70 6f77  en.jsz+admin/pow
-00000520: 6572 5f71 7565 7279 2f63 6f64 656d 6972  er_query/codemir
-00000530: 726f 722f 6163 7469 7665 2d6c 696e 652e  ror/active-line.
-00000540: 6a73 7a28 6164 6d69 6e2f 706f 7765 725f  jsz(admin/power_
-00000550: 7175 6572 792f 636f 6465 6d69 7272 6f72  query/codemirror
-00000560: 2f66 6f6c 6463 6f64 652e 6a73 7a2a 6164  /foldcode.jsz*ad
-00000570: 6d69 6e2f 706f 7765 725f 7175 6572 792f  min/power_query/
-00000580: 636f 6465 6d69 7272 6f72 2f66 6f6c 6467  codemirror/foldg
-00000590: 7574 7465 722e 6a73 7a2b 6164 6d69 6e2f  utter.jsz+admin/
-000005a0: 706f 7765 725f 7175 6572 792f 636f 6465  power_query/code
-000005b0: 6d69 7272 6f72 2f69 6e64 656e 742d 666f  mirror/indent-fo
-000005c0: 6c64 2e6a 737a 2761 646d 696e 2f70 6f77  ld.jsz'admin/pow
-000005d0: 6572 5f71 7565 7279 2f63 6f64 656d 6972  er_query/codemir
-000005e0: 726f 722f 6f76 6572 6c61 792e 6a73 fa26  ror/overlay.js.&
-000005f0: 6164 6d69 6e2f 706f 7765 725f 7175 6572  admin/power_quer
-00000600: 792f 636f 6465 6d69 7272 6f72 2f64 6a61  y/codemirror/dja
-00000610: 6e67 6f2e 6a73 4e29 06da 085f 5f6e 616d  ngo.jsN)...__nam
-00000620: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000630: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0a00  .__qualname__r..
-00000640: 0000 da03 6373 73da 026a 7372 1b00 0000  ....css..jsr....
-00000650: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-00000660: 054d 6564 6961 1500 0000 7324 0000 0008  .Media....s$....
-00000670: 0202 0106 0106 0106 0106 0106 fb02 ff04  ................
-00000680: 0a06 0106 0106 0106 0106 0106 0106 0106  ................
-00000690: 0106 f772 2500 0000 2908 7220 0000 0072  ...r%...).r ...r
-000006a0: 2100 0000 7222 0000 00da 0d74 656d 706c  !...r".....templ
-000006b0: 6174 655f 6e61 6d65 7202 0000 0072 1600  ate_namer....r..
-000006c0: 0000 7225 0000 00da 0d5f 5f63 6c61 7373  ..r%.....__class
-000006d0: 6365 6c6c 5f5f 721b 0000 0072 1b00 0000  cell__r....r....
-000006e0: 7219 0000 0072 1c00 0000 720c 0000 000c  r....r....r.....
-000006f0: 0000 0073 0600 0000 0801 0402 1606 720c  ...s..........r.
-00000700: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000710: 0000 0000 0400 0000 0000 0000 7338 0000  ............s8..
-00000720: 0065 005a 0164 005a 0265 0365 0364 0164  .e.Z.d.Z.e.e.d.d
-00000730: 029c 0387 0066 0164 0364 0484 0c5a 0447  .....f.d.d...Z.G
-00000740: 0064 0564 0684 0064 0665 056a 0683 035a  .d.d...d.e.j...Z
-00000750: 0687 0004 005a 0753 0029 07da 1550 7974  .....Z.S.)...Pyt
-00000760: 686f 6e46 6f72 6d61 7474 6572 4564 6974  honFormatterEdit
-00000770: 6f72 4e72 0d00 0000 6301 0000 0000 0000  orNr....c.......
-00000780: 0000 0000 0003 0000 0004 0000 000f 0000  ................
-00000790: 0073 2000 0000 7400 8300 6a01 7c01 6900  .s ...t...j.|.i.
-000007a0: 7c02 a401 8e01 0100 6401 7c00 6a02 6402  |.......d.|.j.d.
-000007b0: 3c00 6400 5300 2903 4e7a 0d70 7974 686f  <.d.S.).Nz.pytho
-000007c0: 6e2d 6564 6974 6f72 7213 0000 0029 0372  n-editorr....).r
-000007d0: 1500 0000 7216 0000 0072 1700 0000 2903  ....r....r....).
-000007e0: 7218 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-000007f0: 1900 0000 721b 0000 0072 1c00 0000 7216  ....r....r....r.
-00000800: 0000 002d 0000 0073 0400 0000 0001 1201  ...-...s........
-00000810: 7a1e 5079 7468 6f6e 466f 726d 6174 7465  z.PythonFormatte
-00000820: 7245 6469 746f 722e 5f5f 696e 6974 5f5f  rEditor.__init__
-00000830: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000840: 0004 0000 0040 0000 0073 2400 0000 6500  .....@...s$...e.
-00000850: 5a01 6400 5a02 6503 6a04 6a05 6506 6401  Z.d.Z.e.j.j.e.d.
-00000860: 8301 6506 6402 8301 6602 1700 5a05 6403  ..e.d...f...Z.d.
-00000870: 5300 2904 7a1b 5079 7468 6f6e 466f 726d  S.).z.PythonForm
-00000880: 6174 7465 7245 6469 746f 722e 4d65 6469  atterEditor.Medi
-00000890: 6172 1e00 0000 721f 0000 004e 2907 7220  ar....r....N).r 
-000008a0: 0000 0072 2100 0000 7222 0000 0072 0c00  ...r!...r"...r..
-000008b0: 0000 7225 0000 0072 2400 0000 720a 0000  ..r%...r$...r...
-000008c0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
-000008d0: 721c 0000 0072 2500 0000 3100 0000 7308  r....r%...1...s.
-000008e0: 0000 0008 0106 0106 0106 fe72 2500 0000  ...........r%...
-000008f0: 2908 7220 0000 0072 2100 0000 7222 0000  ).r ...r!...r"..
-00000900: 0072 0200 0000 7216 0000 0072 0c00 0000  .r....r....r....
-00000910: 7225 0000 0072 2700 0000 721b 0000 0072  r%...r'...r....r
-00000920: 1b00 0000 7219 0000 0072 1c00 0000 7228  ....r....r....r(
-00000930: 0000 002c 0000 0073 0400 0000 0801 1604  ...,...s........
-00000940: 7228 0000 0063 0000 0000 0000 0000 0000  r(...c..........
-00000950: 0000 0000 0000 0e00 0000 0000 0000 7380  ..............s.
-00000960: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-00000970: 0364 0364 0364 0464 0364 0364 059c 0865  .d.d.d.d.d.d...e
-00000980: 0365 0465 0565 0619 0065 0565 0619 0065  .e.e.e...e.e...e
-00000990: 0565 0619 0065 0365 0565 0319 0065 0765  .e...e.e.e...e.e
-000009a0: 0765 0865 0965 0365 0666 0219 0066 0219  .e.e.e.e.f...f..
-000009b0: 0064 0664 0366 0319 0065 0664 079c 0987  .d.d.f...e.d....
-000009c0: 0066 0164 0864 0984 0e5a 0a65 0665 0364  .f.d.d...Z.e.e.d
-000009d0: 0a9c 0264 0b64 0c84 045a 0b87 0004 005a  ...d.d...Z.....Z
-000009e0: 0c53 0029 0dda 1643 6f6e 7465 6e74 5479  .S.)...ContentTy
-000009f0: 7065 4368 6f69 6365 4669 656c 647a 092d  peChoiceFieldz.-
-00000a00: 2d2d 2d2d 2d2d 2d2d 544e da00 a908 da0b  --------TN......
-00000a10: 656d 7074 795f 6c61 6265 6cda 0872 6571  empty_label..req
-00000a20: 7569 7265 64da 0677 6964 6765 74da 056c  uired..widget..l
-00000a30: 6162 656c da07 696e 6974 6961 6cda 0968  abel..initial..h
-00000a40: 656c 705f 7465 7874 da0d 746f 5f66 6965  elp_text..to_fie
-00000a50: 6c64 5f6e 616d 65da 106c 696d 6974 5f63  ld_name..limit_c
-00000a60: 686f 6963 6573 5f74 6f72 0b00 0000 2909  hoices_tor....).
-00000a70: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
-00000a80: 2f00 0000 7230 0000 0072 3100 0000 7232  /...r0...r1...r2
-00000a90: 0000 0072 3300 0000 720f 0000 0063 0100  ...r3...r....c..
-00000aa0: 0000 0000 0000 0800 0000 0b00 0000 0b00  ................
-00000ab0: 0000 0b00 0000 7338 0000 0074 006a 01a0  ......s8...t.j..
-00000ac0: 0264 0164 02a1 027d 0a74 0383 006a 047c  .d.d...}.t...j.|
-00000ad0: 0a66 017c 017c 027c 037c 047c 057c 067c  .f.|.|.|.|.|.|.|
-00000ae0: 077c 0864 039c 087c 09a4 018e 0101 0064  .|.d...|.......d
-00000af0: 0053 0029 044e da05 6d6f 6465 6cda 0961  .S.).N..model..a
-00000b00: 7070 5f6c 6162 656c 722b 0000 0029 0572  pp_labelr+...).r
-00000b10: 0800 0000 da07 6f62 6a65 6374 73da 086f  ......objects..o
-00000b20: 7264 6572 5f62 7972 1500 0000 7216 0000  rder_byr....r...
-00000b30: 0029 0b72 1800 0000 722c 0000 0072 2d00  .).r....r,...r-.
-00000b40: 0000 722e 0000 0072 2f00 0000 7230 0000  ..r....r/...r0..
-00000b50: 0072 3100 0000 7232 0000 0072 3300 0000  .r1...r2...r3...
-00000b60: 720f 0000 00da 0871 7565 7279 7365 7472  r......querysetr
-00000b70: 1900 0000 721b 0000 0072 1c00 0000 7216  ....r....r....r.
-00000b80: 0000 0039 0000 0073 1e00 0000 000f 0e01  ...9...s........
-00000b90: 0601 02ff 0202 0201 0201 0201 0201 0201  ................
-00000ba0: 0201 0201 02f7 040a 02f6 7a1f 436f 6e74  ..........z.Cont
-00000bb0: 656e 7454 7970 6543 686f 6963 6546 6965  entTypeChoiceFie
-00000bc0: 6c64 2e5f 5f69 6e69 745f 5f29 02da 036f  ld.__init__)...o
-00000bd0: 626a 7210 0000 0063 0200 0000 0000 0000  bjr....c........
-00000be0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000bf0: 7318 0000 007c 016a 00a0 01a1 009b 0064  s....|.j.......d
-00000c00: 017c 016a 029b 0064 029d 0453 0029 034e  .|.j...d...S.).N
-00000c10: 7a02 2028 fa01 2929 03da 046e 616d 65da  z. (..))...name.
-00000c20: 0574 6974 6c65 7235 0000 0029 0272 1800  .titler5...).r..
-00000c30: 0000 7239 0000 0072 1b00 0000 721b 0000  ..r9...r....r...
-00000c40: 0072 1c00 0000 da13 6c61 6265 6c5f 6672  .r......label_fr
-00000c50: 6f6d 5f69 6e73 7461 6e63 6556 0000 0073  om_instanceV...s
-00000c60: 0200 0000 0001 7a2a 436f 6e74 656e 7454  ......z*ContentT
-00000c70: 7970 6543 686f 6963 6546 6965 6c64 2e6c  ypeChoiceField.l
-00000c80: 6162 656c 5f66 726f 6d5f 696e 7374 616e  abel_from_instan
-00000c90: 6365 290d 7220 0000 0072 2100 0000 7222  ce).r ...r!...r"
-00000ca0: 0000 00da 0373 7472 da04 626f 6f6c 7204  .....str..boolr.
-00000cb0: 0000 0072 0200 0000 7206 0000 0072 0900  ...r....r....r..
-00000cc0: 0000 7203 0000 0072 1600 0000 723d 0000  ..r....r....r=..
-00000cd0: 0072 2700 0000 721b 0000 0072 1b00 0000  .r'...r....r....
-00000ce0: 7219 0000 0072 1c00 0000 7229 0000 0038  r....r....r)...8
-00000cf0: 0000 0073 2c00 0000 0804 0201 0201 0201  ...s,...........
-00000d00: 0201 0201 0201 0203 02f4 0403 0201 0201  ................
-00000d10: 0601 0601 0601 0201 0601 0201 18ff 0203  ................
-00000d20: 02f3 101d 7229 0000 004e 2915 da06 7479  ....r)...N)...ty
-00000d30: 7069 6e67 7202 0000 0072 0300 0000 7204  pingr....r....r.
-00000d40: 0000 0072 0500 0000 7206 0000 00da 0664  ...r....r......d
-00000d50: 6a61 6e67 6f72 0700 0000 da22 646a 616e  jangor....."djan
-00000d60: 676f 2e63 6f6e 7472 6962 2e63 6f6e 7465  go.contrib.conte
-00000d70: 6e74 7479 7065 732e 6d6f 6465 6c73 7208  nttypes.modelsr.
-00000d80: 0000 00da 1064 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-00000d90: 6f64 656c 7372 0900 0000 da1a 646a 616e  odelsr......djan
-00000da0: 676f 2e74 656d 706c 6174 6574 6167 732e  go.templatetags.
-00000db0: 7374 6174 6963 720a 0000 00da 1764 6a61  staticr......dja
-00000dc0: 6e67 6f2e 6462 2e6d 6f64 656c 732e 6669  ngo.db.models.fi
-00000dd0: 656c 6473 720b 0000 00da 0854 6578 7461  eldsr......Texta
-00000de0: 7265 6172 0c00 0000 7228 0000 00da 104d  rear....r(.....M
-00000df0: 6f64 656c 4368 6f69 6365 4669 656c 6472  odelChoiceFieldr
-00000e00: 2900 0000 721b 0000 0072 1b00 0000 721b  )...r....r....r.
-00000e10: 0000 0072 1c00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000e20: 653e 0100 0000 7312 0000 001c 020c 010c  e>....s.........
-00000e30: 010c 010c 0204 010c 0312 2010 0c         .......... ..
+00000380: 8301 6503 640d 8301 6607 5a05 640e 5300  ..e.d...f.Z.d.S.
+00000390: 290f 7a15 466f 726d 6174 7465 7245 6469  ).z.FormatterEdi
+000003a0: 746f 722e 4d65 6469 61da 0361 6c6c 7a2b  tor.Media..allz+
+000003b0: 6164 6d69 6e2f 706f 7765 725f 7175 6572  admin/power_quer
+000003c0: 792f 636f 6465 6d69 7272 6f72 2f63 6f64  y/codemirror/cod
+000003d0: 656d 6972 726f 722e 6373 737a 2b61 646d  emirror.cssz+adm
+000003e0: 696e 2f70 6f77 6572 5f71 7565 7279 2f63  in/power_query/c
+000003f0: 6f64 656d 6972 726f 722f 6675 6c6c 7363  odemirror/fullsc
+00000400: 7265 656e 2e63 7373 7a2b 6164 6d69 6e2f  reen.cssz+admin/
+00000410: 706f 7765 725f 7175 6572 792f 636f 6465  power_query/code
+00000420: 6d69 7272 6f72 2f66 6f6c 6467 7574 7465  mirror/foldgutte
+00000430: 722e 6373 737a 2961 646d 696e 2f70 6f77  r.cssz)admin/pow
+00000440: 6572 5f71 7565 7279 2f63 6f64 656d 6972  er_query/codemir
+00000450: 726f 722f 6d69 646e 6967 6874 2e63 7373  ror/midnight.css
+00000460: 7a27 6164 6d69 6e2f 706f 7765 725f 7175  z'admin/power_qu
+00000470: 6572 792f 636f 6465 6d69 7272 6f72 2f61  ery/codemirror/a
+00000480: 6263 6465 662e 6373 737a 2a61 646d 696e  bcdef.cssz*admin
+00000490: 2f70 6f77 6572 5f71 7565 7279 2f63 6f64  /power_query/cod
+000004a0: 656d 6972 726f 722f 636f 6465 6d69 7272  emirror/codemirr
+000004b0: 6f72 2e6a 737a 2a61 646d 696e 2f70 6f77  or.jsz*admin/pow
+000004c0: 6572 5f71 7565 7279 2f63 6f64 656d 6972  er_query/codemir
+000004d0: 726f 722f 6675 6c6c 7363 7265 656e 2e6a  ror/fullscreen.j
+000004e0: 737a 2b61 646d 696e 2f70 6f77 6572 5f71  sz+admin/power_q
+000004f0: 7565 7279 2f63 6f64 656d 6972 726f 722f  uery/codemirror/
+00000500: 6163 7469 7665 2d6c 696e 652e 6a73 7a28  active-line.jsz(
+00000510: 6164 6d69 6e2f 706f 7765 725f 7175 6572  admin/power_quer
+00000520: 792f 636f 6465 6d69 7272 6f72 2f66 6f6c  y/codemirror/fol
+00000530: 6463 6f64 652e 6a73 7a2a 6164 6d69 6e2f  dcode.jsz*admin/
+00000540: 706f 7765 725f 7175 6572 792f 636f 6465  power_query/code
+00000550: 6d69 7272 6f72 2f66 6f6c 6467 7574 7465  mirror/foldgutte
+00000560: 722e 6a73 7a2b 6164 6d69 6e2f 706f 7765  r.jsz+admin/powe
+00000570: 725f 7175 6572 792f 636f 6465 6d69 7272  r_query/codemirr
+00000580: 6f72 2f69 6e64 656e 742d 666f 6c64 2e6a  or/indent-fold.j
+00000590: 737a 2761 646d 696e 2f70 6f77 6572 5f71  sz'admin/power_q
+000005a0: 7565 7279 2f63 6f64 656d 6972 726f 722f  uery/codemirror/
+000005b0: 6f76 6572 6c61 792e 6a73 4e29 06da 085f  overlay.jsN)..._
+000005c0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000005d0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000005e0: 5f72 0a00 0000 da03 6373 73da 026a 7372  _r......css..jsr
+000005f0: 1b00 0000 721b 0000 0072 1b00 0000 721c  ....r....r....r.
+00000600: 0000 00da 054d 6564 6961 1500 0000 7320  .....Media....s 
+00000610: 0000 0008 0202 0106 0106 0106 0106 0106  ................
+00000620: fb02 ff04 0a06 0106 0106 0106 0106 0106  ................
+00000630: 0106 f972 2300 0000 2908 721e 0000 0072  ...r#...).r....r
+00000640: 1f00 0000 7220 0000 00da 0d74 656d 706c  ....r .....templ
+00000650: 6174 655f 6e61 6d65 7202 0000 0072 1600  ate_namer....r..
+00000660: 0000 7223 0000 00da 0d5f 5f63 6c61 7373  ..r#.....__class
+00000670: 6365 6c6c 5f5f 721b 0000 0072 1b00 0000  cell__r....r....
+00000680: 7219 0000 0072 1c00 0000 720c 0000 000c  r....r....r.....
+00000690: 0000 0073 0600 0000 0801 0402 1606 720c  ...s..........r.
+000006a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000006b0: 0000 0000 0400 0000 0000 0000 7338 0000  ............s8..
+000006c0: 0065 005a 0164 005a 0265 0365 0364 0164  .e.Z.d.Z.e.e.d.d
+000006d0: 029c 0387 0066 0164 0364 0484 0c5a 0447  .....f.d.d...Z.G
+000006e0: 0064 0564 0684 0064 0665 056a 0683 035a  .d.d...d.e.j...Z
+000006f0: 0687 0004 005a 0753 0029 07da 1550 7974  .....Z.S.)...Pyt
+00000700: 686f 6e46 6f72 6d61 7474 6572 4564 6974  honFormatterEdit
+00000710: 6f72 4e72 0d00 0000 6301 0000 0000 0000  orNr....c.......
+00000720: 0000 0000 0003 0000 0004 0000 000f 0000  ................
+00000730: 0073 2000 0000 7400 8300 6a01 7c01 6900  .s ...t...j.|.i.
+00000740: 7c02 a401 8e01 0100 6401 7c00 6a02 6402  |.......d.|.j.d.
+00000750: 3c00 6400 5300 2903 4e7a 0d70 7974 686f  <.d.S.).Nz.pytho
+00000760: 6e2d 6564 6974 6f72 7213 0000 0029 0372  n-editorr....).r
+00000770: 1500 0000 7216 0000 0072 1700 0000 2903  ....r....r....).
+00000780: 7218 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00000790: 1900 0000 721b 0000 0072 1c00 0000 7216  ....r....r....r.
+000007a0: 0000 002b 0000 0073 0400 0000 0001 1201  ...+...s........
+000007b0: 7a1e 5079 7468 6f6e 466f 726d 6174 7465  z.PythonFormatte
+000007c0: 7245 6469 746f 722e 5f5f 696e 6974 5f5f  rEditor.__init__
+000007d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000007e0: 0004 0000 0040 0000 0073 2400 0000 6500  .....@...s$...e.
+000007f0: 5a01 6400 5a02 6503 6a04 6a05 6506 6401  Z.d.Z.e.j.j.e.d.
+00000800: 8301 6506 6402 8301 6602 1700 5a05 6403  ..e.d...f...Z.d.
+00000810: 5300 2904 7a1b 5079 7468 6f6e 466f 726d  S.).z.PythonForm
+00000820: 6174 7465 7245 6469 746f 722e 4d65 6469  atterEditor.Medi
+00000830: 617a 2661 646d 696e 2f70 6f77 6572 5f71  az&admin/power_q
+00000840: 7565 7279 2f63 6f64 656d 6972 726f 722f  uery/codemirror/
+00000850: 7079 7468 6f6e 2e6a 737a 2661 646d 696e  python.jsz&admin
+00000860: 2f70 6f77 6572 5f71 7565 7279 2f63 6f64  /power_query/cod
+00000870: 656d 6972 726f 722f 646a 616e 676f 2e6a  emirror/django.j
+00000880: 734e 2907 721e 0000 0072 1f00 0000 7220  sN).r....r....r 
+00000890: 0000 0072 0c00 0000 7223 0000 0072 2200  ...r....r#...r".
+000008a0: 0000 720a 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+000008b0: 0072 1b00 0000 721c 0000 0072 2300 0000  .r....r....r#...
+000008c0: 2f00 0000 7308 0000 0008 0106 0106 0106  /...s...........
+000008d0: fe72 2300 0000 2908 721e 0000 0072 1f00  .r#...).r....r..
+000008e0: 0000 7220 0000 0072 0200 0000 7216 0000  ..r ...r....r...
+000008f0: 0072 0c00 0000 7223 0000 0072 2500 0000  .r....r#...r%...
+00000900: 721b 0000 0072 1b00 0000 7219 0000 0072  r....r....r....r
+00000910: 1c00 0000 7226 0000 002a 0000 0073 0400  ....r&...*...s..
+00000920: 0000 0801 1604 7226 0000 0063 0000 0000  ......r&...c....
+00000930: 0000 0000 0000 0000 0000 0000 0e00 0000  ................
+00000940: 0000 0000 7380 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00000950: 0264 0164 0264 0364 0364 0364 0464 0364  .d.d.d.d.d.d.d.d
+00000960: 0364 059c 0865 0365 0465 0565 0619 0065  .d...e.e.e.e...e
+00000970: 0565 0619 0065 0565 0619 0065 0365 0565  .e...e.e...e.e.e
+00000980: 0319 0065 0765 0765 0865 0965 0365 0666  ...e.e.e.e.e.e.f
+00000990: 0219 0066 0219 0064 0664 0366 0319 0065  ...f...d.d.f...e
+000009a0: 0664 079c 0987 0066 0164 0864 0984 0e5a  .d.....f.d.d...Z
+000009b0: 0a65 0665 0364 0a9c 0264 0b64 0c84 045a  .e.e.d...d.d...Z
+000009c0: 0b87 0004 005a 0c53 0029 0dda 1643 6f6e  .....Z.S.)...Con
+000009d0: 7465 6e74 5479 7065 4368 6f69 6365 4669  tentTypeChoiceFi
+000009e0: 656c 647a 092d 2d2d 2d2d 2d2d 2d2d 544e  eldz.---------TN
+000009f0: da00 a908 da0b 656d 7074 795f 6c61 6265  ......empty_labe
+00000a00: 6cda 0872 6571 7569 7265 64da 0677 6964  l..required..wid
+00000a10: 6765 74da 056c 6162 656c da07 696e 6974  get..label..init
+00000a20: 6961 6cda 0968 656c 705f 7465 7874 da0d  ial..help_text..
+00000a30: 746f 5f66 6965 6c64 5f6e 616d 65da 106c  to_field_name..l
+00000a40: 696d 6974 5f63 686f 6963 6573 5f74 6f72  imit_choices_tor
+00000a50: 0b00 0000 2909 722a 0000 0072 2b00 0000  ....).r*...r+...
+00000a60: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
+00000a70: 2f00 0000 7230 0000 0072 3100 0000 720f  /...r0...r1...r.
+00000a80: 0000 0063 0100 0000 0000 0000 0800 0000  ...c............
+00000a90: 0b00 0000 0b00 0000 0b00 0000 7338 0000  ............s8..
+00000aa0: 0074 006a 01a0 0264 0164 02a1 027d 0a74  .t.j...d.d...}.t
+00000ab0: 0383 006a 047c 0a66 017c 017c 027c 037c  ...j.|.f.|.|.|.|
+00000ac0: 047c 057c 067c 077c 0864 039c 087c 09a4  .|.|.|.|.d...|..
+00000ad0: 018e 0101 0064 0053 0029 044e da05 6d6f  .....d.S.).N..mo
+00000ae0: 6465 6cda 0961 7070 5f6c 6162 656c 7229  del..app_labelr)
+00000af0: 0000 0029 0572 0800 0000 da07 6f62 6a65  ...).r......obje
+00000b00: 6374 73da 086f 7264 6572 5f62 7972 1500  cts..order_byr..
+00000b10: 0000 7216 0000 0029 0b72 1800 0000 722a  ..r....).r....r*
+00000b20: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00000b30: 0000 722e 0000 0072 2f00 0000 7230 0000  ..r....r/...r0..
+00000b40: 0072 3100 0000 720f 0000 00da 0871 7565  .r1...r......que
+00000b50: 7279 7365 7472 1900 0000 721b 0000 0072  rysetr....r....r
+00000b60: 1c00 0000 7216 0000 0037 0000 0073 1e00  ....r....7...s..
+00000b70: 0000 000f 0e01 0601 02ff 0202 0201 0201  ................
+00000b80: 0201 0201 0201 0201 0201 02f7 040a 02f6  ................
+00000b90: 7a1f 436f 6e74 656e 7454 7970 6543 686f  z.ContentTypeCho
+00000ba0: 6963 6546 6965 6c64 2e5f 5f69 6e69 745f  iceField.__init_
+00000bb0: 5f29 02da 036f 626a 7210 0000 0063 0200  _)...objr....c..
+00000bc0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000bd0: 0000 4300 0000 7318 0000 007c 016a 00a0  ..C...s....|.j..
+00000be0: 01a1 009b 0064 017c 016a 029b 0064 029d  .....d.|.j...d..
+00000bf0: 0453 0029 034e 7a02 2028 fa01 2929 03da  .S.).Nz. (..))..
+00000c00: 046e 616d 65da 0574 6974 6c65 7233 0000  .name..titler3..
+00000c10: 0029 0272 1800 0000 7237 0000 0072 1b00  .).r....r7...r..
+00000c20: 0000 721b 0000 0072 1c00 0000 da13 6c61  ..r....r......la
+00000c30: 6265 6c5f 6672 6f6d 5f69 6e73 7461 6e63  bel_from_instanc
+00000c40: 6554 0000 0073 0200 0000 0001 7a2a 436f  eT...s......z*Co
+00000c50: 6e74 656e 7454 7970 6543 686f 6963 6546  ntentTypeChoiceF
+00000c60: 6965 6c64 2e6c 6162 656c 5f66 726f 6d5f  ield.label_from_
+00000c70: 696e 7374 616e 6365 290d 721e 0000 0072  instance).r....r
+00000c80: 1f00 0000 7220 0000 00da 0373 7472 da04  ....r .....str..
+00000c90: 626f 6f6c 7204 0000 0072 0200 0000 7206  boolr....r....r.
+00000ca0: 0000 0072 0900 0000 7203 0000 0072 1600  ...r....r....r..
+00000cb0: 0000 723b 0000 0072 2500 0000 721b 0000  ..r;...r%...r...
+00000cc0: 0072 1b00 0000 7219 0000 0072 1c00 0000  .r....r....r....
+00000cd0: 7227 0000 0036 0000 0073 2c00 0000 0804  r'...6...s,.....
+00000ce0: 0201 0201 0201 0201 0201 0201 0203 02f4  ................
+00000cf0: 0403 0201 0201 0601 0601 0601 0201 0601  ................
+00000d00: 0201 18ff 0203 02f3 101d 7227 0000 004e  ..........r'...N
+00000d10: 2915 da06 7479 7069 6e67 7202 0000 0072  )...typingr....r
+00000d20: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
+00000d30: 0000 00da 0664 6a61 6e67 6f72 0700 0000  .....djangor....
+00000d40: da22 646a 616e 676f 2e63 6f6e 7472 6962  ."django.contrib
+00000d50: 2e63 6f6e 7465 6e74 7479 7065 732e 6d6f  .contenttypes.mo
+00000d60: 6465 6c73 7208 0000 00da 1064 6a61 6e67  delsr......djang
+00000d70: 6f2e 6462 2e6d 6f64 656c 7372 0900 0000  o.db.modelsr....
+00000d80: da1a 646a 616e 676f 2e74 656d 706c 6174  ..django.templat
+00000d90: 6574 6167 732e 7374 6174 6963 720a 0000  etags.staticr...
+00000da0: 00da 1764 6a61 6e67 6f2e 6462 2e6d 6f64  ...django.db.mod
+00000db0: 656c 732e 6669 656c 6473 720b 0000 00da  els.fieldsr.....
+00000dc0: 0854 6578 7461 7265 6172 0c00 0000 7226  .Textarear....r&
+00000dd0: 0000 00da 104d 6f64 656c 4368 6f69 6365  .....ModelChoice
+00000de0: 4669 656c 6472 2700 0000 721b 0000 0072  Fieldr'...r....r
+00000df0: 1b00 0000 721b 0000 0072 1c00 0000 da08  ....r....r......
+00000e00: 3c6d 6f64 756c 653e 0100 0000 7312 0000  <module>....s...
+00000e10: 001c 020c 010c 010c 010c 0204 010c 0312  ................
+00000e20: 1e10 0c                                  ...
```

### Comparing `unicef-power-query-0.3/src/power_query/admin.py` & `unicef-power-query-0.3.1/src/power_query/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,14 +408,19 @@
     @button()
     def preview(self, request: HttpRequest, pk: int) -> TemplateResponse:
         context = self.get_common_context(request, pk, title="Execution Plan")
         return TemplateResponse(
             request, "admin/power_query/queryargs/preview.html", context
         )
 
+    @button()
+    def refresh(self, request: HttpRequest, pk: int) -> None:
+        obj = self.get_object(request, str(pk))
+        obj.refresh()
+
 
 @register(ReportDocument)
 class ReportDocumentAdmin(
     AdminFiltersMixin,
     LinkedObjectsMixin,
     ExtraButtonsMixin,
     DisplayAllMixin,
```

### Comparing `unicef-power-query-0.3/src/power_query/celery_tasks.py` & `unicef-power-query-0.3.1/src/power_query/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/defaults.py` & `unicef-power-query-0.3.1/src/power_query/defaults.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/fixtures.py` & `unicef-power-query-0.3.1/src/power_query/fixtures.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/forms.py` & `unicef-power-query-0.3.1/src/power_query/forms.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/json.py` & `unicef-power-query-0.3.1/src/power_query/json.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/management/commands/pq.py` & `unicef-power-query-0.3.1/src/power_query/management/commands/pq.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/migrations/0001_migration_squashed_0014_migration.py` & `unicef-power-query-0.3.1/src/power_query/migrations/0001_migration_squashed_0014_migration.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/migrations/0015_alter_dataset_description_and_more.py` & `unicef-power-query-0.3.1/src/power_query/migrations/0015_alter_dataset_description_and_more.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jul 18 14:47:19 2023 UTC, .py size: 1003 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 f7a5 b664 eb03 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 eea6 b664 eb03 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 4700 6403 6404  m.Z.m.Z...G.d.d.
 00000050: 8400 6404 6503 6a05 8303 5a05 6405 5300  ..d.e.j...Z.d.S.
 00000060: 2906 e900 0000 0029 01da 0873 6574 7469  )......)...setti
 00000070: 6e67 7329 02da 0a6d 6967 7261 7469 6f6e  ngs)...migration
@@ -13,15 +13,15 @@
 000000c0: 036a 0864 0264 0365 096a 0a64 0464 058d  .j.d.d.e.j.d.d..
 000000d0: 0164 068d 0365 036a 0864 0764 0865 096a  .d...e.j.d.d.e.j
 000000e0: 0b64 0964 0a65 056a 0664 0b8d 0364 068d  .d.d.e.j.d...d..
 000000f0: 0365 036a 0864 0c64 0865 096a 0b64 0964  .e.j.d.d.e.j.d.d
 00000100: 0a65 056a 0664 0b8d 0364 068d 0367 035a  .e.j.d...d...g.Z
 00000110: 0c64 0d53 0029 0eda 094d 6967 7261 7469  .d.S.)...Migrati
 00000120: 6f6e 2902 da0b 706f 7765 725f 7175 6572  on)...power_quer
-00000130: 79da 2630 3030 315f 6d69 6772 6174 696f  y.&0001_migratio
+00000130: 795a 2630 3030 315f 6d69 6772 6174 696f  yZ&0001_migratio
 00000140: 6e5f 7371 7561 7368 6564 5f30 3031 345f  n_squashed_0014_
 00000150: 6d69 6772 6174 696f 6eda 0764 6174 6173  migration..datas
 00000160: 6574 da0b 6465 7363 7269 7074 696f 6ee9  et..description.
 00000170: 6400 0000 2901 da0a 6d61 785f 6c65 6e67  d...)...max_leng
 00000180: 7468 2903 da0a 6d6f 6465 6c5f 6e61 6d65  th)...model_name
 00000190: da04 6e61 6d65 da05 6669 656c 64da 0672  ..name..field..r
 000001a0: 6570 6f72 74da 0f6c 696d 6974 5f61 6363  eport..limit_acc
@@ -34,25 +34,25 @@
 00000210: 00da 1473 7761 7070 6162 6c65 5f64 6570  ...swappable_dep
 00000220: 656e 6465 6e63 7972 0200 0000 da0f 4155  endencyr......AU
 00000230: 5448 5f55 5345 525f 4d4f 4445 4cda 0c64  TH_USER_MODEL..d
 00000240: 6570 656e 6465 6e63 6965 73da 0a41 6c74  ependencies..Alt
 00000250: 6572 4669 656c 6472 0400 0000 da09 4368  erFieldr......Ch
 00000260: 6172 4669 656c 64da 0f4d 616e 7954 6f4d  arField..ManyToM
 00000270: 616e 7946 6965 6c64 da0a 6f70 6572 6174  anyField..operat
-00000280: 696f 6e73 a900 7220 0000 0072 2000 0000  ions..r ...r ...
+00000280: 696f 6e73 a900 721f 0000 0072 1f00 0000  ions..r....r....
 00000290: fa6e 2f55 7365 7273 2f6a 6f6a 6f2f 776f  .n/Users/jojo/wo
 000002a0: 726b 7370 6163 652f 756e 6963 6566 2d70  rkspace/unicef-p
 000002b0: 6f77 6572 2d71 7565 7279 2f73 7263 2f70  ower-query/src/p
 000002c0: 6f77 6572 5f71 7565 7279 2f6d 6967 7261  ower_query/migra
 000002d0: 7469 6f6e 732f 3030 3135 5f61 6c74 6572  tions/0015_alter
 000002e0: 5f64 6174 6173 6574 5f64 6573 6372 6970  _dataset_descrip
 000002f0: 7469 6f6e 5f61 6e64 5f6d 6f72 652e 7079  tion_and_more.py
 00000300: 7205 0000 0007 0000 0073 2e00 0000 0802  r........s......
 00000310: 0a01 02fe 0406 0401 0201 0201 0afd 0405  ................
 00000320: 0401 0201 0201 0401 08ff 04fd 0407 0401  ................
 00000330: 0201 0201 0401 08ff 04fd 04f3 7205 0000  ............r...
 00000340: 004e 2906 da0b 646a 616e 676f 2e63 6f6e  .N)...django.con
 00000350: 6672 0200 0000 da09 646a 616e 676f 2e64  fr......django.d
 00000360: 6272 0300 0000 7204 0000 0072 0500 0000  br....r....r....
-00000370: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
-00000380: 2100 0000 da08 3c6d 6f64 756c 653e 0300  !.....<module>..
+00000370: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00000380: 2000 0000 da08 3c6d 6f64 756c 653e 0300   .....<module>..
 00000390: 0000 7304 0000 000c 0110 03              ..s........
```

### Comparing `unicef-power-query-0.3/src/power_query/mixin.py` & `unicef-power-query-0.3.1/src/power_query/mixin.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/models.py` & `unicef-power-query-0.3.1/src/power_query/models.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/code.css` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/code.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/abcdef.css` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/abcdef.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/active-line.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/active-line.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/codemirror.css` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/codemirror.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/codemirror.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/django.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/django.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/foldcode.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/foldcode.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/foldgutter.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/foldgutter.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/fullscreen.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/fullscreen.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/indent-fold.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/indent-fold.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/matchbrackets.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/midnight.css` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/midnight.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/overlay.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/overlay.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/python.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/python.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/xml.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/xml.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/codemirror/yaml.js` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/codemirror/yaml.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/colorful.css` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/colorful.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/diff.css` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/diff.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/admin/power_query/editor.png` & `unicef-power-query-0.3.1/src/power_query/static/admin/power_query/editor.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/redo.png` & `unicef-power-query-0.3.1/src/power_query/static/redo.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/static/undo.png` & `unicef-power-query-0.3.1/src/power_query/static/undo.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templates/admin/power_query/formatter/change_form.html` & `unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/formatter/change_form.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templates/admin/power_query/query/monitor.html` & `unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/query/monitor.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templates/admin/power_query/query/preview.html` & `unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/query/preview.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templates/admin/power_query/queryargs/change_form.html` & `unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/queryargs/change_form.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templates/admin/power_query/report/monitor.html` & `unicef-power-query-0.3.1/src/power_query/templates/admin/power_query/report/monitor.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templates/power_query/base.html` & `unicef-power-query-0.3.1/src/power_query/templates/power_query/base.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templates/power_query/detail.html` & `unicef-power-query-0.3.1/src/power_query/templates/power_query/detail.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templatetags/__pycache__/power_query.cpython-311.pyc` & `unicef-power-query-0.3.1/src/power_query/templatetags/__pycache__/power_query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc` & `unicef-power-query-0.3.1/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/templatetags/power_query.py` & `unicef-power-query-0.3.1/src/power_query/templatetags/power_query.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/utils.py` & `unicef-power-query-0.3.1/src/power_query/utils.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/views.py` & `unicef-power-query-0.3.1/src/power_query/views.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/src/power_query/widget.py` & `unicef-power-query-0.3.1/src/power_query/widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,22 +26,20 @@
                 static("admin/power_query/codemirror/foldgutter.css"),
                 static("admin/power_query/codemirror/midnight.css"),
                 static("admin/power_query/codemirror/abcdef.css"),
             )
         }
         js = (
             static("admin/power_query/codemirror/codemirror.js"),
-            static("admin/power_query/codemirror/python.js"),
             static("admin/power_query/codemirror/fullscreen.js"),
             static("admin/power_query/codemirror/active-line.js"),
             static("admin/power_query/codemirror/foldcode.js"),
             static("admin/power_query/codemirror/foldgutter.js"),
             static("admin/power_query/codemirror/indent-fold.js"),
             static("admin/power_query/codemirror/overlay.js"),
-            static("admin/power_query/codemirror/django.js"),
         )
 
 
 class PythonFormatterEditor(FormatterEditor):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.attrs["class"] = "python-editor"
```

### Comparing `unicef-power-query-0.3/src/unicef_power_query.egg-info/PKG-INFO` & `unicef-power-query-0.3.1/src/unicef_power_query.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-power-query
-Version: 0.3
+Version: 0.3.1
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `unicef-power-query-0.3/src/unicef_power_query.egg-info/SOURCES.txt` & `unicef-power-query-0.3.1/src/unicef_power_query.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 src/power_query/__pycache__/__init__.cpython-39.pyc
 src/power_query/__pycache__/admin.cpython-311.pyc
 src/power_query/__pycache__/admin.cpython-39.pyc
 src/power_query/__pycache__/apps.cpython-311.pyc
 src/power_query/__pycache__/apps.cpython-39.pyc
 src/power_query/__pycache__/celery_tasks.cpython-311.pyc
 src/power_query/__pycache__/celery_tasks.cpython-39.pyc
-src/power_query/__pycache__/defaults.cpython-39.pyc
+src/power_query/__pycache__/defaults.cpython-311.pyc
 src/power_query/__pycache__/exceptions.cpython-311.pyc
 src/power_query/__pycache__/exceptions.cpython-39.pyc
+src/power_query/__pycache__/fixtures.cpython-311.pyc
 src/power_query/__pycache__/fixtures.cpython-39.pyc
 src/power_query/__pycache__/forms.cpython-311.pyc
 src/power_query/__pycache__/forms.cpython-39.pyc
 src/power_query/__pycache__/json.cpython-311.pyc
 src/power_query/__pycache__/json.cpython-39.pyc
 src/power_query/__pycache__/mixin.cpython-39.pyc
 src/power_query/__pycache__/models.cpython-311.pyc
@@ -49,22 +50,24 @@
 src/power_query/__pycache__/validators.cpython-311.pyc
 src/power_query/__pycache__/validators.cpython-39.pyc
 src/power_query/__pycache__/views.cpython-311.pyc
 src/power_query/__pycache__/views.cpython-39.pyc
 src/power_query/__pycache__/widget.cpython-311.pyc
 src/power_query/__pycache__/widget.cpython-39.pyc
 src/power_query/management/__init__.py
+src/power_query/management/__pycache__/__init__.cpython-311.pyc
 src/power_query/management/__pycache__/__init__.cpython-39.pyc
 src/power_query/management/commands/__init__.py
 src/power_query/management/commands/pq.py
 src/power_query/migrations/0001_migration_squashed_0014_migration.py
 src/power_query/migrations/0015_alter_dataset_description_and_more.py
 src/power_query/migrations/__init__.py
 src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-311.pyc
 src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc
+src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-311.pyc
 src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-39.pyc
 src/power_query/migrations/__pycache__/__init__.cpython-311.pyc
 src/power_query/migrations/__pycache__/__init__.cpython-39.pyc
 src/power_query/static/power_query.css
 src/power_query/static/power_query.css.map
 src/power_query/static/power_query.scss
 src/power_query/static/redo.png
@@ -124,14 +127,15 @@
 tests/test_admin.py
 tests/test_auth.py
 tests/test_celery.py
 tests/test_params.py
 tests/test_queries.py
 tests/test_utils.py
 tests/test_views.py
+tests/__pycache__/__init__.cpython-311.pyc
 tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc
```

### Comparing `unicef-power-query-0.3/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.3.1/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.3.1/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.3.1/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.3.1/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.3.1/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.3.1/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/demoproject/db.sqlite3` & `unicef-power-query-0.3.1/tests/demoproject/db.sqlite3`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc` & `unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/demoproject/demo/__pycache__/models.cpython-311.pyc` & `unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc` & `unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x88d5a364 (Tue Jul  4 08:17:12 2023 UTC)
-files sz: 2590
+moddate:  0x1ba1b764 (Wed Jul 19 08:38:51 2023 UTC)
+files sz: 2626
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a0065006a010000000000000000a0020000000000
@@ -16,15 +16,15 @@
       015a0a67006406a2015a0b64075a0c64085a0d640967006403640a670064
       0ba2016901640c9c0467015a0e640d5a0f640e640f65006a010000000000
       000000a010000000000000000000000000000000000000000065056410a6
       020000ab02000000000000000064119c0269015a11640e6412641364149c
       0269015a1264155a1364165a1464035a1564035a1664175a1764185a1864
       195a19641a5a1a641b5a1b020065006a1c0000000000000000641c641da6
       020000ab0200000000000000005a1d641e651d9b00641f9d0366015a1e64
-      1e651d9b00641f9d035a1f64165a2064035a2164015300
+      1e651d9b00641f9d035a1f64165a2064035a2167005a2264015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
@@ -178,16 +178,19 @@
                398 STORE_NAME              31 (CELERY_RESULT_BACKEND)
    
     99         400 LOAD_CONST              22 ('UTC')
                402 STORE_NAME              32 (CELERY_TIMEZONE)
    
    100         404 LOAD_CONST               3 (True)
                406 STORE_NAME              33 (CELERY_TASK_ALWAYS_EAGER)
-               408 LOAD_CONST               1 (None)
-               410 RETURN_VALUE
+   
+   102         408 BUILD_LIST               0
+               410 STORE_NAME              34 (POWER_QUERY_EXTRA_CONNECTIONS)
+               412 LOAD_CONST               1 (None)
+               414 RETURN_VALUE
    consts
       0
       None
       '&1_8z#^^_nz1o4xuvz4wqq&m&gpe5uq_(=!%sk=cg5e&o^ljqu'
       True
       'django.db.models.BigAutoField'
       ('django.contrib.admin', 'django.contrib.auth', 'django.contrib.contenttypes', 'django.contrib.sessions', 'django.contrib.messages', 'django.contrib.staticfiles', 'adminfilters', 'admin_extra_buttons', 'import_export', 'power_query', 'demo')
@@ -213,18 +216,18 @@
       '/tmp/'
       'vision.VisionLog'
       'demo.User'
       'REDIS_INSTANCE'
       'localhost:6379'
       'redis://'
       '/0'
-   names      ('os', 'path', 'dirname', 'abspath', '__file__', 'BASE_DIR', 'SECRET_KEY', 'DEBUG', 'ALLOWED_HOSTS', 'DEFAULT_AUTO_FIELD', 'INSTALLED_APPS', 'MIDDLEWARE', 'AUTHENTICATION_BACKENDS', 'ROOT_URLCONF', 'TEMPLATES', 'WSGI_APPLICATION', 'join', 'DATABASES', 'CACHES', 'LANGUAGE_CODE', 'TIME_ZONE', 'USE_I18N', 'USE_TZ', 'HOST', 'STATIC_URL', 'MEDIA_ROOT', 'VISION_LOGGER_MODEL', 'AUTH_USER_MODEL', 'getenv', 'REDIS_INSTANCE', 'CELERY_BROKER_URL', 'CELERY_RESULT_BACKEND', 'CELERY_TIMEZONE', 'CELERY_TASK_ALWAYS_EAGER')
+   names      ('os', 'path', 'dirname', 'abspath', '__file__', 'BASE_DIR', 'SECRET_KEY', 'DEBUG', 'ALLOWED_HOSTS', 'DEFAULT_AUTO_FIELD', 'INSTALLED_APPS', 'MIDDLEWARE', 'AUTHENTICATION_BACKENDS', 'ROOT_URLCONF', 'TEMPLATES', 'WSGI_APPLICATION', 'join', 'DATABASES', 'CACHES', 'LANGUAGE_CODE', 'TIME_ZONE', 'USE_I18N', 'USE_TZ', 'HOST', 'STATIC_URL', 'MEDIA_ROOT', 'VISION_LOGGER_MODEL', 'AUTH_USER_MODEL', 'getenv', 'REDIS_INSTANCE', 'CELERY_BROKER_URL', 'CELERY_RESULT_BACKEND', 'CELERY_TIMEZONE', 'CELERY_TASK_ALWAYS_EAGER', 'POWER_QUERY_EXTRA_CONNECTIONS')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jojo/workspace/unicef-power-query/tests/demoproject/demo/settings.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080394040403040204030402080e080a040204040201020102
       0208ff02fc04ff041004050201020134fe04ff04080201020102fe04ff04
-      0904010401040104020402040204010402040222010e010c010401
+      0904010401040104020402040204010402040222010e010c0104010402
```

### Comparing `unicef-power-query-0.3/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc` & `unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc` & `unicef-power-query-0.3.1/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/demoproject/demo/migrations/0001_initial.py` & `unicef-power-query-0.3.1/tests/demoproject/demo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc` & `unicef-power-query-0.3.1/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/demoproject/demo/settings.py` & `unicef-power-query-0.3.1/tests/demoproject/demo/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,7 +94,9 @@
 AUTH_USER_MODEL = "demo.User"
 
 REDIS_INSTANCE = os.getenv("REDIS_INSTANCE", "localhost:6379")
 CELERY_BROKER_URL = (f"redis://{REDIS_INSTANCE}/0",)
 CELERY_RESULT_BACKEND = f"redis://{REDIS_INSTANCE}/0"
 CELERY_TIMEZONE = "UTC"
 CELERY_TASK_ALWAYS_EAGER = True
+
+POWER_QUERY_EXTRA_CONNECTIONS = []
```

### Comparing `unicef-power-query-0.3/tests/test_admin.py` & `unicef-power-query-0.3.1/tests/test_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,20 @@
         cls.superuser = UserFactory(is_superuser=True, is_staff=True, is_active=True)
         cls.user1 = UserFactory(is_superuser=False, is_staff=False, is_active=True)
         cls.user2 = UserFactory(is_superuser=False, is_staff=False, is_active=True)
         create_defaults()
         cls.params = ParametrizerFactory()
         cls.system_params = Parametrizer.objects.get(code="active-business-areas")
 
+    def test_button_refresh(self) -> None:
+        url = reverse("admin:power_query_parametrizer_change", args=[self.system_params.pk])
+        res = self.app.get(url, user=self.superuser)
+        res = res.click("Refresh")
+        assert res.status_code == 302
+
     def test_button_preview(self) -> None:
         url = reverse("admin:power_query_parametrizer_change", args=[self.params.pk])
         res = self.app.get(url, user=self.superuser)
         res = res.click("Preview")
         assert res.status_code == 200
```

### Comparing `unicef-power-query-0.3/tests/test_auth.py` & `unicef-power-query-0.3.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/test_celery.py` & `unicef-power-query-0.3.1/tests/test_celery.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/test_queries.py` & `unicef-power-query-0.3.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/test_utils.py` & `unicef-power-query-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tests/test_views.py` & `unicef-power-query-0.3.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.3/tox.ini` & `unicef-power-query-0.3.1/tox.ini`

 * *Files identical despite different names*

