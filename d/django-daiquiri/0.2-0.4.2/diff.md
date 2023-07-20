# Comparing `tmp/django-daiquiri-0.2.tar.gz` & `tmp/django-daiquiri-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-daiquiri-0.2.tar", last modified: Wed Apr 25 08:06:52 2018, max compression
+gzip compressed data, was "django-daiquiri-0.4.2.tar", last modified: Thu Jul 20 09:24:15 2023, max compression
```

## Comparing `django-daiquiri-0.2.tar` & `django-daiquiri-0.4.2.tar`

### file list

```diff
@@ -1,689 +1,798 @@
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/
--rw-r--r--   0 jochen    (1420) escience   (630)       92 2018-02-16 11:47:27.000000 django-daiquiri-0.2/MANIFEST.in
--rw-r--r--   0 jochen    (1420) escience   (630)     1981 2018-04-25 08:04:42.000000 django-daiquiri-0.2/setup.py
--rw-r--r--   0 jochen    (1420) escience   (630)       38 2018-04-25 08:06:52.000000 django-daiquiri-0.2/setup.cfg
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/django_daiquiri.egg-info/
--rw-r--r--   0 jochen    (1420) escience   (630)    23832 2018-04-25 08:06:52.000000 django-daiquiri-0.2/django_daiquiri.egg-info/SOURCES.txt
--rw-r--r--   0 jochen    (1420) escience   (630)        1 2018-04-25 08:06:52.000000 django-daiquiri-0.2/django_daiquiri.egg-info/dependency_links.txt
--rw-r--r--   0 jochen    (1420) escience   (630)        9 2018-04-25 08:06:52.000000 django-daiquiri-0.2/django_daiquiri.egg-info/top_level.txt
--rw-r--r--   0 jochen    (1420) escience   (630)     4133 2018-04-25 08:06:52.000000 django-daiquiri-0.2/django_daiquiri.egg-info/PKG-INFO
--rw-r--r--   0 jochen    (1420) escience   (630)      496 2018-04-25 08:06:52.000000 django-daiquiri-0.2/django_daiquiri.egg-info/requires.txt
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/
--rw-r--r--   0 jochen    (1420) escience   (630)      159 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/serve/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       55 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/serve/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      448 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/serve/serializers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1431 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/serve/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)      416 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/serve/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/serve/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      574 2018-03-16 15:49:43.000000 django-daiquiri-0.2/daiquiri/serve/urls.py
--rw-r--r--   0 jochen    (1420) escience   (630)      794 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/serve/tasks.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/static/serve/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/static/serve/css/
--rw-r--r--   0 jochen    (1420) escience   (630)      114 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/serve/static/serve/css/table.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/static/serve/js/
--rw-r--r--   0 jochen    (1420) escience   (630)      191 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/serve/static/serve/js/table.js
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/templates/serve/
--rw-r--r--   0 jochen    (1420) escience   (630)     1444 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/serve/templates/serve/table.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/serve/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/serve/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     5645 2018-04-05 14:08:24.000000 django-daiquiri-0.2/daiquiri/serve/tests/test_viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2498 2018-04-05 14:08:24.000000 django-daiquiri-0.2/daiquiri/serve/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3101 2018-03-16 15:49:48.000000 django-daiquiri-0.2/daiquiri/serve/viewsets.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/
--rw-r--r--   0 jochen    (1420) escience   (630)      119 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/responses.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2058 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/permissions.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/templatetags/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templatetags/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2668 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/core/templatetags/core_tags.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2562 2018-04-10 13:18:20.000000 django-daiquiri-0.2/daiquiri/core/renderers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1777 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/constants.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/settings/
--rw-r--r--   0 jochen    (1420) escience   (630)     4403 2018-04-24 16:10:34.000000 django-daiquiri-0.2/daiquiri/core/settings/base.py
--rw-r--r--   0 jochen    (1420) escience   (630)      111 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/settings/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3963 2018-04-23 09:48:03.000000 django-daiquiri-0.2/daiquiri/core/settings/daiquiri.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4475 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/settings/vendor.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2620 2018-03-15 10:03:17.000000 django-daiquiri-0.2/daiquiri/core/settings/logging.py
--rw-r--r--   0 jochen    (1420) escience   (630)      445 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/settings/celery.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1320 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/core/managers.py
--rw-r--r--   0 jochen    (1420) escience   (630)      881 2018-03-15 10:03:17.000000 django-daiquiri-0.2/daiquiri/core/serializers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1347 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/hashers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     6903 2018-04-25 07:52:33.000000 django-daiquiri-0.2/daiquiri/core/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1921 2018-04-09 11:47:16.000000 django-daiquiri-0.2/daiquiri/core/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/adapter/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/adapter/download/
--rw-r--r--   0 jochen    (1420) escience   (630)     2628 2018-04-23 09:48:03.000000 django-daiquiri-0.2/daiquiri/core/adapter/download/base.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/adapter/download/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1544 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/core/adapter/download/pgdump.py
--rw-r--r--   0 jochen    (1420) escience   (630)      946 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/core/adapter/download/mysqldump.py
--rw-r--r--   0 jochen    (1420) escience   (630)      303 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/core/adapter/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1101 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/core/adapter/stream.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/adapter/database/
--rw-r--r--   0 jochen    (1420) escience   (630)     5096 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/core/adapter/database/base.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/adapter/database/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)    11673 2018-04-17 13:39:48.000000 django-daiquiri-0.2/daiquiri/core/adapter/database/mysql.py
--rw-r--r--   0 jochen    (1420) escience   (630)    15300 2018-04-24 16:01:12.000000 django-daiquiri-0.2/daiquiri/core/adapter/database/postgres.py
--rw-r--r--   0 jochen    (1420) escience   (630)      786 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/core/adapter/database/mariadb.py
--rw-r--r--   0 jochen    (1420) escience   (630)      282 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/tasks.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/static/core/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/static/core/img/
--rw-r--r--   0 jochen    (1420) escience   (630)    19025 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/img/daiquiri.jpg
--rw-r--r--   0 jochen    (1420) escience   (630)     1406 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/img/favicon.ico
--rw-r--r--   0 jochen    (1420) escience   (630)      380 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/img/daiquiri32.png
--rw-r--r--   0 jochen    (1420) escience   (630)      459 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/img/favicon.png
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/
--rw-r--r--   0 jochen    (1420) escience   (630)      444 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_text.html
--rw-r--r--   0 jochen    (1420) escience   (630)      428 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_number.html
--rw-r--r--   0 jochen    (1420) escience   (630)      417 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_codemirror.html
--rw-r--r--   0 jochen    (1420) escience   (630)      862 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_selectnumber.html
--rw-r--r--   0 jochen    (1420) escience   (630)      848 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_select.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1115 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_multicheckbox.html
--rw-r--r--   0 jochen    (1420) escience   (630)      457 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_checkbox.html
--rw-r--r--   0 jochen    (1420) escience   (630)      383 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/order-list.html
--rw-r--r--   0 jochen    (1420) escience   (630)      461 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_textarea.html
--rw-r--r--   0 jochen    (1420) escience   (630)      472 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_radio.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1481 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/html/browser.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/
--rw-r--r--   0 jochen    (1420) escience   (630)    11056 2018-04-25 08:01:28.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/base.scss
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/style.scss
--rw-r--r--   0 jochen    (1420) escience   (630)      153 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/codemirror.scss
--rw-r--r--   0 jochen    (1420) escience   (630)     1662 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/browser.scss
--rw-r--r--   0 jochen    (1420) escience   (630)     3605 2018-03-16 11:24:43.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/table.scss
--rw-r--r--   0 jochen    (1420) escience   (630)      827 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/fonts.scss
--rw-r--r--   0 jochen    (1420) escience   (630)     1665 2018-03-16 11:24:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/variables.scss
--rw-r--r--   0 jochen    (1420) escience   (630)      969 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/css/list.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/
--rw-r--r--   0 jochen    (1420) escience   (630)     1606 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/polling.js
--rw-r--r--   0 jochen    (1420) escience   (630)     2660 2018-04-06 09:58:10.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/core.js
--rw-r--r--   0 jochen    (1420) escience   (630)     1236 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/filter.js
--rw-r--r--   0 jochen    (1420) escience   (630)     9139 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/browser.js
--rw-r--r--   0 jochen    (1420) escience   (630)     2632 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/list.js
--rw-r--r--   0 jochen    (1420) escience   (630)    13836 2018-04-09 11:47:16.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/table.js
--rw-r--r--   0 jochen    (1420) escience   (630)     1303 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/multiCheckbox.js
--rw-r--r--   0 jochen    (1420) escience   (630)     1674 2018-03-15 10:03:17.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/stream.js
--rw-r--r--   0 jochen    (1420) escience   (630)      653 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/byNumber.js
--rw-r--r--   0 jochen    (1420) escience   (630)      898 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/js/formgroup.js
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/static/core/fonts/
--rwxr-xr-x   0 jochen    (1420) escience   (630)    48880 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf
--rwxr-xr-x   0 jochen    (1420) escience   (630)    45652 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf
--rwxr-xr-x   0 jochen    (1420) escience   (630)   117072 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSansMono.ttf
--rwxr-xr-x   0 jochen    (1420) escience   (630)    40416 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf
--rwxr-xr-x   0 jochen    (1420) escience   (630)    41028 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSans.ttf
--rwxr-xr-x   0 jochen    (1420) escience   (630)    42480 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSans-Bold.ttf
--rwxr-xr-x   0 jochen    (1420) escience   (630)    43648 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSerif.ttf
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/templates/core/
--rw-r--r--   0 jochen    (1420) escience   (630)      192 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/core/templates/core/500.html
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/base_footer.html
--rw-r--r--   0 jochen    (1420) escience   (630)      161 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/home.html
--rw-r--r--   0 jochen    (1420) escience   (630)      327 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/page.html
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/base_analytics.html
--rw-r--r--   0 jochen    (1420) escience   (630)      935 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/base_head.html
--rw-r--r--   0 jochen    (1420) escience   (630)      177 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/core/templates/core/403.html
--rw-r--r--   0 jochen    (1420) escience   (630)      185 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/404.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/
--rw-r--r--   0 jochen    (1420) escience   (630)      352 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_header.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1903 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/form_field.html
--rw-r--r--   0 jochen    (1420) escience   (630)      665 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_pagination.html
--rw-r--r--   0 jochen    (1420) escience   (630)      925 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_tooltip.html
--rw-r--r--   0 jochen    (1420) escience   (630)     4706 2018-04-18 14:06:55.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_pane.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1390 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_footer.html
--rw-r--r--   0 jochen    (1420) escience   (630)      463 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_search.html
--rw-r--r--   0 jochen    (1420) escience   (630)      322 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/table.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1693 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_modal.html
--rw-r--r--   0 jochen    (1420) escience   (630)      189 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/core/templates/core/partials/form_fields.html
--rw-r--r--   0 jochen    (1420) escience   (630)      188 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/core/templates/core/400.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2644 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/base_navigation.html
--rw-r--r--   0 jochen    (1420) escience   (630)      173 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/templates/core/wide.html
--rw-r--r--   0 jochen    (1420) escience   (630)      396 2018-04-13 13:45:44.000000 django-daiquiri-0.2/daiquiri/core/templates/core/base.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/management/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/management/commands/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/management/commands/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      795 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/management/commands/runworker.py
--rw-r--r--   0 jochen    (1420) escience   (630)      295 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/management/commands/deploy.py
--rw-r--r--   0 jochen    (1420) escience   (630)      704 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/management/commands/rabbitcreate.py
--rw-r--r--   0 jochen    (1420) escience   (630)      244 2018-03-15 13:25:01.000000 django-daiquiri-0.2/daiquiri/core/management/commands/create_admin_user.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4758 2018-04-24 10:57:04.000000 django-daiquiri-0.2/daiquiri/core/management/commands/sqlcreate.py
--rw-r--r--   0 jochen    (1420) escience   (630)      249 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/management/commands/daiquiri_path.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1189 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/core/management/commands/archive_query_jobs.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1933 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/management/commands/download_vendor_files.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/management/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      101 2018-04-03 10:20:54.000000 django-daiquiri-0.2/daiquiri/core/exceptions.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/core/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/tests/test_viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)      494 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2114 2018-04-17 13:21:10.000000 django-daiquiri-0.2/daiquiri/core/tests/test_adapter.py
--rw-r--r--   0 jochen    (1420) escience   (630)      368 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/routers.py
--rw-r--r--   0 jochen    (1420) escience   (630)      118 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/core/http.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2705 2018-04-23 13:17:57.000000 django-daiquiri-0.2/daiquiri/core/generators.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1904 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/core/viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)      164 2018-04-24 15:14:04.000000 django-daiquiri-0.2/daiquiri/core/paginations.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/
--rw-r--r--   0 jochen    (1420) escience   (630)     4133 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/handlers.py
--rw-r--r--   0 jochen    (1420) escience   (630)      208 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       53 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1544 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/adapter.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1995 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/serializers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2204 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/auth/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3637 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      625 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0008_profile_is_pending.py
--rw-r--r--   0 jochen    (1420) escience   (630)      522 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0004_view_permission_typo.py
--rw-r--r--   0 jochen    (1420) escience   (630)      535 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0005_view_permission_fix.py
--rw-r--r--   0 jochen    (1420) escience   (630)      581 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0006_profile_ordering.py
--rw-r--r--   0 jochen    (1420) escience   (630)      526 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0003_view_permission.py
--rw-r--r--   0 jochen    (1420) escience   (630)      366 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0009_delete_detailkey.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2089 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0001_profile_model.py
--rw-r--r--   0 jochen    (1420) escience   (630)      459 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0007_profile_is_confirmed.py
--rw-r--r--   0 jochen    (1420) escience   (630)      486 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/migrations/0002_profile_attributes.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2087 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/auth/forms.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/static/auth/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/static/auth/css/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/static/auth/css/users.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/static/auth/js/
--rw-r--r--   0 jochen    (1420) escience   (630)     1722 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/static/auth/js/users.js
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/
--rw-r--r--   0 jochen    (1420) escience   (630)     2731 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users_options.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1050 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_confirm_user.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1044 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_reject_user.html
--rw-r--r--   0 jochen    (1420) escience   (630)     3020 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_show_user.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1054 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_activate_user.html
--rw-r--r--   0 jochen    (1420) escience   (630)     3331 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_update_user.html
--rw-r--r--   0 jochen    (1420) escience   (630)     6373 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1050 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_disable_user.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1038 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_enable_user.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/
--rw-r--r--   0 jochen    (1420) escience   (630)      238 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/logout_form.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1080 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/signup.html
--rw-r--r--   0 jochen    (1420) escience   (630)      309 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/account_pending.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1594 2018-04-23 09:48:03.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/login_form.html
--rw-r--r--   0 jochen    (1420) escience   (630)      178 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/account_inactive.html
--rw-r--r--   0 jochen    (1420) escience   (630)      511 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/password_set.html
--rw-r--r--   0 jochen    (1420) escience   (630)      769 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/verified_email_required.html
--rw-r--r--   0 jochen    (1420) escience   (630)      853 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/password_reset_from_key.html
--rw-r--r--   0 jochen    (1420) escience   (630)      473 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/password_reset_done.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/
--rw-r--r--   0 jochen    (1420) escience   (630)      556 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/password_reset_key_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       46 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/notify_activation_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      407 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/request_confirmation_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       45 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/notify_rejection_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      308 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/activation_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      308 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/notify_activation_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       55 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/activation_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      392 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      411 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/request_activation_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       54 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/request_confirmation_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       55 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/request_activation_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       46 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/notify_confirmation_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      372 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/notify_confirmation_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       43 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/password_reset_key_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      354 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/notify_rejection_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       62 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email/email_confirmation_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      224 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/login.html
--rw-r--r--   0 jochen    (1420) escience   (630)      588 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/account_token.html
--rw-r--r--   0 jochen    (1420) escience   (630)      254 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/password_change_done.html
--rw-r--r--   0 jochen    (1420) escience   (630)      532 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/password_reset.html
--rw-r--r--   0 jochen    (1420) escience   (630)      546 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/logout.html
--rw-r--r--   0 jochen    (1420) escience   (630)      365 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/verification_sent.html
--rw-r--r--   0 jochen    (1420) escience   (630)      201 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/signup_closed.html
--rw-r--r--   0 jochen    (1420) escience   (630)      341 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/password_reset_from_key_done.html
--rw-r--r--   0 jochen    (1420) escience   (630)      975 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email_confirm.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2783 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/email.html
--rw-r--r--   0 jochen    (1420) escience   (630)      247 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/password_set_done.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1048 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/account_profile.html
--rw-r--r--   0 jochen    (1420) escience   (630)      550 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/account/password_change.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/
--rw-r--r--   0 jochen    (1420) escience   (630)     1211 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/signup.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/snippets/
--rw-r--r--   0 jochen    (1420) escience   (630)      909 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0 jochen    (1420) escience   (630)      435 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/login_cancelled.html
--rw-r--r--   0 jochen    (1420) escience   (630)      303 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/authentication_error.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1879 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/connections.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2139 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/models.py
--rw-r--r--   0 jochen    (1420) escience   (630)      481 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/signals.py
--rw-r--r--   0 jochen    (1420) escience   (630)      274 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/auth/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     5846 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/tests/test_accounts.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4563 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/tests/test_viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)      501 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)      993 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/auth/urls_accounts.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3040 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)      433 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/auth/urls_auth.py
--rw-r--r--   0 jochen    (1420) escience   (630)      241 2018-04-25 08:04:29.000000 django-daiquiri-0.2/daiquiri/__init__.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/
--rw-r--r--   0 jochen    (1420) escience   (630)      272 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/permissions.py
--rw-r--r--   0 jochen    (1420) escience   (630)      158 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       59 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      458 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1337 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/migrations/0001_initial.py
--rw-r--r--   0 jochen    (1420) escience   (630)      401 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/migrations/0003_remove_archivejob_file_path.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1388 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/migrations/0002_collection.py
--rw-r--r--   0 jochen    (1420) escience   (630)      593 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/urls.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1353 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/archive/tasks.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/static/archive/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/static/archive/css/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/static/archive/css/archive.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/static/archive/js/
--rw-r--r--   0 jochen    (1420) escience   (630)     2629 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/static/archive/js/archive.js
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/templates/archive/
--rw-r--r--   0 jochen    (1420) escience   (630)     3000 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/templates/archive/archive.html
--rw-r--r--   0 jochen    (1420) escience   (630)     6243 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/archive/models.py
--rw-r--r--   0 jochen    (1420) escience   (630)      480 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/archive/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4696 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/archive/tests/test_viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)      512 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/archive/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)     5356 2018-04-03 10:37:42.000000 django-daiquiri-0.2/daiquiri/archive/viewsets.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/
--rw-r--r--   0 jochen    (1420) escience   (630)     1023 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/tap/handlers.py
--rw-r--r--   0 jochen    (1420) escience   (630)      195 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4058 2018-04-23 09:48:03.000000 django-daiquiri-0.2/daiquiri/tap/renderers.py
--rw-r--r--   0 jochen    (1420) escience   (630)       51 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1583 2018-04-23 10:45:50.000000 django-daiquiri-0.2/daiquiri/tap/serializers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4788 2018-04-17 13:16:19.000000 django-daiquiri-0.2/daiquiri/tap/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4080 2018-04-13 13:54:30.000000 django-daiquiri-0.2/daiquiri/tap/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3204 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/migrations/0001_initial.py
--rw-r--r--   0 jochen    (1420) escience   (630)      811 2018-04-11 14:58:28.000000 django-daiquiri-0.2/daiquiri/tap/urls.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/static/tap/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/static/tap/css/
--rw-r--r--   0 jochen    (1420) escience   (630)       50 2018-04-13 13:47:56.000000 django-daiquiri-0.2/daiquiri/tap/static/tap/css/examples.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/templates/tap/
--rw-r--r--   0 jochen    (1420) escience   (630)      646 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/templates/tap/root.html
--rw-r--r--   0 jochen    (1420) escience   (630)      933 2018-04-13 13:55:43.000000 django-daiquiri-0.2/daiquiri/tap/templates/tap/examples.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2049 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/models.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/management/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/management/commands/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/management/commands/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      523 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/tap/management/commands/rebuild_tap_schema.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/management/__init__.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/tap/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2027 2018-04-17 13:34:15.000000 django-daiquiri-0.2/daiquiri/tap/tests/test_async.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1497 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/tap/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1609 2018-04-17 13:34:18.000000 django-daiquiri-0.2/daiquiri/tap/tests/test_sync.py
--rw-r--r--   0 jochen    (1420) escience   (630)      888 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/tap/routers.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/
--rw-r--r--   0 jochen    (1420) escience   (630)      692 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/handlers.py
--rw-r--r--   0 jochen    (1420) escience   (630)      265 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/permissions.py
--rw-r--r--   0 jochen    (1420) escience   (630)      203 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       55 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      437 2018-03-05 16:37:54.000000 django-daiquiri-0.2/daiquiri/query/managers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4835 2018-04-23 10:31:17.000000 django-daiquiri-0.2/daiquiri/query/serializers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     8795 2018-04-23 10:59:57.000000 django-daiquiri-0.2/daiquiri/query/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1067 2018-04-06 13:01:29.000000 django-daiquiri-0.2/daiquiri/query/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)      469 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0011_queryjob_native_query.py
--rw-r--r--   0 jochen    (1420) escience   (630)      648 2018-04-13 11:43:07.000000 django-daiquiri-0.2/daiquiri/query/migrations/0017_big_integer_fields.py
--rw-r--r--   0 jochen    (1420) escience   (630)      469 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0012_query_language_length.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1611 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/query/migrations/0015_queryarchivejob.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      447 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/query/migrations/0016_rename_database_to_schema.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2222 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0013_refactoring.py
--rw-r--r--   0 jochen    (1420) escience   (630)      463 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0008_queryjob_pid.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1025 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0003_query_language_and_actual_query.py
--rw-r--r--   0 jochen    (1420) escience   (630)      485 2018-04-18 14:10:33.000000 django-daiquiri-0.2/daiquiri/query/migrations/0018_blank_metadata.py
--rw-r--r--   0 jochen    (1420) escience   (630)      613 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0009_remove_choices.py
--rw-r--r--   0 jochen    (1420) escience   (630)      502 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0002_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      505 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0007_queryjob_metadata.py
--rw-r--r--   0 jochen    (1420) escience   (630)      476 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0010_queue_can_be_null.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1155 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0006_example.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1214 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0001_initial.py
--rw-r--r--   0 jochen    (1420) escience   (630)      702 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0005_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1453 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/migrations/0014_downloadjob.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1149 2018-02-16 16:50:12.000000 django-daiquiri-0.2/daiquiri/query/migrations/0004_table_name.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1115 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/urls.py
--rw-r--r--   0 jochen    (1420) escience   (630)    10468 2018-04-24 15:23:07.000000 django-daiquiri-0.2/daiquiri/query/tasks.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/static/query/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/static/query/css/
--rw-r--r--   0 jochen    (1420) escience   (630)       35 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/static/query/css/examples.scss
--rw-r--r--   0 jochen    (1420) escience   (630)     3784 2018-04-06 12:58:15.000000 django-daiquiri-0.2/daiquiri/query/static/query/css/query.scss
--rw-r--r--   0 jochen    (1420) escience   (630)      214 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/static/query/css/jobs.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/forms/
--rw-r--r--   0 jochen    (1420) escience   (630)     1045 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/forms/cone.js
--rw-r--r--   0 jochen    (1420) escience   (630)     4441 2018-04-23 10:38:48.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/forms/sql.js
--rw-r--r--   0 jochen    (1420) escience   (630)     1254 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/forms/box.js
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/dropdowns/
--rw-r--r--   0 jochen    (1420) escience   (630)     1207 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/dropdowns/simbad.js
--rw-r--r--   0 jochen    (1420) escience   (630)     1893 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/dropdowns/vizier.js
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/services/
--rw-r--r--   0 jochen    (1420) escience   (630)     3792 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/services/jobs.js
--rw-r--r--   0 jochen    (1420) escience   (630)     4073 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/services/download.js
--rw-r--r--   0 jochen    (1420) escience   (630)    11761 2018-04-06 12:59:45.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/services/query.js
--rw-r--r--   0 jochen    (1420) escience   (630)     3109 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/services/examples.js
--rw-r--r--   0 jochen    (1420) escience   (630)     6371 2018-04-24 14:23:56.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/services/plot.js
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/apps/
--rw-r--r--   0 jochen    (1420) escience   (630)      223 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/apps/jobs.js
--rw-r--r--   0 jochen    (1420) escience   (630)     1449 2018-04-06 11:03:34.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/apps/query.js
--rw-r--r--   0 jochen    (1420) escience   (630)      243 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/static/query/js/apps/examples.js
--rw-r--r--   0 jochen    (1420) escience   (630)      597 2018-04-24 15:12:51.000000 django-daiquiri-0.2/daiquiri/query/filters.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/templates/query/
--rw-r--r--   0 jochen    (1420) escience   (630)     4036 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/jobs_modal_show_job.html
--rw-r--r--   0 jochen    (1420) escience   (630)     5832 2018-04-06 12:58:40.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_sidebar.html
--rw-r--r--   0 jochen    (1420) escience   (630)     4576 2018-04-17 15:49:40.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_overview.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1557 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_modal_update_job.html
--rw-r--r--   0 jochen    (1420) escience   (630)     4958 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query.html
--rw-r--r--   0 jochen    (1420) escience   (630)      602 2018-04-05 14:40:15.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_examples.html
--rw-r--r--   0 jochen    (1420) escience   (630)      565 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_columns.html
--rw-r--r--   0 jochen    (1420) escience   (630)     3657 2018-04-24 07:33:20.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_form_box.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1475 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/examples_modal_delete.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2906 2018-04-24 07:33:20.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_form_sql.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2965 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_vizier.html
--rw-r--r--   0 jochen    (1420) escience   (630)     6537 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/jobs.html
--rw-r--r--   0 jochen    (1420) escience   (630)      188 2018-04-24 10:45:31.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_form.html
--rw-r--r--   0 jochen    (1420) escience   (630)     4906 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/examples.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1578 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_download.html
--rw-r--r--   0 jochen    (1420) escience   (630)      582 2018-04-23 12:08:57.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_schemas.html
--rw-r--r--   0 jochen    (1420) escience   (630)      351 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/templates/query/examples_options.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1339 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_modal_archive_job.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2325 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_simbad.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1329 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_modal_abort_job.html
--rw-r--r--   0 jochen    (1420) escience   (630)     3764 2018-04-16 12:34:59.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_plot.html
--rw-r--r--   0 jochen    (1420) escience   (630)       62 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_results.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2560 2018-04-24 07:33:20.000000 django-daiquiri-0.2/daiquiri/query/templates/query/query_form_cone.html
--rw-r--r--   0 jochen    (1420) escience   (630)     4918 2018-04-23 10:54:17.000000 django-daiquiri-0.2/daiquiri/query/templates/query/examples_modal_form.html
--rw-r--r--   0 jochen    (1420) escience   (630)    21474 2018-04-24 16:20:02.000000 django-daiquiri-0.2/daiquiri/query/models.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/management/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/management/commands/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-04-18 14:27:25.000000 django-daiquiri-0.2/daiquiri/query/management/commands/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1949 2018-04-18 15:51:41.000000 django-daiquiri-0.2/daiquiri/query/management/commands/fix_jobs.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-04-18 14:28:57.000000 django-daiquiri-0.2/daiquiri/query/management/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1162 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/query/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/query/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     9052 2018-04-17 13:34:05.000000 django-daiquiri-0.2/daiquiri/query/tests/test_viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)      767 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/query/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3034 2018-04-23 10:20:41.000000 django-daiquiri-0.2/daiquiri/query/tests/test_permissions.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1096 2018-04-10 15:18:50.000000 django-daiquiri-0.2/daiquiri/query/validators.py
--rw-r--r--   0 jochen    (1420) escience   (630)    13224 2018-04-24 18:16:40.000000 django-daiquiri-0.2/daiquiri/query/viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2366 2018-04-10 15:20:21.000000 django-daiquiri-0.2/daiquiri/query/process.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/stats/
--rw-r--r--   0 jochen    (1420) escience   (630)      150 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/stats/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       54 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/stats/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      929 2018-03-08 12:24:03.000000 django-daiquiri-0.2/daiquiri/stats/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/stats/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/stats/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      880 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/stats/migrations/0002_data_migration.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1291 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/stats/migrations/0001_initial.py
--rw-r--r--   0 jochen    (1420) escience   (630)      160 2018-03-08 12:24:03.000000 django-daiquiri-0.2/daiquiri/stats/urls.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/stats/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/stats/templates/stats/
--rw-r--r--   0 jochen    (1420) escience   (630)      730 2018-03-08 12:34:43.000000 django-daiquiri-0.2/daiquiri/stats/templates/stats/management.html
--rw-r--r--   0 jochen    (1420) escience   (630)      835 2018-03-08 11:38:37.000000 django-daiquiri-0.2/daiquiri/stats/models.py
--rw-r--r--   0 jochen    (1420) escience   (630)      296 2018-03-08 11:27:46.000000 django-daiquiri-0.2/daiquiri/stats/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/uws/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/uws/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      839 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/uws/urls.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/uws/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/uws/templates/uws/
--rw-r--r--   0 jochen    (1420) escience   (630)      122 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/uws/templates/uws/root.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/wordpress/
--rw-r--r--   0 jochen    (1420) escience   (630)      563 2018-04-25 07:52:33.000000 django-daiquiri-0.2/daiquiri/wordpress/handlers.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/wordpress/templatetags/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/wordpress/templatetags/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      885 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/wordpress/templatetags/wordpress_tags.py
--rw-r--r--   0 jochen    (1420) escience   (630)      247 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/wordpress/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       63 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/wordpress/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1020 2018-04-25 07:52:33.000000 django-daiquiri-0.2/daiquiri/wordpress/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1567 2018-04-25 07:52:33.000000 django-daiquiri-0.2/daiquiri/wordpress/tasks.py
--rw-r--r--   0 jochen    (1420) escience   (630)      517 2018-04-25 07:52:33.000000 django-daiquiri-0.2/daiquiri/wordpress/rules.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/wordpress/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/wordpress/static/wordpress/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/wordpress/static/wordpress/css/
--rw-r--r--   0 jochen    (1420) escience   (630)     2638 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/wordpress/static/wordpress/css/wordpress.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/wordpress/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/wordpress/templates/wordpress/
--rw-r--r--   0 jochen    (1420) escience   (630)      349 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/wordpress/templates/wordpress/layout.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/cutout/
--rw-r--r--   0 jochen    (1420) escience   (630)      266 2018-03-16 16:38:00.000000 django-daiquiri-0.2/daiquiri/cutout/permissions.py
--rw-r--r--   0 jochen    (1420) escience   (630)      163 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/cutout/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)      350 2018-03-15 10:28:03.000000 django-daiquiri-0.2/daiquiri/cutout/renderers.py
--rw-r--r--   0 jochen    (1420) escience   (630)       57 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/cutout/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      269 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/cutout/adapter.py
--rw-r--r--   0 jochen    (1420) escience   (630)      167 2018-03-16 16:39:59.000000 django-daiquiri-0.2/daiquiri/cutout/urls.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1264 2018-03-16 16:47:46.000000 django-daiquiri-0.2/daiquiri/cutout/viewsets.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/
--rw-r--r--   0 jochen    (1420) escience   (630)      158 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       59 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      571 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/serializers.py
--rw-r--r--   0 jochen    (1420) escience   (630)      603 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/contact/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1383 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      755 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/migrations/0002_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      584 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/migrations/0004_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      582 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/migrations/0003_add_permissions.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1441 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/migrations/0001_initial.py
--rw-r--r--   0 jochen    (1420) escience   (630)      530 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/urls.py
--rw-r--r--   0 jochen    (1420) escience   (630)      841 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/forms.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/static/contact/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/static/contact/css/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/static/contact/css/messages.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/static/contact/js/
--rw-r--r--   0 jochen    (1420) escience   (630)     1556 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/static/contact/js/messages.js
--rw-r--r--   0 jochen    (1420) escience   (630)      476 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/filters.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/
--rw-r--r--   0 jochen    (1420) escience   (630)      674 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/contact.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1986 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/messages_modal_show.html
--rw-r--r--   0 jochen    (1420) escience   (630)     5322 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/messages.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1696 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/messages_options.html
--rw-r--r--   0 jochen    (1420) escience   (630)      252 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/thanks.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/email/
--rw-r--r--   0 jochen    (1420) escience   (630)      407 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/email/new_message_admin_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       48 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/email/new_message_admin_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      326 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/email/new_message_user_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      104 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/email/contact_template.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       49 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/email/new_message_user_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      283 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/templates/contact/messages_mailto.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1586 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/models.py
--rw-r--r--   0 jochen    (1420) escience   (630)      314 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/contact/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1122 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/tests/test_viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2227 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1212 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/contact/viewsets.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/meetings/
--rw-r--r--   0 jochen    (1420) escience   (630)      162 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/meetings/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       61 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/meetings/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      781 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3102 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/meetings/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/meetings/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)      580 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/migrations/0002_meeting_registration_done_message.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/meetings/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4960 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/migrations/0001_initial.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1710 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/migrations/0003_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      910 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/urls.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3236 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/meetings/forms.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/meetings/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/
--rw-r--r--   0 jochen    (1420) escience   (630)      218 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/participants_closed.html
--rw-r--r--   0 jochen    (1420) escience   (630)      203 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/registration_closed.html
--rw-r--r--   0 jochen    (1420) escience   (630)      727 2018-03-15 10:33:04.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/registration.html
--rw-r--r--   0 jochen    (1420) escience   (630)      461 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/contributions.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/email/
--rw-r--r--   0 jochen    (1420) escience   (630)       45 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/email/notify_registration_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      373 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/email/notify_registration_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      418 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/email/registration_message.txt
--rw-r--r--   0 jochen    (1420) escience   (630)       46 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/email/registration_subject.txt
--rw-r--r--   0 jochen    (1420) escience   (630)      386 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/participants.html
--rw-r--r--   0 jochen    (1420) escience   (630)      197 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/registration_done.html
--rw-r--r--   0 jochen    (1420) escience   (630)      220 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/templates/meetings/contributions_closed.html
--rw-r--r--   0 jochen    (1420) escience   (630)     5607 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/models.py
--rw-r--r--   0 jochen    (1420) escience   (630)      782 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/meetings/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/meetings/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/meetings/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     6393 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/meetings/tests/test_views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/conesearch/
--rw-r--r--   0 jochen    (1420) escience   (630)      270 2018-03-16 16:50:40.000000 django-daiquiri-0.2/daiquiri/conesearch/permissions.py
--rw-r--r--   0 jochen    (1420) escience   (630)      179 2018-03-15 10:03:17.000000 django-daiquiri-0.2/daiquiri/conesearch/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)      354 2018-03-15 10:23:21.000000 django-daiquiri-0.2/daiquiri/conesearch/renderers.py
--rw-r--r--   0 jochen    (1420) escience   (630)       65 2018-03-15 10:03:17.000000 django-daiquiri-0.2/daiquiri/conesearch/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2247 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/conesearch/adapter.py
--rw-r--r--   0 jochen    (1420) escience   (630)      169 2018-03-16 16:53:30.000000 django-daiquiri-0.2/daiquiri/conesearch/urls.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1285 2018-04-23 12:31:16.000000 django-daiquiri-0.2/daiquiri/conesearch/viewsets.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/jobs/
--rw-r--r--   0 jochen    (1420) escience   (630)      146 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3038 2018-04-11 15:27:55.000000 django-daiquiri-0.2/daiquiri/jobs/renderers.py
--rw-r--r--   0 jochen    (1420) escience   (630)       53 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      456 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/jobs/managers.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1995 2018-04-11 15:05:22.000000 django-daiquiri-0.2/daiquiri/jobs/serializers.py
--rw-r--r--   0 jochen    (1420) escience   (630)      629 2018-04-11 15:28:02.000000 django-daiquiri-0.2/daiquiri/jobs/utils.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)      539 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0012_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      583 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0005_owner_null_true.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      477 2018-04-05 14:05:53.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0014_blank_run_id.py
--rw-r--r--   0 jochen    (1420) escience   (630)      505 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0009_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      805 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0010_add_fields.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1705 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0001_job_model.py
--rw-r--r--   0 jochen    (1420) escience   (630)      456 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0013_job_error_summary.py
--rw-r--r--   0 jochen    (1420) escience   (630)      874 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0004_phases_to_char.py
--rw-r--r--   0 jochen    (1420) escience   (630)      586 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0003_owner_fk.py
--rw-r--r--   0 jochen    (1420) escience   (630)      473 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0002_execution_duration_default_0.py
--rw-r--r--   0 jochen    (1420) escience   (630)      596 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0006_owner_blank_true.py
--rw-r--r--   0 jochen    (1420) escience   (630)      476 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0008_job_error_summary.py
--rw-r--r--   0 jochen    (1420) escience   (630)      466 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0007_creation_time.py
--rw-r--r--   0 jochen    (1420) escience   (630)      465 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/migrations/0011_job_client_ip.py
--rw-r--r--   0 jochen    (1420) escience   (630)      995 2018-04-11 13:30:34.000000 django-daiquiri-0.2/daiquiri/jobs/filters.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3436 2018-04-11 15:20:06.000000 django-daiquiri-0.2/daiquiri/jobs/models.py
--rw-r--r--   0 jochen    (1420) escience   (630)      270 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/jobs/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)    23688 2018-04-11 15:30:47.000000 django-daiquiri-0.2/daiquiri/jobs/tests/mixins.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/jobs/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1045 2018-04-11 13:38:13.000000 django-daiquiri-0.2/daiquiri/jobs/routers.py
--rw-r--r--   0 jochen    (1420) escience   (630)    10522 2018-04-11 15:25:28.000000 django-daiquiri-0.2/daiquiri/jobs/viewsets.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/
--rw-r--r--   0 jochen    (1420) escience   (630)      261 2018-04-05 15:10:44.000000 django-daiquiri-0.2/daiquiri/metadata/handlers.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/templatetags/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/templatetags/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1462 2018-04-23 09:48:03.000000 django-daiquiri-0.2/daiquiri/metadata/templatetags/metadata_tags.py
--rw-r--r--   0 jochen    (1420) escience   (630)      215 2018-04-05 15:11:06.000000 django-daiquiri-0.2/daiquiri/metadata/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       61 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/__init__.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/serializers/
--rw-r--r--   0 jochen    (1420) escience   (630)     1683 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/serializers/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2676 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/serializers/export.py
--rw-r--r--   0 jochen    (1420) escience   (630)      740 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/serializers/management.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2091 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/serializers/user.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2241 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)      563 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0014_rename_pid_to_doi.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3913 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0007_access_level.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2266 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0016_rename_database_to_schema.py
--rw-r--r--   0 jochen    (1420) escience   (630)      740 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0015_change_doi_to_char.py
--rw-r--r--   0 jochen    (1420) escience   (630)      877 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0003_groups.py
--rw-r--r--   0 jochen    (1420) escience   (630)      583 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0018_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      513 2018-04-13 11:41:58.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0021_table_nrows.py
--rw-r--r--   0 jochen    (1420) escience   (630)      430 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0009_arraysize.py
--rw-r--r--   0 jochen    (1420) escience   (630)      594 2018-04-05 15:25:55.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0020_blank_index_for.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3114 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0005_more_fields.py
--rw-r--r--   0 jochen    (1420) escience   (630)      507 2018-04-13 11:42:03.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0022_table_size.py
--rw-r--r--   0 jochen    (1420) escience   (630)      501 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0004_function_query_string.py
--rw-r--r--   0 jochen    (1420) escience   (630)      578 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0019_column_index_for.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4525 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0001_initial.py
--rw-r--r--   0 jochen    (1420) escience   (630)      499 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0013_remove_directory.py
--rw-r--r--   0 jochen    (1420) escience   (630)    11136 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0006_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      563 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0010_meta.py
--rw-r--r--   0 jochen    (1420) escience   (630)      651 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0017_rename_database_to_schema.py
--rw-r--r--   0 jochen    (1420) escience   (630)      412 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0012_remove_directory_metadata_access_level.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1162 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0008_refactoring.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1073 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0002_published_for.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1672 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/migrations/0011_directory.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1109 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/urls.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/static/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/
--rw-r--r--   0 jochen    (1420) escience   (630)      985 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/pd.png
--rw-r--r--   0 jochen    (1420) escience   (630)     2236 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_nc_sa.png
--rw-r--r--   0 jochen    (1420) escience   (630)     1515 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_nd.png
--rw-r--r--   0 jochen    (1420) escience   (630)     1755 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_sa.png
--rw-r--r--   0 jochen    (1420) escience   (630)     1768 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_nc.png
--rw-r--r--   0 jochen    (1420) escience   (630)     1230 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/cc0.png
--rw-r--r--   0 jochen    (1420) escience   (630)     1331 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/nc.png
--rw-r--r--   0 jochen    (1420) escience   (630)     1173 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by.png
--rw-r--r--   0 jochen    (1420) escience   (630)     1289 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/sa.png
--rw-r--r--   0 jochen    (1420) escience   (630)     2069 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_nc_nd.png
--rw-r--r--   0 jochen    (1420) escience   (630)     1051 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/nd.png
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/css/
--rw-r--r--   0 jochen    (1420) escience   (630)      551 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/css/metadata.scss
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/js/
--rw-r--r--   0 jochen    (1420) escience   (630)     7976 2018-04-16 14:17:34.000000 django-daiquiri-0.2/daiquiri/metadata/static/metadata/js/metadata.js
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/templates/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/
--rw-r--r--   0 jochen    (1420) escience   (630)     1822 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1484 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_delete_columns.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1842 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1492 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_delete_functions.html
--rw-r--r--   0 jochen    (1420) escience   (630)     3187 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2102 2018-04-24 11:40:34.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/table.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1817 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html
--rw-r--r--   0 jochen    (1420) escience   (630)     7039 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1020 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_options.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1503 2018-04-25 07:58:48.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/schema.html
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/tags/
--rw-r--r--   0 jochen    (1420) escience   (630)      482 2018-04-13 12:14:46.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/tags/doi_panel.html
--rw-r--r--   0 jochen    (1420) escience   (630)      429 2018-04-13 12:04:55.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/tags/access_panel.html
--rw-r--r--   0 jochen    (1420) escience   (630)      502 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/tags/license_panel.html
--rw-r--r--   0 jochen    (1420) escience   (630)      349 2018-04-18 10:52:49.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/tags/schemas_menu.html
--rw-r--r--   0 jochen    (1420) escience   (630)     4865 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_functions.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1702 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_delete_tables.html
--rw-r--r--   0 jochen    (1420) escience   (630)     9185 2018-04-13 11:27:45.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_tables.html
--rw-r--r--   0 jochen    (1420) escience   (630)     9339 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_columns.html
--rw-r--r--   0 jochen    (1420) escience   (630)     2253 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_display.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1717 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html
--rw-r--r--   0 jochen    (1420) escience   (630)     1847 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html
--rw-r--r--   0 jochen    (1420) escience   (630)    10957 2018-04-13 11:42:01.000000 django-daiquiri-0.2/daiquiri/metadata/models.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/management/
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/management/commands/
--rw-r--r--   0 jochen    (1420) escience   (630)     1019 2018-04-24 12:22:05.000000 django-daiquiri-0.2/daiquiri/metadata/management/commands/update_access_level.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/management/commands/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)      739 2018-03-16 14:01:34.000000 django-daiquiri-0.2/daiquiri/metadata/management/commands/dump_table.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/management/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1524 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/metadata/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)      655 2018-03-07 15:54:10.000000 django-daiquiri-0.2/daiquiri/metadata/tests/test_tags.py
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/metadata/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3579 2018-03-15 10:03:17.000000 django-daiquiri-0.2/daiquiri/metadata/tests/test_viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)     3062 2018-04-05 14:08:24.000000 django-daiquiri-0.2/daiquiri/metadata/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)     9156 2018-04-24 12:37:03.000000 django-daiquiri-0.2/daiquiri/metadata/viewsets.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/files/
--rw-r--r--   0 jochen    (1420) escience   (630)      159 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/files/apps.py
--rw-r--r--   0 jochen    (1420) escience   (630)       55 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/files/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     2566 2018-04-03 10:37:42.000000 django-daiquiri-0.2/daiquiri/files/utils.py
--rw-r--r--   0 jochen    (1420) escience   (630)      528 2018-03-16 16:35:24.000000 django-daiquiri-0.2/daiquiri/files/views.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/files/migrations/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/files/migrations/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1355 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/files/migrations/0001_initial.py
--rw-r--r--   0 jochen    (1420) escience   (630)      670 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/files/migrations/0002_depth.py
--rw-r--r--   0 jochen    (1420) escience   (630)      373 2018-03-16 16:06:36.000000 django-daiquiri-0.2/daiquiri/files/urls.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1479 2018-03-16 10:58:42.000000 django-daiquiri-0.2/daiquiri/files/models.py
--rw-r--r--   0 jochen    (1420) escience   (630)      349 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/files/admin.py
-drwxr-xr-x   0 jochen    (1420) escience   (630)        0 2018-04-25 08:06:52.000000 django-daiquiri-0.2/daiquiri/files/tests/
--rw-r--r--   0 jochen    (1420) escience   (630)        0 2018-02-16 11:47:27.000000 django-daiquiri-0.2/daiquiri/files/tests/__init__.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1701 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/files/tests/test_viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)     1513 2018-02-16 12:42:24.000000 django-daiquiri-0.2/daiquiri/files/tests/test_views.py
--rw-r--r--   0 jochen    (1420) escience   (630)      918 2018-03-16 16:02:26.000000 django-daiquiri-0.2/daiquiri/files/viewsets.py
--rw-r--r--   0 jochen    (1420) escience   (630)     4133 2018-04-25 08:06:52.000000 django-daiquiri-0.2/PKG-INFO
--rw-r--r--   0 jochen    (1420) escience   (630)     2744 2018-03-07 15:54:10.000000 django-daiquiri-0.2/README.rst
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.426122 django-daiquiri-0.4.2/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      451 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/AUTHORS
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11359 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/LICENSE
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       92 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/MANIFEST.in
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7407 2023-07-19 07:53:11.000000 django-daiquiri-0.4.2/NOTICE
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6177 2023-07-20 09:24:15.426122 django-daiquiri-0.4.2/PKG-INFO
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5302 2023-07-20 09:22:46.000000 django-daiquiri-0.4.2/README.md
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      249 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1571 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      432 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3695 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/auth/forms.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4902 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/handlers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2089 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0001_profile_model.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      486 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0002_profile_attributes.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      526 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0003_view_permission.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      522 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0004_view_permission_typo.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      535 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0005_view_permission_fix.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      581 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0006_profile_ordering.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0007_profile_is_confirmed.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      625 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0008_profile_is_pending.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      366 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0009_delete_detailkey.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0010_profile_consent.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      774 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0011_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      448 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0012_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0013_alter_profile_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      567 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0014_use_django_jsonfield.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2358 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      367 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2055 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      145 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/settings.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      266 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/signals.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/auth/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/auth/static/auth/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/static/auth/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/static/auth/css/users.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/static/auth/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1724 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/static/auth/js/users.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/auth/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/templates/account/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      178 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_inactive.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      309 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_pending.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1124 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_profile.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      588 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_token.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      308 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/activation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       55 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/activation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      392 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       62 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/email_confirmation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      308 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_activation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       46 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_activation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      372 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_confirmation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       46 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_confirmation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_password_changed_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       44 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_password_changed_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      354 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_rejection_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       45 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_rejection_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/password_reset_key_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       43 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/password_reset_key_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      411 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/request_activation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       55 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/request_activation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      407 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/request_confirmation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       54 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/request_confirmation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2783 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      975 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email_confirm.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      224 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/login.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1594 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/login_form.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      546 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/logout.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      383 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/logout_form.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      550 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_change.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      254 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_change_done.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      532 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset_done.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      853 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset_from_key.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      511 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_set.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_set_done.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3164 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/signup.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      201 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/signup_closed.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       17 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/terms_of_use.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      365 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/verification_sent.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      769 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/verified_email_required.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6370 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1054 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_activate_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_confirm_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_disable_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1038 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_enable_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1044 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_reject_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3020 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_show_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3331 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_update_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2167 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_options.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/authentication_error.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1879 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/connections.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      766 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/login.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      435 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3294 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/signup.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/snippets/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      904 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/snippets/provider_list.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6328 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_accounts.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2301 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_honeypot.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      552 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2728 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_viewset_group.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7451 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_viewset_profile.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      968 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/urls_accounts.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      447 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/urls_auth.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      760 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/validators.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3472 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/conesearch/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/conesearch/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5814 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/conesearch/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      171 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      270 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      354 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/renderers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      273 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/conesearch/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/conesearch/templates/conesearch/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      508 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/templates/conesearch/root.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      652 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1347 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/viewsets.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3198 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      314 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      158 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/filters.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      815 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/contact/forms.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1441 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      755 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0002_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      582 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0003_add_permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      584 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0004_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      440 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0005_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      449 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0006_alter_contactmessage_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1376 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      571 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/serializers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/contact/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/contact/static/contact/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/static/contact/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/static/contact/css/messages.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/static/contact/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/static/contact/js/messages.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/contact/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      959 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/contact.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      104 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/contact_template.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      407 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/new_message_admin_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       48 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/new_message_admin_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      326 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/new_message_user_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       49 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/new_message_user_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5319 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      283 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_mailto.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1986 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_modal_show.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1028 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_options.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/thanks.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/contact/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2336 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3477 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/tests/test_viewset_contact_messages.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1104 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/tests/test_viewset_status.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      541 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      822 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1546 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1215 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/adapter/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/adapter/database/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12923 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/base.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/mariadb.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8216 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/mysql.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12800 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/postgres.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/adapter/download/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/download/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5237 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/download/base.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1011 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/download/mysqldump.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1618 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/download/pgdump.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1100 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/stream.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      936 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/celery.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1707 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/constants.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      219 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/encoders.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2584 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/env.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      101 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/exceptions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14347 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/core/generators.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1346 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/hashers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      118 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/http.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      586 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/activate_user.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      244 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/create_admin_user.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      246 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/daiquiri_path.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2417 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/delete_users.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      295 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/deploy.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5286 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/find_users.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      606 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/promote_user.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      679 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/rabbitcreate.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1021 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/runworker.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      434 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/setup_groups.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      223 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/show_databases.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4661 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/sqlcreate.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1718 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/workers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1338 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/managers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      675 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/middleware.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      164 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/paginations.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2058 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/permissions.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/renderers/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2636 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6120 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/datacite.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1596 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/dublincore.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3960 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/voresource.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6832 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/vosi.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      118 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/responses.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2007 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/routers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1158 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/serializers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/settings/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/settings/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      805 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/settings/daiquiri.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7551 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/settings/django.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3471 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/settings/logging.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4462 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/settings/vendor.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/core/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/core/static/core/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11581 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/base.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1874 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/browser.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4889 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/codehilite.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      153 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/codemirror.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      827 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/fonts.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/list.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/style.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4551 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/table.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1665 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/variables.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    42480 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSans-Bold.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    41028 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSans.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)   117072 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSansMono.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    48880 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    45652 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    40416 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    43648 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif.ttf
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/html/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1759 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/browser.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      457 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_checkbox.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      417 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_codemirror.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      421 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_date.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      471 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_file.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1115 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_multicheckbox.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      428 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_number.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      472 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_radio.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      848 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_select.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      862 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_selectnumber.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      444 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_text.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      461 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_textarea.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      486 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_textareasplit.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      383 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/order-list.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/img/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    19025 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/img/daiquiri.jpg
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      380 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/img/daiquiri32.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1406 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/img/favicon.ico
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/img/favicon.png
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9139 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/browser.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      653 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/byNumber.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4597 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/core.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1435 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/filter.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      917 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/formgroup.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/list.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/multiCheckbox.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1606 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/polling.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1839 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/stream.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14578 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/table.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      224 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/tasks.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/core/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/templates/core/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      188 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/400.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      177 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/403.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      185 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/404.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      192 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/500.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      396 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_analytics.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_footer.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1024 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_head.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1801 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      568 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation_account.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation_admin.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1391 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation_management.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      156 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/home.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/page.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1903 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/form_field.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      189 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/form_fields.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      322 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1390 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_footer.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      352 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_header.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2637 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_modal.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      665 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_pagination.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5391 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_pane.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      463 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_search.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1007 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_tooltip.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      183 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/wide.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/core/templatetags/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templatetags/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1495 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/templatetags/core_tags.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/core/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1862 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/tests/test_adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      384 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12749 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/core/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2720 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2092 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/viewsets.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      319 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/cutout/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/cutout/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      269 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      154 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/renderers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       88 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/settings.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      191 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1326 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/datalink/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9541 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/datalink/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4909 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/constants.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      579 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/management/commands/rebuild_datalink_table.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1320 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      426 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/migrations/0002_alter_datalink_content_length.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      450 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/datalink/migrations/0003_alter_datalink_content_length.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1209 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/datalink/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1724 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       91 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/datalink/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/templates/datalink/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1719 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/datalink/templates/datalink/datalink.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/templates/datalink/root.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      690 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/datalink/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      959 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      697 2023-04-27 21:33:15.000000 django-daiquiri-0.4.2/daiquiri/datalink/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1728 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/viewsets.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2789 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      371 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/apps.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1355 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      670 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0002_depth.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      660 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0003_python3.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      410 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0004_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      496 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0005_directory_layout.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      451 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0006_alter_directory_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0007_alter_directory_layout.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1470 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5211 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/files/search.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      217 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/files/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/templates/files/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      194 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/files/templates/files/layout.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1409 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templates/files/list-results.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      261 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templates/files/search-input.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      220 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templates/files/search-results.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/templatetags/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templatetags/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templatetags/search_highlight.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1891 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      252 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2991 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2045 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/views.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/jobs/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/jobs/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      898 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/jobs/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      146 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      101 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/exceptions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      995 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/filters.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      454 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/managers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/jobs/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1705 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0001_job_model.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0002_execution_duration_default_0.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      586 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0003_owner_fk.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      874 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0004_phases_to_char.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      583 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0005_owner_null_true.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      596 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0006_owner_blank_true.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      466 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0007_creation_time.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0008_job_error_summary.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      505 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0009_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      805 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0010_add_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      465 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0011_job_client_ip.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      539 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0012_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      456 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0013_job_error_summary.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      477 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0014_blank_run_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1088 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0015_job_index.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      400 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0016_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3378 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/jobs/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3038 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/renderers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1041 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/routers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2766 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/jobs/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      919 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/jobs/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11152 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/jobs/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/metadata/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1893 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      215 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3187 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/handlers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/metadata/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/metadata/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      739 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/management/commands/dump_table.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1019 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/management/commands/update_access_level.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4525 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1073 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0002_published_for.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      877 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0003_groups.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      501 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0004_function_query_string.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0005_more_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11136 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0006_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3913 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0007_access_level.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0008_refactoring.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      430 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0009_arraysize.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0010_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1672 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0011_directory.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      412 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0012_remove_directory_metadata_access_level.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      499 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0013_remove_directory.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0014_rename_pid_to_doi.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0015_change_doi_to_char.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0016_rename_database_to_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1307 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0017_rename_database_to_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      583 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0018_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      578 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0019_column_index_for.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      594 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0020_blank_index_for.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      513 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0021_table_nrows.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0022_table_size.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5264 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0023_python3.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1010 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0024_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      974 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0025_add_published_updated.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1060 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0026_add_creators_and_contributors.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1798 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0027_auto_20201202_1625.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2392 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0028_add_related_identifiers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1089 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0029_alter_ids.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0030_move_licenses_to_settings.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1059 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0031_change_order.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1714 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0032_data_migration.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9659 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0033_refactor_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12036 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/models.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/serializers/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2218 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5021 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/datacite.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1965 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/dublincore.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2676 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/export.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/management.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2118 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/user.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1923 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/metadata/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      694 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/css/metadata.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1173 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1768 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2069 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc_nd.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2236 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc_sa.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1515 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nd.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1755 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_sa.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1230 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/cc0.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1331 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/nc.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1051 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/nd.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      985 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/pd.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1289 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/sa.png
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8560 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/js/metadata.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/metadata/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3508 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2916 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_display.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1484 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_columns.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1492 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_functions.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1717 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1702 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_tables.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9346 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_columns.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4872 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_functions.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8059 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1841 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3754 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_contributors.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3702 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_creators.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1866 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    10199 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1835 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3751 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_contributors.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3699 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_creators.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1860 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1020 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_options.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1514 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/schema.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2228 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/table.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      442 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/access_panel.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      501 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/doi_panel.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      523 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/license_panel.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/schemas_menu.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/templatetags/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templatetags/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1710 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/templatetags/metadata_tags.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_tags.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3579 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3975 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_column.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4329 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_function.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4355 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3922 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_table.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1150 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      727 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2271 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9261 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/oai/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/oai/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    15252 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/oai/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      142 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/apps.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/oai/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/oai/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/management/commands/rebuild_oai_schema.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/oai/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1069 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      682 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0002_resource_type.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      443 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0003_record_set_spec.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      445 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0004_alter_record_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0005_alter_record_resource_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0006_alter_record_resource_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1195 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/oai/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7874 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/renderers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1236 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/settings.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      141 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2522 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11305 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/views.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/query/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1285 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      523 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      597 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/filters.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      692 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/handlers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/query/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/query/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2482 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/archive_query_jobs.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1915 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/fix_query_jobs.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1808 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/scrub_query_jobs.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1981 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/scrub_user_tables.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      437 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/managers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1214 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      502 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0002_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1025 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0003_query_language_and_actual_query.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1149 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0004_table_name.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      702 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0005_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1155 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0006_example.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      505 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0007_queryjob_metadata.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      463 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0008_queryjob_pid.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      613 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0009_remove_choices.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0010_queue_can_be_null.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      469 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0011_queryjob_native_query.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      469 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0012_query_language_length.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2222 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0013_refactoring.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1453 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0014_downloadjob.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1611 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0015_queryarchivejob.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      447 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0016_rename_database_to_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      648 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0017_big_integer_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      485 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0018_blank_metadata.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      516 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0019_remove_sync_jobs.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      669 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0020_python3.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1014 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0021_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1277 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0022_blank_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      422 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0023_queryjob_uploads.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      728 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0024_fix_jsonfield.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      446 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0025_alter_example_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      779 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0026_use_django_jsonfield.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      525 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0027_rename_job_to_query_job.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    20749 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/query/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      265 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    13390 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/query/process.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6071 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3716 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/query/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/query/static/query/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       35 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/css/examples.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      214 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/css/jobs.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       89 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/css/plot.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3784 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/css/query.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/query/static/query/js/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      243 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/examples.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      223 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/jobs.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2010 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/query.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/downloads/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/downloads/archive.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1207 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/simbad.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1893 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/vizier.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1254 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/box.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1045 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/cone.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4545 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/sql.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      857 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/upload.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2970 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/download.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3109 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/examples.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3793 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/jobs.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    27091 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/plot.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12546 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/query.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12660 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/query/tasks.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/query/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/templates/query/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4903 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/examples.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1475 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_modal_delete.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4918 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_modal_form.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_options.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6534 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/jobs.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4036 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/jobs_modal_show_job.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5289 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      409 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_download.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      572 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_download_archive.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      806 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_download_table.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      565 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_columns.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      602 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_examples.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      591 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_functions.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      582 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_schemas.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2282 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_simbad.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2922 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_vizier.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      188 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3657 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_box.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2560 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_cone.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3128 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_sql.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1945 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_upload.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1329 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_abort_job.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1339 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_archive_job.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1138 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_logout.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1557 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_update_job.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4684 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_overview.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2241 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1478 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_histogram.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4381 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_scatter.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1836 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_scatter_cmap.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       62 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_results.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5899 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_sidebar.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_sidebar_status_extra.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2454 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1169 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1093 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_download.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1076 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_dropdown.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4394 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_example.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1083 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_form.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12329 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_job.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1122 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_status.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1216 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    10213 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/query/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3242 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/query/validators.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1127 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14163 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/query/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/registry/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/registry/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1204 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      135 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/registry/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/registry/templates/registry/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1196 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/templates/registry/root.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      551 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      956 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4143 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/serve/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      159 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/apps.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      448 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       48 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/serve/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/serve/static/serve/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/static/serve/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/static/serve/css/table.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/static/serve/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      191 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/static/serve/js/table.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      736 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/tasks.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/serve/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/templates/serve/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1441 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/templates/serve/table.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2410 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/serve/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4860 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/serve/tests/test_viewsets.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      609 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/serve/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      218 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      719 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3057 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/stats/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/stats/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      296 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      150 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/apps.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/stats/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1291 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      927 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0002_data_migration.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0003_data_migration.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      603 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0004_set_record_null.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      411 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0005_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0006_alter_record_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      380 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0007_use_django_jsonfield.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      461 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0008_alter_record_resource.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      717 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/stats/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      405 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/stats/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/stats/templates/stats/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      730 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/templates/stats/management.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      174 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      929 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/views.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      142 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11624 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/constants.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      524 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/management/commands/rebuild_tap_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3212 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/management/commands/setup_tap_metadata.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3204 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      856 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/migrations/0002_alter_ids.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1952 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      161 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/tap/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/tap/static/tap/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/static/tap/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       50 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/static/tap/css/examples.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/tap/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/templates/tap/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      928 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/templates/tap/examples.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      806 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/templates/tap/root.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    27429 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/tests/test_async.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4970 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/tests/test_sync.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1464 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      883 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5004 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1039 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3771 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/uws/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/uws/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/uws/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/uws/templates/uws/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      122 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/uws/templates/uws/root.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      861 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/uws/urls.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.426122 django-daiquiri-0.4.2/django_daiquiri.egg-info/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6177 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/PKG-INFO
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    28901 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/SOURCES.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        1 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/dependency_links.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      720 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/requires.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        9 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/top_level.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      253 2023-07-20 09:24:15.426122 django-daiquiri-0.4.2/setup.cfg
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1376 2023-07-20 09:24:11.000000 django-daiquiri-0.4.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-daiquiri-0.2/django_daiquiri.egg-info/SOURCES.txt` & `django-daiquiri-0.4.2/django_daiquiri.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,46 @@
+AUTHORS
+LICENSE
 MANIFEST.in
-README.rst
+NOTICE
+README.md
+setup.cfg
 setup.py
 daiquiri/__init__.py
-daiquiri/archive/__init__.py
-daiquiri/archive/admin.py
-daiquiri/archive/apps.py
-daiquiri/archive/models.py
-daiquiri/archive/permissions.py
-daiquiri/archive/tasks.py
-daiquiri/archive/urls.py
-daiquiri/archive/views.py
-daiquiri/archive/viewsets.py
-daiquiri/archive/migrations/0001_initial.py
-daiquiri/archive/migrations/0002_collection.py
-daiquiri/archive/migrations/0003_remove_archivejob_file_path.py
-daiquiri/archive/migrations/__init__.py
-daiquiri/archive/static/archive/css/archive.scss
-daiquiri/archive/static/archive/js/archive.js
-daiquiri/archive/templates/archive/archive.html
-daiquiri/archive/tests/__init__.py
-daiquiri/archive/tests/test_views.py
-daiquiri/archive/tests/test_viewsets.py
 daiquiri/auth/__init__.py
 daiquiri/auth/adapter.py
 daiquiri/auth/admin.py
 daiquiri/auth/apps.py
 daiquiri/auth/forms.py
 daiquiri/auth/handlers.py
 daiquiri/auth/models.py
+daiquiri/auth/permissions.py
 daiquiri/auth/serializers.py
+daiquiri/auth/settings.py
 daiquiri/auth/signals.py
 daiquiri/auth/urls_accounts.py
 daiquiri/auth/urls_auth.py
 daiquiri/auth/utils.py
+daiquiri/auth/validators.py
 daiquiri/auth/views.py
 daiquiri/auth/viewsets.py
 daiquiri/auth/migrations/0001_profile_model.py
 daiquiri/auth/migrations/0002_profile_attributes.py
 daiquiri/auth/migrations/0003_view_permission.py
 daiquiri/auth/migrations/0004_view_permission_typo.py
 daiquiri/auth/migrations/0005_view_permission_fix.py
 daiquiri/auth/migrations/0006_profile_ordering.py
 daiquiri/auth/migrations/0007_profile_is_confirmed.py
 daiquiri/auth/migrations/0008_profile_is_pending.py
 daiquiri/auth/migrations/0009_delete_detailkey.py
+daiquiri/auth/migrations/0010_profile_consent.py
+daiquiri/auth/migrations/0011_meta.py
+daiquiri/auth/migrations/0012_django2.py
+daiquiri/auth/migrations/0013_alter_profile_id.py
+daiquiri/auth/migrations/0014_use_django_jsonfield.py
 daiquiri/auth/migrations/__init__.py
 daiquiri/auth/static/auth/css/users.scss
 daiquiri/auth/static/auth/js/users.js
 daiquiri/auth/templates/account/account_inactive.html
 daiquiri/auth/templates/account/account_pending.html
 daiquiri/auth/templates/account/account_profile.html
 daiquiri/auth/templates/account/account_token.html
@@ -63,24 +56,27 @@
 daiquiri/auth/templates/account/password_reset_done.html
 daiquiri/auth/templates/account/password_reset_from_key.html
 daiquiri/auth/templates/account/password_reset_from_key_done.html
 daiquiri/auth/templates/account/password_set.html
 daiquiri/auth/templates/account/password_set_done.html
 daiquiri/auth/templates/account/signup.html
 daiquiri/auth/templates/account/signup_closed.html
+daiquiri/auth/templates/account/terms_of_use.html
 daiquiri/auth/templates/account/verification_sent.html
 daiquiri/auth/templates/account/verified_email_required.html
 daiquiri/auth/templates/account/email/activation_message.txt
 daiquiri/auth/templates/account/email/activation_subject.txt
 daiquiri/auth/templates/account/email/email_confirmation_message.txt
 daiquiri/auth/templates/account/email/email_confirmation_subject.txt
 daiquiri/auth/templates/account/email/notify_activation_message.txt
 daiquiri/auth/templates/account/email/notify_activation_subject.txt
 daiquiri/auth/templates/account/email/notify_confirmation_message.txt
 daiquiri/auth/templates/account/email/notify_confirmation_subject.txt
+daiquiri/auth/templates/account/email/notify_password_changed_message.txt
+daiquiri/auth/templates/account/email/notify_password_changed_subject.txt
 daiquiri/auth/templates/account/email/notify_rejection_message.txt
 daiquiri/auth/templates/account/email/notify_rejection_subject.txt
 daiquiri/auth/templates/account/email/password_reset_key_message.txt
 daiquiri/auth/templates/account/email/password_reset_key_subject.txt
 daiquiri/auth/templates/account/email/request_activation_message.txt
 daiquiri/auth/templates/account/email/request_activation_subject.txt
 daiquiri/auth/templates/account/email/request_confirmation_message.txt
@@ -92,28 +88,35 @@
 daiquiri/auth/templates/auth/users_modal_enable_user.html
 daiquiri/auth/templates/auth/users_modal_reject_user.html
 daiquiri/auth/templates/auth/users_modal_show_user.html
 daiquiri/auth/templates/auth/users_modal_update_user.html
 daiquiri/auth/templates/auth/users_options.html
 daiquiri/auth/templates/socialaccount/authentication_error.html
 daiquiri/auth/templates/socialaccount/connections.html
+daiquiri/auth/templates/socialaccount/login.html
 daiquiri/auth/templates/socialaccount/login_cancelled.html
 daiquiri/auth/templates/socialaccount/signup.html
 daiquiri/auth/templates/socialaccount/snippets/provider_list.html
 daiquiri/auth/tests/__init__.py
 daiquiri/auth/tests/test_accounts.py
+daiquiri/auth/tests/test_honeypot.py
 daiquiri/auth/tests/test_views.py
-daiquiri/auth/tests/test_viewsets.py
+daiquiri/auth/tests/test_viewset_group.py
+daiquiri/auth/tests/test_viewset_profile.py
 daiquiri/conesearch/__init__.py
 daiquiri/conesearch/adapter.py
 daiquiri/conesearch/apps.py
 daiquiri/conesearch/permissions.py
 daiquiri/conesearch/renderers.py
+daiquiri/conesearch/settings.py
 daiquiri/conesearch/urls.py
+daiquiri/conesearch/views.py
 daiquiri/conesearch/viewsets.py
+daiquiri/conesearch/vo.py
+daiquiri/conesearch/templates/conesearch/root.html
 daiquiri/contact/__init__.py
 daiquiri/contact/admin.py
 daiquiri/contact/apps.py
 daiquiri/contact/filters.py
 daiquiri/contact/forms.py
 daiquiri/contact/models.py
 daiquiri/contact/serializers.py
@@ -121,14 +124,16 @@
 daiquiri/contact/utils.py
 daiquiri/contact/views.py
 daiquiri/contact/viewsets.py
 daiquiri/contact/migrations/0001_initial.py
 daiquiri/contact/migrations/0002_meta.py
 daiquiri/contact/migrations/0003_add_permissions.py
 daiquiri/contact/migrations/0004_meta.py
+daiquiri/contact/migrations/0005_django2.py
+daiquiri/contact/migrations/0006_alter_contactmessage_id.py
 daiquiri/contact/migrations/__init__.py
 daiquiri/contact/static/contact/css/messages.scss
 daiquiri/contact/static/contact/js/messages.js
 daiquiri/contact/templates/contact/contact.html
 daiquiri/contact/templates/contact/messages.html
 daiquiri/contact/templates/contact/messages_mailto.html
 daiquiri/contact/templates/contact/messages_modal_show.html
@@ -137,61 +142,76 @@
 daiquiri/contact/templates/contact/email/contact_template.txt
 daiquiri/contact/templates/contact/email/new_message_admin_message.txt
 daiquiri/contact/templates/contact/email/new_message_admin_subject.txt
 daiquiri/contact/templates/contact/email/new_message_user_message.txt
 daiquiri/contact/templates/contact/email/new_message_user_subject.txt
 daiquiri/contact/tests/__init__.py
 daiquiri/contact/tests/test_views.py
-daiquiri/contact/tests/test_viewsets.py
+daiquiri/contact/tests/test_viewset_contact_messages.py
+daiquiri/contact/tests/test_viewset_status.py
 daiquiri/core/__init__.py
+daiquiri/core/celery.py
 daiquiri/core/constants.py
+daiquiri/core/encoders.py
+daiquiri/core/env.py
 daiquiri/core/exceptions.py
 daiquiri/core/generators.py
 daiquiri/core/hashers.py
 daiquiri/core/http.py
 daiquiri/core/managers.py
+daiquiri/core/middleware.py
 daiquiri/core/paginations.py
 daiquiri/core/permissions.py
-daiquiri/core/renderers.py
 daiquiri/core/responses.py
 daiquiri/core/routers.py
 daiquiri/core/serializers.py
 daiquiri/core/tasks.py
 daiquiri/core/utils.py
 daiquiri/core/views.py
 daiquiri/core/viewsets.py
+daiquiri/core/vo.py
 daiquiri/core/adapter/__init__.py
 daiquiri/core/adapter/stream.py
 daiquiri/core/adapter/database/__init__.py
 daiquiri/core/adapter/database/base.py
 daiquiri/core/adapter/database/mariadb.py
 daiquiri/core/adapter/database/mysql.py
 daiquiri/core/adapter/database/postgres.py
 daiquiri/core/adapter/download/__init__.py
 daiquiri/core/adapter/download/base.py
 daiquiri/core/adapter/download/mysqldump.py
 daiquiri/core/adapter/download/pgdump.py
 daiquiri/core/management/__init__.py
 daiquiri/core/management/commands/__init__.py
-daiquiri/core/management/commands/archive_query_jobs.py
+daiquiri/core/management/commands/activate_user.py
 daiquiri/core/management/commands/create_admin_user.py
 daiquiri/core/management/commands/daiquiri_path.py
+daiquiri/core/management/commands/delete_users.py
 daiquiri/core/management/commands/deploy.py
-daiquiri/core/management/commands/download_vendor_files.py
+daiquiri/core/management/commands/find_users.py
+daiquiri/core/management/commands/promote_user.py
 daiquiri/core/management/commands/rabbitcreate.py
 daiquiri/core/management/commands/runworker.py
+daiquiri/core/management/commands/setup_groups.py
+daiquiri/core/management/commands/show_databases.py
 daiquiri/core/management/commands/sqlcreate.py
+daiquiri/core/management/commands/workers.py
+daiquiri/core/renderers/__init__.py
+daiquiri/core/renderers/datacite.py
+daiquiri/core/renderers/dublincore.py
+daiquiri/core/renderers/voresource.py
+daiquiri/core/renderers/vosi.py
 daiquiri/core/settings/__init__.py
-daiquiri/core/settings/base.py
-daiquiri/core/settings/celery.py
 daiquiri/core/settings/daiquiri.py
+daiquiri/core/settings/django.py
 daiquiri/core/settings/logging.py
 daiquiri/core/settings/vendor.py
 daiquiri/core/static/core/css/base.scss
 daiquiri/core/static/core/css/browser.scss
+daiquiri/core/static/core/css/codehilite.scss
 daiquiri/core/static/core/css/codemirror.scss
 daiquiri/core/static/core/css/fonts.scss
 daiquiri/core/static/core/css/list.scss
 daiquiri/core/static/core/css/style.scss
 daiquiri/core/static/core/css/table.scss
 daiquiri/core/static/core/css/variables.scss
 daiquiri/core/static/core/fonts/DroidSans-Bold.ttf
@@ -200,21 +220,24 @@
 daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf
 daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf
 daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf
 daiquiri/core/static/core/fonts/DroidSerif.ttf
 daiquiri/core/static/core/html/browser.html
 daiquiri/core/static/core/html/formgroup_checkbox.html
 daiquiri/core/static/core/html/formgroup_codemirror.html
+daiquiri/core/static/core/html/formgroup_date.html
+daiquiri/core/static/core/html/formgroup_file.html
 daiquiri/core/static/core/html/formgroup_multicheckbox.html
 daiquiri/core/static/core/html/formgroup_number.html
 daiquiri/core/static/core/html/formgroup_radio.html
 daiquiri/core/static/core/html/formgroup_select.html
 daiquiri/core/static/core/html/formgroup_selectnumber.html
 daiquiri/core/static/core/html/formgroup_text.html
 daiquiri/core/static/core/html/formgroup_textarea.html
+daiquiri/core/static/core/html/formgroup_textareasplit.html
 daiquiri/core/static/core/html/order-list.html
 daiquiri/core/static/core/img/daiquiri.jpg
 daiquiri/core/static/core/img/daiquiri32.png
 daiquiri/core/static/core/img/favicon.ico
 daiquiri/core/static/core/img/favicon.png
 daiquiri/core/static/core/js/browser.js
 daiquiri/core/static/core/js/byNumber.js
@@ -231,14 +254,17 @@
 daiquiri/core/templates/core/404.html
 daiquiri/core/templates/core/500.html
 daiquiri/core/templates/core/base.html
 daiquiri/core/templates/core/base_analytics.html
 daiquiri/core/templates/core/base_footer.html
 daiquiri/core/templates/core/base_head.html
 daiquiri/core/templates/core/base_navigation.html
+daiquiri/core/templates/core/base_navigation_account.html
+daiquiri/core/templates/core/base_navigation_admin.html
+daiquiri/core/templates/core/base_navigation_management.html
 daiquiri/core/templates/core/home.html
 daiquiri/core/templates/core/page.html
 daiquiri/core/templates/core/wide.html
 daiquiri/core/templates/core/partials/form_field.html
 daiquiri/core/templates/core/partials/form_fields.html
 daiquiri/core/templates/core/partials/table.html
 daiquiri/core/templates/core/partials/table_footer.html
@@ -249,39 +275,72 @@
 daiquiri/core/templates/core/partials/table_search.html
 daiquiri/core/templates/core/partials/table_tooltip.html
 daiquiri/core/templatetags/__init__.py
 daiquiri/core/templatetags/core_tags.py
 daiquiri/core/tests/__init__.py
 daiquiri/core/tests/test_adapter.py
 daiquiri/core/tests/test_views.py
-daiquiri/core/tests/test_viewsets.py
 daiquiri/cutout/__init__.py
 daiquiri/cutout/adapter.py
 daiquiri/cutout/apps.py
 daiquiri/cutout/permissions.py
 daiquiri/cutout/renderers.py
+daiquiri/cutout/settings.py
 daiquiri/cutout/urls.py
 daiquiri/cutout/viewsets.py
+daiquiri/datalink/__init__.py
+daiquiri/datalink/adapter.py
+daiquiri/datalink/apps.py
+daiquiri/datalink/constants.py
+daiquiri/datalink/models.py
+daiquiri/datalink/serializers.py
+daiquiri/datalink/settings.py
+daiquiri/datalink/urls.py
+daiquiri/datalink/utils.py
+daiquiri/datalink/views.py
+daiquiri/datalink/viewsets.py
+daiquiri/datalink/vo.py
+daiquiri/datalink/management/__init__.py
+daiquiri/datalink/management/commands/__init__.py
+daiquiri/datalink/management/commands/rebuild_datalink_table.py
+daiquiri/datalink/migrations/0001_initial.py
+daiquiri/datalink/migrations/0002_alter_datalink_content_length.py
+daiquiri/datalink/migrations/0003_alter_datalink_content_length.py
+daiquiri/datalink/migrations/__init__.py
+daiquiri/datalink/templates/datalink/datalink.html
+daiquiri/datalink/templates/datalink/root.html
 daiquiri/files/__init__.py
 daiquiri/files/admin.py
 daiquiri/files/apps.py
 daiquiri/files/models.py
+daiquiri/files/search.py
+daiquiri/files/settings.py
 daiquiri/files/urls.py
 daiquiri/files/utils.py
 daiquiri/files/views.py
-daiquiri/files/viewsets.py
 daiquiri/files/migrations/0001_initial.py
 daiquiri/files/migrations/0002_depth.py
+daiquiri/files/migrations/0003_python3.py
+daiquiri/files/migrations/0004_django2.py
+daiquiri/files/migrations/0005_directory_layout.py
+daiquiri/files/migrations/0006_alter_directory_id.py
+daiquiri/files/migrations/0007_alter_directory_layout.py
 daiquiri/files/migrations/__init__.py
+daiquiri/files/templates/files/layout.html
+daiquiri/files/templates/files/list-results.html
+daiquiri/files/templates/files/search-input.html
+daiquiri/files/templates/files/search-results.html
+daiquiri/files/templatetags/__init__.py
+daiquiri/files/templatetags/search_highlight.py
 daiquiri/files/tests/__init__.py
 daiquiri/files/tests/test_views.py
-daiquiri/files/tests/test_viewsets.py
 daiquiri/jobs/__init__.py
 daiquiri/jobs/admin.py
 daiquiri/jobs/apps.py
+daiquiri/jobs/exceptions.py
 daiquiri/jobs/filters.py
 daiquiri/jobs/managers.py
 daiquiri/jobs/models.py
 daiquiri/jobs/renderers.py
 daiquiri/jobs/routers.py
 daiquiri/jobs/serializers.py
 daiquiri/jobs/utils.py
@@ -296,48 +355,25 @@
 daiquiri/jobs/migrations/0008_job_error_summary.py
 daiquiri/jobs/migrations/0009_meta.py
 daiquiri/jobs/migrations/0010_add_fields.py
 daiquiri/jobs/migrations/0011_job_client_ip.py
 daiquiri/jobs/migrations/0012_meta.py
 daiquiri/jobs/migrations/0013_job_error_summary.py
 daiquiri/jobs/migrations/0014_blank_run_id.py
+daiquiri/jobs/migrations/0015_job_index.py
+daiquiri/jobs/migrations/0016_django2.py
 daiquiri/jobs/migrations/__init__.py
-daiquiri/jobs/tests/__init__.py
-daiquiri/jobs/tests/mixins.py
-daiquiri/meetings/__init__.py
-daiquiri/meetings/admin.py
-daiquiri/meetings/apps.py
-daiquiri/meetings/forms.py
-daiquiri/meetings/models.py
-daiquiri/meetings/urls.py
-daiquiri/meetings/utils.py
-daiquiri/meetings/views.py
-daiquiri/meetings/migrations/0001_initial.py
-daiquiri/meetings/migrations/0002_meeting_registration_done_message.py
-daiquiri/meetings/migrations/0003_meta.py
-daiquiri/meetings/migrations/__init__.py
-daiquiri/meetings/templates/meetings/contributions.html
-daiquiri/meetings/templates/meetings/contributions_closed.html
-daiquiri/meetings/templates/meetings/participants.html
-daiquiri/meetings/templates/meetings/participants_closed.html
-daiquiri/meetings/templates/meetings/registration.html
-daiquiri/meetings/templates/meetings/registration_closed.html
-daiquiri/meetings/templates/meetings/registration_done.html
-daiquiri/meetings/templates/meetings/email/notify_registration_message.txt
-daiquiri/meetings/templates/meetings/email/notify_registration_subject.txt
-daiquiri/meetings/templates/meetings/email/registration_message.txt
-daiquiri/meetings/templates/meetings/email/registration_subject.txt
-daiquiri/meetings/tests/__init__.py
-daiquiri/meetings/tests/test_views.py
 daiquiri/metadata/__init__.py
 daiquiri/metadata/admin.py
 daiquiri/metadata/apps.py
 daiquiri/metadata/handlers.py
 daiquiri/metadata/models.py
+daiquiri/metadata/settings.py
 daiquiri/metadata/urls.py
+daiquiri/metadata/utils.py
 daiquiri/metadata/views.py
 daiquiri/metadata/viewsets.py
 daiquiri/metadata/management/__init__.py
 daiquiri/metadata/management/commands/__init__.py
 daiquiri/metadata/management/commands/dump_table.py
 daiquiri/metadata/management/commands/update_access_level.py
 daiquiri/metadata/migrations/0001_initial.py
@@ -358,16 +394,29 @@
 daiquiri/metadata/migrations/0016_rename_database_to_schema.py
 daiquiri/metadata/migrations/0017_rename_database_to_schema.py
 daiquiri/metadata/migrations/0018_meta.py
 daiquiri/metadata/migrations/0019_column_index_for.py
 daiquiri/metadata/migrations/0020_blank_index_for.py
 daiquiri/metadata/migrations/0021_table_nrows.py
 daiquiri/metadata/migrations/0022_table_size.py
+daiquiri/metadata/migrations/0023_python3.py
+daiquiri/metadata/migrations/0024_django2.py
+daiquiri/metadata/migrations/0025_add_published_updated.py
+daiquiri/metadata/migrations/0026_add_creators_and_contributors.py
+daiquiri/metadata/migrations/0027_auto_20201202_1625.py
+daiquiri/metadata/migrations/0028_add_related_identifiers.py
+daiquiri/metadata/migrations/0029_alter_ids.py
+daiquiri/metadata/migrations/0030_move_licenses_to_settings.py
+daiquiri/metadata/migrations/0031_change_order.py
+daiquiri/metadata/migrations/0032_data_migration.py
+daiquiri/metadata/migrations/0033_refactor_fields.py
 daiquiri/metadata/migrations/__init__.py
 daiquiri/metadata/serializers/__init__.py
+daiquiri/metadata/serializers/datacite.py
+daiquiri/metadata/serializers/dublincore.py
 daiquiri/metadata/serializers/export.py
 daiquiri/metadata/serializers/management.py
 daiquiri/metadata/serializers/user.py
 daiquiri/metadata/static/metadata/css/metadata.scss
 daiquiri/metadata/static/metadata/img/by.png
 daiquiri/metadata/static/metadata/img/by_nc.png
 daiquiri/metadata/static/metadata/img/by_nc_nd.png
@@ -386,50 +435,80 @@
 daiquiri/metadata/templates/metadata/management_modal_delete_functions.html
 daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html
 daiquiri/metadata/templates/metadata/management_modal_delete_tables.html
 daiquiri/metadata/templates/metadata/management_modal_form_columns.html
 daiquiri/metadata/templates/metadata/management_modal_form_functions.html
 daiquiri/metadata/templates/metadata/management_modal_form_schemas.html
 daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html
+daiquiri/metadata/templates/metadata/management_modal_form_schemas_contributors.html
+daiquiri/metadata/templates/metadata/management_modal_form_schemas_creators.html
 daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html
 daiquiri/metadata/templates/metadata/management_modal_form_tables.html
 daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html
+daiquiri/metadata/templates/metadata/management_modal_form_tables_contributors.html
+daiquiri/metadata/templates/metadata/management_modal_form_tables_creators.html
 daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html
 daiquiri/metadata/templates/metadata/management_options.html
 daiquiri/metadata/templates/metadata/schema.html
 daiquiri/metadata/templates/metadata/table.html
 daiquiri/metadata/templates/metadata/tags/access_panel.html
 daiquiri/metadata/templates/metadata/tags/doi_panel.html
 daiquiri/metadata/templates/metadata/tags/license_panel.html
 daiquiri/metadata/templates/metadata/tags/schemas_menu.html
 daiquiri/metadata/templatetags/__init__.py
 daiquiri/metadata/templatetags/metadata_tags.py
 daiquiri/metadata/tests/__init__.py
 daiquiri/metadata/tests/test_tags.py
 daiquiri/metadata/tests/test_views.py
-daiquiri/metadata/tests/test_viewsets.py
+daiquiri/metadata/tests/test_viewset_column.py
+daiquiri/metadata/tests/test_viewset_function.py
+daiquiri/metadata/tests/test_viewset_schema.py
+daiquiri/metadata/tests/test_viewset_table.py
+daiquiri/oai/__init__.py
+daiquiri/oai/adapter.py
+daiquiri/oai/apps.py
+daiquiri/oai/models.py
+daiquiri/oai/renderers.py
+daiquiri/oai/settings.py
+daiquiri/oai/urls.py
+daiquiri/oai/utils.py
+daiquiri/oai/views.py
+daiquiri/oai/management/__init__.py
+daiquiri/oai/management/commands/__init__.py
+daiquiri/oai/management/commands/rebuild_oai_schema.py
+daiquiri/oai/migrations/0001_initial.py
+daiquiri/oai/migrations/0002_resource_type.py
+daiquiri/oai/migrations/0003_record_set_spec.py
+daiquiri/oai/migrations/0004_alter_record_id.py
+daiquiri/oai/migrations/0005_alter_record_resource_id.py
+daiquiri/oai/migrations/0006_alter_record_resource_id.py
+daiquiri/oai/migrations/__init__.py
 daiquiri/query/__init__.py
 daiquiri/query/admin.py
 daiquiri/query/apps.py
 daiquiri/query/filters.py
 daiquiri/query/handlers.py
 daiquiri/query/managers.py
 daiquiri/query/models.py
 daiquiri/query/permissions.py
 daiquiri/query/process.py
 daiquiri/query/serializers.py
+daiquiri/query/settings.py
 daiquiri/query/tasks.py
 daiquiri/query/urls.py
 daiquiri/query/utils.py
 daiquiri/query/validators.py
 daiquiri/query/views.py
 daiquiri/query/viewsets.py
 daiquiri/query/management/__init__.py
 daiquiri/query/management/commands/__init__.py
-daiquiri/query/management/commands/fix_jobs.py
+daiquiri/query/management/commands/archive_query_jobs.py
+daiquiri/query/management/commands/fix_query_jobs.py
+daiquiri/query/management/commands/scrub_query_jobs.py
+daiquiri/query/management/commands/scrub_user_tables.py
 daiquiri/query/migrations/0001_initial.py
 daiquiri/query/migrations/0002_meta.py
 daiquiri/query/migrations/0003_query_language_and_actual_query.py
 daiquiri/query/migrations/0004_table_name.py
 daiquiri/query/migrations/0005_meta.py
 daiquiri/query/migrations/0006_example.py
 daiquiri/query/migrations/0007_queryjob_metadata.py
@@ -440,62 +519,97 @@
 daiquiri/query/migrations/0012_query_language_length.py
 daiquiri/query/migrations/0013_refactoring.py
 daiquiri/query/migrations/0014_downloadjob.py
 daiquiri/query/migrations/0015_queryarchivejob.py
 daiquiri/query/migrations/0016_rename_database_to_schema.py
 daiquiri/query/migrations/0017_big_integer_fields.py
 daiquiri/query/migrations/0018_blank_metadata.py
+daiquiri/query/migrations/0019_remove_sync_jobs.py
+daiquiri/query/migrations/0020_python3.py
+daiquiri/query/migrations/0021_django2.py
+daiquiri/query/migrations/0022_blank_fields.py
+daiquiri/query/migrations/0023_queryjob_uploads.py
+daiquiri/query/migrations/0024_fix_jsonfield.py
+daiquiri/query/migrations/0025_alter_example_id.py
+daiquiri/query/migrations/0026_use_django_jsonfield.py
+daiquiri/query/migrations/0027_rename_job_to_query_job.py
 daiquiri/query/migrations/__init__.py
 daiquiri/query/static/query/css/examples.scss
 daiquiri/query/static/query/css/jobs.scss
+daiquiri/query/static/query/css/plot.scss
 daiquiri/query/static/query/css/query.scss
 daiquiri/query/static/query/js/apps/examples.js
 daiquiri/query/static/query/js/apps/jobs.js
 daiquiri/query/static/query/js/apps/query.js
+daiquiri/query/static/query/js/downloads/archive.js
 daiquiri/query/static/query/js/dropdowns/simbad.js
 daiquiri/query/static/query/js/dropdowns/vizier.js
 daiquiri/query/static/query/js/forms/box.js
 daiquiri/query/static/query/js/forms/cone.js
 daiquiri/query/static/query/js/forms/sql.js
+daiquiri/query/static/query/js/forms/upload.js
 daiquiri/query/static/query/js/services/download.js
 daiquiri/query/static/query/js/services/examples.js
 daiquiri/query/static/query/js/services/jobs.js
 daiquiri/query/static/query/js/services/plot.js
 daiquiri/query/static/query/js/services/query.js
 daiquiri/query/templates/query/examples.html
 daiquiri/query/templates/query/examples_modal_delete.html
 daiquiri/query/templates/query/examples_modal_form.html
 daiquiri/query/templates/query/examples_options.html
 daiquiri/query/templates/query/jobs.html
 daiquiri/query/templates/query/jobs_modal_show_job.html
 daiquiri/query/templates/query/query.html
 daiquiri/query/templates/query/query_download.html
+daiquiri/query/templates/query/query_download_archive.html
+daiquiri/query/templates/query/query_download_table.html
 daiquiri/query/templates/query/query_dropdown_columns.html
 daiquiri/query/templates/query/query_dropdown_examples.html
+daiquiri/query/templates/query/query_dropdown_functions.html
 daiquiri/query/templates/query/query_dropdown_schemas.html
 daiquiri/query/templates/query/query_dropdown_simbad.html
 daiquiri/query/templates/query/query_dropdown_vizier.html
 daiquiri/query/templates/query/query_form.html
 daiquiri/query/templates/query/query_form_box.html
 daiquiri/query/templates/query/query_form_cone.html
 daiquiri/query/templates/query/query_form_sql.html
+daiquiri/query/templates/query/query_form_upload.html
 daiquiri/query/templates/query/query_modal_abort_job.html
 daiquiri/query/templates/query/query_modal_archive_job.html
+daiquiri/query/templates/query/query_modal_logout.html
 daiquiri/query/templates/query/query_modal_update_job.html
 daiquiri/query/templates/query/query_overview.html
 daiquiri/query/templates/query/query_plot.html
+daiquiri/query/templates/query/query_plot_histogram.html
+daiquiri/query/templates/query/query_plot_scatter.html
+daiquiri/query/templates/query/query_plot_scatter_cmap.html
 daiquiri/query/templates/query/query_results.html
 daiquiri/query/templates/query/query_sidebar.html
+daiquiri/query/templates/query/query_sidebar_status_extra.html
 daiquiri/query/tests/__init__.py
 daiquiri/query/tests/test_permissions.py
 daiquiri/query/tests/test_views.py
-daiquiri/query/tests/test_viewsets.py
+daiquiri/query/tests/test_viewset_download.py
+daiquiri/query/tests/test_viewset_dropdown.py
+daiquiri/query/tests/test_viewset_example.py
+daiquiri/query/tests/test_viewset_form.py
+daiquiri/query/tests/test_viewset_job.py
+daiquiri/query/tests/test_viewset_status.py
+daiquiri/registry/__init__.py
+daiquiri/registry/apps.py
+daiquiri/registry/serializers.py
+daiquiri/registry/settings.py
+daiquiri/registry/urls.py
+daiquiri/registry/views.py
+daiquiri/registry/vo.py
+daiquiri/registry/templates/registry/root.html
 daiquiri/serve/__init__.py
 daiquiri/serve/apps.py
 daiquiri/serve/serializers.py
+daiquiri/serve/settings.py
 daiquiri/serve/tasks.py
 daiquiri/serve/urls.py
 daiquiri/serve/utils.py
 daiquiri/serve/views.py
 daiquiri/serve/viewsets.py
 daiquiri/serve/migrations/__init__.py
 daiquiri/serve/static/serve/css/table.scss
@@ -504,53 +618,52 @@
 daiquiri/serve/tests/__init__.py
 daiquiri/serve/tests/test_views.py
 daiquiri/serve/tests/test_viewsets.py
 daiquiri/stats/__init__.py
 daiquiri/stats/admin.py
 daiquiri/stats/apps.py
 daiquiri/stats/models.py
+daiquiri/stats/settings.py
 daiquiri/stats/urls.py
 daiquiri/stats/views.py
 daiquiri/stats/migrations/0001_initial.py
 daiquiri/stats/migrations/0002_data_migration.py
+daiquiri/stats/migrations/0003_data_migration.py
+daiquiri/stats/migrations/0004_set_record_null.py
+daiquiri/stats/migrations/0005_django2.py
+daiquiri/stats/migrations/0006_alter_record_id.py
+daiquiri/stats/migrations/0007_use_django_jsonfield.py
+daiquiri/stats/migrations/0008_alter_record_resource.py
 daiquiri/stats/migrations/__init__.py
 daiquiri/stats/templates/stats/management.html
 daiquiri/tap/__init__.py
 daiquiri/tap/apps.py
-daiquiri/tap/handlers.py
+daiquiri/tap/constants.py
 daiquiri/tap/models.py
-daiquiri/tap/renderers.py
-daiquiri/tap/routers.py
 daiquiri/tap/serializers.py
+daiquiri/tap/settings.py
 daiquiri/tap/urls.py
 daiquiri/tap/utils.py
 daiquiri/tap/views.py
+daiquiri/tap/vo.py
 daiquiri/tap/management/__init__.py
 daiquiri/tap/management/commands/__init__.py
 daiquiri/tap/management/commands/rebuild_tap_schema.py
+daiquiri/tap/management/commands/setup_tap_metadata.py
 daiquiri/tap/migrations/0001_initial.py
+daiquiri/tap/migrations/0002_alter_ids.py
 daiquiri/tap/migrations/__init__.py
 daiquiri/tap/static/tap/css/examples.scss
 daiquiri/tap/templates/tap/examples.html
 daiquiri/tap/templates/tap/root.html
 daiquiri/tap/tests/__init__.py
 daiquiri/tap/tests/test_async.py
 daiquiri/tap/tests/test_sync.py
 daiquiri/tap/tests/test_views.py
 daiquiri/uws/__init__.py
 daiquiri/uws/urls.py
 daiquiri/uws/templates/uws/root.html
-daiquiri/wordpress/__init__.py
-daiquiri/wordpress/apps.py
-daiquiri/wordpress/handlers.py
-daiquiri/wordpress/rules.py
-daiquiri/wordpress/tasks.py
-daiquiri/wordpress/utils.py
-daiquiri/wordpress/static/wordpress/css/wordpress.scss
-daiquiri/wordpress/templates/wordpress/layout.html
-daiquiri/wordpress/templatetags/__init__.py
-daiquiri/wordpress/templatetags/wordpress_tags.py
 django_daiquiri.egg-info/PKG-INFO
 django_daiquiri.egg-info/SOURCES.txt
 django_daiquiri.egg-info/dependency_links.txt
 django_daiquiri.egg-info/requires.txt
 django_daiquiri.egg-info/top_level.txt
```

### Comparing `django-daiquiri-0.2/daiquiri/serve/urls.py` & `django-daiquiri-0.4.2/daiquiri/serve/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from django.conf.urls import url, include
-
+from django.urls import include, path, re_path
 from rest_framework import routers
 
-from .views import table
-from .viewsets import RowViewSet, ColumnViewSet, ReferenceViewSet
+from .views import reference, table
+from .viewsets import ColumnViewSet, RowViewSet
 
-router = routers.DefaultRouter()
-router.register(r'rows', RowViewSet, base_name='row')
-router.register(r'columns', ColumnViewSet, base_name='column')
-router.register(r'references', ReferenceViewSet, base_name='reference')
+app_name = 'serve'
 
+router = routers.DefaultRouter()
+router.register(r'rows', RowViewSet, basename='row')
+router.register(r'columns', ColumnViewSet, basename='column')
 
 urlpatterns = [
-    url(r'^table/(?P<schema_name>[A-Za-z0-9_]+)/(?P<table_name>[A-Za-z0-9_]+)/$', table, name='table'),
+    re_path(r'^table/(?P<schema_name>[A-Za-z0-9_]+)/(?P<table_name>[A-Za-z0-9_]+)/$', table, name='table'),
+    re_path(r'^references/(?P<key>[-\w]+)/(?P<value>.+)/$', reference, name='reference'),
 
     # rest api
-    url(r'^api/', include(router.urls)),
+    path('api/', include(router.urls)),
 ]
```

### Comparing `django-daiquiri-0.2/daiquiri/serve/tasks.py` & `django-daiquiri-0.4.2/daiquiri/serve/tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, unicode_literals
-
 import logging
 import os
 import zipfile
 
 from celery import shared_task
 
 from daiquiri.core.tasks import Task
```

### Comparing `django-daiquiri-0.2/daiquiri/serve/templates/serve/table.html` & `django-daiquiri-0.4.2/daiquiri/serve/templates/serve/table.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core/wide.html' %}
-{% load staticfiles %}
+{% load static %}
 {% load compress %}
 {% load i18n %}
-{% load core_tags %}
+{% load vendor_tags %}
 
 {% block bodyargs %}
     ng-app="table"
     ng-controller="TableController"
     ng-init="service.table.init({
         rows_url: 'serve/api/rows/',
         columns_url: 'serve/api/columns/',
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends 'core/wide.html' %} {% load staticfiles %} {% load compress %} {%
-load i18n %} {% load core_tags %} {% block bodyargs %} ng-app="table" ng-
+{% extends 'core/wide.html' %} {% load static %} {% load compress %} {% load
+i18n %} {% load vendor_tags %} {% block bodyargs %} ng-app="table" ng-
 controller="TableController" ng-init="service.table.init({ rows_url: 'serve/
 api/rows/', columns_url: 'serve/api/columns/', files_url: 'files/api/files/',
 params: { schema: '{{ schema }}', table: '{{ table }}' } })" {% endblock %} {%
 block headextra %} {% vendor 'angular' %} {% compress css %}
 
 
  {% endcompress css %} {% compress js %}
```

### Comparing `django-daiquiri-0.2/daiquiri/serve/viewsets.py` & `django-daiquiri-0.4.2/daiquiri/serve/viewsets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 from collections import OrderedDict
 
-from django.shortcuts import redirect
-
 from rest_framework import viewsets
 from rest_framework.response import Response
 from rest_framework.exceptions import NotFound
 
 from daiquiri.core.viewsets import RowViewSetMixin
 from daiquiri.core.adapter import DatabaseAdapter
+from daiquiri.core.utils import fix_for_json
+from daiquiri.metadata.utils import get_user_columns
 
 from .serializers import ColumnSerializer
-from .utils import get_columns, get_resolver
 
 
 class RowViewSet(RowViewSetMixin, viewsets.GenericViewSet):
 
     def list(self, request, *args, **kwargs):
 
         # get schema, table and column_names from the querystring
         schema_name = self.request.GET.get('schema')
         table_name = self.request.GET.get('table')
         column_names = self.request.GET.getlist('column')
 
-        # get the columns using the utils function
-        columns = get_columns(self.request.user, schema_name, table_name, column_names)
-
-        if columns:
-            # get column names from the checked columns (again)
-            column_names = [column.name for column in columns]
+        # get the columns which the user is allowed to access
+        user_columns = get_user_columns(self.request.user, schema_name, table_name)
 
+        if user_columns:
             # get the row query params from the request
-            ordering, page, page_size, search, filters = self._get_query_params(column_names)
+            ordering, page, page_size, search, filters = self._get_query_params(user_columns)
+
+            # filter by input column names by the the allowed columns
+            if column_names:
+                column_names = [column.name for column in user_columns if column.name in column_names]
+            else:
+                column_names = [column.name for column in user_columns]
 
             # get database adapter
             adapter = DatabaseAdapter()
 
             # query the database for the total number of rows
             count = adapter.count_rows(schema_name, table_name, column_names, search, filters)
 
             # query the paginated rowset
             results = adapter.fetch_rows(schema_name, table_name, column_names, ordering, page, page_size, search, filters)
 
             # return ordered dict to be send as json
             return Response(OrderedDict((
                 ('count', count),
-                ('results', results),
+                ('results', fix_for_json(results)),
                 ('next', self._get_next_url(page, page_size, count)),
                 ('previous', self._get_previous_url(page))
             )))
 
         # if nothing worked, return 404
         raise NotFound()
 
@@ -58,36 +60,21 @@
     def list(self, request, *args, **kwargs):
 
         # get database, table and column_names from the querystring
         schema_name = self.request.GET.get('schema')
         table_name = self.request.GET.get('table')
         column_names = self.request.GET.getlist('column')
 
-        # get the columns using the utils function
-        columns = get_columns(self.request.user, schema_name, table_name, column_names)
+        # get the columns which the user is allowed to access
+        user_columns = get_user_columns(self.request.user, schema_name, table_name)
 
-        if columns:
-            # get column names from the checked columns (again)
-            columns = [column for column in columns if column.name in column_names]
+        if user_columns:
+            # filter by input column names by the the allowed columns
+            if column_names:
+                columns = [column for column in user_columns if column.name in column_names]
+            else:
+                columns = [column for column in user_columns]
 
             return Response(ColumnSerializer(columns, many=True).data)
 
         # if nothing worked, return 404
         raise NotFound()
-
-
-class ReferenceViewSet(viewsets.ViewSet):
-
-    def list(self, request):
-
-        key = request.GET.get('key', None)
-        value = request.GET.get('value', None)
-
-        resolver = get_resolver()
-        if resolver is None:
-            raise NotFound()
-
-        url = resolver.resolve(key, value)
-        if url is None:
-            raise NotFound()
-
-        return redirect(url)
```

### Comparing `django-daiquiri-0.2/daiquiri/core/permissions.py` & `django-daiquiri-0.4.2/daiquiri/core/permissions.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/renderers.py` & `django-daiquiri-0.4.2/daiquiri/core/renderers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,49 @@
+import io
+
 from django.utils.xmlutils import SimplerXMLGenerator
-from django.utils.six.moves import StringIO
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 
 from rest_framework.renderers import BaseRenderer
 
 
 class XMLRenderer(BaseRenderer):
 
     media_type = 'application/xml'
     charset = 'utf-8'
     format = 'xml'
 
     def render(self, data, accepted_media_type=None, renderer_context=None):
         if data is None:
             return ''
 
-        stream = StringIO()
+        stream = io.StringIO()
 
         self.xml = SimplerXMLGenerator(stream, self.charset)
         self.xml.startDocument()
         self.render_document(data, accepted_media_type, renderer_context)
         self.xml.endDocument()
         return stream.getvalue()
 
     def render_document(self, data, accepted_media_type=None, renderer_context=None):
         raise NotImplementedError()
 
-    def start(self, tag, attr={}):
-        self.xml.startElement(tag, attr)
+    def start(self, tag, attrs={}):
+        self.xml.startElement(tag, {k: v for k, v in attrs.items() if v is not None})
 
     def end(self, tag):
         self.xml.endElement(tag)
 
-    def node(self, tag, attr, text):
-        if not text:
-            attr.update({'xsi:nil': 'true'})
-        self.xml.startElement(tag, attr)
+    def node(self, tag, attrs, text=''):
+        if text is None:
+            attrs.update({'xsi:nil': 'true'})
+
+        self.xml.startElement(tag, {k: str(v) for k, v in attrs.items() if v is not None})
         if text:
-            self.xml.characters(smart_text(text))
+            self.xml.characters(smart_str(text))
         self.xml.endElement(tag)
 
     def _to_camel_case(self, snake_str):
         components = snake_str.split('_')
         return components[0] + "".join(x.title() for x in components[1:])
```

### Comparing `django-daiquiri-0.2/daiquiri/core/settings/daiquiri.py` & `django-daiquiri-0.4.2/daiquiri/query/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,38 @@
-import os
+import daiquiri.core.env as env
 
-from .base import BASE_DIR
-
-ASYNC = False
-
-IPV4_PRIVACY_MASK = 16
-IPV6_PRIVACY_MASK = 32
-
-DOWNLOAD_PREPEND = {}
-
-ARCHIVE_ANONYMOUS = False
-ARCHIVE_SCHEMA = 'daiquiri_archive'
-ARCHIVE_TABLE = 'files'
-ARCHIVE_COLUMNS = [
-    {
-        'name': 'id',
-        'hidden': True
-    },
-    {
-        'name': 'timestamp',
-        'label': 'Timestamp'
-    },
-    {
-        'name': 'file',
-        'label': 'Filename',
-        'ucd': 'meta.file'
-    },
-    {
-        'name': 'collection',
-        'hidden': True
-    },
-    {
-        'name': 'path',
-        'hidden': True
-    }
-]
-ARCHIVE_BASE_PATH = os.path.join(BASE_DIR, 'files')
-ARCHIVE_DOWNLOAD_DIR = os.path.join(BASE_DIR, 'download')
-
-AUTH_SIGNUP = False
-AUTH_WORKFLOW = None
-AUTH_DETAIL_KEYS = []
-
-CONESEARCH_ADAPTER = 'daiquiri.conesearch.adapter.SimpleConeSearchAdapter'
-CONESEARCH_ANONYMOUS = False
-
-CUTOUT_ADAPTER = 'daiquiri.cutout.adapter.SimpleCutOutAdapter'
-CUTOUT_ANONYMOUS = False
-
-FILES_BASE_PATH = os.path.join(BASE_DIR, 'files')
-FILES_SEARCH_URL = None
-
-MEETINGS_CONTRIBUTION_TYPES = [
-    (None, 'no contribution'),
-    ('talk', 'Talk'),
-    ('poster', 'Poster')
-]
-MEETINGS_PARTICIPANT_DETAIL_KEYS = []
-MEETINGS_ABSTRACT_MAX_LENGTH = 2000
-
-METADATA_COLUMN_PERMISSIONS = False
+QUERY_DOWNLOAD_DIR = env.get_abspath('QUERY_DOWNLOAD_DIR')
+QUERY_UPLOAD_DIR = env.get_abspath('QUERY_UPLOAD_DIR')
 
 QUERY_ANONYMOUS = False
 QUERY_USER_SCHEMA_PREFIX = 'daiquiri_user_'
 QUERY_QUOTA = {
     'anonymous': '100Mb',
-    'user': '100Mb',
+    'user': '10000Mb',
     'users': {},
     'groups': {}
 }
+QUERY_SYNC_TIMEOUT = 5
 QUERY_MAX_ACTIVE_JOBS = {
     'anonymous': '1'
 }
 QUERY_QUEUES = [
     {
-        'key': 'default',
-        'label': 'Default',
-        'timeout': 10,
-        'priority': 1
+        'key': 'short',
+        'label': '30 seconds',
+        'timeout': 30,
+        'access_level': 'PUBLIC',
+        'groups': []
+    },
+    {
+        'key': 'long',
+        'label': '1 Hour',
+        'timeout': 3600,
+        'access_level': 'PUBLIC',
+        'groups': []
     }
 ]
 QUERY_LANGUAGES = [
     {
         'key': 'adql',
         'version': 2.0,
         'label': 'ADQL',
@@ -91,16 +42,42 @@
 ]
 QUERY_FORMS = [
     {
         'key': 'sql',
         'label': 'SQL query',
         'service': 'query/js/forms/sql.js',
         'template': 'query/query_form_sql.html'
+    },
+    {
+        'key': 'upload',
+        'label': 'Upload VOTable',
+        'service': 'query/js/forms/upload.js',
+        'template': 'query/query_form_upload.html'
+    }
+]
+
+QUERY_PLOTS = [
+    {
+        'key': 'scatter_plot',
+        'label': 'Scatter',
+        'is_active': True,
+    },
+    {
+        'key': 'scatter_cmap_plot',
+        'label': 'Scatter (color coded)',
+        'is_active': True,
+    },
+    {
+        'key': 'histogram',
+        'label': 'Histogram',
+        'is_active': True,
     }
 ]
+
+QUERY_DROPDOWN_FUNCTIONS = False;
 QUERY_DROPDOWNS = [
     {
         'key': 'simbad',
         'service': 'query/js/dropdowns/simbad.js',
         'template': 'query/query_dropdown_simbad.html',
         'options': {
             'url': 'http://simbad.u-strasbg.fr/simbad/sim-id'
@@ -112,59 +89,54 @@
         'template': 'query/query_dropdown_vizier.html',
         'options': {
             'url': 'http://vizier.u-strasbg.fr/viz-bin/votable',
             'catalogs': ['I/322A', 'I/259']
         }
     }
 ]
-QUERY_DOWNLOAD_DIR = os.path.join(BASE_DIR, 'download')
-QUERY_DEFAULT_DOWNLOAD_FORMAT = 'votable'
-QUERY_DOWNLOAD_FORMATS = [
+QUERY_DOWNLOADS = [
     {
-        'key': 'csv',
-        'extension': 'csv',
-        'content_type': 'text/csv',
-        'label': 'Comma separated Values',
-        'help': 'A text file with a line for each row of the table. The fields are delimited by a comma and quoted by double quotes. Use this option for a later import into a spreadsheed application or a custom script. Use this option if you are unsure what to use.'
+        'key': 'table',
+        'model': 'daiquiri.query.models.DownloadJob',
+        'template': 'query/query_download_table.html',
+        'params': ['format_key']
     },
     {
+        'key': 'archive',
+        'model': 'daiquiri.query.models.QueryArchiveJob',
+        'template': 'query/query_download_archive.html',
+        'service': 'query/js/downloads/archive.js',
+        'params': ['column_name']
+    }
+]
+QUERY_DEFAULT_DOWNLOAD_FORMAT = 'votable'
+QUERY_DOWNLOAD_FORMATS = [
+    {
         'key': 'votable',
         'extension': 'xml',
         'content_type': 'application/xml',
         'label': 'IVOA VOTable XML file - TABLEDATA serialization',
         'help': 'A XML file using the IVOA VOTable format. Use this option if you intend to use VO compatible software to further process the data.'
-    }
-]
-
-SERVE_DOWNLOAD_DIR = os.path.join(BASE_DIR, 'download')
-SERVE_RESOLVER = None
-
-STATS_RESOURCE_TYPES = [
-    {
-        'key': 'ARCHIVE_DOWNLOAD',
-        'label': 'Archive downloads'
-    },
-    {
-        'key': 'CONESEARCH',
-        'label': 'Performed cone searches'
-    },
-    {
-        'key': 'CUTOUT',
-        'label': 'Performed cutouts'
     },
     {
-        'key': 'FILE',
-        'label': 'File downloads'
+        'key': 'csv',
+        'extension': 'csv',
+        'content_type': 'text/csv',
+        'label': 'Comma separated Values',
+        'help': 'A text file with a line for each row of the table. The fields are delimited by a comma and quoted by double quotes. Use this option for a later import into a spreadsheed application or a custom script. Use this option if you are unsure what to use.'
     },
     {
-        'key': 'QUERY_JOB',
-        'label': 'Query jobs'
+        'key': 'fits',
+        'extension': 'fits',
+        'content_type': 'application/fits',
+        'label': 'FITS',
+        'help': 'Flexible Image Transport System (FITS) file format.'
     }
 ]
-
-UWS_RESOURCES = []
-
-TAP_SCHEMA = 'TAP_SCHEMA'
-
-WORDPRESS_URL = '/cms/'
-WORDPRESS_CLI = '/opt/wp-cli/wp'
-WORDPRESS_PATH = '/opt/wordpress'
+QUERY_UPLOAD = True
+QUERY_UPLOAD_LIMIT = {
+    'anonymous': '10Mb',
+    'user': '100Mb',
+    'users': {},
+    'groups': {}
+}
+QUERY_PROCESSOR_CACHE = True
```

### Comparing `django-daiquiri-0.2/daiquiri/core/settings/vendor.py` & `django-daiquiri-0.4.2/daiquiri/core/settings/vendor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-VENDOR_CDN = True
+import daiquiri.core.env as env
 
+VENDOR_CDN = env.get_bool('VENDOR_CDN')
 VENDOR = {
     'jquery': {
         'url': 'https://code.jquery.com/',
         'js': [
             {
                 'path': 'jquery-3.2.1.min.js',
                 'sri': 'sha256-hwg4gsxgFZhOsEEamdOYGBf13FyQuiTwlAQgxVSNgt4=',
@@ -100,15 +101,15 @@
                 'path': 'codemirror.min.js',
                 'sri': 'sha256-0LRLvWWVXwt0eH0/Bzd0PHICg/bSMDIe5sXgaDSpZaA='
             },
             {
                 'path': 'addon/mode/overlay.min.js',
                 'sri': 'sha256-ffWkw3Pn4ieMygm1vwdRKcMtBJ6E6kuBi8GlVVPXWEs='
             },
-                        {
+            {
                 'path': 'mode/sql/sql.min.js',
                 'sri': 'sha256-AYn1SMwJJCzQwlDkZLt7gAA3v8M14QZ7X5fGnJ2juYU='
             },
             {
                 'path': 'mode/markdown/markdown.min.js',
                 'sri': 'sha256-NzPBTZOCkVLaG/iTZe2XXF4cIyer9J0C0Z1FRN3WqNc='
             },
@@ -121,30 +122,24 @@
             {
                 'path': 'codemirror.min.css',
                 'sri': 'sha256-wluO/w4cnorJpS0JmcdTSYzwdb5E6u045qa4Ervfb1k='
             }
         ]
     },
     'Bokeh': {
-        'url': 'https://cdnjs.cloudflare.com/ajax/libs/bokeh/0.12.9/',
+        'url': 'https://cdnjs.cloudflare.com/ajax/libs/bokeh/2.4.3/',
         'js': [
             {
                 'path': 'bokeh.min.js',
-                'sri': 'sha256-gm+i+GziZJeKlRYH8akT+7hC0yT0tK+VCoxApQ/uU1A='
+                'sri': 'sha512-PGHpUrgIu340bOgopWWl8jqvdwjQNPqdCQZAOBM1XUW7To2LCyOpPwMsdoMdTwIhhG8oaZx/UUfKpi4NMWaDFA=='
             },
-                        {
+            {
                 'path': 'bokeh-gl.min.js',
-                'sri': 'sha256-lle0sk6DP7Leca/0dBodUdbkGTqtqNUTLkbVZa1PceE='
+                'sri': 'sha512-5d8x/ZAQ6s/wqnLTFSZGBLXjSXK6RFrOpvzpgIDuzzOs8tKYYSY2D6qlhSgTz/oW9vb0iJkjMYMA8GJJfALaTg=='
             },
             {
                 'path': 'bokeh-api.min.js',
-                'sri': 'sha256-v22ko+YNfTgeB3sa9OjSWmHds7uwi3KjjVBFLhhGdy0='
-            }
-        ],
-        'css': [
-            {
-                'path': 'bokeh.min.css',
-                'sri': 'sha256-Gke8Knvnof6hLUSaaUp++1Chsbh5yxwdjslBLRO5iK4='
+                'sri': 'sha512-M4sK7tJZoaDdYHfN4iRKfbD3W4P3hB9GGj3HnisgfQJCmrZUy4ajqjdxsMZjH+R7+tsN7+PsR4ouMiXYT2mJlA=='
             }
         ]
     }
 }
```

### Comparing `django-daiquiri-0.2/daiquiri/core/settings/logging.py` & `django-daiquiri-0.4.2/daiquiri/core/settings/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,108 @@
 import os
 
-LOGGING = {
-    'version': 1,
-    'disable_existing_loggers': True,
-    'filters': {
-        'require_debug_false': {
-            '()': 'django.utils.log.RequireDebugFalse'
-        },
-        'require_debug_true': {
-            '()': 'django.utils.log.RequireDebugTrue'
-        }
-    },
-    'formatters': {
-        'default': {
-            'format': '[%(asctime)s] %(levelname)s: %(message)s'
-        },
-        'name': {
-            'format': '[%(asctime)s] %(levelname)s %(name)s %(funcName)s: %(message)s'
-        },
-        'console': {
-            'format': '[%(asctime)s] %(message)s'
-        }
-    },
-    'handlers': {
-        'mail_admins': {
-            'level': 'ERROR',
-            'filters': ['require_debug_false'],
-            'class': 'django.utils.log.AdminEmailHandler'
-        },
-        'error_log': {
-            'level': 'ERROR',
-            'class': 'logging.FileHandler',
-            'filename': 'error.log',
-            'formatter': 'default'
-        },
-        'daiquiri_log': {
-            'level': 'DEBUG',
-            'class': 'logging.FileHandler',
-            'filename': 'daiquiri.log',
-            'formatter': 'name'
-        },
-        'sql_log': {
-            'level': 'DEBUG',
-            'filters': ['require_debug_true'],
-            'class': 'logging.FileHandler',
-            'filename': 'sql.log',
-            'formatter': 'default'
-        },
-        'rules_log': {
-            'level': 'DEBUG',
-            'filters': ['require_debug_true'],
-            'class': 'logging.FileHandler',
-            'filename': 'rules.log',
-            'formatter': 'default'
-        },
-        'console': {
-            'level': 'DEBUG',
-            'filters': ['require_debug_true'],
-            'class': 'logging.StreamHandler',
-            'formatter': 'console'
-        }
-    },
-    'loggers': {
-        'django': {
-            'handlers': ['console'],
-            'level': 'INFO',
-            'propagate': False
-        },
-        'django.request': {
-            'handlers': ['mail_admins', 'error_log'],
-            'level': 'ERROR',
-            'propagate': True
-        },
-        'django.db.backends': {
-            'handlers': ['sql_log'],
-            'level': os.getenv('DJANGO_LOG_LEVEL', 'INFO'),
-            'propagate': False
-        },
-        'daiquiri': {
-            'handlers': ['daiquiri_log'],
-            'level': os.getenv('DJANGO_LOG_LEVEL', 'INFO'),
-            'propagate': False
-        },
-        'rules': {
-            'handlers': ['rules_log'],
-            'level': os.getenv('DJANGO_LOG_LEVEL', 'INFO'),
-            'propagate': False
+import daiquiri.core.env as env
+
+LOG_LEVEL = env.get('LOG_LEVEL')
+LOG_DIR = env.get('LOG_DIR')
+
+if LOG_DIR:
+    LOGGING = {
+        'version': 1,
+        'disable_existing_loggers': True,
+        'filters': {
+            'require_debug_false': {
+                '()': 'django.utils.log.RequireDebugFalse'
+            },
+            'require_debug_true': {
+                '()': 'django.utils.log.RequireDebugTrue'
+            }
+        },
+        'formatters': {
+            'default': {
+                'format': '[%(asctime)s] %(levelname)s: %(message)s'
+            },
+            'name': {
+                'format': '[%(asctime)s] %(levelname)s %(name)s %(funcName)s: %(message)s'
+            },
+            'console': {
+                'format': '[%(asctime)s] %(message)s'
+            }
+        },
+        'handlers': {
+            'mail_admins': {
+                'level': 'ERROR',
+                'filters': ['require_debug_false'],
+                'class': 'django.utils.log.AdminEmailHandler'
+            },
+            'error_log': {
+                'level': 'ERROR',
+                'class': 'logging.FileHandler',
+                'filename': os.path.join(LOG_DIR, 'error.log'),
+                'formatter': 'default'
+            },
+            'daiquiri_log': {
+                'level': 'DEBUG',
+                'class': 'logging.FileHandler',
+                'filename': os.path.join(LOG_DIR, 'daiquiri.log'),
+                'formatter': 'name'
+            },
+            'query_log': {
+                'level': 'DEBUG',
+                'class': 'logging.FileHandler',
+                'filename': os.path.join(LOG_DIR, 'query.log'),
+                'formatter': 'default'
+            },
+            'sql_log': {
+                'level': 'DEBUG',
+                'filters': ['require_debug_true'],
+                'class': 'logging.FileHandler',
+                'filename': os.path.join(LOG_DIR, 'sql.log'),
+                'formatter': 'default'
+            },
+            'rules_log': {
+                'level': 'DEBUG',
+                'filters': ['require_debug_true'],
+                'class': 'logging.FileHandler',
+                'filename': os.path.join(LOG_DIR, 'rules.log'),
+                'formatter': 'default'
+            },
+            'console': {
+                'level': 'DEBUG',
+                'filters': ['require_debug_true'],
+                'class': 'logging.StreamHandler',
+                'formatter': 'console'
+            }
+        },
+        'loggers': {
+            'django': {
+                'handlers': ['console'],
+                'level': 'INFO',
+                'propagate': False
+            },
+            'django.request': {
+                'handlers': ['mail_admins', 'error_log'],
+                'level': 'ERROR',
+                'propagate': True
+            },
+            'django.db.backends': {
+                'handlers': ['sql_log'],
+                'level': LOG_LEVEL,
+                'propagate': False
+            },
+            'daiquiri': {
+                'handlers': ['daiquiri_log'],
+                'level': LOG_LEVEL,
+                'propagate': False
+            },
+            'query': {
+                'handlers': ['query_log'],
+                'level': LOG_LEVEL,
+                'propagate': False
+            },
+            'rules': {
+                'handlers': ['rules_log'],
+                'level': LOG_LEVEL,
+                'propagate': False
+            }
         }
     }
-}
```

### Comparing `django-daiquiri-0.2/daiquiri/core/managers.py` & `django-daiquiri-0.4.2/daiquiri/core/managers.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from .constants import ACCESS_LEVEL_PUBLIC, ACCESS_LEVEL_INTERNAL
 
 
 class AccessLevelQuerySet(models.QuerySet):
 
     def filter_by_access_level(self, user):
-        if not user or user.is_anonymous():
+        if not user or user.is_anonymous:
             return self.filter(access_level=ACCESS_LEVEL_PUBLIC)
         else:
             q = models.Q(access_level=ACCESS_LEVEL_PUBLIC) | \
                 models.Q(access_level=ACCESS_LEVEL_INTERNAL) | \
                 models.Q(groups__in=user.groups.all())
-            return self.filter(q)
+            return self.filter(q).distinct()
 
     def filter_by_metadata_access_level(self, user):
-        if not user or user.is_anonymous():
+        if not user or user.is_anonymous:
             return self.filter(metadata_access_level=ACCESS_LEVEL_PUBLIC)
         else:
             q = models.Q(metadata_access_level=ACCESS_LEVEL_PUBLIC) | \
                 models.Q(metadata_access_level=ACCESS_LEVEL_INTERNAL) | \
                 models.Q(groups__in=user.groups.all())
-            return self.filter(q)
+            return self.filter(q).distinct()
 
 
 class AccessLevelManager(models.Manager):
 
     def get_queryset(self):
         return AccessLevelQuerySet(self.model, using=self._db)
```

### Comparing `django-daiquiri-0.2/daiquiri/core/serializers.py` & `django-daiquiri-0.4.2/daiquiri/core/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,36 @@
 from rest_framework import serializers
 
 from .utils import make_query_dict_upper_case
 
 
-class JSONField(serializers.JSONField):
+class JSONDictField(serializers.JSONField):
+
+    initial = dict
 
     def to_internal_value(self, data):
+        data = super().to_internal_value(data)
+
         if not isinstance(data, dict):
             self.fail('invalid')
 
-        return super(JSONField, self).to_internal_value(data)
+        return data
+
+
+class JSONListField(serializers.JSONField):
+
+    initial = list
+
+    def to_internal_value(self, data):
+        data = super().to_internal_value(data)
+
+        if not isinstance(data, list):
+            self.fail('invalid')
+
+        return data
 
 
 class ChoicesSerializer(serializers.Serializer):
     id = serializers.SerializerMethodField()
     text = serializers.SerializerMethodField()
 
     def get_id(self, obj):
```

### Comparing `django-daiquiri-0.2/daiquiri/core/hashers.py` & `django-daiquiri-0.4.2/daiquiri/core/hashers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # inspired by https://djangosnippets.org/snippets/10572/
 
 from collections import OrderedDict
+
 from django.contrib.auth.hashers import CryptPasswordHasher, mask_hash
+from django.utils.crypto import constant_time_compare, get_random_string
 from django.utils.encoding import force_str
-from django.utils.crypto import get_random_string, constant_time_compare
-from django.utils.translation import ugettext_noop as _
+from django.utils.translation import gettext_noop as _
 
 
 class CrypdSHA512PasswordHasher(CryptPasswordHasher):
 
     algorithm = 'crypt_sha512'
 
     def salt(self):
-        return '$6$' + get_random_string(16)
+        return '$6$' + get_random_string(8)
 
     def encode(self, password, salt):
         crypt = self._load_library()
         data = crypt.crypt(force_str(password), salt)
         return "%s%s" % (self.algorithm, data)
 
     def verify(self, password, encoded):
```

### Comparing `django-daiquiri-0.2/daiquiri/core/views.py` & `django-daiquiri-0.4.2/daiquiri/core/views.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,50 +2,55 @@
 from django.contrib.auth.mixins import (
     AccessMixin,
     PermissionRequiredMixin as DjangoPermissionRequiredMixin
 )
 from django.contrib.auth.views import redirect_to_login
 from django.core.exceptions import PermissionDenied
 from django.shortcuts import render
+from django.views.generic import View
+from django.views.decorators.csrf import ensure_csrf_cookie
+from django.utils.decorators import method_decorator
+
+from daiquiri.core.utils import render_to_xml
 
 from allauth.account.forms import LoginForm
 
 from rules.contrib.views import PermissionRequiredMixin as RulesPermissionRequiredMixin
 
 
 def home(request):
-    if not request.user.is_authenticated():
+    if not request.user.is_authenticated:
         login_form = LoginForm()
         login_form.fields['login'].widget.attrs.pop("autofocus", None)
     else:
         login_form = None
 
     return render(request, 'core/home.html', {'form': login_form})
 
 
-def bad_request(request):
+def bad_request(request, exception):
     return render(request, 'core/400.html', status=400)
 
 
-def forbidden(request):
+def forbidden(request, exception):
     return render(request, 'core/403.html', status=403)
 
 
-def not_found(request):
+def not_found(request, exception):
     return render(request, 'core/404.html', status=404)
 
 
 def internal_server_error(request):
     return render(request, 'core/500.html', status=500)
 
 
 class PermissionRedirectMixin(object):
 
     def handle_no_permission(self):
-        if self.request.user.is_authenticated():
+        if self.request.user.is_authenticated:
             raise PermissionDenied(self.get_permission_denied_message())
 
         return redirect_to_login(self.request.get_full_path(), self.get_login_url(), self.get_redirect_field_name())
 
 
 class ModelPermissionMixin(PermissionRedirectMixin, DjangoPermissionRequiredMixin, object):
     pass
@@ -58,7 +63,31 @@
 class AnonymousAccessMixin(AccessMixin):
     anonymous_setting = None
 
     def dispatch(self, request, *args, **kwargs):
         if not getattr(settings, self.anonymous_setting) and not request.user.is_authenticated:
             return self.handle_no_permission()
         return super(AnonymousAccessMixin, self).dispatch(request, *args, **kwargs)
+
+
+class SingleObjectXMLMixin(View):
+
+    def get(self, request, *args, **kwargs):
+        self.object = self.get_object()
+
+        context = self.get_context_data()
+        renderer = self.renderer_class()
+
+        return render_to_xml(request, renderer, context)
+
+    def get_object(self):
+        raise NotImplementedError()
+
+    def get_context_data(self):
+        raise NotImplementedError()
+
+
+class CSRFViewMixin(View):
+
+    @method_decorator(ensure_csrf_cookie)
+    def get(self, request, *args, **kwargs):
+        return super().get(self, request, *args, **kwargs)
```

### Comparing `django-daiquiri-0.2/daiquiri/core/adapter/download/pgdump.py` & `django-daiquiri-0.4.2/daiquiri/core/adapter/download/pgdump.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from .base import BaseDownloadAdapter
 
 logger = logging.getLogger(__name__)
 
 
 class PgDumpAdapter(BaseDownloadAdapter):
 
-    def set_args(self, schema_name, table_name):
+    def set_args(self, schema_name, table_name, data_only=False):
         # command line for pg_dump:
-        # pg_dump -a --inserts --dbname=postgresql://user:password@host:port/database --table=schema.table
-        # pg_dump -a --inserts --user=user --host=host --port=port --dbname=database --table=schema.table
+        # pg_dump ... --dbname=postgresql://user:password@host:port/database --table=schema.table
+        # pg_dump ... --user=user --host=host --port=port --dbname=database --table=schema.table
 
-        self.args = ['pg_dump', '-a', '--inserts']
+        self.args = ['pg_dump', '--no-owner']
+        if data_only:
+            self.args += ['--data-only', '--inserts']
 
         if 'PASSWORD' in self.database_config and self.database_config['PASSWORD']:
             if 'PORT' in self.database_config and self.database_config['PORT']:
                 dbname = '--dbname=postgresql://%(USER)s:%(PASSWORD)s@%(HOST)s:%(PORT)s/%(NAME)s'
             else:
                 dbname = '--dbname=postgresql://%(USER)s:%(PASSWORD)s@%(HOST)s/%(NAME)s'
 
@@ -29,8 +31,8 @@
                 self.args.append('--host=%(HOST)s' % self.database_config)
 
             if 'PORT' in self.database_config and self.database_config['PORT']:
                 self.args.append('--port=%(PORT)d' % self.database_config)
 
             self.args.append('--dbname=%(NAME)s' % self.database_config)
 
-        self.args.append('--table=%s.%s' % (schema_name, table_name))
+        self.args.append('--table="%s"."%s"' % (schema_name, table_name))
```

### Comparing `django-daiquiri-0.2/daiquiri/core/adapter/download/mysqldump.py` & `django-daiquiri-0.4.2/daiquiri/core/adapter/download/mysqldump.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from .base import BaseDownloadAdapter
 
 logger = logging.getLogger(__name__)
 
 
 class MysqldumpAdapter(BaseDownloadAdapter):
 
-    def set_args(self, schema_name, table_name):
-        self.args = ['mysqldump', '--compact', '--skip-extended-insert']
+    def set_args(self, schema_name, table_name, data_only=False):
+        self.args = ['mysqldump']
+        if data_only:
+            self.args += ['--compact', '--skip-extended-insert']
 
         if 'USER' in self.database_config and self.database_config['USER']:
             self.args.append('--user=%(USER)s' % self.database_config)
 
         if 'PASSWORD' in self.database_config and self.database_config['PASSWORD']:
             self.args.append('--password=%(PASSWORD)s' % self.database_config)
```

### Comparing `django-daiquiri-0.2/daiquiri/core/adapter/stream.py` & `django-daiquiri-0.4.2/daiquiri/core/adapter/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from daiquiri.core.utils import make_query_dict_upper_case
 
 
 class BaseServiceAdapter(object):
 
     def clean(self, request, resource):
```

### Comparing `django-daiquiri-0.2/daiquiri/core/adapter/database/mariadb.py` & `django-daiquiri-0.4.2/daiquiri/core/adapter/database/mariadb.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,7 +13,20 @@
             'max_records': max_records
         }
 
         if max_records is not None:
             return 'SET STATEMENT max_statement_time=%(timeout)s FOR CREATE TABLE %(schema)s.%(table)s ENGINE=ARIA ( %(query)s ) LIMIT %(max_records)s;' % params
         else:
             return 'SET STATEMENT max_statement_time=%(timeout)s FOR CREATE TABLE %(schema)s.%(table)s ENGINE=ARIA ( %(query)s );' % params
+
+    def build_sync_query(self, query, timeout, max_records):
+        # construct the actual query
+        params = {
+            'query': query,
+            'timeout': timeout,
+            'max_records': max_records
+        }
+
+        if max_records is not None:
+            return 'SET STATEMENT max_statement_time=%(timeout)s FOR %(query)s LIMIT %(max_records)s;' % params
+        else:
+            return 'SET STATEMENT max_statement_time=%(timeout)s FOR %(query)s;' % params
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/img/daiquiri.jpg` & `django-daiquiri-0.4.2/daiquiri/core/static/core/img/daiquiri.jpg`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/img/favicon.ico` & `django-daiquiri-0.4.2/daiquiri/core/static/core/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_selectnumber.html` & `django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_selectnumber.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_select.html` & `django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_select.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/html/formgroup_multicheckbox.html` & `django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_multicheckbox.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/html/browser.html` & `django-daiquiri-0.4.2/daiquiri/core/static/core/html/browser.html`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,20 @@
 
         <ul class="daiquiri-browser-body nav nav-pills nav-stacked">
 
             <li ng-repeat="item in column.items | filter: column.filter_string"
                 ng-class="{ 'active': browser.isActive(browserId, $parent.$index, $index) }">
                 <a href=""
                     ng-click="itemClicked(browserId, item, $parent.$index, $index);"
-                    ng-dblclick="itemDblClicked(browserId, item, $parent.$index, $index);">
+                    ng-dblclick="itemDblClicked(browserId, item, $parent.$index, $index);"
+                    data-toggle="tooltip"
+                    data-html="true"
+                    data-placement="left"
+                    data-container="body"
+                    title="{{item.description}}{{ item.unit ? '</br><b>Unit:</b> ' : '' }}{{ item.unit }}" tooltip>
                     <i class="pull-right fa fa-chevron-right" ng-show="column.selected == $index"></i>
                     {$ item.name $}
                 </a>
             </li>
         </ul>
     </div>
 </div>
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/css/base.scss` & `django-daiquiri-0.4.2/daiquiri/core/static/core/css/base.scss`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,21 @@
 body {
     // make footer sticky
     @media (min-width: $screen-sm-max) {
         margin: 0 0 ($footer-content-height + $footer-bottom-height);
     }
 }
 
-.page,
-.wide,
-.sidebar {
-    margin-top: 100px;
-    margin-bottom: 100px;
-
-    @media (max-width: $screen-sm-max) {
-        margin-top: 20px;
-        margin-bottom: 20px;
-
-        &:first-child {
-            margin-top: 100px;
-        }
-        &:last-child {
-            margin-bottom: 40px;
-        }
+main {
+    padding-top: 70px;
+    padding-bottom: 20px;
+
+    @media (min-width: $screen-xs-max) {
+        padding-top: 100px;
+        padding-bottom: 100px;
     }
 }
 
 /* typography */
 
 html, body {
     color: $text-color;
@@ -88,15 +79,19 @@
     }
     &:hover {
         color: $link-color-hover;
     }
     &:focus {
         color: $link-color-focus;
     }
-    &.btn {
+    &.btn-primary,
+    &.btn-success,
+    &.btn-info,
+    &.btn-warning,
+    &.btn-danger {
         color: white;
     }
     &.fa {
         text-decoration: none;
     }
 }
 
@@ -324,51 +319,67 @@
 }
 
 /* modals */
 
 .modal-body {
     max-height: calc(100vh - 225px);
     overflow-y: auto;
+
+    img {
+        max-width: 100%;
+    }
+    dl {
+        margin-top: 5px;
+        margin-bottom: 0;
+    }
+    dl:first-child {
+        margin-top: 0;
+    }
 }
-.modal-body img {
-    max-width: 100%;
-}
-.modal-body dl {
-    margin-top: 5px;
-    margin-bottom: 0;
-}
-.modal-body dl:first-child {
-    margin-top: 0;
-}
+
 .modal-seperator {
     margin-left: -15px;
     margin-right: -15px;
     margin-top: 15px;
     margin-bottom: 15px;
     border-bottom: 1px solid #e5e5e5;
 }
 
 /* daiquiri-widget */
 
 .daiquiri-widget {
     border: 1px solid $border-color;
     padding: 10px 15px;
-}
 
-.daiquiri-widget :last-child {
-    margin-bottom: 0;
+    margin-bottom: 20px;
+
+    &:last-child {
+        margin-bottom: 0;
+    }
+
+    .caption {
+        margin-top: 5px;
+        margin-bottom: 0;
+    }
 }
 
 /* panel */
 
 .panel {
-    .panel-body p:last-child {
+    .panel-body p:last-child,
+    .panel-body dl:last-child {
         margin-bottom: 0;
     }
 
+    .panel-footer {
+        ul, p {
+            margin: 0;
+        }
+    }
+
     li {
         &.list-group-link {
             padding: 0;
         }
         &.list-group-link:last-child > a {
             border-bottom-right-radius: 4px;
             border-bottom-left-radius: 4px;
@@ -398,15 +409,15 @@
 }
 
 div.control-label {
     margin-bottom: 5px;
     font-weight: bold;
 }
 
-.daiquiri-multi-checkbox > :first-child {
+.daiquiri-multi-checkbox >:first-child {
     margin-top: 0;
 }
 .daiquiri-multi-checkbox > :last-child {
     margin-bottom: 0;
 }
 
 div.fieldset {
@@ -414,17 +425,25 @@
 }
 
 .form-group {
     .radio {
         margin-top: 0px;
         margin-bottom: 5px;
     }
-}
 
+    .file {
+        input {
+            padding-bottom: 100px;
+        }
+    }
+}
 
+.form-inline-button {
+    margin-top: 25px;
+}
 
 /* misc */
 
 .expand {
     display: block;
     width: 100%;
 }
@@ -435,67 +454,95 @@
 
 .hide-overflow {
     width: 100%;
     overflow: hidden;
     text-overflow: ellipsis;
 }
 
-.email-form label,
-.connections-form label {
-    display: block;
-    margin: 0;
-    line-height: 40px;
-    border-bottom: 1px solid $modal-border-color;
-}
-.email-form label:first-child,
-.connections-form label:first-child {
-    border-top: 1px solid $modal-border-color;
-}
-.email-form label input,
-.connections-form label input {
-    margin-left: 5px;
-    margin-right: 5px;
+.email-form,
+.connections-form {
+    label {
+        display: block;
+        margin: 0;
+        line-height: 40px;
+        border-bottom: 1px solid $modal-border-color;
+
+        &:first-child {
+            border-top: 1px solid $modal-border-color;
+        }
+
+        input {
+            margin-left: 5px;
+            margin-right: 5px;
+        }
+    }
 }
 .email-form .email-form-buttons,
 .connections-form .connections-form-buttons {
     margin-top: 10px;
 }
+
 .socialaccount_providers {
     margin: 0;
     padding: 0;
     height: 42px;
-}
-.socialaccount_providers li {
-    float: left;
-    margin-right: 10px;
-    list-style: none;
+
+    li {
+        float: left;
+        margin-right: 10px;
+        list-style: none;
+    }
 }
 .socialaccount_provider_name {
     line-height: 29px;
     font-weight: bold;
 }
 
 .logout-form {
     margin: 0;
+
+    .btn-link {
+        padding: 3px 20px;
+        display: block;
+        width: 100%;
+        text-align: left;
+        border: none;
+        clear: both;
+        font-weight: 400;
+        line-height: 1.42857143;
+        white-space: nowrap;
+    }
+    .btn-link:hover {
+        color: $navigation-dropdown-hover-color;
+        background-color: $navigation-dropdown-hover-background-color;
+        text-decoration: none;
+    }
+    .btn-link:focus {
+        color: $navigation-dropdown-hover-color;
+        background-color: $navigation-dropdown-hover-background-color;
+        text-decoration: none;
+        outline: none;
+    }
 }
-.logout-form .btn-link {
-    padding: 3px 20px;
-    display: block;
+
+.pager-vertical {
+    a {
+        margin-bottom: 10px;
+
+        display: block;
+        width: 100%;
+    }
+}
+
+.table-fixed {
+    table-layout: fixed;
+}
+
+.w-50 {
+    width: 50%;
+}
+.w-75 {
+    width: 75%;
+}
+.w-100 {
     width: 100%;
-    text-align: left;
-    border: none;
-    clear: both;
-    font-weight: 400;
-    line-height: 1.42857143;
-    white-space: nowrap;
-}
-.logout-form .btn-link:hover {
-    color: $navigation-dropdown-hover-color;
-    background-color: $navigation-dropdown-hover-background-color;
-    text-decoration: none;
-}
-.logout-form .btn-link:focus {
-    color: $navigation-dropdown-hover-color;
-    background-color: $navigation-dropdown-hover-background-color;
-    text-decoration: none;
-    outline: none;
 }
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/css/browser.scss` & `django-daiquiri-0.4.2/daiquiri/core/static/core/css/browser.scss`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,24 @@
     border-radius: 0;
 
     text-overflow: ellipsis;
     white-space: nowrap;
     overflow: hidden;
 }
 
+.daiquiri-browser .nav-pills > li.active > a {
+    color: $panel-active-color;
+    background-color: $panel-active-background-color;
+}
+
 .daiquiri-browser .nav-header {
     padding: 5px 15px;
 }
 
 .daiquiri-browser i.fa {
     padding-top: 4px;
-}
+}
+
+.tooltip-inner {
+    max-width: 250px !important;
+    text-align: left;
+}
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/css/table.scss` & `django-daiquiri-0.4.2/daiquiri/core/static/core/css/table.scss`

 * *Files 23% similar despite different names*

```diff
@@ -139,7 +139,58 @@
             line-height: 34px;
         }
         .daiquiri-table-page-size {
 
         }
     }
 }
+
+.daiquiri-table-modal {
+    .modal-body {
+        min-height: 100px;
+
+        ul {
+            margin-top: 40px;
+            margin-bottom: 40px;
+        }
+    }
+
+    .modal-pagination {
+        a {
+            position: absolute;
+            z-index: 1100;
+
+            display: block;
+
+            opacity: 0.1;
+
+            width: 40px;
+            height: 56px;
+
+            &:hover {
+                opacity: 1.0;
+            }
+        }
+
+        .modal-pagination-left,
+        .modal-pagination-right {
+            top: 50%;
+        }
+        .modal-pagination-left {
+            left: 5px;
+        }
+        .modal-pagination-right {
+            right: 5px;
+        }
+        .modal-pagination-up,
+        .modal-pagination-down {
+            left: 50%;
+            margin-left: -30px;
+        }
+        .modal-pagination-up {
+            top: 50px;
+        }
+        .modal-pagination-down {
+            bottom: 55px;
+        }
+    }
+}
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/css/fonts.scss` & `django-daiquiri-0.4.2/daiquiri/core/static/core/css/fonts.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/css/variables.scss` & `django-daiquiri-0.4.2/daiquiri/core/static/core/css/variables.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/css/list.scss` & `django-daiquiri-0.4.2/daiquiri/core/static/core/css/list.scss`

 * *Files 19% similar despite different names*

```diff
@@ -8,19 +8,25 @@
         form,
         .pagination {
             margin-top: 0;
             margin-bottom: 10px;
         }
         .count {
             display: inline-block;
-            line-height: 34px;
+            padding: 7px 0;
         }
         .pagination {
             margin-left: 5px;
         }
+
+        @media (max-width: $screen-md-max) {
+            .pull-right {
+                float: none!important;
+            }
+        }
     }
     .daiquiri-list-table {
         th .order {
             cursor: pointer;
 
             i {
                 opacity: 0.2;
@@ -42,8 +48,19 @@
 
                 a.dropdown-toggle {
                     cursor: pointer;
                 }
             }
         }
     }
+    .daiquiri-list-filter {
+        label {
+            margin-left: 10px;
+            font-weight: normal;
+
+            input[type=checkbox] {
+                margin: 0 0 2px 0;
+                vertical-align: middle;
+            }
+        }
+    }
 }
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/js/polling.js` & `django-daiquiri-0.4.2/daiquiri/core/static/core/js/polling.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/js/browser.js` & `django-daiquiri-0.4.2/daiquiri/core/static/core/js/browser.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/js/list.js` & `django-daiquiri-0.4.2/daiquiri/core/static/core/js/list.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -59,14 +59,17 @@
                     }
                     service.idle = true;
                     service.ready = true;
 
                     if (response.next) {
                         service.fetch();
                     }
+                }, function() {
+                    service.idle = true;
+                    service.ready = true;
                 }).$promise;
             }
         };
 
         service.search = function() {
             service.params.search = service.search_string;
             service.reload();
@@ -78,15 +81,15 @@
             } else {
                 service.params.ordering = column_name;
             }
             service.reload();
         };
 
         service.reset = function() {
-            service.params.page = 1;
+            service.params.search = null;
             service.params.ordering = null;
             service.reload();
         };
 
         service.reload = function() {
             service.params.page = 1;
             service.fetch();
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/js/table.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/query.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,405 +1,377 @@
-angular.module('core')
+app.factory('QueryService', ['$resource', '$http', '$injector', '$q', '$filter', 'PollingService', 'PlotService', 'DownloadService', 'TableService', 'BrowserService', function($resource, $http, $injector, $q, $filter, PollingService, PlotService, DownloadService, TableService, BrowserService) {
 
-    .factory('TableService', ['$http', '$resource', '$q', '$document', '$timeout', '$rootScope', '$compile', '$templateCache', function($http, $resource, $q, $document, $timeout, $rootScope, $compile, $templateCache) {
+    /* get the base url */
 
-        /* get the base url */
+    var baseurl = angular.element('meta[name="baseurl"]').attr('content');
 
-        var baseurl = angular.element('meta[name="baseurl"]').attr('content');
+    /* configure resources */
 
-        /* configure the resources */
-
-        var resources = {};
-
-        /* create the metadata service */
-
-        var service = {
-            params: {
-                page: 1,
-                page_size: 10,
-                ordering: null,
-                search: null
-            },
-            page_sizes: [10, 20, 100],
-            active: {},
-            modal: {},
-            getter: {
-                row_id: function(row) {
-                    return JSON.stringify(row);
-                },
-                file_url: function(row, column_index) {
-                    return service.files_url + '?search=' + window.encodeURIComponent(row[column_index]);
-                },
-                reference_url: function(row, column_index) {
-                    var key = window.encodeURIComponent(service.columns[column_index].name),
-                        value = window.encodeURIComponent(row[column_index]);
-
-                    return service.references_url + '?key=' + key + '&value=' + value;
-                },
-                link_url: function(row, column_index) {
-                    return row[column_index];
-                }
-            }
-        };
-
-        service.init = function(opt) {
-            service.ready = false;
-
-            // set up resources and urls
-            if (angular.isDefined(opt.rows_url)) {
-                resources.rows = $resource(baseurl + opt.rows_url);
-            }
-            if (angular.isDefined(opt.columns_url)) {
-                resources.columns = $resource(baseurl + opt.columns_url);
-            }
-            if (angular.isDefined(opt.files_url)) {
-                service.files_url = baseurl + opt.files_url;
-            }
-            if (angular.isDefined(opt.references_url)) {
-                service.references_url = baseurl + opt.references_url;
-            }
-
-            // update params
-            if (angular.isDefined(opt.params)) {
-                angular.extend(service.params, opt.params);
-            }
+    var resources = {
+        status: $resource(baseurl + 'query/api/status/'),
+        forms: $resource(baseurl + 'query/api/forms/'),
+        dropdowns: $resource(baseurl + 'query/api/dropdowns/'),
+        jobs: $resource(baseurl + 'query/api/jobs/:id/:detail_action/'),
+        examples: $resource(baseurl + 'query/api/examples/user/'),
+        queues: $resource(baseurl + 'query/api/queues/'),
+        querylanguages: $resource(baseurl + 'query/api/querylanguages/'),
+        phases: $resource(baseurl + 'query/api/phases/'),
+        schemas: $resource(baseurl + 'metadata/api/schemas/user/'),
+        functions: $resource(baseurl + 'metadata/api/functions/user/'),
+    };
+
+    var upload_url = baseurl + 'query/api/jobs/upload/';
+
+    /* initialise the browser service */
+
+    BrowserService.init('schemas', ['schemas', 'tables', 'columns'])
+    BrowserService.init('columns', ['columns'], true)
+    BrowserService.init('functions', ['functions'])
+    BrowserService.init('examples', ['examples'])
+
+    /* create the query service */
+
+    var service = {
+        first_form: null,
+        submitting: false,
+        show: {
+            '': true
+        },
+        forms: {},
+        dropdowns: {},
+        values: {},
+        errors: {}
+    };
+
+    service.init = function() {
+        // fetch queues,  query languages and then load forms
+        service.queues = resources.queues.query();
+        service.query_languages = resources.querylanguages.query();
+
+        $q.all([service.queues.$promise, service.query_languages.$promise]).then(function() {
+            service.active_queue = service.queues[0].id;
+
+            resources.forms.query(function(response) {
+                angular.forEach(response, function(form) {
+                    service.forms[form.key] = $injector.get(form.form_service);
+
+                    // remember the first form
+                    if (!service.first_form) {
+                        service.first_form = service.forms[form.key];
+                    }
+                });
 
-            // set pages_sizes
-            if (angular.isDefined(opt.page_sizes)) {
-                service.page_sizes = opt.page_sizes;
-                service.params.page_size = opt.page_sizes[0];
-            }
+                // activate the first form
+                service.first_form.activate();
+            });
+        });
 
-            // set custom getter functions
-            if (angular.isDefined(opt.getter)) {
-                angular.forEach(opt.getter, function(func, key) {
-                    service.getter[key] = func;
-                })
-            }
+        // fetch job phases
+        service.phases = resources.phases.query();
 
-            // set additional options
-            angular.forEach(opt, function(value, key) {
-                if ([
-                        'rows_url',
-                        'columns_url',
-                        'files_url',
-                        'references_url',
-                        'params',
-                        'page_sizes',
-                        'getter'
-                    ].indexOf(key) == -1) {
-                    service[key] = opt[key];
-                }
+        // load dropdowns
+        resources.dropdowns.query(function(response) {
+            angular.forEach(response, function(dropdown) {
+                service.dropdowns[dropdown.key] = $injector.get(dropdown.dropdown_service);
+                service.dropdowns[dropdown.key].options = dropdown.options;
             });
+        });
 
-            // add params from the dom to service.params and fetch the data
-            if (angular.isUndefined(opt.fetch) || opt.fetch) {
+        // fetch status
+        service.fetch_status();
 
-                resources.columns.query(service.params, function(response) {
-                    service.columns = response;
-
-                    // check column ucds for display mode
-                    angular.forEach(service.columns, function(column) {
-                        // the default display mode is 'text'
-                        column.display = 'text'
-
-                        if (column.ucd) {
-                            if (column.ucd.indexOf('meta.note') > -1) {
-                                if (service.files_url) {
-                                    column.display = 'modal';
-                                } else {
-                                    column.display = 'link';
-                                }
-                            } else if (column.ucd.indexOf('meta.preview') > -1) {
-                                if (service.files_url) {
-                                    column.display = 'modal';
-                                } else {
-                                    column.display = 'link';
-                                }
-                            } else if (column.ucd.indexOf('meta.file') > -1) {
-                                if (service.files_url) {
-                                    column.display = 'file';
-                                } else {
-                                    column.display = 'link';
-                                }
-                            } else if (column.ucd.indexOf('meta.ref') > -1) {
-                                if (service.references_url) {
-                                    column.display = 'reference';
-                                } else {
-                                    column.display = 'link';
-                                }
-                            } else if (column.ucd.indexOf('meta.ref.uri') > -1) {
-                                column.display = 'link';
-                            } else if (column.ucd.indexOf('meta.ref.url') > -1) {
-                                column.display = 'link';
-                            }
-                        }
+        // fetch functions
+        resources.functions.query(function(response) {
+            BrowserService.render('functions', response);
+        });
+
+        // fetch examples
+        resources.examples.query(function(response) {
+            BrowserService.render('examples', response);
+        });
+
+        // fetch schemas
+        resources.schemas.query(function(response) {
+            service.schemas = response;
+
+            service.columns = []
+            angular.forEach(service.schemas, function(schema) {
+                angular.forEach(schema.tables, function(table) {
+                    angular.forEach(table.columns, function(column) {
+                        var column_copy = angular.copy(column);
+                        column_copy.name = schema.name + '.' + table.name + '.' + column.name;
+                        service.columns.push(column_copy);
                     });
-
-                    if (service.tooltips) {
-                        $timeout(function() {
-                            var template = $templateCache.get('tooltip.html');
-
-                            angular.forEach(service.columns, function(column, index) {
-                                var isolated_scope = $rootScope.$new(true);
-                                isolated_scope.column = column;
-                                isolated_scope.table = service;
-
-                                $('[data-column-index="' + index + '"] .info').popover({
-                                    title: '<strong>' + column.name + '</strong>',
-                                    content: $compile(template)(isolated_scope),
-                                    html: true,
-                                    trigger: 'hover',
-                                    placement: 'bottom',
-                                    container: '.daiquiri-table'
-                                });
-                            });
-                        });
-                    }
-
-                    if (service.column_widths) {
-                        $timeout(function() {
-                            angular.forEach(service.column_widths, function(column_width, column_index) {
-                                angular.element('[data-column-index="' + column_index + '"]').width(column_width);
-                            });
-                        });
-                    }
-
-                    service.reset();
                 });
-            }
-        };
-
-        service.clear = function() {
-            service.columns = [];
-            service.rows = [];
-            service.ready = true;
-        };
-
-        service.fetch = function() {
-            return resources.rows.paginate(service.params, function(response) {
-                service.count = response.count;
-                service.rows = response.results;
-
-                service.page_count = Math.ceil(service.count / service.params.page_size);
-
-                service.first_page = (service.params.page == 1);
-                service.last_page = (service.params.page * service.params.page_size >= service.count);
+            });
 
-                if (service.checkboxes) {
-                    service.update_checked_all();
+            // fetch user schema and init browser
+            service.fetch_user_schema();
+        });
+
+        // fetch joblist
+        service.fetch_jobs();
+
+        // activate overview tab
+        service.tab = 'overview';
+
+        // start the polling service
+        service.polling = PollingService
+        service.polling.init();
+        service.polling.register('status', service.fetch_status, {}, true, false);
+        service.polling.register('jobs', service.fetch_jobs, {}, true, false);
+        service.polling.register('schema', service.fetch_user_schema, {}, true, false);
+
+        // load the other services
+        service.table = TableService;
+        service.plot = PlotService;
+        service.downloads = DownloadService;
+    };
+
+    service.fetch_status = function() {
+        return resources.status.query(function(response) {
+            if (angular.isDefined(service.status) && service.status.guest != response[0].guest) {
+                // the user has been logged out
+                $('#logout-modal').modal('show');
+            }
+            service.status = response[0];
+        }).$promise;
+    };
+
+    service.fetch_user_schema = function() {
+        return resources.jobs.query({
+            'detail_action': 'tables'
+        }, function(response) {
+            var user_schema = response[0];
+
+            BrowserService.render('schemas', service.schemas.concat(user_schema));
+            BrowserService.render('columns', service.columns);
+        }).$promise;
+    }
+
+    service.fetch_jobs = function() {
+        return resources.jobs.paginate({
+            page_size: 1000,
+            archived: ''
+        }, function(response) {
+            service.jobs = response.results;
+
+            service.run_ids = service.jobs.map(function(job) {
+                return job.run_id;
+            }).filter(function(run_id, index, run_ids) {
+                return run_id && run_ids.indexOf(run_id) == index;
+            }).sort();
+            service.run_ids.push('');
+
+            if (service.job) {
+                // show the run id of the current job
+                service.show[service.job.run_id] = true;
+
+                // get the current job from the jobs list
+                var current_job = $filter('filter')(service.jobs, {
+                    'id': service.job.id
+                })[0];
+
+                // if the phase has changed, fetch it again
+                if (current_job && current_job.phase != service.job.phase) {
+                    service.activate_job(service.job);
                 }
-
-                service.ready = true;
-            }).$promise;
-        };
-
-        service.first = function() {
-            if (!service.first_page) {
-                service.params.page = 1;
-                service.fetch();
             }
-        };
 
-        service.previous = function() {
-            if (!service.first_page) {
-                service.params.page -= 1;
-                return service.fetch();
-            }
-        };
-
-        service.next = function() {
-            if (!service.last_page) {
-                service.params.page += 1;
-                return service.fetch();
-            }
-        };
-
-        service.last = function() {
-            if (!service.last_page) {
-                service.params.page = Math.ceil(service.count / service.params.page_size);
-                service.fetch();
-            }
-        };
-
-        service.reset = function() {
-            service.params.page = 1;
-            service.params.ordering = null;
-            service.params.search = null;
-            service.search_string = null;
-            service.checked = {};
-            service.fetch();
-        };
-
-        service.search = function() {
-            service.params.search = service.search_string;
-            service.fetch();
-        };
-
-        service.order = function(column_name) {
-            if (service.params.ordering == column_name) {
-                service.params.ordering = '-' + column_name;
-            } else {
-                service.params.ordering = column_name;
-            }
-            service.fetch();
-        };
-
-        service.resize = function(column_index) {
-            var zero = event.pageX;
-            var table = angular.element('.daiquiri-table-pane .table');
-            var th = angular.element('[data-column-index="' + column_index + '"]');
-            var width = th.width();
-
-            table.addClass('no-select');
-
-            function enterResize(event) {
-                var newWidth = width + event.pageX - zero;
-                if (newWidth >= 40) th.width(newWidth);
-            }
-
-            function exitResize() {
-                table.removeClass('no-select');
-                $document.off('mousemove', enterResize);
-                $document.off('mouseup', exitResize);
-            }
-
-            $document.on('mousemove', enterResize);
-            $document.on('mouseup', exitResize);
-        };
-
-        service.activate = function(column_index, row_index) {
-            service.active = {
-                column_index: column_index,
-                row_index: row_index
-            }
-        };
+        }).$promise;
+    };
 
-        service.check_all = function() {
-            angular.forEach(service.rows, function(row) {
-                service.checked[service.getter.id(row)] = service.checked_all;
-            })
-        };
-
-        service.update_checked_all = function() {
-            service.checked_all = service.rows.map(function(row) {
-                return service.checked[service.getter.id(row)];
-            }).every(function(element) {
-                return element === true;
+    service.fetch_job = function(job) {
+        return resources.jobs.get({
+            id: job.id
+        }, function(response) {
+            service.job = response;
+
+            // get the current job in the jobs list
+            var jobs_job = $filter('filter')(service.jobs, {
+                'id': service.job.id
+            })[0]
+
+            if (angular.isUndefined(jobs_job) || jobs_job.phase != service.job.phase) {
+                // if the phase has changed, fetch the job list again
+                service.fetch_jobs();
+            }
+        }).$promise;
+    };
+
+    service.activate_form = function(key) {
+        // this function should be called from the form service
+        service.form = key;
+        service.job = null;
+    };
+
+    service.submit_job = function(values) {
+        // this function should be called from the form service
+        values = angular.extend({}, values, {
+            'queue': service.active_queue
+        });
+
+        service.submitting = true;
+        return resources.jobs.save(values).$promise
+            .then(function(job) {
+                service.fetch_status();
+                service.activate_job(job);
+            }).finally(function() {
+                service.submitting = false;
             });
-        };
-
-
-        service.modal_open = function(event, column_index, row_index) {
-            event.preventDefault();
-            event.stopPropagation();
+    };
 
-            service.modal.pre = null;
-            service.modal.src = null;
+    service.upload_job = function(values) {
+        // a special version of submit_job for the upload
 
-            service.activate(column_index, row_index);
-
-            service.modal_update().then(function() {
-                // add a litte delay to the modal so that a change in service.modal.src
-                // does not make the image flicker/change in size after opening.
-                $timeout(function() {
-                    $('#daiquiri-table-modal').modal('show');
-                }, 100);
+        // put the payload in a FormData object
+        var formdata = new FormData();
+        angular.forEach(values, function(value, key) {
+            if (angular.isDefined(value) && value) {
+                formdata.append(key, value);
+            }
+        });
+
+        service.submitting = true;
+        return $http({
+                method: 'POST',
+                url: upload_url,
+                headers: {
+                    'Content-Type': undefined
+                },
+                data: formdata
             })
-        };
-
-        service.modal_update = function() {
-            var file_path = service.rows[service.active.row_index][service.active.column_index];
-            var url = service.files_url + '?search=' + file_path;
-            var column = service.columns[service.active.column_index];
-
-            service.modal.title = file_path;
-
-            if (column.ucd.indexOf('meta.note') > -1) {
-                return $http.get(url).then(function(result) {
-                    service.modal.pre = result.data;
-                    service.modal.src = null;
-                });
-            } else if (column.ucd.indexOf('meta.preview') > -1) {
-                service.modal.pre = null;
-                service.modal.src = url;
+            .then(function(response) {
+                service.fetch_status();
+                service.activate_job(response.data);
+            }).finally(function() {
+                service.submitting = false;
+            });
+    }
 
-                return $q.when();
+    service.activate_job = function(job) {
+        service.form = null;
+        service.fetch_job(job).then(function() {
+            service.table.ready = false;
+            service.plot.ready = false;
+
+            if (service.job.phase == 'COMPLETED') {
+                // re-init current tab
+                service.init_tab(service.tab);
             } else {
-                return $q.when();
+                // activate overview tab
+                service.activate_tab('overview');
             }
-        };
 
-        service.modal_up = function() {
-            if (service.active.row_index > 0) {
-                // decrement the row_index and update modal
-                service.active.row_index -= 1;
-                service.modal_update();
-            } else if (!service.first_page) {
-                // first load previous page
-                service.previous().then(function() {
-                    // set row_index to the last row and update modal
-                    service.active.row_index = service.rows.length - 1;
-                    service.modal_update();
-                });
+            CodeMirror.runMode(service.job.query, "text/x-sql", angular.element('#query')[0]);
+
+            if (service.job.native_query) {
+                CodeMirror.runMode(service.job.native_query, "text/x-sql", angular.element('#native-query')[0]);
             }
-        };
+            if (service.job.actual_query) {
+                CodeMirror.runMode(service.job.actual_query, "text/x-sql", angular.element('#actual-query')[0]);
+            }
+        });
+    };
+
+    service.modal = function(modal_id) {
+        service.errors = {};
+        service.values = service.job;
+
+        $('#' + modal_id).modal('show');
+    };
+
+    service.update_job = function() {
+        resources.jobs.update({
+            id: service.values.id
+        }, service.values).$promise.then(function() {
+            service.fetch_jobs();
+            $('.modal').modal('hide');
+        }, function(response) {
+            service.errors = response.data;
+        });
+    };
+
+    service.abort_job = function() {
+        resources.jobs.update({
+            id: service.values.id,
+            detail_action: 'abort'
+        }, {}, function() {
+            service.fetch_status();
+            service.fetch_jobs();
+            $('.modal').modal('hide');
+        });
+    };
+
+    service.archive_job = function() {
+        var index = service.jobs.indexOf($filter('filter')(service.jobs, {
+            'id': service.job.id
+        })[0]);
+
+        var next_job = null;
+        if (index == 0 && angular.isDefined(service.jobs[1])) {
+            next_job = service.jobs[1];
+        } else if (angular.isDefined(service.jobs[index - 1])) {
+            next_job = service.jobs[index - 1];
+        }
+
+        resources.jobs.delete({
+            id: service.values.id
+        }, function() {
+            service.fetch_status();
+            service.fetch_jobs();
 
-        service.modal_down = function() {
-            if (service.active.row_index < service.rows.length - 1) {
-                // increment the row_index and update modal
-                service.active.row_index += 1;
-                service.modal_update();
-            } else if (!service.last_page) {
-                // first load next page
-                service.next().then(function() {
-                    // set row_index to 0 and update modal
-                    service.active.row_index = 0;
-                    service.modal_update();
-                });
+            if (next_job) {
+                service.activate_job(next_job);
+            } else {
+                service.first_form.activate();
             }
-        };
 
-        service.modal_left = function() {
-            var next_column_index = null,
-                current_column_index = service.active.column_index;
-
-            while (next_column_index === null) {
-                if (current_column_index > 0) {
-                    current_column_index -= 1;
+            $('.modal').modal('hide');
+        });
+    };
+
+    service.activate_tab = function(tab) {
+        service.init_tab(tab);
+        service.tab = tab;
+    };
+
+    service.init_tab = function(tab) {
+        if (tab == 'results') {
+            if (!service.table.ready) {
+                if (service.job && service.job.phase == 'COMPLETED') {
+                    service.table.init({
+                        tooltips: true,
+                        rows_url: 'query/api/jobs/' + service.job.id + '/rows/',
+                        columns_url: 'query/api/jobs/' + service.job.id + '/columns/',
+                        files_url: 'files/',
+                        references_url: 'serve/references/',
+                        datalink_url: 'datalink/',
+                        params: {
+                            job: service.job.id
+                        }
+                    });
                 } else {
-                    current_column_index = service.columns.length - 1;
-                }
-
-                var column = service.columns[current_column_index];
-                if (column.ucd !== null && (column.ucd.indexOf('meta.note') > -1 || column.ucd.indexOf('meta.preview') > -1)) {
-                    next_column_index = current_column_index;
+                    service.table.clear();
                 }
             }
-
-            service.active.column_index = current_column_index;
-            service.modal_update();
-        };
-
-        service.modal_right = function() {
-            var next_column_index = null,
-                current_column_index = service.active.column_index;
-
-            while (next_column_index === null) {
-                if (current_column_index < service.columns.length - 1) {
-                    current_column_index += 1;
+        } else if (tab == 'plot') {
+            if (!service.plot.ready) {
+                if (service.job && service.job.phase == 'COMPLETED') {
+                    service.plot.init({
+                        rows_url: 'query/api/jobs/' + service.job.id + '/rows/',
+                        columns: service.job.columns
+                    });
                 } else {
-                    current_column_index = 0;
-                }
-
-                var column = service.columns[current_column_index];
-                if (column.ucd !== null && (column.ucd.indexOf('meta.note') > -1 || column.ucd.indexOf('meta.preview') > -1)) {
-                    next_column_index = current_column_index;
+                    service.plot.clear();
                 }
             }
+        } else if (tab == 'download') {
+            service.downloads.init({
+                job: service.job
+            });
+        }
+    }
 
-            service.active.column_index = current_column_index;
-            service.modal_update();
-        };
+    return service;
 
-        return service;
-    }]);
+}]);
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/js/multiCheckbox.js` & `django-daiquiri-0.4.2/daiquiri/core/static/core/js/multiCheckbox.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/js/stream.js` & `django-daiquiri-0.4.2/daiquiri/core/static/core/js/stream.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -23,27 +23,32 @@
                 service.resource = opt.resource;
             }
 
             service.reset();
         };
 
         service.reset = function() {
-            console.log(service.defaults);
             angular.forEach(service.defaults, function(value, key) {
                 service.values[key] = value;
             });
         };
 
         service.download = function() {
             // construct the url for the stream
             var url = service.stream_url + '/' + service.resource + '/?' + $httpParamSerializer(service.values);
 
             $http.get(url + '&download=').then(function() {
-                // download the file, headers will prevent the browser reloading the page
-                window.location.href = url;
+                // download the file using an iframe
+                var iframe = document.createElement('iframe');
+                iframe.style.display = 'none';
+                iframe.src = url;
+                iframe.onload = function() {
+                    this.parentNode.removeChild(this)
+                }
+                document.body.appendChild(iframe)
             }, function(result) {
                 service.errors = result.data;
             });
         }
 
         service.build_query_params = function() {
             service.query_params = $httpParamSerializer(service.values);
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/js/byNumber.js` & `django-daiquiri-0.4.2/daiquiri/core/static/core/js/byNumber.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/js/formgroup.js` & `django-daiquiri-0.4.2/daiquiri/core/static/core/js/formgroup.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
                 optionsNull: '@',
                 optionsEmpty: '@'
             },
             templateUrl: function(element, attrs) {
                 var staticurl = angular.element('meta[name="staticurl"]').attr('content');
                 return staticurl + 'core/html/formgroup_' + attrs.type + '.html';
             },
-            link: function(scope, element, attrs) {
+            link: function(scope, element, attrs, ngModelController) {
                 if (!attrs.optionsId) {
                     attrs.optionsId = 'id';
                 }
 
                 scope.label = $sce.trustAsHtml(scope.label);
             }
         };
```

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf` & `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf` & `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSansMono.ttf` & `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSansMono.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf` & `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSans.ttf` & `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSans.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSans-Bold.ttf` & `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/static/core/fonts/DroidSerif.ttf` & `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/templates/core/base_head.html` & `django-daiquiri-0.4.2/daiquiri/core/templates/core/base_head.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-{% load staticfiles %}
+{% load static %}
 {% load compress %}
-{% load core_tags %}
+{% load vendor_tags %}
 
 <title>{{ request.site.name }}</title>
 
 <meta charset="UTF-8" />
 <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
 
 <meta property="og:title" content="{{ request.site.name }}" />
@@ -19,8 +19,9 @@
 {% vendor 'bootstrap' %}
 {% vendor 'font-awesome' %}
 
 {% compress css %}
 <link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/base.scss' %}" />
 <link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/fonts.scss' %}" />
 <link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/style.scss' %}" />
+<link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/codehilite.scss' %}" />
 {% endcompress %}
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-{% load staticfiles %} {% load compress %} {% load core_tags %}
+{% load static %} {% load compress %} {% load vendor_tags %}
 
 
 
 
 
 
  {% vendor 'jquery' %} {% vendor 'bootstrap' %} {% vendor 'font-awesome' %} {%
 compress css %}
 
 
+
  {% endcompress %}
```

### Comparing `django-daiquiri-0.2/daiquiri/core/templates/core/partials/form_field.html` & `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/form_field.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_pagination.html` & `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_pagination.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_tooltip.html` & `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_tooltip.html`

 * *Files 19% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     <div ng-show="column.datatype">
         <strong>{% trans 'Data type' %}</strong> {$ column.datatype $}
     </div>
     <div ng-show="column.arraysize">
         <strong>{% trans 'Array size' %}</strong> {$ column.arraysize $}
     </div>
     <div>
-        <strong ng-show="column.principal">{% trans 'Principal' %}</strong>
+        <span ng-show="column.principal">{% trans 'This column is considered a core part of the service.' %}</span>
     </div>
     <div>
-        <strong ng-show="column.indexed">{% trans 'Indexed' %}</strong>
+        <span ng-show="column.indexed">{% trans 'This column is indexed.' %}</span>
     </div>
     <div>
-        <strong ng-show="column.std">{% trans 'Std' %}</strong>
+        <span ng-show="column.std">{% trans 'This column is defined by a standard.' %}</span>
     </div>
 </script>
```

### Comparing `django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_pane.html` & `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_pane.html`

 * *Files 9% similar despite different names*

```diff
@@ -42,36 +42,47 @@
 
                 <td ng-repeat="column in service.table.columns"
                     ng-if="!column.hidden"
                     ng-init="column_index = $index"
                     ng-class="{'selected': column_index == service.table.active.column_index}">
 
                     <div class="daiquiri-table-cell" ng-click="service.table.activate(column_index, row_index)">
-                        <div ng-if="column.display == 'modal'">
+                        <div ng-if="column.meta == 'note'">
                             <a href="{$ service.table.getter.file_url(row, column_index) $}"
                                 ng-click="service.table.modal_open($event, column_index, row_index)">
-                                {$ row[column_index] $}
+                                {$ row[column_index]|basename $}
+                            </a>
+                        </div>
+                        <div ng-if="column.meta == 'image'">
+                            <a href="{$ service.table.getter.file_url(row, column_index) $}"
+                                ng-click="service.table.modal_open($event, column_index, row_index)">
+                                {$ row[column_index]|basename $}
                             </a>
                         </div>
-                        <div ng-if="column.display == 'file'">
+                        <div ng-if="column.meta == 'file'">
                             <a href="{$ service.table.getter.file_url(row, column_index) $}">
+                                {$ row[column_index]|basename $}
+                            </a>
+                        </div>
+                        <div ng-if="column.meta == 'link'">
+                            <a href="{$ service.table.getter.link_url(row, column_index) $}" target="_blank">
                                 {$ row[column_index] $}
                             </a>
                         </div>
-                        <div ng-if="column.display == 'reference'">
+                        <div ng-if="column.meta == 'reference'">
                             <a href="{$ service.table.getter.reference_url(row, column_index) $}" target="_blank">
                                 {$ row[column_index] $}
                             </a>
                         </div>
-                        <div ng-if="column.display == 'link'">
-                            <a href="{$ service.table.getter.link_url(row, column_index) $}" target="_blank">
+                        <div ng-if="column.meta == 'datalink'">
+                            <a href="{$ service.table.getter.datalink_url(row, column_index) $}" target="_blank">
                                 {$ row[column_index] $}
                             </a>
                         </div>
-                        <div ng-if="column.display == 'text'">
+                        <div ng-if="column.meta == 'text'">
                             <div ng-if="service.table.column_round[column_index]">
                                 {$ row[column_index] | number : service.table.column_round[column_index] $}
                             </div>
                             <div ng-if="!service.table.column_round[column_index]">
                                 {$ row[column_index] $}
                             </div>
                         </div>
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
 {% load i18n %}
 ⁰                                   {$ column.label $} {$ column.name $}
-                                      {$_row[column_index]_$}
-                                      {$_row[column_index]_$}
+                                      {$_row[column_index]|basename_$}
+                                      {$_row[column_index]|basename_$}
+                                      {$_row[column_index]|basename_$}
                                       {$_row[column_index]_$}
 ⁰                                   {$_row[column_index]_$}
+                                      {$_row[column_index]_$}
                                       {$ row[column_index] | number :
                                       service.table.column_round[column_index]
                                       $}
                                       {$ row[column_index] $}
 {% trans 'No rows were retrieved.' %}
```

### Comparing `django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_footer.html` & `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_footer.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/core/templates/core/partials/table_modal.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_archive_job.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 {% load i18n %}
 
-<div class="modal" id="daiquiri-table-modal" tabindex="-1">
-    <div class="modal-dialog modal-lg">
+<div class="modal" id="archive-job-modal" tabindex="-1">
+    <div class="modal-dialog">
         <div class="modal-content">
             <div class="modal-header">
                 <button type="button" class="close" data-dismiss="modal">
                     <span aria-hidden="true">&times;</span>
                 </button>
                 <h4 class="modal-title">
-                    {$ service.table.modal.title $}
+                    {% trans 'Archive job' %}
                 </h4>
             </div>
 
             <div class="modal-body">
-                <pre ng-show="service.table.modal.pre">{$ service.table.modal.pre $}</pre>
-                <img class="center-block" ng-show="service.table.modal.src" ng-src="{$ service.table.modal.src $}" />
+                <p>
+                    {% blocktrans trimmed with table_name='{$ service.values.table_name $}' %}
+                    You are about to archive the job <code>{{ table_name }}</code>.
+                    {% endblocktrans %}
+                </p>
+                <p class="text-danger">
+                    {% trans 'This action cannot be undone!' %}
+                </p>
             </div>
 
             <div class="modal-footer">
-                <div class="pull-left">
-                    <button type="button" class="btn btn-default" ng-click="service.table.modal_left()">
-                        {% trans 'Previous column' %}
-                    </button>
-                    <button type="button" class="btn btn-default" ng-click="service.table.modal_right()">
-                        {% trans 'Next column' %}
-                    </button>
-                </div>
-                <div>
-                    <button type="button" class="btn btn-default" ng-click="service.table.modal_up()">
-                        {% trans 'Previous row' %}
-                    </button>
-                    <button type="button" class="btn btn-default" ng-click="service.table.modal_down()">
-                        {% trans 'Next row' %}
-                    </button>
-                </div>
+                <button type="button" class="btn btn-default" data-dismiss="modal">
+                    {% trans 'Close' %}
+                </button>
+                <button type="button" class="btn btn-danger"
+                        ng-click="service.archive_job()">
+                    {% trans 'Archive' %}
+                </button>
             </div>
         </div>
     </div>
 </div>
```

### Comparing `django-daiquiri-0.2/daiquiri/core/management/commands/rabbitcreate.py` & `django-daiquiri-0.4.2/daiquiri/core/management/commands/rabbitcreate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from urllib.parse import urlparse
+
 from django.conf import settings
 from django.core.management.base import BaseCommand
-from django.utils.six.moves.urllib.parse import urlparse
 
 
 class Command(BaseCommand):
 
-    requires_system_checks = False
+    requires_system_checks = []
     can_import_settings = True
 
     def handle(self, *args, **options):
 
         parsed_url = urlparse(settings.CELERY_BROKER_URL)
 
         vhost = parsed_url.path.lstrip('/')
```

### Comparing `django-daiquiri-0.2/daiquiri/core/viewsets.py` & `django-daiquiri-0.4.2/daiquiri/core/viewsets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from rest_framework import mixins, viewsets
+from rest_framework.exceptions import ParseError
 
 from .serializers import ChoicesSerializer
 
-from rest_framework.exceptions import ParseError
-
 
 class ChoicesViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
     serializer_class = ChoicesSerializer
 
 
 class RowViewSetMixin(object):
 
-    def _get_query_params(self, column_names):
+    def _get_query_params(self, columns):
         # get the ordering
         ordering = self.request.GET.get('ordering')
 
         # get the search string
         search = self.request.GET.get('search')
 
         # get the page from the querystring and make sure it is an int
@@ -30,14 +29,20 @@
         try:
             page_size = int(self.request.GET.get('page_size', '30'))
         except ValueError:
             raise ParseError(_('page_size must be an integer'))
 
         # get additional filters from the querystring
         filters = {}
+        try:
+            column_names = [column.name for column in columns]
+        except AttributeError:
+            column_names = [column['name'] for column in columns]
+
+        filters = {}
         for key, value in self.request.GET.items():
             if key in column_names:
                 filters[key] = value
 
         return ordering, page, page_size, search, filters
 
     def _get_next_url(self, page, page_size, count):
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/handlers.py` & `django-daiquiri-0.4.2/daiquiri/auth/handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import logging
 
 from django.conf import settings
 from django.contrib.auth.models import User
 from django.dispatch import receiver
-from django.db.models.signals import post_save, m2m_changed
+from django.db.models.signals import post_save, post_delete, m2m_changed
 
-from allauth.account.signals import email_confirmed
+from allauth.account.signals import email_confirmed, password_changed, password_reset
 
 from .models import Profile
 
 from .signals import (
     user_created,
     user_updated,
+    user_deleted,
     user_groups_updated,
     user_confirmed,
     user_rejected,
     user_activated,
     user_disabled,
     user_enabled
 )
 
 from .utils import (
     send_request_confirmation,
     send_request_activation,
     send_notify_confirmation,
     send_notify_rejection,
     send_notify_activation,
-    send_activation
+    send_activation,
+    send_notify_password_changed,
 )
 
 logger = logging.getLogger(__name__)
 
 
 @receiver(post_save, sender=User)
 def post_save_user(sender, **kwargs):
@@ -47,14 +49,22 @@
 
         elif kwargs['update_fields'] is None:
             # a login triggers this handler with update_fields=last_login
             user_updated.send(sender=User, user=user)
             logger.info('user \'%s\' updated.' % user.username)
 
 
+@receiver(post_delete, sender=User)
+def post_delete_user(sender, **kwargs):
+    if not kwargs.get('raw', False):
+        user = kwargs['instance']
+        user_deleted.send(sender=User, user=user)
+        logger.info('user \'%s\' deleted.' % user.username)
+
+
 @receiver(m2m_changed, sender=User.groups.through)
 def m2m_changed_user(sender, **kwargs):
     if not kwargs.get('raw', False):
         user = kwargs['instance']
 
         # fire the signal only one per change
         if kwargs['action'] in ('post_add', 'post_remove', 'post_clear'):
@@ -138,7 +148,21 @@
     '''
     Gets notified when a user was disabled by a manager.
     '''
     request = kwargs['request']
     user = kwargs['user']
 
     logger.info('user \'%s\' enabled by \'%s\'.' % (user.username, request.user.username))
+
+
+@receiver(password_changed)
+@receiver(password_reset)
+def password_changed_handler(sender, **kwargs):
+    '''
+    Gets notified when a user was disabled by a manager.
+    '''
+    request = kwargs['request']
+    user = kwargs['user']
+
+    logger.info('user \'%s\' changed his/her password.' % user.username)
+    if settings.AUTH_WORKFLOW == 'confirmation':
+        send_notify_password_changed(request, user)
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/adapter.py` & `django-daiquiri-0.4.2/daiquiri/auth/adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 
 from django.conf import settings
-from django.core.urlresolvers import reverse
 from django.http import HttpResponseRedirect
+from django.urls import reverse
 
 from allauth.account.adapter import DefaultAccountAdapter
-from allauth.socialaccount.adapter import DefaultSocialAccountAdapter
 from allauth.exceptions import ImmediateHttpResponse
+from allauth.socialaccount.adapter import DefaultSocialAccountAdapter
 
 logger = logging.getLogger(__name__)
 
 
 class DaiquiriAccountAdapter(DefaultAccountAdapter):
 
     def is_safe_url(self, url):
-        from django.utils.http import is_safe_url
-        return is_safe_url(url, allowed_hosts=settings.ALLOWED_HOSTS)
+        from django.utils.http import url_has_allowed_host_and_scheme
+        return url_has_allowed_host_and_scheme(url, allowed_hosts=settings.ALLOWED_HOSTS)
 
     def save_user(self, request, user, form, commit=True):
         super(DaiquiriAccountAdapter, self).save_user(request, user, form)
 
         if settings.AUTH_WORKFLOW:
             user.save()
             user.profile.is_pending = True
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/serializers.py` & `django-daiquiri-0.4.2/daiquiri/auth/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.contrib.auth.models import User, Group
 
 from rest_framework import serializers
 
 from allauth.account.models import EmailAddress
 
-from daiquiri.core.serializers import JSONField
+from daiquiri.core.serializers import JSONDictField
 
 from .models import Profile
 
 
 class UserSerializer(serializers.ModelSerializer):
 
     class Meta:
@@ -48,29 +48,30 @@
         fields = ('email', 'verified')
 
 
 class ProfileSerializer(serializers.ModelSerializer):
 
     user = UserSerializer()
     emails = serializers.SerializerMethodField(read_only=True)
-    details = JSONField(allow_null=True)
-    attributes = JSONField(allow_null=True, read_only=True)
+    details = JSONDictField(allow_null=True)
+    attributes = JSONDictField(allow_null=True)
 
     class Meta:
         model = Profile
         fields = ('id', 'full_name', 'user', 'is_confirmed', 'is_pending', 'emails', 'details', 'attributes')
 
     def update(self, obj, validated_data):
-        user = validated_data.pop('user')
+        if 'user' in validated_data:
+            user = validated_data.pop('user')
 
-        # update the user for this profile seperately
-        obj.user.first_name = user['first_name']
-        obj.user.last_name = user['last_name']
-        obj.user.groups = user['groups']
-        obj.user.save()
+            # update the user for this profile seperately
+            obj.user.first_name = user['first_name']
+            obj.user.last_name = user['last_name']
+            obj.user.groups.set(user['groups'])
+            obj.user.save()
 
         return super(ProfileSerializer, self).update(obj, validated_data)
 
     def get_emails(self, obj):
         emails = EmailAddress.objects.filter(user=obj.user)
         serializer = EmailAddressSerializer(instance=emails, many=True)
         return serializer.data
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/views.py` & `django-daiquiri-0.4.2/daiquiri/auth/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 
 from django.conf import settings
 from django.contrib.auth.decorators import login_required
-from django.core.urlresolvers import reverse
+from django.urls import reverse
 from daiquiri.core.utils import get_referer_path_info, get_next
 from django.views.generic import TemplateView
 from django.http import HttpResponseRedirect, JsonResponse
 from django.shortcuts import render
 from django.urls import reverse_lazy
-
 from rest_framework.authtoken.models import Token
 
 from allauth.account.views import (
     logout as allauth_logout,
     PasswordChangeView as AllauthPasswordChangeView,
     PasswordSetView as AllauthPasswordSetView
 )
 
-from daiquiri.core.views import ModelPermissionMixin
+from daiquiri.core.views import CSRFViewMixin, ModelPermissionMixin
 
 from .forms import UserForm, ProfileForm
 
 
 @login_required()
 def profile_update(request):
     user_form = UserForm(request.POST or None, instance=request.user)
@@ -63,34 +62,29 @@
         'token': token
     })
 
 
 def logout(request, *args, **kwargs):
     response = allauth_logout(request, *args, **kwargs)
 
-    # delete wordpress cookies
-    for cookie in request.COOKIES:
-        if cookie.startswith('wordpress') or cookie.startswith('wp-settings'):
-            response.delete_cookie(cookie)
-
     return response
 
 
-class UsersView(ModelPermissionMixin, TemplateView):
+class UsersView(ModelPermissionMixin, CSRFViewMixin, TemplateView):
     template_name = 'auth/users.html'
     permission_required = 'daiquiri_auth.view_profile'
 
     def get_context_data(self, **kwargs):
         # get urls to the admin interface to be used with angular
         user_admin_url = reverse('admin:auth_user_change', args=['row.id']).replace('row.id', '{$ row.id $}')
         profile_admin_url = reverse('admin:daiquiri_auth_profile_change', args=['row.id']).replace('row.id', '{$ row.id $}')
 
         detail_keys = settings.AUTH_DETAIL_KEYS
         for detail_key in detail_keys:
-            detail_key['options_json'] = json.dumps(detail_key['options'])
+            detail_key['options_json'] = json.dumps(detail_key.get('options', {}))
             detail_key['model'] = 'service.current_row.details.%s' % detail_key['key']
             detail_key['errors'] = 'service.errors.%s' % detail_key['key']
 
         context = super(UsersView, self).get_context_data(**kwargs)
         context.update({
             'detail_keys': detail_keys,
             'user_admin_url': user_admin_url,
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/migrations/0008_profile_is_pending.py` & `django-daiquiri-0.4.2/daiquiri/auth/migrations/0008_profile_is_pending.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/migrations/0004_view_permission_typo.py` & `django-daiquiri-0.4.2/daiquiri/auth/migrations/0004_view_permission_typo.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/migrations/0005_view_permission_fix.py` & `django-daiquiri-0.4.2/daiquiri/auth/migrations/0005_view_permission_fix.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/migrations/0006_profile_ordering.py` & `django-daiquiri-0.4.2/daiquiri/auth/migrations/0006_profile_ordering.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/migrations/0003_view_permission.py` & `django-daiquiri-0.4.2/daiquiri/auth/migrations/0003_view_permission.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/migrations/0001_profile_model.py` & `django-daiquiri-0.4.2/daiquiri/auth/migrations/0001_profile_model.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/static/auth/js/users.js` & `django-daiquiri-0.4.2/daiquiri/auth/static/auth/js/users.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
     /* get the base url */
 
     var baseurl = angular.element('meta[name="baseurl"]').attr('content');
 
     /* configure resources */
 
     var resources = {
-        profiles: $resource(baseurl + 'auth/api/profiles/:id/:detail_route/'),
+        profiles: $resource(baseurl + 'auth/api/profiles/:id/:detail_action/'),
         groups: $resource(baseurl + 'auth/api/groups/:id/')
     }
 
     /* init the list service */
 
     ListService.init(resources.profiles);
 
@@ -38,15 +38,15 @@
     };
 
     service.store_profile = function(action) {
         service.errors = {};
 
         resources.profiles.update({
             id: service.current_row.id,
-            detail_route: action
+            detail_action: action
         }, service.current_row, function(response) {
             // copy the data back to the rows array and close the modal
             service.list.rows[service.current_index] = response;
 
             $('.modal').modal('hide');
         }, function(result) {
             service.errors = result.data;
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users_options.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_options.html`

 * *Files 25% similar despite different names*

```diff
@@ -15,54 +15,35 @@
         </a>
         <a href="" class="fa fa-check-circle"
             ng-show="!row.user.is_active" title="{% trans 'Enable user' %}"
             ng-click="service.modal('enable-user-modal', $index)">
         </a>
     </span>
 
+    {% if settings.AUTH_WORKFLOW == 'confirmation' %}
+    <span ng-show="row.is_pending && !row.is_confirmed">
+        <a href="" class="fa fa-thumbs-up" title="{% trans 'Confirm the user' %}"
+            ng-click="service.modal('confirm-user-modal', $index)">
+        </a>
+        <a href="" class="fa fa-thumbs-down" title="{% trans 'Reject the user' %}"
+            ng-click="service.modal('reject-user-modal', $index)">
+        </a>
+    </span>
+    {% elif settings.AUTH_WORKFLOW == 'activation' %}
     <span ng-show="row.is_pending">
-        {% if settings.AUTH_WORKFLOW == 'confirmation' %}
-        <span ng-show="!row.is_confirmed">
-            <a href="" class="fa fa-check" title="{% trans 'Confirm the user' %}"
-                ng-click="service.modal('confirm-user-modal', $index)">
-            </a>
-            <a href="" class="fa fa-times" title="{% trans 'Reject the user' %}"
-                ng-click="service.modal('reject-user-modal', $index)">
-            </a>
-        </span>
-        {% endif %}
-
-        {% if settings.AUTH_WORKFLOW == 'activation' %}
         <a href="" class="fa fa-check" title="{% trans 'Activate the user' %}"
             ng-click="service.modal('activate-user-modal', $index)">
         </a>
         <a href="" class="fa fa-times" title="{% trans 'Reject the user' %}"
             ng-click="service.modal('reject-user-modal', $index)">
         </a>
-        {% endif %}
     </span>
+    {% endif %}
 
     {% if user.is_staff %}
-    <div class="dropdown">
-        <a class="dropdown-toggle" type="button" id="users-options"
-            data-toggle="dropdown" aria-haspopup="true" aria-expanded="true"
-            title="{% trans 'Show options' %}">
-            <span class="fa fa-ellipsis-h"></span>
-        </a>
-        <ul class="dropdown-menu dropdown-menu-right" aria-labelledby="users-options">
-            {% if settings.AUTH_WORKFLOW == 'confirmation' %}
-            <li>
-                <a href="" ng-show="row.is_pending && row.is_confirmed" ng-click="service.modal('activate-user-modal', $index)">
-                    {% trans 'Activate the user' %}
-                </a>
-            <li>
-            {% endif %}
-            <li>
-                <a href="{{ user_admin_url }}">{% trans 'User Admin' %}</a>
-            </li>
-            <li>
-                <a href="{{ profile_admin_url }}">{% trans 'Profile Admin' %}</a>
-            </li>
-        </ul>
-    </div>
-
+    {% if settings.AUTH_WORKFLOW == 'confirmation' %}
+    <a href="" class="fa fa-check" ng-show="row.is_pending && row.is_confirmed"
+        ng-click="service.modal('activate-user-modal', $index)"></a>
+    {% endif %}
+    <a href="{{ user_admin_url }}" class="fa fa-user" title="{% trans 'User Admin' %}"></a>
+    <a href="{{ profile_admin_url }}" class="fa fa-user-circle-o" title="{% trans 'Profile Admin' %}"></a>
     {% endif %}
```

#### html2text {}

```diff
@@ -1,9 +1,4 @@
-{% load i18n %} {% load core_tags %}        {% if settings.AUTH_WORKFLOW ==
-'confirmation' %}     {% endif %} {% if settings.AUTH_WORKFLOW == 'activation'
-%}   {% endif %}  {% if user.is_staff %}
-    * {% if settings.AUTH_WORKFLOW == 'confirmation' %}
-    * {% trans 'Activate the user' %}
-    * {% endif %}
-    * {%_trans_'User_Admin'_%}
-    * {%_trans_'Profile_Admin'_%}
-{% endif %}
+{% load i18n %} {% load core_tags %}       {% if settings.AUTH_WORKFLOW ==
+'confirmation' %}     {% elif settings.AUTH_WORKFLOW == 'activation' %}     {%
+endif %} {% if user.is_staff %} {% if settings.AUTH_WORKFLOW == 'confirmation'
+%}  {% endif %}   {% endif %}
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_confirm_user.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_confirm_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_reject_user.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_reject_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_show_user.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_show_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_activate_user.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_activate_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_update_user.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_update_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core/wide.html' %}
-{% load staticfiles %}
+{% load static %}
 {% load i18n %}
 {% load compress %}
-{% load core_tags %}
+{% load vendor_tags %}
 
 {% block bodyargs %}ng-app="users" ng-controller="UsersController"{% endblock %}
 
 {% block headextra %}
     {% vendor 'angular' %}
     {% vendor 'ng-infinite-scroll' %}
 
@@ -59,16 +59,16 @@
 
             <div class="table-responsive">
                 <table class="table daiquiri-list-table" infinite-scroll="service.list.fetch()" infinite-scroll-distance="0.2">
                     <thead>
                         <th style="width: 25%;">{% trans 'Name (Username)' %}</th>
                         <th style="width: 25%;">{% trans 'Email' %}</th>
                         <th style="width: 20%;">{% trans 'Status' %}</th>
-                        <th style="width: 20%;">{% trans 'Groups' %}</th>
-                        <th style="width: 10%;"></th>
+                        <th style="width: 10%;">{% trans 'Groups' %}</th>
+                        <th style="width: 20%;"></th>
                     </thead>
                     <tbody>
                         <tr ng-repeat="row in service.list.rows">
                             <td>
                                 <a href="" ng-click="service.modal('show-user-modal', $index)">
                                     {$ row.full_name $}
                                 </a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends 'core/wide.html' %} {% load staticfiles %} {% load i18n %} {% load
-compress %} {% load core_tags %} {% block bodyargs %}ng-app="users" ng-
+{% extends 'core/wide.html' %} {% load static %} {% load i18n %} {% load
+compress %} {% load vendor_tags %} {% block bodyargs %}ng-app="users" ng-
 controller="UsersController"{% endblock %} {% block headextra %} {% vendor
 'angular' %} {% vendor 'ng-infinite-scroll' %} {% compress css %}
 
  {% endcompress css %} {% compress js %}
  {% endcompress js %} {% endblock %} {% block wide %}
 ****** User management ******
 [                    ]
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_disable_user.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_disable_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/auth/users_modal_enable_user.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_enable_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/signup.html` & `django-daiquiri-0.4.2/daiquiri/contact/templates/contact/contact.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,60 @@
 00000000: 7b25 2065 7874 656e 6473 2027 636f 7265  {% extends 'core
 00000010: 2f70 6167 652e 6874 6d6c 2720 257d 0a7b  /page.html' %}.{
 00000020: 2520 6c6f 6164 2069 3138 6e20 257d 0a0a  % load i18n %}..
 00000030: 7b25 2062 6c6f 636b 2070 6167 6520 257d  {% block page %}
 00000040: 0a0a 2020 2020 3c68 313e 7b25 2074 7261  ..    <h1>{% tra
-00000050: 6e73 2022 4372 6561 7465 2061 206e 6577  ns "Create a new
-00000060: 2061 6363 6f75 6e74 2220 257d 3c2f 6831   account" %}</h1
-00000070: 3e0a 0a20 2020 207b 2520 6966 2073 6574  >..    {% if set
-00000080: 7469 6e67 732e 4155 5448 5f57 4f52 4b46  tings.AUTH_WORKF
-00000090: 4c4f 5720 257d 0a20 2020 203c 703e 0a20  LOW %}.    <p>. 
-000000a0: 2020 2020 2020 207b 2520 7472 616e 7320         {% trans 
-000000b0: 2750 6c65 6173 6520 6e6f 7465 2074 6861  'Please note tha
-000000c0: 7420 6166 7465 7220 7265 6769 7374 7261  t after registra
-000000d0: 7469 6f6e 2c20 796f 7572 2061 6363 6f75  tion, your accou
-000000e0: 6e74 206e 6565 6473 2074 6f20 6265 206d  nt needs to be m
-000000f0: 616e 7561 6c6c 7920 6163 7469 7661 7465  anually activate
-00000100: 6420 6279 2061 6e20 6164 6d69 6e2e 2054  d by an admin. T
-00000110: 6869 7320 6361 6e20 7461 6b65 206f 6e65  his can take one
-00000120: 206f 7220 7477 6f20 6461 7973 2e20 596f   or two days. Yo
-00000130: 7520 7769 6c6c 2072 6563 6569 7665 2061  u will receive a
-00000140: 6e20 656d 6169 6c20 7768 656e 2079 6f75  n email when you
-00000150: 2063 616e 206c 6f67 2069 6e2e 2725 7d0a   can log in.'%}.
-00000160: 2020 2020 3c2f 703e 0a20 2020 207b 2520      </p>.    {% 
-00000170: 656e 6469 6620 257d 0a0a 2020 2020 3c70  endif %}..    <p
-00000180: 3e7b 2520 626c 6f63 6b74 7261 6e73 2025  >{% blocktrans %
-00000190: 7d41 6c72 6561 6479 2068 6176 6520 616e  }Already have an
-000001a0: 2061 6363 6f75 6e74 3f20 5468 656e 2070   account? Then p
-000001b0: 6c65 6173 6520 3c61 2068 7265 663d 227b  lease <a href="{
-000001c0: 7b20 6c6f 6769 6e5f 7572 6c20 7d7d 223e  { login_url }}">
-000001d0: 7369 676e 2069 6e3c 2f61 3e2e 7b25 2065  sign in</a>.{% e
-000001e0: 6e64 626c 6f63 6b74 7261 6e73 2025 7d3c  ndblocktrans %}<
-000001f0: 2f70 3e0a 0a20 2020 203c 666f 726d 206d  /p>..    <form m
-00000200: 6574 686f 643d 2270 6f73 7422 2061 6374  ethod="post" act
-00000210: 696f 6e3d 227b 2520 7572 6c20 2761 6363  ion="{% url 'acc
-00000220: 6f75 6e74 5f73 6967 6e75 7027 2025 7d22  ount_signup' %}"
-00000230: 206e 6f76 616c 6964 6174 653e 0a20 2020   novalidate>.   
-00000240: 2020 2020 207b 2520 6373 7266 5f74 6f6b       {% csrf_tok
-00000250: 656e 2025 7d0a 0a20 2020 2020 2020 207b  en %}..        {
-00000260: 2520 6966 2072 6564 6972 6563 745f 6669  % if redirect_fi
-00000270: 656c 645f 7661 6c75 6520 257d 0a20 2020  eld_value %}.   
-00000280: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
-00000290: 3d22 6869 6464 656e 2220 6e61 6d65 3d22  ="hidden" name="
-000002a0: 7b7b 2072 6564 6972 6563 745f 6669 656c  {{ redirect_fiel
-000002b0: 645f 6e61 6d65 207d 7d22 2076 616c 7565  d_name }}" value
-000002c0: 3d22 7b7b 2072 6564 6972 6563 745f 6669  ="{{ redirect_fi
-000002d0: 656c 645f 7661 6c75 6520 7d7d 2220 2f3e  eld_value }}" />
-000002e0: 0a20 2020 2020 2020 207b 2520 656e 6469  .        {% endi
-000002f0: 6620 257d 0a0a 2020 2020 2020 2020 7b25  f %}..        {%
-00000300: 2069 6e63 6c75 6465 2027 636f 7265 2f70   include 'core/p
-00000310: 6172 7469 616c 732f 666f 726d 5f66 6965  artials/form_fie
-00000320: 6c64 732e 6874 6d6c 2720 257d 0a0a 2020  lds.html' %}..  
-00000330: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-00000340: 653d 2273 7562 6d69 7422 2063 6c61 7373  e="submit" class
-00000350: 3d22 6274 6e20 6274 6e2d 7072 696d 6172  ="btn btn-primar
-00000360: 7922 2076 616c 7565 3d22 7b25 2074 7261  y" value="{% tra
-00000370: 6e73 2027 4372 6561 7465 2061 6363 6f75  ns 'Create accou
-00000380: 6e74 2720 257d 2220 2f3e 0a20 2020 203c  nt' %}" />.    <
-00000390: 2f66 6f72 6d3e 0a0a 2020 2020 3c75 6c20  /form>..    <ul 
-000003a0: 636c 6173 733d 226c 6973 742d 756e 7374  class="list-unst
-000003b0: 796c 6564 2074 6578 742d 6461 6e67 6572  yled text-danger
-000003c0: 223e 0a20 2020 207b 2520 666f 7220 6572  ">.    {% for er
-000003d0: 726f 7220 696e 2066 6f72 6d2e 6e6f 6e5f  ror in form.non_
-000003e0: 6669 656c 645f 6572 726f 7273 2025 7d0a  field_errors %}.
-000003f0: 2020 2020 2020 2020 3c6c 693e 7b7b 2065          <li>{{ e
-00000400: 7272 6f72 207d 7d3c 2f6c 693e 0a20 2020  rror }}</li>.   
-00000410: 207b 2520 656e 6466 6f72 2025 7d0a 2020   {% endfor %}.  
-00000420: 2020 3c2f 756c 3e0a 0a7b 2520 656e 6462    </ul>..{% endb
-00000430: 6c6f 636b 2025 7d0a                      lock %}.
+00000050: 6e73 2022 436f 6e74 6163 7420 466f 726d  ns "Contact Form
+00000060: 2220 257d 3c2f 6831 3e0a 0a20 2020 207b  " %}</h1>..    {
+00000070: 2520 6966 2075 7365 722e 6973 5f61 7574  % if user.is_aut
+00000080: 6865 6e74 6963 6174 6564 2025 7d0a 2020  henticated %}.  
+00000090: 2020 2020 2020 3c70 3e0a 2020 2020 2020        <p>.      
+000000a0: 2020 2020 2020 7b25 2074 7261 6e73 2022        {% trans "
+000000b0: 506c 6561 7365 2065 6e74 6572 2079 6f75  Please enter you
+000000c0: 7220 6d65 7373 6167 652e 2220 257d 0a20  r message." %}. 
+000000d0: 2020 2020 2020 203c 2f70 3e0a 2020 2020         </p>.    
+000000e0: 2020 2020 3c70 3e0a 2020 2020 2020 2020      <p>.        
+000000f0: 2020 2020 7b25 2074 7261 6e73 2022 5468      {% trans "Th
+00000100: 6520 616e 7377 6572 2077 696c 6c20 6265  e answer will be
+00000110: 2073 656e 7420 746f 2022 2025 7d3c 623e   sent to " %}<b>
+00000120: 7b7b 2075 7365 722e 656d 6169 6c20 7d7d  {{ user.email }}
+00000130: 3c2f 623e 0a20 2020 2020 2020 203c 2f70  </b>.        </p
+00000140: 3e0a 0a20 2020 2020 2020 203c 666f 726d  >..        <form
+00000150: 206d 6574 686f 643d 2270 6f73 7422 2061   method="post" a
+00000160: 6374 696f 6e3d 227b 2520 7572 6c20 2763  ction="{% url 'c
+00000170: 6f6e 7461 6374 3a63 6f6e 7461 6374 2720  ontact:contact' 
+00000180: 257d 2220 6e6f 7661 6c69 6461 7465 3e0a  %}" novalidate>.
+00000190: 2020 2020 2020 2020 2020 2020 7b25 2063              {% c
+000001a0: 7372 665f 746f 6b65 6e20 257d 0a20 2020  srf_token %}.   
+000001b0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+000001c0: 7479 7065 3d22 6869 6464 656e 2220 6e61  type="hidden" na
+000001d0: 6d65 3d22 6e65 7874 2220 7661 6c75 653d  me="next" value=
+000001e0: 227b 7b20 6e65 7874 207d 7d22 202f 3e0a  "{{ next }}" />.
+000001f0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00000200: 696e 636c 7564 6520 2763 6f72 652f 7061  include 'core/pa
+00000210: 7274 6961 6c73 2f66 6f72 6d5f 6669 656c  rtials/form_fiel
+00000220: 6473 2e68 746d 6c27 2025 7d0a 0a20 2020  ds.html' %}..   
+00000230: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+00000240: 7479 7065 3d22 7375 626d 6974 2220 7661  type="submit" va
+00000250: 6c75 653d 227b 2520 7472 616e 7320 2753  lue="{% trans 'S
+00000260: 656e 6420 6d65 7373 6167 6527 2025 7d22  end message' %}"
+00000270: 2063 6c61 7373 3d22 6274 6e20 7b7b 2073   class="btn {{ s
+00000280: 7562 6d69 745f 6461 6e67 6572 7c79 6573  ubmit_danger|yes
+00000290: 6e6f 3a27 6274 6e2d 6461 6e67 6572 2c62  no:'btn-danger,b
+000002a0: 746e 2d70 7269 6d61 7279 2720 7d7d 2220  tn-primary' }}" 
+000002b0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+000002c0: 696e 7075 7420 7479 7065 3d22 7375 626d  input type="subm
+000002d0: 6974 2220 6e61 6d65 3d22 6361 6e63 656c  it" name="cancel
+000002e0: 2220 7661 6c75 653d 227b 2520 7472 616e  " value="{% tran
+000002f0: 7320 2743 616e 6365 6c27 2025 7d22 2063  s 'Cancel' %}" c
+00000300: 6c61 7373 3d22 6274 6e20 6274 6e2d 6465  lass="btn btn-de
+00000310: 6661 756c 7422 202f 3e0a 2020 2020 2020  fault" />.      
+00000320: 2020 3c2f 666f 726d 3e0a 2020 2020 7b25    </form>.    {%
+00000330: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
+00000340: 203c 703e 0a20 2020 2020 2020 2020 2020   <p>.           
+00000350: 207b 2520 7472 616e 7320 2250 6c65 6173   {% trans "Pleas
+00000360: 6520 6c6f 6720 696e 2074 6f20 6265 2061  e log in to be a
+00000370: 626c 6520 746f 2066 696c 6c20 7468 6520  ble to fill the 
+00000380: 636f 6e74 6163 7420 666f 726d 2e22 2025  contact form." %
+00000390: 7d0a 2020 2020 2020 2020 3c2f 703e 0a20  }.        </p>. 
+000003a0: 2020 207b 2520 656e 6469 6620 257d 0a0a     {% endif %}..
+000003b0: 7b25 2065 6e64 626c 6f63 6b20 257d 0a    {% endblock %}.
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/login_form.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/login_form.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/verified_email_required.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/password_reset_from_key.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/email/password_reset_key_message.txt` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/password_reset_key_message.txt`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/account_token.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_token.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/password_reset.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/logout.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/email_confirm.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/email.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/account/password_change.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/signup.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_profile.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,71 @@
 00000000: 7b25 2065 7874 656e 6473 2027 636f 7265  {% extends 'core
 00000010: 2f70 6167 652e 6874 6d6c 2720 257d 0a7b  /page.html' %}.{
 00000020: 2520 6c6f 6164 2069 3138 6e20 257d 0a0a  % load i18n %}..
 00000030: 7b25 2062 6c6f 636b 2070 6167 6520 257d  {% block page %}
 00000040: 0a0a 2020 2020 3c68 313e 7b25 2074 7261  ..    <h1>{% tra
-00000050: 6e73 2022 4372 6561 7465 2061 206e 6577  ns "Create a new
-00000060: 2061 6363 6f75 6e74 2220 257d 3c2f 6831   account" %}</h1
-00000070: 3e0a 0a20 2020 203c 703e 0a20 2020 2020  >..    <p>.     
-00000080: 2020 207b 2520 626c 6f63 6b74 7261 6e73     {% blocktrans
-00000090: 2074 7269 6d6d 6564 2077 6974 6820 7072   trimmed with pr
-000000a0: 6f76 6964 6572 5f6e 616d 653d 6163 636f  ovider_name=acco
-000000b0: 756e 742e 6765 745f 7072 6f76 6964 6572  unt.get_provider
-000000c0: 2e6e 616d 6520 7369 7465 5f6e 616d 653d  .name site_name=
-000000d0: 7369 7465 2e6e 616d 6520 257d 0a20 2020  site.name %}.   
-000000e0: 2020 2020 2059 6f75 2061 7265 2061 626f       You are abo
-000000f0: 7574 2074 6f20 7573 6520 796f 7572 203c  ut to use your <
-00000100: 7374 726f 6e67 3e7b 7b70 726f 7669 6465  strong>{{provide
-00000110: 725f 6e61 6d65 7d7d 3c2f 7374 726f 6e67  r_name}}</strong
-00000120: 3e20 6163 636f 756e 7420 746f 206c 6f67  > account to log
-00000130: 696e 2074 6f20 7b7b 7369 7465 5f6e 616d  in to {{site_nam
-00000140: 657d 7d2e 0a20 2020 2020 2020 207b 2520  e}}..        {% 
-00000150: 656e 6462 6c6f 636b 7472 616e 7320 257d  endblocktrans %}
-00000160: 0a20 2020 203c 2f70 3e0a 0a20 2020 207b  .    </p>..    {
-00000170: 2520 6966 2073 6574 7469 6e67 732e 4155  % if settings.AU
-00000180: 5448 5f57 4f52 4b46 4c4f 5720 257d 0a20  TH_WORKFLOW %}. 
-00000190: 2020 203c 703e 0a20 2020 2020 2020 207b     <p>.        {
-000001a0: 2520 7472 616e 7320 2750 6c65 6173 6520  % trans 'Please 
-000001b0: 6e6f 7465 2074 6861 7420 6166 7465 7220  note that after 
-000001c0: 7265 6769 7374 7261 7469 6f6e 2c20 796f  registration, yo
-000001d0: 7572 2061 6363 6f75 6e74 206e 6565 6473  ur account needs
-000001e0: 2074 6f20 6265 206d 616e 7561 6c6c 7920   to be manually 
-000001f0: 6163 7469 7661 7465 6420 6279 2061 6e20  activated by an 
-00000200: 6164 6d69 6e2e 2054 6869 7320 6361 6e20  admin. This can 
-00000210: 7461 6b65 206f 6e65 206f 7220 7477 6f20  take one or two 
-00000220: 6461 7973 2e20 596f 7520 7769 6c6c 2072  days. You will r
-00000230: 6563 6569 7665 2061 6e20 656d 6169 6c20  eceive an email 
-00000240: 7768 656e 2079 6f75 2063 616e 206c 6f67  when you can log
-00000250: 2069 6e2e 2725 7d0a 2020 2020 3c2f 703e   in.'%}.    </p>
-00000260: 0a20 2020 207b 2520 656e 6469 6620 257d  .    {% endif %}
-00000270: 0a0a 2020 2020 3c66 6f72 6d20 6d65 7468  ..    <form meth
-00000280: 6f64 3d22 706f 7374 2220 6163 7469 6f6e  od="post" action
-00000290: 3d22 7b25 2075 726c 2027 736f 6369 616c  ="{% url 'social
-000002a0: 6163 636f 756e 745f 7369 676e 7570 2720  account_signup' 
-000002b0: 257d 2220 6e6f 7661 6c69 6461 7465 3e0a  %}" novalidate>.
-000002c0: 2020 2020 2020 2020 7b25 2063 7372 665f          {% csrf_
-000002d0: 746f 6b65 6e20 257d 0a0a 2020 2020 2020  token %}..      
-000002e0: 2020 7b25 2069 6620 7265 6469 7265 6374    {% if redirect
-000002f0: 5f66 6965 6c64 5f76 616c 7565 2025 7d0a  _field_value %}.
-00000300: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
-00000310: 7970 653d 2268 6964 6465 6e22 206e 616d  ype="hidden" nam
-00000320: 653d 227b 7b20 7265 6469 7265 6374 5f66  e="{{ redirect_f
-00000330: 6965 6c64 5f6e 616d 6520 7d7d 2220 7661  ield_name }}" va
-00000340: 6c75 653d 227b 7b20 7265 6469 7265 6374  lue="{{ redirect
-00000350: 5f66 6965 6c64 5f76 616c 7565 207d 7d22  _field_value }}"
-00000360: 202f 3e0a 2020 2020 2020 2020 7b25 2065   />.        {% e
-00000370: 6e64 6966 2025 7d0a 0a20 2020 2020 2020  ndif %}..       
-00000380: 207b 2520 696e 636c 7564 6520 2763 6f72   {% include 'cor
-00000390: 652f 7061 7274 6961 6c73 2f66 6f72 6d5f  e/partials/form_
-000003a0: 6669 656c 6473 2e68 746d 6c27 2025 7d0a  fields.html' %}.
-000003b0: 0a20 2020 2020 2020 203c 696e 7075 7420  .        <input 
-000003c0: 7479 7065 3d22 7375 626d 6974 2220 636c  type="submit" cl
-000003d0: 6173 733d 2262 746e 2062 746e 2d70 7269  ass="btn btn-pri
-000003e0: 6d61 7279 2220 7661 6c75 653d 227b 2520  mary" value="{% 
-000003f0: 7472 616e 7320 2743 7265 6174 6520 6163  trans 'Create ac
-00000400: 636f 756e 7427 2025 7d22 202f 3e0a 2020  count' %}" />.  
-00000410: 2020 3c2f 666f 726d 3e0a 0a20 2020 203c    </form>..    <
-00000420: 756c 2063 6c61 7373 3d22 6c69 7374 2d75  ul class="list-u
-00000430: 6e73 7479 6c65 6420 7465 7874 2d64 616e  nstyled text-dan
-00000440: 6765 7222 3e0a 2020 2020 7b25 2066 6f72  ger">.    {% for
-00000450: 2065 7272 6f72 2069 6e20 666f 726d 2e6e   error in form.n
-00000460: 6f6e 5f66 6965 6c64 5f65 7272 6f72 7320  on_field_errors 
-00000470: 257d 0a20 2020 2020 2020 203c 6c69 3e7b  %}.        <li>{
-00000480: 7b20 6572 726f 7220 7d7d 3c2f 6c69 3e0a  { error }}</li>.
-00000490: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
-000004a0: 0a20 2020 203c 2f75 6c3e 0a0a 7b25 2065  .    </ul>..{% e
-000004b0: 6e64 626c 6f63 6b20 257d 0a              ndblock %}.
+00000050: 6e73 2022 5570 6461 7465 2070 726f 6669  ns "Update profi
+00000060: 6c65 2220 257d 3c2f 6831 3e0a 0a20 2020  le" %}</h1>..   
+00000070: 203c 703e 0a20 2020 2020 2020 207b 2520   <p>.        {% 
+00000080: 7572 6c20 2761 6363 6f75 6e74 5f63 6861  url 'account_cha
+00000090: 6e67 655f 7061 7373 776f 7264 2720 6173  nge_password' as
+000000a0: 2070 6173 7377 6f72 645f 7572 6c20 257d   password_url %}
+000000b0: 0a20 2020 2020 2020 207b 2520 7572 6c20  .        {% url 
+000000c0: 2761 6363 6f75 6e74 5f65 6d61 696c 2720  'account_email' 
+000000d0: 6173 2065 6d61 696c 5f75 726c 2025 7d0a  as email_url %}.
+000000e0: 2020 2020 2020 2020 7b25 2062 6c6f 636b          {% block
+000000f0: 7472 616e 7320 7472 696d 6d65 6420 257d  trans trimmed %}
+00000100: 0a20 2020 2020 2020 2050 6c65 6173 6520  .        Please 
+00000110: 656e 7465 7220 796f 7572 2075 7064 6174  enter your updat
+00000120: 6564 2061 6363 6f75 6e74 2069 6e66 6f72  ed account infor
+00000130: 6d61 7469 6f6e 2e20 596f 7520 6361 6e20  mation. You can 
+00000140: 6368 616e 6765 2079 6f75 7220 7061 7373  change your pass
+00000150: 776f 7264 0a20 2020 2020 2020 2075 7369  word.        usi
+00000160: 6e67 2074 6865 203c 6120 6872 6566 3d22  ng the <a href="
+00000170: 7b7b 2070 6173 7377 6f72 645f 7572 6c20  {{ password_url 
+00000180: 7d7d 223e 7061 7373 776f 7264 2066 6f72  }}">password for
+00000190: 6d3c 2f61 3e20 616e 6420 7570 6461 7465  m</a> and update
+000001a0: 0a20 2020 2020 2020 2079 6f75 7220 652d  .        your e-
+000001b0: 6d61 696c 2075 7369 6e67 2074 6865 203c  mail using the <
+000001c0: 6120 6872 6566 3d22 7b7b 2065 6d61 696c  a href="{{ email
+000001d0: 5f75 726c 207d 7d22 3e65 2d6d 6169 6c20  _url }}">e-mail 
+000001e0: 666f 726d 3c2f 613e 2e0a 2020 2020 2020  form</a>..      
+000001f0: 2020 7b25 2065 6e64 626c 6f63 6b74 7261    {% endblocktra
+00000200: 6e73 2025 7d0a 2020 2020 3c2f 703e 0a0a  ns %}.    </p>..
+00000210: 2020 2020 3c66 6f72 6d20 6d65 7468 6f64      <form method
+00000220: 3d22 706f 7374 2220 6163 7469 6f6e 3d22  ="post" action="
+00000230: 7b25 2075 726c 2027 6163 636f 756e 745f  {% url 'account_
+00000240: 7072 6f66 696c 6527 2025 7d22 206e 6f76  profile' %}" nov
+00000250: 616c 6964 6174 653e 0a20 2020 2020 2020  alidate>.       
+00000260: 207b 2520 6373 7266 5f74 6f6b 656e 2025   {% csrf_token %
+00000270: 7d0a 2020 2020 2020 2020 3c69 6e70 7574  }.        <input
+00000280: 2074 7970 653d 2268 6964 6465 6e22 206e   type="hidden" n
+00000290: 616d 653d 226e 6578 7422 2076 616c 7565  ame="next" value
+000002a0: 3d22 7b7b 206e 6578 7420 7d7d 2220 2f3e  ="{{ next }}" />
+000002b0: 0a0a 2020 2020 2020 2020 3c70 3e3c 623e  ..        <p><b>
+000002c0: 5573 6572 6e61 6d65 3a20 7b7b 2072 6571  Username: {{ req
+000002d0: 7565 7374 2e75 7365 722e 7573 6572 6e61  uest.user.userna
+000002e0: 6d65 207d 7d3c 2f62 3e3c 2f70 3e0a 2020  me }}</b></p>.  
+000002f0: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
+00000300: 2027 636f 7265 2f70 6172 7469 616c 732f   'core/partials/
+00000310: 666f 726d 5f66 6965 6c64 732e 6874 6d6c  form_fields.html
+00000320: 2720 7769 7468 2066 6f72 6d3d 7573 6572  ' with form=user
+00000330: 5f66 6f72 6d20 257d 0a20 2020 2020 2020  _form %}.       
+00000340: 207b 2520 696e 636c 7564 6520 2763 6f72   {% include 'cor
+00000350: 652f 7061 7274 6961 6c73 2f66 6f72 6d5f  e/partials/form_
+00000360: 6669 656c 6473 2e68 746d 6c27 2077 6974  fields.html' wit
+00000370: 6820 666f 726d 3d70 726f 6669 6c65 5f66  h form=profile_f
+00000380: 6f72 6d20 257d 0a0a 2020 2020 2020 2020  orm %}..        
+00000390: 3c69 6e70 7574 2074 7970 653d 2273 7562  <input type="sub
+000003a0: 6d69 7422 2076 616c 7565 3d22 7b25 2074  mit" value="{% t
+000003b0: 7261 6e73 2027 5570 6461 7465 2070 726f  rans 'Update pro
+000003c0: 6669 6c65 2720 257d 2220 636c 6173 733d  file' %}" class=
+000003d0: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
+000003e0: 2220 2f3e 0a20 2020 2020 2020 203c 696e  " />.        <in
+000003f0: 7075 7420 7479 7065 3d22 7375 626d 6974  put type="submit
+00000400: 2220 6e61 6d65 3d22 6361 6e63 656c 2220  " name="cancel" 
+00000410: 7661 6c75 653d 227b 2520 7472 616e 7320  value="{% trans 
+00000420: 2743 616e 6365 6c27 2025 7d22 2063 6c61  'Cancel' %}" cla
+00000430: 7373 3d22 6274 6e20 6274 6e2d 6465 6661  ss="btn btn-defa
+00000440: 756c 7422 202f 3e0a 2020 2020 3c2f 666f  ult" />.    </fo
+00000450: 726d 3e0a 0a7b 2520 656e 6462 6c6f 636b  rm>..{% endblock
+00000460: 2025 7d0a                                 %}.
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/snippets/provider_list.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/snippets/provider_list.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% load socialaccount %}
-{% load staticfiles %}
+{% load static %}
 
 {% get_providers as socialaccount_providers %}
 
 {% for provider in socialaccount_providers %}
 
 {% if provider.id == "openid" %}
 {% for brand in provider.get_brands %}
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/templates/socialaccount/connections.html` & `django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/auth/models.py` & `django-daiquiri-0.4.2/daiquiri/auth/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-from __future__ import unicode_literals
-
 import logging
 
 from django.contrib.auth.models import User
 from django.db import models
-from django.utils.encoding import python_2_unicode_compatible
-from django.utils.translation import ugettext_lazy as _
-
-from jsonfield import JSONField
+from django.utils.translation import gettext_lazy as _
 
+from .signals import (user_activated, user_confirmed, user_disabled,
+                      user_enabled, user_rejected)
 from .utils import get_full_name
-from .signals import (
-    user_confirmed,
-    user_rejected,
-    user_activated,
-    user_disabled,
-    user_enabled
-)
 
 logger = logging.getLogger(__name__)
 
 
-@python_2_unicode_compatible
 class Profile(models.Model):
 
-    user = models.OneToOneField(User)
-    is_pending = models.BooleanField(default=False)
-    is_confirmed = models.BooleanField(default=False)
-    details = JSONField(null=True, blank=True)
-    attributes = JSONField(null=True, blank=True)
+    user = models.OneToOneField(User, on_delete=models.CASCADE)
+
+    is_pending = models.BooleanField(
+        default=False,
+        help_text='Designates whether the user waiting on confirmation by a manager.')
+    is_confirmed = models.BooleanField(
+        default=False,
+        help_text='Designates whether the user was confirmed by a manager.')
+    details = models.JSONField(null=True, blank=True)
+    attributes = models.JSONField(null=True, blank=True)
+    consent = models.BooleanField(
+        default=False,
+        help_text='Designates whether the user has agreed to the terms of use.',
+        verbose_name='Consent'
+    )
 
     class Meta:
         ordering = ('user__last_name', 'user__last_name', 'user__username')
 
         verbose_name = _('Profile')
         verbose_name_plural = _('Profiles')
 
-        permissions = (('view_profile', 'Can view Profile'),)
-
     def __str__(self):
         return self.user.username
 
     @property
     def full_name(self):
         return get_full_name(self.user)
 
@@ -50,32 +47,30 @@
         self.save()
 
         user_confirmed.send(sender=self.__class__, request=request, user=self.user)
 
     def reject(self, request):
         self.is_pending = False
         self.user.is_active = False
+        self.user.save(update_fields=['is_active'])
         self.save()
 
         user_rejected.send(sender=self.__class__, request=request, user=self.user)
 
-
     def activate(self, request):
         self.is_confirmed = True
         self.is_pending = False
         self.save()
 
         user_activated.send(sender=self.__class__, request=request, user=self.user)
 
-
     def disable(self, request):
         self.user.is_active = False
         self.user.save(update_fields=['is_active'])
 
         user_disabled.send(sender=self.__class__, request=request, user=self.user)
 
-
     def enable(self, request):
         self.user.is_active = True
         self.user.save(update_fields=['is_active'])
 
         user_enabled.send(sender=self.__class__, request=request, user=self.user)
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/urls_accounts.py` & `django-daiquiri-0.4.2/daiquiri/auth/urls_accounts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from django.conf.urls import url, include
+from django.urls import include, re_path
 from django.views.generic import TemplateView
 
 from .views import profile_update, profile_json, token, logout, password_change, password_set
 
 
 urlpatterns = [
-    url(r'^profile/$', profile_update, name='account_profile'),
-    url(r'^profile.json/$', profile_json, name='account_profile_json'),
-    url(r'^token/$', token, name='account_token'),
-    url(r'^pending/$', TemplateView.as_view(template_name='account/account_pending.html'), name='account_pending'),
+    re_path(r'^profile/$', profile_update, name='account_profile'),
+    re_path(r'^profile.json/$', profile_json, name='account_profile_json'),
+    re_path(r'^token/$', token, name='account_token'),
+    re_path(r'^pending/$', TemplateView.as_view(template_name='account/account_pending.html'), name='account_pending'),
 
-    # override login by allauth to remove wordpress cookies
-    url(r"^logout/$", logout, name="account_logout"),
+    re_path(r"^logout/$", logout, name="account_logout"),
 
     # include allauth patterns
-    url(r'^password/change/$', password_change, name='account_change_password'),
-    url(r'^password/change/done/$', TemplateView.as_view(template_name='account/password_change_done.html'), name='account_change_password_done'),
-    url(r'^password/set/$', password_set, name='account_password_set'),
-    url(r'^', include('allauth.urls')),
+    re_path(r'^password/change/$', password_change, name='account_change_password'),
+    re_path(r'^password/change/done/$', TemplateView.as_view(template_name='account/password_change_done.html'), name='account_change_password_done'),
+    re_path(r'^password/set/$', password_set, name='account_password_set'),
+    re_path(r'^', include('allauth.urls')),
 ]
```

### Comparing `django-daiquiri-0.2/daiquiri/auth/viewsets.py` & `django-daiquiri-0.4.2/daiquiri/auth/viewsets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 from django.conf import settings
 from django.contrib.auth.models import Group
 from django.shortcuts import get_object_or_404
 
 from rest_framework import viewsets, mixins, filters
-from rest_framework.decorators import detail_route
+from rest_framework.decorators import action
 from rest_framework.exceptions import MethodNotAllowed
 from rest_framework.response import Response
 from rest_framework.authentication import SessionAuthentication, TokenAuthentication
 
 from daiquiri.core.permissions import HasModelPermission
 from daiquiri.core.paginations import ListPagination
 
 from .models import Profile
 from .serializers import ProfileSerializer, GroupSerializer
+from .permissions import IsAuthManager
 
 
 class ProfileViewSet(mixins.UpdateModelMixin, mixins.ListModelMixin, mixins.RetrieveModelMixin, viewsets.GenericViewSet):
     permission_classes = (HasModelPermission, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
 
     queryset = Profile.objects.all()
     serializer_class = ProfileSerializer
     pagination_class = ListPagination
 
     filter_backends = (filters.SearchFilter, filters.OrderingFilter)
     ordering_fields = ('user__username', 'user__email', 'user__first_name', 'user__last_name')
     search_fields = ('user__username', 'user__email', 'user__first_name', 'user__last_name')
 
-    @detail_route(methods=['put'], permission_classes=[HasModelPermission])
+    @action(detail=True, methods=['put'], permission_classes=[HasModelPermission])
     def confirm(self, request, pk=None):
         if not settings.AUTH_WORKFLOW:
             raise MethodNotAllowed('put')
 
         profile = get_object_or_404(Profile, pk=pk)
         profile.confirm(request)
         return Response(self.get_serializer(profile).data)
 
-    @detail_route(methods=['put'], permission_classes=[HasModelPermission])
+    @action(detail=True, methods=['put'], permission_classes=[HasModelPermission])
     def reject(self, request, pk=None):
         if not settings.AUTH_WORKFLOW:
             raise MethodNotAllowed('put')
 
         profile = get_object_or_404(Profile, pk=pk)
         profile.reject(request)
         return Response(self.get_serializer(profile).data)
 
-    @detail_route(methods=['put'], permission_classes=[HasModelPermission])
+    @action(detail=True, methods=['put'], permission_classes=[HasModelPermission])
     def activate(self, request, pk=None):
         if not settings.AUTH_WORKFLOW:
             raise MethodNotAllowed('put')
 
         profile = get_object_or_404(Profile, pk=pk)
         profile.activate(request)
         return Response(self.get_serializer(profile).data)
 
-    @detail_route(methods=['put'], permission_classes=[HasModelPermission])
+    @action(detail=True, methods=['put'], permission_classes=[HasModelPermission])
     def disable(self, request, pk=None):
         profile = get_object_or_404(Profile, pk=pk)
         profile.disable(request)
         return Response(self.get_serializer(profile).data)
 
-    @detail_route(methods=['put'], permission_classes=[HasModelPermission])
+    @action(detail=True, methods=['put'], permission_classes=[HasModelPermission])
     def enable(self, request, pk=None):
         profile = get_object_or_404(Profile, pk=pk)
         profile.enable(request)
         return Response(self.get_serializer(profile).data)
 
 
 class GroupViewSet(viewsets.ReadOnlyModelViewSet):
-    permission_classes = (HasModelPermission, )
+    permission_classes = (IsAuthManager, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
 
-    queryset = Group.objects.all()
+    queryset = Group.objects.order_by('name')
     serializer_class = GroupSerializer
```

### Comparing `django-daiquiri-0.2/daiquiri/archive/migrations/0001_initial.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0015_queryarchivejob.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # -*- coding: utf-8 -*-
-# Generated by Django 1.11.4 on 2017-12-12 11:20
+# Generated by Django 1.11.9 on 2018-01-10 14:18
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 import jsonfield.fields
 
 
 class Migration(migrations.Migration):
 
-    initial = True
-
     dependencies = [
         ('daiquiri_jobs', '0012_meta'),
+        ('daiquiri_query', '0014_downloadjob'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='ArchiveJob',
+            name='QueryArchiveJob',
             fields=[
                 ('job_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='daiquiri_jobs.Job')),
-                ('data', jsonfield.fields.JSONField(help_text='Input data for archive creation.', verbose_name='Data')),
+                ('column_name', models.CharField(help_text='Column name for this download.', max_length=32, verbose_name='Column name')),
                 ('files', jsonfield.fields.JSONField(help_text='List of files in the archive.', verbose_name='Files')),
-                ('file_path', models.CharField(help_text='Path to the archive file.', max_length=256, verbose_name='Path')),
+                ('job', models.ForeignKey(help_text='QueryJob this ArchiveJob belongs to.', on_delete=django.db.models.deletion.CASCADE, related_name='archives', to='daiquiri_query.QueryJob', verbose_name='QueryJob')),
             ],
             options={
                 'ordering': ('start_time',),
-                'verbose_name': 'ArchiveJob',
-                'verbose_name_plural': 'ArchiveJobs',
-                'permissions': (('view_archivejob', 'Can view ArchiveJob'),),
+                'verbose_name': 'QueryArchiveJob',
+                'verbose_name_plural': 'QueryArchiveJob',
+                'permissions': (('view_queryarchivejob', 'Can view QueryArchiveJob'),),
             },
             bases=('daiquiri_jobs.job',),
         ),
+        migrations.RemoveField(
+            model_name='downloadjob',
+            name='file_path',
+        ),
     ]
```

### Comparing `django-daiquiri-0.2/daiquiri/archive/migrations/0002_collection.py` & `django-daiquiri-0.4.2/daiquiri/files/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
-# Generated by Django 1.11.4 on 2017-12-12 13:31
+# Generated by Django 1.11.4 on 2017-09-14 12:48
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
+    initial = True
+
     dependencies = [
         ('auth', '0008_alter_user_username_max_length'),
-        ('daiquiri_archive', '0001_initial'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='Collection',
+            name='Directory',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(help_text='Name of the collection.', max_length=32, verbose_name='Name')),
+                ('path', models.CharField(help_text='Path of the directory.', max_length=256, verbose_name='Path')),
                 ('access_level', models.CharField(choices=[(b'PRIVATE', 'Private - access must be granted by group'), (b'INTERNAL', 'Internal - logged in users can access'), (b'PUBLIC', 'Public - anonymous visitors can access')], max_length=8, verbose_name='Access level')),
                 ('groups', models.ManyToManyField(blank=True, help_text='The groups which have access to this function.', to='auth.Group', verbose_name='Groups')),
             ],
             options={
-                'ordering': ('name',),
-                'verbose_name': 'Collection',
-                'verbose_name_plural': 'Collections',
-                'permissions': (('view_collection', 'Can view Collection'),),
+                'ordering': ('path',),
+                'verbose_name': 'Directory',
+                'verbose_name_plural': 'Directory',
+                'permissions': (('view_function', 'Can view Directory'),),
             },
         ),
     ]
```

### Comparing `django-daiquiri-0.2/daiquiri/archive/static/archive/js/archive.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/download.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,97 +1,86 @@
-var app = angular.module('archive', ['core']);
-
-app.factory('ArchiveService', ['$http', 'TableService', 'PollingService', function($http, TableService, PollingService) {
+app.factory('DownloadService', ['$http', '$resource', '$injector', 'PollingService', function($http, $resource, $injector, PollingService) {
 
     /* get the base url */
 
     var baseurl = angular.element('meta[name="baseurl"]').attr('content');
 
     /* configure resources */
 
-    var archive_url = baseurl + 'archive/api/archives/'
-
-    /* create the messages service */
-
-    var service = {
-        table: TableService
+    var resources = {
+        downloads: $resource(baseurl + 'query/api/downloads/')
     };
 
-    service.init = function() {
+    /* configure urls */
 
-    };
+    var base_download_url = baseurl + 'query/api/jobs/';
 
-    service.get_id = function(row, column_index) {
-        return row[0];
-    }
-
-    service.get_file_url = function(row, column_index) {
-        return service.table.files_url + row[0];
-    }
+    var service = {
+        pending_downloads: 0
+    };
 
-    service.download_checked = function() {
-        var file_ids = [];
-        angular.forEach(service.table.checked, function(value, key) {
-            if (value) {
-                file_ids.push(key);
-            }
-        })
+    service.init = function(opt) {
+        service.job = opt.job;
 
-        if (file_ids.length) {
-            service.start_download({
-                file_ids: file_ids
+        // inject download services
+        resources.downloads.query(function(response) {
+            angular.forEach(response, function(download) {
+                if (download.download_service) {
+                    service[download.key] = $injector.get(download.download_service);
+                    service[download.key].init(download.options);
+                }
             });
-        }
-    }
-
-    service.download_all = function() {
-        service.download_failed = false;
-
-        service.start_download({
-            search: service.table.params.search
         });
     }
 
-    service.start_download = function(data) {
-        service.download_failed = false;
+    service.start_download = function(download_key, params) {
+        service.job.download_failed = false;
 
-        $http.post(archive_url, data).then(function(result) {
-            var download_id = result.data.id;
+        var url = base_download_url + service.job.id + '/download/' + download_key + '/';
+        $http.post(url, params).then(function(result) {
+            var download_job_id = result.data.id;
 
             service.pending_downloads++;
-            PollingService.register(download_id, service.poll_download, {
-                download_id: download_id
+            PollingService.register(download_job_id, service.poll_download, {
+                download_key: download_key,
+                job: service.job,
+                download_job_id: download_job_id
             });
         }, function() {
             // display error message
-            service.download_failed = true;
+            service.job.download_failed = true;
         });
-    }
+    };
 
     service.poll_download = function(options) {
-        var url = archive_url + options.download_id + '/';
+        var url = base_download_url + options.job.id + '/download/' + options.download_key + '/' + options.download_job_id + '/';
         $http.get(url + '?download=').then(function(result) {
             if (result.data == 'COMPLETED') {
                 service.pending_downloads--;
-                PollingService.unregister(options.download_id);
+                PollingService.unregister(options.download_job_id);
 
-                // download the file, headers will prevent the browser reloading the page
-                window.location.href = url;
+                // download the file using an iframe
+                var iframe = document.createElement('iframe');
+                iframe.style.display = 'none';
+                iframe.src = url;
+                iframe.onload = function() {
+                    this.parentNode.removeChild(this)
+                }
+                document.body.appendChild(iframe)
+            } else if (result.data == 'ERROR') {
+                service.pending_downloads--;
+                PollingService.unregister(options.download_job_id);
+
+                // display error message
+                options.job.download_failed = true;
             }
         }, function() {
             service.pending_downloads--;
-            PollingService.unregister(options.download_id);
+            PollingService.unregister(options.download_job_id);
 
             // display error message
-            service.download_failed = true;
+            options.job.download_failed = true;
         });
     };
 
     return service;
-}]);
-
-app.controller('ArchiveController', ['$scope', 'ArchiveService', function($scope, ArchiveService) {
-
-    $scope.service = ArchiveService;
-    $scope.service.init();
-
 }]);
```

### Comparing `django-daiquiri-0.2/daiquiri/tap/serializers.py` & `django-daiquiri-0.4.2/daiquiri/metadata/serializers/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,87 @@
 from django.conf import settings
 
 from rest_framework import serializers
 
-from daiquiri.metadata.models import Schema, Table, Column
+from ..models import Schema, Table, Column, Function
 
 
 class ColumnSerializer(serializers.ModelSerializer):
 
     class Meta:
         model = Column
         fields = (
+            'id',
+            'order',
             'name',
-            'datatype',
-            'ucd',
+            'query_strings',
+            'description',
             'unit',
-            'indexed',
+            'ucd',
+            'utype',
+            'datatype',
+            'arraysize',
             'principal',
+            'indexed',
             'std'
         )
 
 
-
-
 class TableSerializer(serializers.ModelSerializer):
 
     columns = serializers.SerializerMethodField()
 
     class Meta:
         model = Table
         fields = (
+            'id',
+            'order',
             'name',
+            'query_strings',
             'description',
-            'columns',
-            'doi',
-            'nrows'
+            'type',
+            'utype',
+            'columns'
         )
 
     def get_columns(self, obj):
         # filter the columns which are published for the groups of the user
-        if settings.METADATA_COLUMN_PERMISSIONS:
-            queryset = obj.columns.filter_by_access_level(self.context['request'].user)
-        else:
+        if not settings.METADATA_COLUMN_PERMISSIONS:
             queryset = obj.columns.all()
-
+        else:
+            queryset = obj.columns.filter_by_access_level(self.context['request'].user)
         return ColumnSerializer(queryset, context=self.context, many=True).data
 
 
 class SchemaSerializer(serializers.ModelSerializer):
 
     tables = serializers.SerializerMethodField()
 
     class Meta:
         model = Schema
         fields = (
+            'id',
+            'order',
             'name',
+            'query_strings',
             'description',
+            'utype',
             'tables'
         )
 
     def get_tables(self, obj):
         # filter the tables which are published for the groups of the user
         queryset = obj.tables.filter_by_access_level(self.context['request'].user)
         return TableSerializer(queryset, context=self.context, many=True).data
+
+
+class FunctionSerializer(serializers.ModelSerializer):
+
+    class Meta:
+        model = Function
+        fields = (
+            'id',
+            'order',
+            'name',
+            'description',
+            'query_string'
+        )
```

### Comparing `django-daiquiri-0.2/daiquiri/tap/utils.py` & `django-daiquiri-0.4.2/daiquiri/tap/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,36 +19,41 @@
 
 
 def update_schema(schema):
     '''
     Update or create the schema in the TAP_SCHEMA.
     '''
     if check_tap_visibility(schema):
-        try:
-            tap_schema = TapSchema.objects.get(pk=schema.id)
-        except TapSchema.DoesNotExist:
-            tap_schema = TapSchema.objects.create(pk=schema.id)
+        tap_schema, created = TapSchema.objects.get_or_create(pk=schema.id)
 
         tap_schema.schema_name = schema.name
         tap_schema.utype = None
         if schema.description:
             tap_schema.description = schema.description[:255]
         tap_schema.save()
 
+        if created:
+            # call the handler for each table of the schema
+            for table in schema.tables.all():
+                update_table(table)
+
     else:
         # remove the schema from the TAP_SCHEMA (if it exists)
         try:
-            TapSchema.objects.get(pk=schema.id).delete()
+            tap_schema = TapSchema.objects.get(pk=schema.id)
+            tap_schema.delete()
+
+            # remove tables and colums
+            for tap_table in tap_schema.tables.all():
+                tap_table.columns.all().delete()
+                tap_table.delete()
+
         except TapSchema.DoesNotExist:
             pass
 
-    # call the handler for each table of the schema
-    for table in schema.tables.all():
-        update_table(table)
-
 
 def delete_schema(schema):
     '''
     Remove the schema from the TAP_SCHEMA (if it exists).
     '''
     try:
         TapSchema.objects.get(pk=schema.id).delete()
@@ -64,41 +69,41 @@
     # get the schema from the TAP_SCHEMA
     try:
         tap_schema = TapSchema.objects.get(pk=table.schema.id)
     except TapSchema.DoesNotExist:
         tap_schema = None
 
     if check_tap_visibility(table) and tap_schema:
-        try:
-            tap_table = TapTable.objects.get(pk=table.id)
-            tap_table.schema = tap_schema
-        except TapTable.DoesNotExist:
-            tap_table = TapTable.objects.create(pk=table.id, schema=tap_schema)
+        tap_table, created = TapTable.objects.get_or_create(pk=table.id, defaults={'schema': tap_schema})
 
         tap_table.schema_name = str(table.schema)
-        tap_table.table_name = table.name
+        tap_table.table_name = str(table.schema) + '.' + str(table.name)
         tap_table.table_type = table.type
         tap_table.utype = table.utype
         if table.description:
             tap_table.description = table.description[:255]
         tap_table.table_index = table.order
-
         tap_table.save()
 
+        if created:
+            # call the handler for each table of the schema
+            for column in table.columns.all():
+                update_column(column)
+
     else:
         # remove the table from the TAP_SCHEMA (if it exists)
         try:
-            TapTable.objects.get(pk=table.id).delete()
+            tap_table = TapTable.objects.get(pk=table.id)
+            tap_table.delete()
+
+            # remove columns
+            tap_table.columns.all().delete()
         except TapTable.DoesNotExist:
             pass
 
-    # call the handler for each column of the table
-    for column in table.columns.all():
-        update_column(column)
-
 
 def delete_table(table):
     '''
     Remove the table from the TAP_SCHEMA (if it exists).
     '''
     try:
         TapTable.objects.get(pk=table.id).delete()
```

### Comparing `django-daiquiri-0.2/daiquiri/tap/views.py` & `django-daiquiri-0.4.2/daiquiri/tap/vo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,117 @@
 from django.conf import settings
-from django.http import HttpResponse
-from django.shortcuts import render
 from django.urls import reverse
 
+from daiquiri.core.constants import ACCESS_LEVEL_PUBLIC
+from daiquiri.core.vo import get_curation
 from daiquiri.metadata.models import Schema
-from daiquiri.query.models import Example
 
 from .serializers import SchemaSerializer
-from .renderers import (
-    AvailabilityRenderer,
-    CapabilitiesRenderer,
-    TablesetRenderer
-)
 
 
-def examples(request):
-    return render(request, 'tap/examples.html', {
-        'examples': Example.objects.filter_by_access_level(request.user)
-    })
+def get_resource():
+    return {
+        'service': 'tap',
+        'identifier': 'ivo://%s/tap' % settings.SITE_IDENTIFIER,
+        'title': '%s TAP Service' % settings.SITE_TITLE,
+        'curation': get_curation(),
+        'content': {
+            'subjects': settings.TAP_SUBJECTS,
+            'type': 'Catalog',
+            'description': 'The TAP Service registry for %s.' % settings.SITE_IDENTIFIER,
+            'referenceURL': settings.SITE_URL.rstrip('/') + reverse('tap:root').rstrip('/')
+        },
+        'capabilities': get_capabilities(),
+        'tableset': get_tableset(),
+        'created': settings.SITE_CREATED,
+        'updated': settings.SITE_UPDATED,
+        'type': 'vs:CatalogResource',
+        'status': 'active'
+    }
 
 
-def availability(request):
-    data = {
+def get_availability():
+    return {
         'available': 'true',
         'note': 'service is accepting queries'
     }
-    return HttpResponse(AvailabilityRenderer().render(data), content_type="application/xml")
 
 
-def capabilities(request):
-    data = [
+def get_capabilities():
+    return [
         {
-            'schemaID': 'ivo://ivoa.net/std/TAP',
+            'id': 'ivo://ivoa.net/std/TAP',
             'interface': {
-                'attrs': {
-                    'xsi:type': 'vs:ParamHTTP',
-                    'role': 'std'
-                },
-                'accessURL': {
-                    'attrs': {},
-                    'text': request.build_absolute_uri(reverse('tap:root'))
+                'type': 'vs:ParamHTTP',
+                'role': 'std',
+                'access_url': {
+                    'use': 'base',
+                    'url': settings.SITE_URL.rstrip('/') + reverse('tap:root').rstrip('/')
                 }
             },
             'languages': [{
                 'name': language['key'],
                 'version': language['version'],
                 'description': language['description'],
             } for language in settings.QUERY_LANGUAGES]
-
         },
         {
-            'schemaID': 'ivo://ivoa.net/std/TAP#async-1.1',
+            'id': 'ivo://ivoa.net/std/TAP#async-1.1',
             'interface': {
-                'attrs': {
-                    'xsi:type': 'vs:ParamHTTP',
-                    'role': 'std',
-                    'version': '1.1'
-                },
-                'accessURL': {
-                    'attrs': {
-                        'use': 'base'
-                    },
-                    'text': request.build_absolute_uri(reverse('tap:async-list'))
+                'type': 'vs:ParamHTTP',
+                'role': 'std',
+                'version': '1.1',
+                'access_url': {
+                    'use': 'base',
+                    'url': settings.SITE_URL.rstrip('/') + reverse('tap:async-list').rstrip('/')
                 }
             }
         },
         {
-            'schemaID': 'ivo://ivoa.net/std/TAP#sync-1.1',
+            'id': 'ivo://ivoa.net/std/TAP#sync-1.1',
             'interface': {
-            'attrs': {
-                'xsi:type': 'vs:ParamHTTP',
+                'type': 'vs:ParamHTTP',
                 'role': 'std',
-                'version': '1.1'
-                },
-                'accessURL': {
-                    'attrs': {
-                        'use': 'base'
-                    },
-                    'text': request.build_absolute_uri(reverse('tap:sync-list'))
+                'version': '1.1',
+                'access_url': {
+                    'use': 'base',
+                    'url': settings.SITE_URL.rstrip('/') + reverse('tap:sync-list').rstrip('/')
                 }
             }
         },
         {
-            'schemaID': 'ivo://ivoa.net/std/VOSI#capabilities',
+            'id': 'ivo://ivoa.net/std/VOSI#capabilities',
             'interface': {
-            'attrs': {
-                'xsi:type': 'vs:ParamHTTP',
-                },
-                'accessURL': {
-                    'attrs': {
-                        'use': 'full'
-                    },
-                    'text': request.build_absolute_uri(reverse('tap:capabilities'))
+                'type': 'vs:ParamHTTP',
+                'access_url': {
+                    'use': 'full',
+                    'url': settings.SITE_URL.rstrip('/') + reverse('tap:capabilities').rstrip('/')
                 }
             }
         },
         {
-            'schemaID': 'ivo://ivoa.net/std/VOSI#tables',
+            'id': 'ivo://ivoa.net/std/VOSI#tables',
             'interface': {
-            'attrs': {
-                'xsi:type': 'vs:ParamHTTP',
-                },
-                'accessURL': {
-                    'attrs': {
-                        'use': 'full'
-                    },
-                    'text': request.build_absolute_uri(reverse('tap:tables'))
+                'type': 'vs:ParamHTTP',
+                'access_url': {
+                    'use': 'full',
+                    'url': settings.SITE_URL.rstrip('/') + reverse('tap:tables').rstrip('/')
                 }
             }
         },
         {
-            'schemaID': 'ivo://ivoa.net/std/DALI#examples',
+            'id': 'ivo://ivoa.net/std/DALI#examples',
             'interface': {
-            'attrs': {
-                'xsi:type': 'vr:WebBrowser',
-                },
-                'accessURL': {
-                    'attrs': {
-                        'use': 'full'
-                    },
-                    'text': request.build_absolute_uri(reverse('tap:examples'))
+                'type': 'vr:WebBrowser',
+                'access_url': {
+                    'use': 'full',
+                    'url': settings.SITE_URL.rstrip('/') + reverse('tap:examples').rstrip('/')
                 }
             }
         }
     ]
 
-    return HttpResponse(CapabilitiesRenderer().render(data), content_type="application/xml")
 
-def tables(request):
-    queryset = Schema.objects.filter_by_access_level(request.user)
-    serializer = SchemaSerializer(queryset, context={'request': request}, many=True)
-    return HttpResponse(TablesetRenderer().render(serializer.data), content_type="application/xml")
+def get_tableset():
+    queryset = Schema.objects.filter(metadata_access_level=ACCESS_LEVEL_PUBLIC, published__isnull=False)
+    serializer = SchemaSerializer(queryset, many=True)
+    return serializer.data
```

### Comparing `django-daiquiri-0.2/daiquiri/tap/migrations/0001_initial.py` & `django-daiquiri-0.4.2/daiquiri/tap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/tap/urls.py` & `django-daiquiri-0.4.2/daiquiri/tap/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from django.conf.urls import url, include
-from django.views.generic import TemplateView
-
 from daiquiri.jobs.routers import JobRouter
-from daiquiri.query.viewsets import SyncQueryJobViewSet, AsyncQueryJobViewSet
+from daiquiri.query.viewsets import AsyncQueryJobViewSet, SyncQueryJobViewSet
+from django.urls import include, path, re_path
+from django.views.generic import TemplateView
 
-from .views import availability, capabilities, tables, examples
+from .views import availability, capabilities, examples, resource, tables
 
+app_name = 'tap'
 
 router = JobRouter(trailing_slash=False)
-router.register(r'sync', SyncQueryJobViewSet, base_name='sync')
-router.register(r'async', AsyncQueryJobViewSet, base_name='async')
+router.register(r'sync', SyncQueryJobViewSet, basename='sync')
+router.register(r'async', AsyncQueryJobViewSet, basename='async')
 
 urlpatterns = [
-    url(r'^$', TemplateView.as_view(template_name='tap/root.html'), name='root'),
-    url(r'^availability$', availability, name='availability'),
-    url(r'^capabilities$', capabilities, name='capabilities'),
-    url(r'^tables$', tables, name='tables'),
-    url(r'^examples$', examples, name='examples'),
+    path('', TemplateView.as_view(template_name='tap/root.html'), name='root'),
+    path('resource', resource, name='resource'),
+    path('availability', availability, name='availability'),
+    path('capabilities', capabilities, name='capabilities'),
+    path('tables', tables, name='tables'),
+    path('examples', examples, name='examples'),
 
-    url(r'^', include(router.urls)),
+    re_path(r'^', include(router.urls)),
 ]
```

### Comparing `django-daiquiri-0.2/daiquiri/tap/templates/tap/root.html` & `django-daiquiri-0.4.2/daiquiri/tap/templates/tap/root.html`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,26 @@
     <ul>
         <li>
             <a href="{% url 'tap:sync-list' %}">{% trans 'sync' %}</a>
         </li>
         <li>
             <a href="{% url 'tap:async-list' %}">{% trans 'async' %}</a>
         </li>
+    </ul>
+    <ul>
+        <li>
+            <a href="{% url 'tap:resource' %}">{% trans 'VOResource Record' %}</a>
+        </li>
         <li>
-            <a href="{% url 'tap:capabilities' %}">{% trans 'capabilities' %}</a>
+            <a href="{% url 'tap:capabilities' %}">{% trans 'VOSI capabilities' %}</a>
         </li>
         <li>
-            <a href="{% url 'tap:tables' %}">{% trans 'tables' %}</a>
+            <a href="{% url 'tap:tables' %}">{% trans 'VOSI tableset' %}</a>
         </li>
+    </ul>
+    <ul>
         <li>
             <a href="{% url 'tap:examples' %}">{% trans 'examples' %}</a>
         </li>
     </ul>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% extends 'core/wide.html' %} {% load i18n %} {% block wide %}
 ****** {% trans 'TAP service' %} ******
     * {%_trans_'sync'_%}
     * {%_trans_'async'_%}
-    * {%_trans_'capabilities'_%}
-    * {%_trans_'tables'_%}
+    * {%_trans_'VOResource_Record'_%}
+    * {%_trans_'VOSI_capabilities'_%}
+    * {%_trans_'VOSI_tableset'_%}
     * {%_trans_'examples'_%}
 {% endblock %}
```

### Comparing `django-daiquiri-0.2/daiquiri/tap/templates/tap/examples.html` & `django-daiquiri-0.4.2/daiquiri/tap/templates/tap/examples.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'core/wide.html' %}
-{% load staticfiles %}
+{% load static %}
 {% load compress %}
 {% load i18n %}
 
 {% block headextra %}
     {% compress css %}
     <link rel="stylesheet" type="text/x-scss" href="{% static 'tap/css/examples.scss' %}" />
     {% endcompress css %}
```

### Comparing `django-daiquiri-0.2/daiquiri/tap/models.py` & `django-daiquiri-0.4.2/daiquiri/tap/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from django.db import models
-from django.utils.encoding import python_2_unicode_compatible
 
 
-@python_2_unicode_compatible
 class Schema(models.Model):
 
     schema_name = models.CharField(max_length=256)
     utype = models.CharField(max_length=256, null=True, blank=True)
     description = models.CharField(max_length=256, null=True, blank=True)
 
     class Meta:
         db_table = 'schemas'
 
     def __str__(self):
         return self.schema_name
 
 
-@python_2_unicode_compatible
 class Table(models.Model):
 
-    schema = models.ForeignKey(Schema, related_name='tables')
+    schema = models.ForeignKey(Schema, related_name='tables', on_delete=models.CASCADE)
 
     schema_name = models.CharField(max_length=256)
     table_name = models.CharField(max_length=256)
     table_type = models.CharField(max_length=256)
     utype = models.CharField(max_length=256, null=True, blank=True)
     description = models.CharField(max_length=256, null=True, blank=True)
     table_index = models.IntegerField(null=True, blank=True)
@@ -31,18 +28,17 @@
     class Meta:
         db_table = 'tables'
 
     def __str__(self):
         return '%s.%s' % (self.schema_name, self.table_name)
 
 
-@python_2_unicode_compatible
 class Column(models.Model):
 
-    table = models.ForeignKey(Table, related_name='columns')
+    table = models.ForeignKey(Table, related_name='columns', on_delete=models.CASCADE)
 
     table_name = models.CharField(max_length=256)
     column_name = models.CharField(max_length=256)
     datatype = models.CharField(max_length=256)
     arraysize = models.IntegerField(null=True, blank=True)
     size = models.IntegerField(null=True, blank=True)
     description = models.CharField(max_length=256, null=True, blank=True)
```

### Comparing `django-daiquiri-0.2/daiquiri/tap/management/commands/rebuild_tap_schema.py` & `django-daiquiri-0.4.2/daiquiri/tap/management/commands/rebuild_tap_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from daiquiri.tap.models import (
     Schema as TapSchema,
     Table as TapTable,
     Column as TapColumn,
 )
 from daiquiri.tap.utils import update_schema
 
+
 class Command(BaseCommand):
 
     def handle(self, *args, **options):
 
         TapSchema.objects.all().delete()
         TapTable.objects.all().delete()
         TapColumn.objects.all().delete()
```

### Comparing `django-daiquiri-0.2/daiquiri/query/handlers.py` & `django-daiquiri-0.4.2/daiquiri/query/handlers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/serializers.py` & `django-daiquiri-0.4.2/daiquiri/query/serializers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rest_framework import serializers
 
 from daiquiri.jobs.serializers import SyncJobSerializer, AsyncJobSerializer
 
 from .models import QueryJob, Example
-from .validators import TableNameValidator
+from .validators import TableNameValidator, UploadFileValidator, UploadParamValidator
 
 
 class FormSerializer(serializers.Serializer):
 
     key = serializers.CharField()
     form_service = serializers.SerializerMethodField()
 
@@ -24,14 +24,30 @@
     def get_dropdown_service(self, obj):
         return obj['key'][0].upper() + obj['key'][1:] + 'DropdownService'
 
     def get_options(self, obj):
         return obj['options']
 
 
+class DownloadSerializer(serializers.Serializer):
+
+    key = serializers.CharField()
+    download_service = serializers.SerializerMethodField()
+    options = serializers.SerializerMethodField()
+
+    def get_download_service(self, obj):
+        if obj.get('service'):
+            return obj['key'][0].upper() + obj['key'][1:] + 'DownloadService'
+        else:
+            return None
+
+    def get_options(self, obj):
+        return obj.get('options', {})
+
+
 class QueryJobSerializer(serializers.ModelSerializer):
 
     class Meta:
         model = QueryJob
         fields = (
             'id',
         )
@@ -85,25 +101,25 @@
 
     def get_sources(self, obj):
         if obj.metadata:
             return obj.metadata.get('sources', [])
         else:
             return []
 
-
     def get_columns(self, obj):
         if obj.metadata:
             return obj.metadata.get('columns', [])
         else:
             return []
 
 
 class QueryJobCreateSerializer(serializers.ModelSerializer):
 
-    table_name = serializers.CharField(required=False, allow_blank=True, validators=[TableNameValidator()])
+    table_name = serializers.CharField(required=False, allow_blank=True, max_length=256,
+                                       validators=[TableNameValidator()])
     queue = serializers.CharField(required=False)
     query_language = serializers.CharField(required=True)
     query = serializers.CharField(required=True)
     run_id = serializers.CharField(default='')
 
     class Meta:
         model = QueryJob
@@ -126,14 +142,29 @@
         fields = (
             'id',
             'table_name',
             'run_id'
         )
 
 
+class QueryJobUploadSerializer(serializers.ModelSerializer):
+
+    table_name = serializers.CharField(required=False, validators=[TableNameValidator()])
+    run_id = serializers.CharField(default='')
+    file = serializers.FileField(max_length=None, allow_empty_file=False, validators=[UploadFileValidator()])
+
+    class Meta:
+        model = QueryJob
+        fields = (
+            'table_name',
+            'run_id',
+            'file'
+        )
+
+
 class QueryLanguageSerializer(serializers.Serializer):
 
     id = serializers.SerializerMethodField(required=False)
     text = serializers.CharField(source='label')
     quote_char = serializers.CharField()
 
     def get_id(self, obj):
@@ -172,21 +203,25 @@
 
 
 class SyncQueryJobSerializer(SyncJobSerializer):
 
     RESPONSEFORMAT = serializers.CharField(required=False)
     FORMAT = serializers.CharField(required=False)
 
-    TABLE_NAME = serializers.CharField(required=False, validators=[TableNameValidator()])
+    TABLE_NAME = serializers.CharField(required=False, max_length=256, validators=[TableNameValidator()])
     LANG = serializers.CharField(required=True)
     QUERY = serializers.CharField(required=True)
 
+    UPLOAD = serializers.CharField(required=False, default='', validators=[UploadParamValidator()])
+
 
 class AsyncQueryJobSerializer(AsyncJobSerializer):
 
     RESPONSEFORMAT = serializers.CharField(required=False)
     FORMAT = serializers.CharField(required=False)
 
-    TABLE_NAME = serializers.CharField(required=False, validators=[TableNameValidator()])
+    TABLE_NAME = serializers.CharField(required=False, max_length=256, validators=[TableNameValidator()])
     QUEUE = serializers.CharField(required=False)
     LANG = serializers.CharField(required=True)
     QUERY = serializers.CharField(required=True)
+
+    UPLOAD = serializers.CharField(required=False, default='', validators=[UploadParamValidator()])
```

### Comparing `django-daiquiri-0.2/daiquiri/query/views.py` & `django-daiquiri-0.4.2/daiquiri/query/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.views.generic import TemplateView
 
-from daiquiri.core.views import ModelPermissionMixin, AnonymousAccessMixin
+from daiquiri.core.views import AnonymousAccessMixin, CSRFViewMixin, ModelPermissionMixin
 from daiquiri.core.utils import get_model_field_meta
 
 from .models import QueryJob, Example
 
 
-class QueryView(AnonymousAccessMixin, TemplateView):
+class QueryView(AnonymousAccessMixin, CSRFViewMixin, TemplateView):
     template_name = 'query/query.html'
     anonymous_setting = 'QUERY_ANONYMOUS'
 
 
-class JobsView(LoginRequiredMixin, TemplateView):
+class JobsView(LoginRequiredMixin, CSRFViewMixin, TemplateView):
     template_name = 'query/jobs.html'
 
     def get_context_data(self, **kwargs):
         context = super(JobsView, self).get_context_data(**kwargs)
         context['phases'] = QueryJob.PHASE_CHOICES
         return context
 
 
-class ExamplesView(ModelPermissionMixin, TemplateView):
+class ExamplesView(ModelPermissionMixin, CSRFViewMixin, TemplateView):
 
     template_name = 'query/examples.html'
     permission_required = 'daiquiri_query.view_example'
 
     def get_context_data(self, **kwargs):
         context = super(ExamplesView, self).get_context_data(**kwargs)
         context['meta'] = {
```

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0017_big_integer_fields.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0017_big_integer_fields.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0015_queryarchivejob.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0014_downloadjob.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 # -*- coding: utf-8 -*-
-# Generated by Django 1.11.9 on 2018-01-10 14:18
+# Generated by Django 1.11.5 on 2017-12-09 14:59
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
-import jsonfield.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('daiquiri_jobs', '0012_meta'),
-        ('daiquiri_query', '0014_downloadjob'),
+        ('daiquiri_query', '0013_refactoring'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='QueryArchiveJob',
+            name='DownloadJob',
             fields=[
                 ('job_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='daiquiri_jobs.Job')),
-                ('column_name', models.CharField(help_text='Column name for this download.', max_length=32, verbose_name='Column name')),
-                ('files', jsonfield.fields.JSONField(help_text='List of files in the archive.', verbose_name='Files')),
-                ('job', models.ForeignKey(help_text='QueryJob this ArchiveJob belongs to.', on_delete=django.db.models.deletion.CASCADE, related_name='archives', to='daiquiri_query.QueryJob', verbose_name='QueryJob')),
+                ('format_key', models.CharField(help_text='Format key for this download.', max_length=32, verbose_name='Format key')),
+                ('file_path', models.CharField(help_text='Path to the file.', max_length=256, verbose_name='Path')),
+                ('job', models.ForeignKey(help_text='QueryJob this DownloadJob belongs to.', on_delete=django.db.models.deletion.CASCADE, related_name='downloads', to='daiquiri_query.QueryJob', verbose_name='QueryJob')),
             ],
             options={
                 'ordering': ('start_time',),
-                'verbose_name': 'QueryArchiveJob',
-                'verbose_name_plural': 'QueryArchiveJob',
-                'permissions': (('view_queryarchivejob', 'Can view QueryArchiveJob'),),
+                'verbose_name': 'DownloadJob',
+                'verbose_name_plural': 'DownloadJobs',
+                'permissions': (('view_downloadjob', 'Can view DownloadJob'),),
             },
             bases=('daiquiri_jobs.job',),
         ),
-        migrations.RemoveField(
-            model_name='downloadjob',
-            name='file_path',
-        ),
     ]
```

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0013_refactoring.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0013_refactoring.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0003_query_language_and_actual_query.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0003_query_language_and_actual_query.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0009_remove_choices.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0009_remove_choices.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0006_example.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0006_example.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0001_initial.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0005_meta.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0005_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/migrations/0004_table_name.py` & `django-daiquiri-0.4.2/daiquiri/query/migrations/0004_table_name.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/urls.py` & `django-daiquiri-0.4.2/daiquiri/query/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-from django.conf.urls import url, include
-
+from django.urls import include, path
 from rest_framework import routers
 
-from .views import QueryView, JobsView, ExamplesView
-from .viewsets import (
-    StatusViewSet,
-    FormViewSet,
-    DropdownViewSet,
-    QueryJobViewSet,
-    ExampleViewSet,
-    QueueViewSet,
-    QueryLanguageViewSet,
-    PhaseViewSet
-)
+from .views import ExamplesView, JobsView, QueryView
+from .viewsets import (DropdownViewSet, ExampleViewSet, FormViewSet,
+                       PhaseViewSet, QueryJobViewSet, QueryLanguageViewSet,
+                       QueueViewSet, StatusViewSet, DownloadViewSet)
+
+app_name = 'query'
 
 router = routers.DefaultRouter()
-router.register(r'status', StatusViewSet, base_name='status')
-router.register(r'forms', FormViewSet, base_name='form')
-router.register(r'dropdowns', DropdownViewSet, base_name='dropdown')
-router.register(r'jobs', QueryJobViewSet, base_name='job')
-router.register(r'examples', ExampleViewSet, base_name='example')
-router.register(r'queues', QueueViewSet, base_name='queue')
-router.register(r'querylanguages', QueryLanguageViewSet, base_name='querylanguage')
-router.register(r'phases', PhaseViewSet, base_name='phase')
+router.register(r'status', StatusViewSet, basename='status')
+router.register(r'forms', FormViewSet, basename='form')
+router.register(r'dropdowns', DropdownViewSet, basename='dropdown')
+router.register(r'downloads', DownloadViewSet, basename='download')
+router.register(r'jobs', QueryJobViewSet, basename='job')
+router.register(r'examples', ExampleViewSet, basename='example')
+router.register(r'queues', QueueViewSet, basename='queue')
+router.register(r'querylanguages', QueryLanguageViewSet, basename='querylanguage')
+router.register(r'phases', PhaseViewSet, basename='phase')
 
 urlpatterns = [
-    url(r'^$', QueryView.as_view(), name='query'),
-    url(r'^jobs/$', JobsView.as_view(), name='jobs'),
-    url(r'^examples/$', ExamplesView.as_view(), name='examples'),
+    path(r'', QueryView.as_view(), name='query'),
+    path(r'jobs/', JobsView.as_view(), name='jobs'),
+    path(r'examples/', ExamplesView.as_view(), name='examples'),
 
     # rest api
-    url(r'^api/', include(router.urls)),
+    path(r'api/', include(router.urls)),
 ]
```

### Comparing `django-daiquiri-0.2/daiquiri/query/tasks.py` & `django-daiquiri-0.4.2/daiquiri/query/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from __future__ import absolute_import, unicode_literals
-
 import logging
 import os
 import zipfile
 
-from celery import shared_task
-
 from django.conf import settings
-from django.core.urlresolvers import reverse
-from django.db.utils import OperationalError, ProgrammingError, InternalError
+from django.db.utils import InternalError, OperationalError, ProgrammingError
 from django.utils.timezone import now
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
+
+from celery import shared_task
 
 from daiquiri.core.tasks import Task
 
 
 class RunQueryTask(Task):
 
     def on_failure(self, exc, task_id, args, kwargs, einfo):
@@ -36,20 +33,20 @@
         job = QueryJob.objects.get(pk=job_id)
         job.phase = job.PHASE_ERROR
         job.error_summary = str(_('There has been an server error with your job.'))
         job.save()
 
 
 @shared_task(base=RunQueryTask)
-def run_query(job_id):
+def run_database_query_task(job_id):
     # always import daiquiri packages inside the task
     from daiquiri.core.adapter import DatabaseAdapter
-    from daiquiri.metadata.models import Table, Column
     from daiquiri.query.models import QueryJob
-    from daiquiri.query.utils import get_quota
+    from daiquiri.query.utils import (get_job_columns, get_job_sources,
+                                      get_quota, ingest_uploads)
     from daiquiri.stats.models import Record
 
     # get logger
     logger = logging.getLogger(__name__)
 
     # get the job object from the database
     job = QueryJob.objects.get(pk=job_id)
@@ -73,30 +70,30 @@
             job.phase = job.PHASE_ERROR
             job.error_summary = str(_('Quota is exceeded. Please remove some of your jobs.'))
             job.save()
 
             return job.phase
 
         # set database and start time
-        job.start_time = now()
-
         job.pid = adapter.fetch_pid()
         job.actual_query = adapter.build_query(job.schema_name, job.table_name, job.native_query, job.timeout, job.max_records)
         job.phase = job.PHASE_EXECUTING
         job.start_time = now()
         job.save()
 
         logger.info('job %s started' % job.id)
 
         # get the actual query and submit the job to the database
         try:
+            job.metadata['upload_columns'] = ingest_uploads(job.uploads, job.owner)
+
             # this is where the work ist done (and the time is spend)
             adapter.submit_query(job.actual_query)
 
-        except (ProgrammingError, InternalError) as e:
+        except (ProgrammingError, InternalError, ValueError) as e:
             job.phase = job.PHASE_ERROR
             job.error_summary = str(e)
             logger.info('job %s failed (%s)' % (job.id, job.error_summary))
 
         except OperationalError as e:
             # load the job again and check if the job was killed
             job = QueryJob.objects.get(pk=job_id)
@@ -117,102 +114,145 @@
 
             # get additional information about the completed job
             if job.phase == job.PHASE_COMPLETED:
                 job.nrows = adapter.count_rows(job.schema_name, job.table_name)
                 job.size = adapter.fetch_size(job.schema_name, job.table_name)
 
                 # fetch the metadata for used tables
-                job.metadata['sources'] = []
+                job.metadata['sources'] = get_job_sources(job)
 
-                if 'sources' in job.metadata:
-                    for schema_name, table_name in job.metadata['tables']:
-                        table = {
-                            'schema_name': schema_name,
-                            'table_name': table_name
-                        }
-
-                        # fetch additional metadata from the metadata store
-                        try:
-                            original_table = Table.objects.get(
-                                name=table_name,
-                                schema__name=schema_name
-                            )
-
-                            table.update({
-                                'title': original_table.title,
-                                'description': original_table.description,
-                                'attribution': original_table.attribution,
-                                'license': original_table.license,
-                                'doi': original_table.doi,
-                                'url': reverse('metadata:table', args=[schema_name, table_name])
-                            })
-
-                            job.metadata['sources'].append(table)
-
-                        except Table.DoesNotExist:
-                            pass
-
-                # fetch the metadata for the columns
-                job.metadata['columns'] = adapter.fetch_columns(job.schema_name, job.table_name)
-
-                # fetch additional metadata from the metadata store
-                for column in job.metadata['columns']:
-                    if column['name'] in job.metadata['display_columns']:
-
-                        try:
-                            schema_name, table_name, column_name = job.metadata['display_columns'][column['name']]
-                        except ValueError:
-                            continue
-
-                        try:
-                            original_column = Column.objects.get(
-                                name=column_name,
-                                table__name=table_name,
-                                table__schema__name=schema_name
-                            )
-
-                            column.update({
-                                'description': original_column.description,
-                                'unit': original_column.unit,
-                                'ucd': original_column.ucd,
-                                'utype': original_column.utype,
-                                'principal': original_column.principal,
-                                'indexed': False,
-                                'std': original_column.std
-                            })
-
-                        except Column.DoesNotExist:
-                            pass
+                # fetch the metadata for the columns and fetch additional metadata from the metadata store
+                job.metadata['columns'] = get_job_columns(job)
 
             # remove unneeded metadata
             job.metadata.pop('display_columns', None)
             job.metadata.pop('tables', None)
+            job.metadata.pop('upload_columns', None)
+            job.metadata.pop('user_columns', None)
 
             # create a stats record for this job
             Record.objects.create(
                 time=job.end_time,
-                resource_type='QUERY_JOB',
+                resource_type='QUERY',
                 resource={
                     'job_id': job.id,
                     'job_type': job.job_type,
+                    'query': job.query,
+                    'query_language': job.query_language,
                     'sources': job.metadata.get('sources', [])
                 },
                 client_ip=job.client_ip,
                 user=job.owner
             )
 
             job.save()
 
     return job.phase
 
 
 @shared_task(base=Task)
-def create_download_file(download_id):
+def run_database_ingest_task(job_id, file_path):
+    from daiquiri.core.adapter import DatabaseAdapter
+    from daiquiri.query.models import QueryJob
+    from daiquiri.query.utils import get_quota, ingest_table
+    from daiquiri.stats.models import Record
+
+    # get logger
+    logger = logging.getLogger(__name__)
+
+    # get the job object from the database
+    job = QueryJob.objects.get(pk=job_id)
+
+    if job.phase == job.PHASE_QUEUED:
+        # get the adapter with the database specific functions
+        adapter = DatabaseAdapter()
+
+        # create the database of the user if it not already exists
+        try:
+            adapter.create_user_schema_if_not_exists(job.schema_name)
+        except OperationalError as e:
+            job.phase = job.PHASE_ERROR
+            job.error_summary = str(e)
+            job.save()
+
+            return job.phase
+
+        # check if the quota is exceeded
+        if QueryJob.objects.get_size(job.owner) > get_quota(job.owner):
+            job.phase = job.PHASE_ERROR
+            job.error_summary = str(_('Quota is exceeded. Please remove some of your jobs.'))
+            job.save()
+
+            return job.phase
+
+        # set database and start time
+        job.pid = adapter.fetch_pid()
+        job.phase = job.PHASE_EXECUTING
+        job.start_time = now()
+        job.save()
+
+        logger.info('job %s started' % job.id)
+
+        # create the table and insert the data
+        try:
+            columns = ingest_table(job.schema_name, job.table_name, file_path)
+
+        except (ProgrammingError, InternalError, ValueError) as e:
+            job.phase = job.PHASE_ERROR
+            job.error_summary = str(e)
+            logger.info('job %s failed (%s)' % (job.id, job.error_summary))
+
+        except OperationalError as e:
+            # load the job again and check if the job was killed
+            job = QueryJob.objects.get(pk=job_id)
+
+            if job.phase != job.PHASE_ABORTED:
+                job.phase = job.PHASE_ERROR
+                job.error_summary = str(e)
+                logger.info('job %s failed (%s)' % (job.id, job.error_summary))
+
+        else:
+            # get additional information about the completed job
+            job.phase = job.PHASE_COMPLETED
+            logger.info('job %s completed' % job.id)
+
+        finally:
+            # get timing and save the job object
+            job.end_time = now()
+
+            # get additional information about the completed job
+            if job.phase == job.PHASE_COMPLETED:
+                job.nrows = adapter.count_rows(job.schema_name, job.table_name)
+                job.size = adapter.fetch_size(job.schema_name, job.table_name)
+
+                # store the metadata for the columns from the VOTable
+                job.metadata = {
+                    'columns': columns
+                }
+
+            # create a stats record for this job
+            Record.objects.create(
+                time=job.end_time,
+                resource_type='UPLOAD',
+                resource={
+                    'job_id': job.id,
+                    'job_type': job.job_type,
+                },
+                client_ip=job.client_ip,
+                user=job.owner
+            )
+
+            job.save()
+
+    return job.phase
+
+
+@shared_task(base=Task)
+def create_download_table_task(download_id):
     # always import daiquiri packages inside the task
-    from daiquiri.core.adapter import DownloadAdapter
     from daiquiri.query.models import DownloadJob
 
     # get logger
     logger = logging.getLogger(__name__)
 
     # get the job object from the database
     download_job = DownloadJob.objects.get(pk=download_id)
@@ -228,34 +268,41 @@
             pass
 
         download_job.phase = download_job.PHASE_EXECUTING
         download_job.start_time = now()
         download_job.save()
 
         # write file using the generator in the adapter
+        if download_job.format_key == 'fits':
+            write_label = 'wb'
+        else:
+            write_label = 'w'
         try:
-            with open(download_job.file_path, 'w') as f:
-                for line in download_job.job.stream(download_job.format_key):
+
+            with open(download_job.file_path, write_label) as f:
+                for line in download_job.query_job.stream(download_job.format_key):
                     f.write(line)
 
         except Exception as e:
             download_job.phase = download_job.PHASE_ERROR
             download_job.error_summary = str(e)
             download_job.save()
             logger.info('download_job %s failed (%s)' % (download_job.id, download_job.error_summary))
+
+            raise e
         else:
             download_job.phase = download_job.PHASE_COMPLETED
             logger.info('download_job %s completed' % download_job.file_path)
         finally:
             download_job.end_time = now()
             download_job.save()
 
 
 @shared_task(track_started=True, base=Task)
-def create_archive_file(archive_id):
+def create_download_archive_task(archive_id):
     # always import daiquiri packages inside the task
     from daiquiri.query.models import QueryArchiveJob
 
     # get logger
     logger = logging.getLogger(__name__)
 
     # get the job object from the database
@@ -272,18 +319,56 @@
             pass
 
         archive_job.phase = archive_job.PHASE_EXECUTING
         archive_job.start_time = now()
         archive_job.save()
 
         # create a zipfile with all files
-        with zipfile.ZipFile(archive_job.file_path, 'w') as z:
-            for file_path in archive_job.files:
-                os.chdir(settings.ARCHIVE_BASE_PATH)
-                z.write(file_path)
+        try:
+            with zipfile.ZipFile(archive_job.file_path, 'w') as z:
+                os.chdir(settings.FILES_BASE_PATH)
+                for file_path in archive_job.files:
+                    z.write(file_path)
+
+        except Exception as e:
+            archive_job.phase = archive_job.PHASE_ERROR
+            archive_job.error_summary = str(e)
+            archive_job.save()
+            logger.info('archive_job %s failed (%s)' % (archive_job.id, archive_job.error_summary))
+            raise e
 
         archive_job.end_time = now()
         archive_job.phase = archive_job.PHASE_COMPLETED
         archive_job.save()
 
         # log completion
         logger.info('create_archive_zip_file %s completed' % archive_job.file_path)
+
+
+@shared_task(base=Task)
+def rename_database_table_task(schema_name, table_name, new_table_name):
+    from daiquiri.core.adapter import DatabaseAdapter
+
+    DatabaseAdapter().rename_table(schema_name, table_name, new_table_name)
+
+
+@shared_task(base=Task)
+def drop_database_table_task(schema_name, table_name):
+    from daiquiri.core.adapter import DatabaseAdapter
+
+    # drop the corresponding database table, but fail silently
+    try:
+        DatabaseAdapter().drop_table(schema_name, table_name)
+    except ProgrammingError:
+        pass
+
+
+@shared_task(base=Task)
+def abort_databae_query_task(pid):
+    from daiquiri.core.adapter import DatabaseAdapter
+
+    # abort the job on the database
+    try:
+        DatabaseAdapter().abort_query(pid)
+    except OperationalError:
+        # the query was probably killed before
+        pass
```

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/css/query.scss` & `django-daiquiri-0.4.2/daiquiri/query/static/query/css/query.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/forms/cone.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/cone.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/forms/sql.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/sql.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -91,14 +91,18 @@
         var editor = $('.CodeMirror')[0].CodeMirror;
 
         if (resource == 'examples') {
             service.values.query = item.query_string;
             service.values.query_language = item.query_language;
 
             editor.refresh();
+        } else if (resource == 'functions') {
+
+            editor.replaceSelection(item.query_string);
+
         } else {
             var query_language = $filter('filter')(QueryService.query_languages, {
                 id: service.values.query_language
             })[0];
             var quote_char = query_language.quote_char;
 
             var query_strings = [];
```

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/forms/box.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/box.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/dropdowns/simbad.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/simbad.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/dropdowns/vizier.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/vizier.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/services/jobs.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/jobs.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     /* get the base url */
 
     var baseurl = angular.element('meta[name="baseurl"]').attr('content');
 
     /* configure resources */
 
     var resources = {
-        jobs: $resource(baseurl + 'query/api/jobs/:id/:detail_route/'),
+        jobs: $resource(baseurl + 'query/api/jobs/:id/:detail_action/'),
         queues: $resource(baseurl + 'query/api/queues/:id/'),
         phases: $resource(baseurl + 'query/api/phases/:id/')
     }
 
     /* create the service */
 
     var service = {
```

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/services/query.js` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/js/metadata.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,350 +1,270 @@
-app.factory('QueryService', ['$resource', '$injector', '$q', '$filter', 'PollingService', 'PlotService', 'DownloadService', 'TableService', 'BrowserService', function($resource, $injector, $q, $filter, PollingService, PlotService, DownloadService, TableService, BrowserService) {
+angular.module('metadata', ['core'])
 
-    /* get the base url */
+    .factory('MetadataService', ['$resource', '$q', '$filter', '$timeout', 'BrowserService', function($resource, $q, $filter, $timeout, BrowserService) {
 
-    var baseurl = angular.element('meta[name="baseurl"]').attr('content');
+        /* get the base url */
 
-    /* configure resources */
+        var baseurl = angular.element('meta[name="baseurl"]').attr('content');
 
-    var resources = {
-        status: $resource(baseurl + 'query/api/status/'),
-        forms: $resource(baseurl + 'query/api/forms/'),
-        dropdowns: $resource(baseurl + 'query/api/dropdowns/'),
-        jobs: $resource(baseurl + 'query/api/jobs/:id/:detail_route/'),
-        examples: $resource(baseurl + 'query/api/examples/user/'),
-        queues: $resource(baseurl + 'query/api/queues/'),
-        querylanguages: $resource(baseurl + 'query/api/querylanguages/'),
-        phases: $resource(baseurl + 'query/api/phases/'),
-        schemas: $resource(baseurl + 'metadata/api/schemas/user/'),
-        functions: $resource(baseurl + 'metadata/api/functions/user/'),
-    };
-
-    /* initialise the browser service */
-
-    BrowserService.init('schemas', ['schemas', 'tables', 'columns'])
-    BrowserService.init('columns', ['columns'], true)
-    BrowserService.init('functions', ['functions'])
-    BrowserService.init('examples', ['examples'])
-
-    /* create the query service */
-
-    var service = {
-        first_form: null,
-        submitting: false,
-        show: {
-            '': true
-        },
-        forms: {},
-        dropdowns: {},
-        values: {},
-        errors: {}
-    };
-
-    service.init = function() {
-        // fetch queues,  query languages and then load forms
-        service.queues = resources.queues.query();
-        service.query_languages = resources.querylanguages.query();
-
-        $q.all([service.queues.$promise, service.query_languages.$promise]).then(function() {
-            service.active_queue = service.queues[0].id;
-
-            resources.forms.query(function(response) {
-                angular.forEach(response, function(form) {
-                    service.forms[form.key] = $injector.get(form.form_service);
-
-                    // remember the first form
-                    if (!service.first_form) {
-                        service.first_form = service.forms[form.key];
-                    }
-                });
-
-                // activate the first form
-                service.first_form.activate();
-            });
-        });
-
-        // fetch job phases
-        service.phases = resources.phases.query();
-
-        // load dropdowns
-        resources.dropdowns.query(function(response) {
-            angular.forEach(response, function(dropdown) {
-                service.dropdowns[dropdown.key] = $injector.get(dropdown.dropdown_service);
-                service.dropdowns[dropdown.key].options = dropdown.options;
-            });
-        });
-
-        // fetch status
-        service.fetch_status();
-
-        // fetch functions
-        resources.functions.query(function(response) {
-            BrowserService.render('functions', response);
-        });
+        /* create the metadata service */
+
+        var service = {
+            ready: false,
+            browser: BrowserService
+        };
+
+        /* configure the resources */
+
+        var resources = {
+            'schemas': $resource(baseurl + 'metadata/api/schemas/:list_action/:id/'),
+            'tables': $resource(baseurl + 'metadata/api/tables/:list_action/:id/'),
+            'columns': $resource(baseurl + 'metadata/api/columns/:list_action/:id/'),
+            'functions': $resource(baseurl + 'metadata/api/functions/:list_action/:id/'),
+            'tabletypes': $resource(baseurl + 'metadata/api/tabletypes/:id/'),
+            'licenses': $resource(baseurl + 'metadata/api/licenses/:id/'),
+            'accesslevels': $resource(baseurl + 'metadata/api/accesslevels/:id/'),
+            'groups': $resource(baseurl + 'auth/api/groups/:id/'),
+        };
+
+        /* configure the factory for new items */
+
+        service.factory = {
+            schemas: function() {
+                return {
+                    access_level: 'PRIVATE',
+                    metadata_access_level: 'PRIVATE',
+                    discover: true,
+                    groups: []
+                };
+            },
+            tables: function() {
+                return {
+                    schema: service.browser.getSelectedItem('schemas', 0).id,
+                    access_level: 'PRIVATE',
+                    metadata_access_level: 'PRIVATE',
+                    discover: true,
+                    groups: []
+                };
+            },
+            columns: function() {
+                return {
+                    table: service.browser.getSelectedItem('schemas', 1).id,
+                    access_level: 'PRIVATE',
+                    metadata_access_level: 'PRIVATE',
+                    groups: []
+                };
+            },
+            functions: function() {
+                return {
+                    access_level: 'PRIVATE',
+                    metadata_access_level: 'PRIVATE',
+                    groups: []
+                };
+            },
+            persons: function() {
+                return {
+                    name: '',
+                    first_name: '',
+                    last_name: '',
+                    orcid: '',
+                    affiliations: ''
+                }
+            }
+        };
 
-        // fetch examples
-        resources.examples.query(function(response) {
-            BrowserService.render('examples', response);
-        });
+        /* define service functions */
 
-        // fetch schemas
-        resources.schemas.query(function(response) {
-            service.schemas = response;
-
-            service.columns = []
-            angular.forEach(service.schemas, function(schema) {
-                angular.forEach(schema.tables, function(table) {
-                    angular.forEach(table.columns, function(column) {
-                        var column_copy = angular.copy(column);
-                        column_copy.name = schema.name + '.' + table.name + '.' + column.name;
-                        service.columns.push(column_copy);
+        service.init = function() {
+            service.tabletypes = resources.tabletypes.query();
+            service.groups = resources.groups.query();
+            service.licenses = resources.licenses.query();
+            service.accesslevels = resources.accesslevels.query();
+
+            BrowserService.init('schemas', ['schemas', 'tables', 'columns']);
+            BrowserService.init('functions', ['functions']);
+
+            schemas_promise = service.initSchemasBrowser();
+            functions_promise = service.initFunctionsBrowser();
+
+            $q.all([schemas_promise, functions_promise]).then(function() {
+                service.ready = true;
+            })
+        };
+
+        service.initSchemasBrowser = function() {
+            return resources.schemas.query({
+                'list_action': 'management'
+            }, function(response) {
+                service.schemas = response;
+
+                service.tables = [];
+                angular.forEach(service.schemas, function(schema) {
+                    schema.label = schema.name;
+                    angular.forEach(schema.tables, function(table) {
+                        table.label = schema.name + '.' + table.name;
+                        service.tables.push(table);
                     });
                 });
+
+                BrowserService.render('schemas', service.schemas, service.active);
+            }).$promise;
+        };
+
+        service.initFunctionsBrowser = function() {
+            return resources.functions.query({
+                'list_action': 'management'
+            }, function(response) {
+                service.functions = response;
+
+                BrowserService.render('functions', service.functions, service.active);
+            }).$promise;
+        };
+
+        service.activateItem = function(resource, id) {
+            return resources[resource].get({
+                id: id
+            }, function(item) {
+                item.resource = resource;
+
+                // create a string for the groups
+                if (angular.isDefined(item.groups)) {
+                    item.published_for = $filter('filter')(service.groups, function(group) {
+                        return item.groups.indexOf(group.id) !== -1;
+                    }).map(function(group) {
+                        return group.name;
+                    }).join(', ');
+                }
+
+                service.active = item;
             });
+        };
 
-            // load user schema when schemas have been fetched
-            service.fetch_user_schema();
-        });
+        service.openFormModal = function(resource, create, modal) {
+            service.errors = {};
+            service.values = {};
+
+            if (angular.isDefined(create) && create) {
+                service.values = service.factory[resource]();
+            } else {
+                service.values = angular.copy(service.active);
+            }
 
-        // fetch joblist
-        service.fetch_jobs();
+            $timeout(function() {
+                var modal_id;
+                if (angular.isDefined(modal) && modal) {
+                    modal_id = '#' + resource + '-' + modal + '-form-modal';
+                } else {
+                    modal_id = '#' + resource + '-form-modal';
+                }
 
-        // activate overview tab
-        service.tab = 'overview';
+                $(modal_id).modal('show');
 
-        // start the polling service
-        service.polling = PollingService
-        service.polling.init();
-        service.polling.register('status', service.fetch_status, {}, true, false);
-        service.polling.register('jobs', service.fetch_jobs, {}, true, false);
-        service.polling.register('schema', service.fetch_user_schema, {}, true, false);
-
-        // load the other services
-        service.table = TableService;
-        service.plot = PlotService;
-        service.downloads = DownloadService;
-    };
-
-    service.fetch_status = function() {
-        return resources.status.query(function(response) {
-            service.status = response[0];
-        }).$promise;
-    };
-
-    service.fetch_user_schema = function() {
-        return resources.jobs.query({
-            'detail_route': 'tables'
-        }, function(response) {
-            var user_schema = response[0];
-
-            var user_columns = [];
-            angular.forEach(user_schema.tables, function(table) {
-                angular.forEach(table.columns, function(column) {
-                    var column_copy = angular.copy(column);
-                    column_copy.name = user_schema.name + '.' + table.name + '.' + column.name;
-                    user_columns.push(column_copy);
+                $timeout(function() {
+                    if (angular.element(modal_id + ' .CodeMirror').length) {
+                        angular.element(modal_id + ' .CodeMirror')[0].CodeMirror.refresh();
+                    }
                 });
             });
+        };
 
-            BrowserService.render('schemas', service.schemas.concat(user_schema));
-            BrowserService.render('columns', service.columns.concat(user_columns));
-        }).$promise;
-    }
-
-    service.fetch_jobs = function() {
-        return resources.jobs.paginate({
-            page_size: 1000,
-            archived: ''
-        }, function(response) {
-            service.jobs = response.results;
-
-            service.run_ids = service.jobs.map(function(job) {
-                return job.run_id;
-            }).filter(function(run_id, index, run_ids) {
-                return run_id && run_ids.indexOf(run_id) == index;
-            }).sort();
-            service.run_ids.push('');
-
-            if (service.job) {
-                // show the run id of the current job
-                service.show[service.job.run_id] = true;
-
-                // get the current job from the jobs list
-                var current_job = $filter('filter')(service.jobs, {
-                    'id': service.job.id
-                })[0];
-
-                // if the phase has changed, fetch it again
-                if (current_job && current_job.phase != service.job.phase) {
-                    service.activate_job(service.job);
-                }
+        service.submitFormModal = function(resource, close) {
+
+            var promise;
+            if (angular.isDefined(service.values.id)) {
+                promise = resources[resource].update({
+                    id: service.values.id
+                }, service.values).$promise;
+            } else {
+                promise = resources[resource].save(service.values).$promise;
             }
 
-        }).$promise;
-    };
+            promise.then(function(result) {
+                if (angular.isUndefined(close) || close) {
+                    $('.modal').modal('hide');
+
+                    service.activateItem(resource, result.id).$promise.then(function() {
+                        if (resource === 'functions') {
+                            service.initFunctionsBrowser();
+                        } else {
+                            service.initSchemasBrowser();
+                        }
+                    });
+                }
+            }, function(result) {
+                service.errors = result.data;
+            });
+        };
 
-    service.fetch_job = function(job) {
-        return resources.jobs.get({
-            id: job.id
-        }, function(response) {
-            service.job = response;
-
-            // get the current job in the jobs list
-            var jobs_job = $filter('filter')(service.jobs, {
-                'id': service.job.id
-            })[0]
-
-            if (angular.isUndefined(jobs_job) || jobs_job.phase != service.job.phase) {
-                // if the phase has changed, fetch the job list again
-                service.fetch_jobs();
-            }
-        }).$promise;
-    };
+        service.openDeleteModal = function(resource) {
+            service.values = service.active;
+            $('#' + resource + '-delete-modal').modal('show');
+        };
+
+        service.submitDeleteModal = function(resource) {
+            return resources[resource].remove({
+                id: service.values.id
+            }, function() {
+                $('#' + resource + '-delete-modal').modal('hide');
 
-    service.activate_form = function(key) {
-        // this function should be called from the form service
-        service.form = key;
-        service.job = null;
-    };
-
-    service.submit_job = function(values) {
-        // this function should be called from the form service
-        values = angular.extend({}, values, {
-            'queue': service.active_queue
-        });
+                service.active = false;
 
-        service.submitting = true;
-        return resources.jobs.save(values).$promise
-            .then(function(job) {
-                service.fetch_status();
-                service.activate_job(job);
-            }).finally(function() {
-                service.submitting = false;
+                if (resource === 'functions') {
+                    service.initFunctionsBrowser();
+                } else {
+                    service.initSchemasBrowser();
+                }
             });
-    };
+        };
 
-    service.activate_job = function(job) {
-        service.form = null;
-        service.fetch_job(job).then(function() {
-            service.table.ready = false;
-            service.plot.ready = false;
-
-            if (service.job.phase == 'COMPLETED') {
-                // re-init current tab
-                service.init_tab(service.tab);
-            } else {
-                // activate overview tab
-                service.activate_tab('overview');
+        service.discoverItem = function(resource) {
+            var parameters = {
+                list_action: 'discover'
+            };
+
+            if (resource === 'tables') {
+                parameters['schema'] = $filter('filter')(service.schemas, {
+                    'id': service.values.schema
+                })[0].name;
+                parameters['table'] = service.values.name;
+            } else if (resource === 'columns') {
+                var split = $filter('filter')(service.tables, {
+                    'id': service.values.table
+                })[0].label.split('.');
+
+                parameters['schema'] = split[0];
+                parameters['table'] = split[1];
+                parameters['column'] = service.values.name;
             }
 
-            CodeMirror.runMode(service.job.query, "text/x-sql", angular.element('#query')[0]);
+            return resources[resource].query(parameters, function(response) {
+                angular.extend(service.values, response[0]);
+            });
+        };
 
-            if (service.job.native_query) {
-                CodeMirror.runMode(service.job.native_query, "text/x-sql", angular.element('#native-query')[0]);
+        service.addPerson = function(person_type) {
+            if (service.values[person_type] === null) {
+                service.values[person_type] = []
             }
-            if (service.job.actual_query) {
-                CodeMirror.runMode(service.job.actual_query, "text/x-sql", angular.element('#actual-query')[0]);
-            }
-        });
-    };
+            service.values[person_type].push(service.factory.persons());
+        };
 
-    service.modal = function(modal_id) {
-        service.errors = {};
-        service.values = service.job;
-
-        $('#' + modal_id).modal('show');
-    };
-
-    service.update_job = function() {
-        resources.jobs.update({
-            id: service.values.id
-        }, service.values).$promise.then(function() {
-            service.fetch_jobs();
-            $('.modal').modal('hide');
-        }, function(response) {
-            service.errors = response.data;
-        });
-    };
+        service.removePerson = function(person_type, index) {
+            service.values[person_type].splice(index, 1);
+        };
 
-    service.abort_job = function() {
-        resources.jobs.update({
-            id: service.values.id,
-            detail_route: 'abort'
-        }, {}, function() {
-            service.fetch_status();
-            service.fetch_jobs();
-            $('.modal').modal('hide');
-        });
-    };
+        return service;
+    }])
 
-    service.archive_job = function() {
-        var index = service.jobs.indexOf($filter('filter')(service.jobs, {
-            'id': service.job.id
-        })[0]);
-
-        var next_job = null;
-        if (index == 0 && angular.isDefined(service.jobs[1])) {
-            next_job = service.jobs[1];
-        } else if (angular.isDefined(service.jobs[index - 1])) {
-            next_job = service.jobs[index - 1];
-        }
-
-        resources.jobs.delete({
-            id: service.values.id
-        }, function() {
-            service.fetch_status();
-            service.fetch_jobs();
+    .controller('MetadataController', ['$scope', 'MetadataService', function($scope, MetadataService) {
 
-            if (next_job) {
-                service.activate_job(next_job);
-            } else {
-                service.first_form.activate();
-            }
+        $scope.service = MetadataService;
+        $scope.service.init();
 
-            $('.modal').modal('hide');
+        $scope.$on('browserItemClicked', function(event, resource, item) {
+            MetadataService.activateItem(resource, item.id);
         });
-    };
-
-    service.activate_tab = function(tab) {
-        service.init_tab(tab);
-        service.tab = tab;
-    };
-
-    service.init_tab = function(tab) {
-        if (tab == 'results') {
-            if (!service.table.ready) {
-                if (service.job && service.job.phase == 'COMPLETED') {
-                    service.table.init({
-                        rows_url: 'query/api/jobs/' + service.job.id + '/rows/',
-                        columns_url: 'query/api/jobs/' + service.job.id + '/columns/',
-                        files_url: 'files/api/files/',
-                        references_url: 'serve/api/references/',
-                        params: {
-                            job: service.job.id
-                        }
-                    });
-                } else {
-                    service.table.clear();
-                }
-            }
-        } else if (tab == 'plot') {
-            if (!service.plot.ready) {
-                if (service.job && service.job.phase == 'COMPLETED') {
-                    service.plot.init({
-                        rows_url: 'query/api/jobs/' + service.job.id + '/rows/',
-                        columns: service.job.columns
-                    });
-                } else {
-                    service.plot.clear();
-                }
-            }
-        } else if (tab == 'download') {
-            service.downloads.init({
-                job: service.job
-            });
-        }
-    }
-
-    return service;
 
-}]);
+        $scope.$on('browserDblItemClicked', function(event, resource, item) {
+            MetadataService.openFormModal(resource);
+        });
+    }]);
```

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/services/examples.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/examples.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/static/query/js/apps/query.js` & `django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/query.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -23,14 +23,32 @@
                     scope.timeout = null;
                 }
             });
         }
     };
 }]);
 
+
+app.directive('tooltip', function() {
+    return {
+        restrict: 'A',
+        link: function(scope, element, attrs) {
+            element.hover(function() {
+                element.tooltip('show');
+            }, function() {
+                element.tooltip('hide');
+                // hide all other open tooltips
+                // clarification: sometimes tooltips are rendered multiple times due to the re-rendering after an API request
+                $('[data-toggle="tooltip"], .tooltip').tooltip("hide");
+            });
+        }
+    };
+});
+
+
 app.controller('QueryController', ['$scope', 'QueryService', function($scope, QueryService) {
 
     $scope.service = QueryService;
     $scope.service.init();
 
 
     $('.daiquiri-query-dropdowns .dropdown-menu').on('click', function(event) {
```

### Comparing `django-daiquiri-0.2/daiquiri/query/filters.py` & `django-daiquiri-0.4.2/daiquiri/query/filters.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/jobs_modal_show_job.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/jobs_modal_show_job.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_sidebar.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_sidebar.html`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
                     You are using {{ size }} of your quota of {{ quota }}.
                     {% endblocktrans %}
                 </p>
                 <p ng-show="service.status.size > service.status.quota">
                     {% trans 'The Quota is exceeded. Please remove some  jobs.' %}
                 </p>
             </div>
+
+            {% include 'query/query_sidebar_status_extra.html' %}
         </div>
     </div>
 
     <div class="panel panel-default">
         <div class="panel-heading">
             {% trans 'New query job' %}
         </div>
```

#### html2text {}

```diff
@@ -8,14 +8,15 @@
 {% blocktrans with size='{$ service.status.size | bytes $}' quota='{$
 service.status.quota | bytes $}' %} The guest user is using {{ size }} of its
 quota of {{ quota }}. {% endblocktrans %}
 {% blocktrans with size='{$ service.status.size | bytes $}' quota='{$
 service.status.quota | bytes $}' %} You are using {{ size }} of your quota of {
 { quota }}. {% endblocktrans %}
 {% trans 'The Quota is exceeded. Please remove some jobs.' %}
+{% include 'query/query_sidebar_status_extra.html' %}
 {% trans 'New query job' %}
     * {% for form in settings.QUERY_FORMS %}
     * {{ form.label }}
     * {% endfor %}
 {% trans 'Job list' %}
     * {% trans 'No jobs found.' %}
     *
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_overview.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_overview.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load i18n %}
 
 <p>
     On this page, you can find an overview about a submitted query job. For a table view of the results, the plotting tool, and to access the download form, please use the tabs at the top of the page.
 </p>
 
-<div class="panel panel-default">
+<div class="panel panel-default" ng-show="service.job.query">
     <div class="panel-heading">
         {% trans 'Query' %}
     </div>
     <div class="panel-body">
         <div class="cm-s-default" id="query">
             {$ service.job.query $}
         </div>
@@ -45,16 +45,18 @@
 
             <dt>{% trans 'Internal job id' %}</dt>
             <dd>{$ service.job.id $}</dd>
 
             <dt>{% trans 'Time submitted' %}</dt>
             <dd>{$ service.job.creation_time $}</dd>
 
-            <dt>{% trans 'Queue' %}</dt>
-            <dd>{$ (service.queues|filter: {'id': service.job.queue})[0].text $}</dd>
+            <div ng-show="service.job.queue">
+                <dt>{% trans 'Queue' %}</dt>
+                <dd>{$ (service.queues|filter: {'id': service.job.queue})[0].text $}</dd>
+            </div>
 
             <div ng-show="service.job.start_time && service.job.creation_time">
                 <dt>{% trans 'Time in queue' %}</dt>
                 <dd>{$ service.job.time_queue $} s</dd>
             </div>
 
             <div ng-show="service.job.end_time && service.job.start_time">
@@ -68,15 +70,15 @@
             </div>
 
             <div ng-show="service.job.size != null">
                 <dt>{% trans 'Size of the table' %}</dt>
                 <dd>{$ service.job.size | bytes $}</dd>
             </div>
 
-            <div ng-show="service.job.sources">
+            <div ng-show="service.job.sources.length">
                 <dt>{% trans 'Source tables' %}</dt>
                 <dd ng-repeat="source in service.job.sources">
                     <a href="{$ source.url $}" target="blank">
                         {$ source.schema_name $}.{$ source.table_name $}
                     </a>
                 </dd>
             </div>
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_modal_update_job.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_update_job.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core/wide.html' %}
-{% load staticfiles %}
+{% load static %}
 {% load compress %}
 {% load i18n %}
-{% load core_tags %}
+{% load vendor_tags %}
 
 {% block bodyargs %}ng-app="query" ng-controller="QueryController"{% endblock %}
 
 {% block headextra %}
     {% vendor 'angular' %}
     {% vendor 'ng-infinite-scroll' %}
     {% vendor 'codemirror' %}
@@ -15,14 +15,15 @@
 
     {% compress css %}
     <link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/browser.scss' %}" />
     <link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/table.scss' %}" />
     <link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/codemirror.scss' %}" />
 
     <link rel="stylesheet" type="text/x-scss" href="{% static 'query/css/query.scss' %}" />
+    <link rel="stylesheet" type="text/x-scss" href="{% static 'query/css/plot.scss' %}" />
     {% endcompress css %}
 
     {% compress js %}
     <script type="text/javascript" src="{% static 'core/js/core.js' %}" ></script>
     <script type="text/javascript" src="{% static 'core/js/filter.js' %}" ></script>
     <script type="text/javascript" src="{% static 'core/js/multiCheckbox.js' %}" ></script>
     <script type="text/javascript" src="{% static 'core/js/byNumber.js' %}" ></script>
@@ -32,14 +33,20 @@
     <script type="text/javascript" src="{% static 'core/js/polling.js' %}" ></script>
 
     <script type="text/javascript" src="{% static 'query/js/apps/query.js' %}" ></script>
     <script type="text/javascript" src="{% static 'query/js/services/query.js' %}" ></script>
     <script type="text/javascript" src="{% static 'query/js/services/plot.js' %}" ></script>
     <script type="text/javascript" src="{% static 'query/js/services/download.js' %}" ></script>
 
+    {% for download in settings.QUERY_DOWNLOADS %}
+    {% if download.service %}
+    <script type="text/javascript" src="{% static download.service %}" ></script>
+    {% endif %}
+    {% endfor %}
+
     {% for dropdown in settings.QUERY_DROPDOWNS %}
     <script type="text/javascript" src="{% static dropdown.service %}" ></script>
     {% endfor %}
 
     {% for form in settings.QUERY_FORMS %}
     <script type="text/javascript" src="{% static form.service %}" ></script>
     {% endfor %}
@@ -105,9 +112,10 @@
 
         </div>
     </div>
 
 {% include 'query/query_modal_update_job.html' %}
 {% include 'query/query_modal_abort_job.html' %}
 {% include 'query/query_modal_archive_job.html' %}
+{% include 'query/query_modal_logout.html' %}
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
-{% extends 'core/wide.html' %} {% load staticfiles %} {% load compress %} {%
-load i18n %} {% load core_tags %} {% block bodyargs %}ng-app="query" ng-
+{% extends 'core/wide.html' %} {% load static %} {% load compress %} {% load
+i18n %} {% load vendor_tags %} {% block bodyargs %}ng-app="query" ng-
 controller="QueryController"{% endblock %} {% block headextra %} {% vendor
 'angular' %} {% vendor 'ng-infinite-scroll' %} {% vendor 'codemirror' %} {%
 vendor 'moment' %} {% vendor 'Bokeh' %} {% compress css %}
 
 
 
+
  {% endcompress css %} {% compress js %}
- {% for dropdown in settings.QUERY_DROPDOWNS %}
+ {% for download in settings.QUERY_DOWNLOADS %} {% if download.service %}
+ {% endif %} {% endfor %} {% for dropdown in settings.QUERY_DROPDOWNS %}
  {% endfor %} {% for form in settings.QUERY_FORMS %}
  {% endfor %} {% endcompress js %} {% endblock %} {% block wide %}
 ****** {% trans 'Query interface' %} ******
 {% include 'query/query_sidebar.html' %}
 {% for form in settings.QUERY_FORMS %} {% include 'query/query_form.html' %} {%
 endfor %}
 ***** {% trans 'Query job' %} `{$ service.job.table_name $}` *****
@@ -21,8 +23,8 @@
     * {% trans 'Download' %}
 {% include 'query/query_overview.html' %}
 {% include 'query/query_results.html' %}
 {% include 'query/query_plot.html' %}
 {% include 'query/query_download.html' %}
 {% include 'query/query_modal_update_job.html' %} {% include 'query/
 query_modal_abort_job.html' %} {% include 'query/query_modal_archive_job.html'
-%} {% endblock %}
+%} {% include 'query/query_modal_logout.html' %} {% endblock %}
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_examples.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_examples.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_columns.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_columns.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_form_box.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_box.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/examples_modal_delete.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_modal_delete.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_form_sql.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_sql.html`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,20 @@
     {% endblocktrans %}
 </p>
 
 <div class="daiquiri-query-dropdowns">
     {% include 'query/query_dropdown_schemas.html' %}
     {% include 'query/query_dropdown_columns.html' %}
 
+    {% if user.is_authenticated %}
+      {% if settings.QUERY_DROPDOWN_FUNCTIONS %}
+          {% include 'query/query_dropdown_functions.html' %}
+      {% endif %}
+    {% endif %}
+
     {% for dropdown in settings.QUERY_DROPDOWNS %}
     {% include dropdown.template %}
     {% endfor %}
 
     {% include 'query/query_dropdown_examples.html' %}
 </div>
 
@@ -70,17 +76,19 @@
 </div>
 
 <div class="form-group">
     <button class="btn btn-primary" ng-click="service.forms.sql.submit()">
         {% trans 'Submit new SQL Query' %} <submitting />
     </button>
 
-    <button class="btn btn-default pull-right" ng-click="service.forms.sql.clear_query()">
-        {% trans 'Clear input window' %}
-    </button>
+    <div class="pull-right">
+        <button class="btn btn-default" ng-click="service.forms.sql.clear_query()">
+            {% trans 'Clear input window' %}
+        </button>
+    </div>
 </div>
 
 <p class="text-danger" ng-show="service.forms.sql.errors.detail">
     {$ service.forms.sql.errors.detail $}
 </p>
 <p class="text-danger" ng-show="service.forms.sql.errors.server_error">
     {% trans 'There has been an error on the server. Please contact the maintainers of this site, if the problem persists.' %}
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_vizier.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_vizier.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     <div class="daiquiri-query-dropdown-head">
         <form class="daiquiri-query-dropdown-form" ng-submit="service.dropdowns.vizier.query()">
             <div class="input-group">
                 <input type="text" class="form-control"
                     placeholder="{% trans 'Object name or coordinates' %}"
                     ng-model="service.dropdowns.vizier.values.query"/>
                 <span class="input-group-btn">
-                    <input type="submit" class="btn btn-default">
-                        {% trans 'Search on VizieR' %}
-                    </input>
+                    <input type="submit" class="btn btn-default" value="{% trans 'Search on VizieR' %}" />
                 </span>
             </div>
         </form>
     </div>
 
     <div class="daiquiri-query-dropdown-body">
         <ul class="text-danger list-unstyled">
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 {% load i18n %}  {% trans 'VizieR' %}
-[                    ]  [Submit] {% trans 'Search on VizieR' %}
+[                    ]  [{% trans 'Search on VizieR' %}]
     * {$ error $}
 {$ row.id $} {$ row.ra $} {$ row.de $} {$ row.distance $} {$ row.catalog $}
 {% trans 'A click will paste a value into the query field.' %}
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/jobs.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/jobs.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core/wide.html' %}
-{% load staticfiles %}
+{% load static %}
 {% load i18n %}
 {% load compress %}
-{% load core_tags %}
+{% load vendor_tags %}
 
 {% block bodyargs %}
     ng-app="jobs"
     ng-controller="JobsController"
 {% endblock %}
 
 {% block headextra %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends 'core/wide.html' %} {% load staticfiles %} {% load i18n %} {% load
-compress %} {% load core_tags %} {% block bodyargs %} ng-app="jobs" ng-
+{% extends 'core/wide.html' %} {% load static %} {% load i18n %} {% load
+compress %} {% load vendor_tags %} {% block bodyargs %} ng-app="jobs" ng-
 controller="JobsController" {% endblock %} {% block headextra %} {% vendor
 'angular' %} {% vendor 'ng-infinite-scroll' %} {% vendor 'codemirror' %} {%
 compress css %}
 
 
  {% endcompress css %} {% compress js %}
  {% endcompress js %} {% endblock %} {% block wide %}
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/examples.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/examples.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core/wide.html' %}
-{% load staticfiles %}
+{% load static %}
 {% load i18n %}
 {% load compress %}
-{% load core_tags %}
+{% load vendor_tags %}
 
 {% block bodyargs %}ng-app="examples" ng-controller="ExamplesController"{% endblock %}
 
 {% block headextra %}
     {% vendor 'angular' %}
     {% vendor 'ng-infinite-scroll' %}
     {% vendor 'codemirror' %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends 'core/wide.html' %} {% load staticfiles %} {% load i18n %} {% load
-compress %} {% load core_tags %} {% block bodyargs %}ng-app="examples" ng-
+{% extends 'core/wide.html' %} {% load static %} {% load i18n %} {% load
+compress %} {% load vendor_tags %} {% block bodyargs %}ng-app="examples" ng-
 controller="ExamplesController"{% endblock %} {% block headextra %} {% vendor
 'angular' %} {% vendor 'ng-infinite-scroll' %} {% vendor 'codemirror' %} {%
 compress css %}
 
 
  {% endcompress css %} {% compress js %}
  {% endcompress js %} {% endblock %} {% block wide %}
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_schemas.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_schemas.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_modal_archive_job.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_abort_job.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 {% load i18n %}
 
-<div class="modal" id="archive-job-modal" tabindex="-1">
+<div class="modal" id="abort-job-modal" tabindex="-1">
     <div class="modal-dialog">
         <div class="modal-content">
             <div class="modal-header">
                 <button type="button" class="close" data-dismiss="modal">
                     <span aria-hidden="true">&times;</span>
                 </button>
                 <h4 class="modal-title">
-                    {% trans 'Archive job' %}
+                    {% trans 'Abort job' %}
                 </h4>
             </div>
 
             <div class="modal-body">
                 <p>
                     {% blocktrans trimmed with table_name='{$ service.values.table_name $}' %}
-                    You are about to archive the job <code>{{ table_name }}</code>.
+                    You are about to abort the job <code>{{ table_name }}</code>.
                     {% endblocktrans %}
                 </p>
                 <p class="text-danger">
                     {% trans 'This action cannot be undone!' %}
                 </p>
             </div>
 
             <div class="modal-footer">
                 <button type="button" class="btn btn-default" data-dismiss="modal">
                     {% trans 'Close' %}
                 </button>
                 <button type="button" class="btn btn-danger"
-                        ng-click="service.archive_job()">
-                    {% trans 'Archive' %}
+                        ng-click="service.abort_job()">
+                    {% trans 'Abort' %}
                 </button>
             </div>
         </div>
     </div>
 </div>
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_dropdown_simbad.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_simbad.html`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     <div class="daiquiri-query-dropdown-head">
         <form class="daiquiri-query-dropdown-form" ng-submit="service.dropdowns.simbad.query()">
             <div class="input-group">
                 <input type="text" class="form-control"
                     placeholder="{% trans 'Object name' %}"
                     ng-model="service.dropdowns.simbad.values.query"/>
                 <span class="input-group-btn">
-                    <input type="submit" class="btn btn-default">
-                        {% trans 'Search on SIMBAD' %}
-                    </input>
+                    <input type="submit" class="btn btn-default" value="{% trans 'Search on SIMBAD' %}" />
                 </span>
             </div>
         </form>
     </div>
 
     <div class="daiquiri-query-dropdown-body">
         <ul class="text-danger list-unstyled">
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 {% load i18n %}  {% trans 'Simbad' %}
-[                    ]  [Submit] {% trans 'Search on SIMBAD' %}
+[                    ]  [{% trans 'Search on SIMBAD' %}]
     * {$ error $}
 {$ row.object $} {$ row.type $} {$ row.ra $} {$ row.de $}
 {% trans 'A click will paste a coordinate into the query field.' %}
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_modal_abort_job.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_functions.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 {% load i18n %}
 
-<div class="modal" id="abort-job-modal" tabindex="-1">
-    <div class="modal-dialog">
-        <div class="modal-content">
-            <div class="modal-header">
-                <button type="button" class="close" data-dismiss="modal">
-                    <span aria-hidden="true">&times;</span>
-                </button>
-                <h4 class="modal-title">
-                    {% trans 'Abort job' %}
-                </h4>
-            </div>
+    <div class="modal" id="functions-delete-modal" tabindex="-1">
+        <div class="modal-dialog">
+            <div class="modal-content">
+                <div class="modal-header">
+                    <button type="button" class="close" data-dismiss="modal">
+                        <span aria-hidden="true">&times;</span>
+                    </button>
+                    <h4 class="modal-title">
+                        {% trans 'Delete function' %}
+                    </h4>
+                </div>
 
-            <div class="modal-body">
-                <p>
-                    {% blocktrans trimmed with table_name='{$ service.values.table_name $}' %}
-                    You are about to abort the job <code>{{ table_name }}</code>.
-                    {% endblocktrans %}
-                </p>
-                <p class="text-danger">
-                    {% trans 'This action cannot be undone!' %}
-                </p>
-            </div>
+                <div class="modal-body">
+                    <p>
+                        {% blocktrans trimmed %}
+                        You are about to permanently delete the metadata for the function <strong>{$ service.values.name $}</strong>.
+                        {% endblocktrans %}
+                    </p>
+                    <p class="text-danger">
+                        {% trans 'This action cannot be undone!' %}
+                    </p>
+                </div>
 
-            <div class="modal-footer">
-                <button type="button" class="btn btn-default" data-dismiss="modal">
-                    {% trans 'Close' %}
-                </button>
-                <button type="button" class="btn btn-danger"
-                        ng-click="service.abort_job()">
-                    {% trans 'Abort' %}
-                </button>
+                <div class="modal-footer">
+                    <button type="button" class="btn btn-default" data-dismiss="modal">
+                        {% trans 'Close' %}
+                    </button>
+                    <button type="button" class="btn btn-danger"
+                            ng-click="service.submitDeleteModal('functions')">
+                        {% trans 'Delete' %}
+                    </button>
+                </div>
             </div>
         </div>
     </div>
-</div>
```

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/query_form_cone.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_cone.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/templates/query/examples_modal_form.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_modal_form.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/query/models.py` & `django-daiquiri-0.4.2/daiquiri/query/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,74 @@
-import json
 import logging
 import os
-import six
-
 from collections import OrderedDict
 
-from celery.task.control import revoke
-
 from django.conf import settings
 from django.contrib.auth.models import Group
-from django.core.cache import cache
 from django.db import models
-from django.db.utils import OperationalError, ProgrammingError
-from django.urls import reverse
-from django.utils.encoding import python_2_unicode_compatible
+from django.db.utils import (DataError, InternalError, OperationalError,
+                             ProgrammingError)
 from django.utils.functional import cached_property
-from django.utils.translation import ugettext_lazy as _
+from django.utils.timezone import now
+from django.utils.translation import gettext_lazy as _
 
 from rest_framework.exceptions import ValidationError
 
-from jsonfield import JSONField
-
-from queryparser.mysql import MySQLQueryProcessor
-from queryparser.postgresql import PostgreSQLQueryProcessor
-from queryparser.adql import ADQLQueryTranslator
-from queryparser.exceptions import QueryError, QuerySyntaxError
-
 from daiquiri.core.adapter import DatabaseAdapter, DownloadAdapter
 from daiquiri.core.constants import ACCESS_LEVEL_CHOICES
-from daiquiri.jobs.models import Job
+from daiquiri.core.generators import generate_votable
+from daiquiri.files.utils import check_file
 from daiquiri.jobs.managers import JobManager
-from daiquiri.files.utils import check_file, search_file
+from daiquiri.jobs.models import Job
+from daiquiri.stats.models import Record
 
-from .managers import QueryJobManager, ExampleManager
-from .utils import (
-    get_quota,
-    get_max_active_jobs,
-    get_default_table_name,
-    get_format_config,
-    get_user_schema_name,
-    get_asterisk_columns,
-    get_indexed_objects,
-    check_permissions
-)
-from .process import (
-    process_schema_name,
-    process_table_name,
-    process_query_language,
-    process_queue,
-    process_response_format
-)
-from .tasks import run_query, create_download_file, create_archive_file
+from .managers import ExampleManager, QueryJobManager
+from .process import (check_number_of_active_jobs, check_permissions,
+                      check_quota, process_display_columns, process_user_columns, process_query,
+                      process_query_language, process_queue,
+                      process_response_format, process_schema_name,
+                      process_table_name, translate_query)
+from .tasks import (abort_databae_query_task, create_download_archive_task,
+                    create_download_table_task, drop_database_table_task,
+                    rename_database_table_task, run_database_ingest_task,
+                    run_database_query_task)
+from .utils import get_format_config, get_job_columns, get_job_sources
 
 logger = logging.getLogger(__name__)
+query_logger = logging.getLogger('query')
 
 
 class QueryJob(Job):
 
     objects = QueryJobManager()
 
     schema_name = models.CharField(max_length=256)
     table_name = models.CharField(max_length=256)
-    queue = models.CharField(max_length=16)
+    queue = models.CharField(max_length=16, blank=True)
 
-    query_language = models.CharField(max_length=16)
-    query = models.TextField()
-    native_query = models.TextField(null=True, blank=True)
-    actual_query = models.TextField(null=True, blank=True)
+    query_language = models.CharField(max_length=16, blank=True)
+    query = models.TextField(blank=True)
+    native_query = models.TextField(blank=True)
+    actual_query = models.TextField(blank=True)
 
-    queue = models.CharField(max_length=16, null=True, blank=True)
+    queue = models.CharField(max_length=16, blank=True)
     nrows = models.BigIntegerField(null=True, blank=True)
     size = models.BigIntegerField(null=True, blank=True)
 
-    metadata = JSONField(blank=True)
+    metadata = models.JSONField(null=True, blank=True)
+    uploads = models.JSONField(null=True, blank=True)
 
     pid = models.IntegerField(null=True, blank=True)
 
     class Meta:
         ordering = ('start_time', )
 
         verbose_name = _('QueryJob')
         verbose_name_plural = _('QueryJobs')
 
-        permissions = (('view_queryjob', 'Can view QueryJob'),)
-
     @property
     def parameters(self):
         return {
             'schema_name': self.schema_name,
             'table_name': self.table_name,
             'query_language': self.query_language,
             'query': self.query,
@@ -96,15 +77,15 @@
             'queue': self.queue,
             'nrows': self.nrows,
             'size': self.size
         }
 
     @property
     def formats(self):
-        return {item['key']: item['content_type'] for item in settings.QUERY_DOWNLOAD_FORMATS}
+        return OrderedDict((item['key'], item['content_type']) for item in settings.QUERY_DOWNLOAD_FORMATS)
 
     @property
     def result_status(self):
         return 'OK' if self.max_records is None else 'OVERFLOW'
 
     @property
     def quote(self):
@@ -123,254 +104,241 @@
             return (self.end_time - self.start_time).total_seconds()
         else:
             return None
 
     @property
     def timeout(self):
         if self.queue:
-            return six.next((queue['timeout'] for queue in settings.QUERY_QUEUES if queue['key'] == self.queue))
+            return next((queue['timeout'] for queue in settings.QUERY_QUEUES if queue['key'] == self.queue))
         else:
             return 10
 
-    @property
-    def priority(self):
-        return six.next((queue['priority'] for queue in settings.QUERY_QUEUES if queue['key'] == self.queue))
-
     @cached_property
     def column_names(self):
         return [column['name'] for column in self.metadata['columns']]
 
-    def process(self):
+    def process(self, upload=False):
+        # log the query to the query log
+        query_logger.info('"%s" %s %s', self.query, self.query_language, self.owner or 'anonymous')
+
+        # check quota and number of active jobs
+        check_quota(self)
+        check_number_of_active_jobs(self)
 
-        # process all the things!
-        self.schema_name = process_schema_name(self.schema_name, self.owner)
+        # process schema_name, table_name and response format
+        self.schema_name = process_schema_name(self.owner, self.schema_name)
         self.table_name = process_table_name(self.table_name)
-        self.query_language = process_query_language(self.query_language)
-        self.queue = process_queue(self.queue)
         self.response_format = process_response_format(self.response_format)
 
-        # set the execution_duration to the queues timeout
-        self.execution_duration = self.timeout
-
-        # check quota
-        if QueryJob.objects.get_size(self.owner) > get_quota(self.owner):
-            raise ValidationError({
-                'query': [_('Quota is exceeded. Please remove some of your jobs.')]
-            })
-
-        # check number of active jobs
-        max_active_jobs = get_max_active_jobs(self.owner)
-        if max_active_jobs and max_active_jobs <= QueryJob.objects.get_active(self.owner).count():
-            raise ValidationError({
-                'query': [_('Too many active jobs. Please abort some of your active jobs or wait until they are completed.')]
-            })
-
-        # get the adapter
-        adapter = DatabaseAdapter()
-
-        # log the input query
-        logger.debug('query = "%s"', self.query)
-
-        # translate adql -> mysql string
-        if self.query_language == 'adql-2.0':
-            try:
-                translator = cache.get_or_set('translator', ADQLQueryTranslator(), 3600)
-                translator.set_query(self.query)
-
-                if adapter.database_config['ENGINE'] == 'django.db.backends.mysql':
-                    translated_query = translator.to_mysql()
-                elif adapter.database_config['ENGINE'] == 'django.db.backends.postgresql':
-                    translated_query = translator.to_postgresql()
-                else:
-                    raise Exception('Unknown database engine')
-
-            except QuerySyntaxError as e:
-                raise ValidationError({
-                    'query': {
-                        'messages': [_('There has been an error while translating your query.')],
-                        'positions': json.dumps(e.syntax_errors),
-                    }
-                })
-
-            except QueryError as e:
+        if upload:
+            self.query = ''
+            self.query_language = ''
+            self.queue = ''
+            self.execution_duration = 0.0
+
+        else:
+            self.query_language = process_query_language(self.owner, self.query_language)
+            self.queue = process_queue(self.owner, self.queue)
+            self.response_format = process_response_format(self.response_format)
+
+            # set the execution_duration to the queues timeout
+            self.execution_duration = self.timeout
+
+            # log the input query to the debug log
+            logger.debug('query = "%s"', self.query)
+
+            # translate the query from adql
+            translated_query = translate_query(self.query_language, self.query)
+
+            # log the translated query to the debug log
+            logger.debug('translated_query = "%s"', translated_query)
+
+            processor = process_query(translated_query)
+
+            # log the processor output to the debug log
+            logger.debug('native_query = "%s"', processor.query)
+            logger.debug('processor.keywords = %s', processor.keywords)
+            logger.debug('processor.tables = %s', processor.tables)
+            logger.debug('processor.columns = %s', processor.columns)
+            logger.debug('processor.functions = %s', processor.functions)
+
+            # check permissions
+            permission_messages = check_permissions(
+                self.owner,
+                processor.keywords,
+                processor.tables,
+                processor.columns,
+                processor.functions
+            )
+            if permission_messages:
                 raise ValidationError({
-                    'query': {
-                        'messages': e.messages,
-                    }
+                    'query': permission_messages
                 })
 
-        else:
-            translated_query = self.query
-
-        # log the translated query
-        logger.debug('translated_query = "%s"', translated_query)
+            # initialize metadata and store map of aliases
+            self.metadata = {
+                'display_columns': process_display_columns(processor.display_columns),
+                'user_columns': process_user_columns(self, processor.tables),
+                'tables': processor.tables
+            }
 
-        # parse the query
-        try:
-            if adapter.database_config['ENGINE'] == 'django.db.backends.mysql':
-                processor = MySQLQueryProcessor(translated_query)
-            elif adapter.database_config['ENGINE'] == 'django.db.backends.postgresql':
-
-                processor = cache.get_or_set('processor', PostgreSQLQueryProcessor(indexed_objects=get_indexed_objects()), 3600)
-                processor.set_query(translated_query)
-                processor.process_query()
-            else:
-                raise Exception('Unknown database engine')
+            # get the native query from the processor (without trailing semicolon)
+            self.native_query = processor.query.rstrip(';')
 
-            processor.process_query(replace_schema_name={
-                'TAP_SCHEMA': settings.TAP_SCHEMA
-            })
+            # set clean flag
+            self.is_clean = True
 
-        except QuerySyntaxError as e:
-            raise ValidationError({
-                'query': {
-                    'messages': [_('There has been an error while parsing your query.')],
-                    'positions': json.dumps(e.syntax_errors),
-                }
-            })
-
-        except QueryError as e:
-            raise ValidationError({
-                'query': {
-                    'messages': e.messages,
-                }
-            })
-
-        # log the native query
-        logger.debug('native_query = "%s"', processor.query)
+    def run(self):
+        if not self.is_clean:
+            raise Exception('job.process() was not called.')
 
-        # log the processor output
-        logger.debug('processor.keywords = %s', processor.keywords)
-        logger.debug('processor.tables = %s', processor.tables)
-        logger.debug('processor.columns = %s', processor.columns)
-        logger.debug('processor.functions = %s', processor.functions)
-
-        # check permissions
-        permission_messages = check_permissions(self.owner, processor.keywords, processor.tables, processor.columns, processor.functions)
-        if permission_messages:
-            raise ValidationError({
-                'query': permission_messages
-            })
+        if self.phase == self.PHASE_PENDING:
+            self.phase = self.PHASE_QUEUED
+            self.save()
 
-        # process display_columns to expand *
-        display_columns = []
-        for display_column in processor.display_columns:
-            if display_column[0] == '*':
-                display_columns += get_asterisk_columns(display_column)
-            else:
-                display_columns.append(display_column)
+            # start the submit_query task in a syncronous or asuncronous way
+            job_id = str(self.id)
+            if not settings.ASYNC:
+                logger.info('job %s submitted (sync)' % self.id)
+                run_database_query_task.apply((job_id, ), task_id=job_id, throw=True)
 
-        # check for duplicate columns in display_columns
-        display_column_names = [column_name for column_name, column in display_columns]
-        seen = set()
-        duplicate_columns = []
-        for column_name in display_column_names:
-            if column_name not in seen:
-                seen.add(column_name)
             else:
-                duplicate_columns.append(column_name)
+                queue = 'query_{}'.format(self.queue)
+                logger.info('job %s submitted (async, queue=%s)' % (self.id, queue))
+                run_database_query_task.apply_async((job_id, ), task_id=job_id, queue=queue)
 
-        if duplicate_columns:
+        else:
             raise ValidationError({
-                'query': [_('Duplicate column name \'%(column)s\'') % {
-                    'column': duplicate_column
-                } for duplicate_column in duplicate_columns]
+                'phase': ['Job is not PENDING.']
             })
 
-        # initialize metadata and store map of aliases
-        self.metadata = {
-            'display_columns': OrderedDict(display_columns),
-            'tables': processor.tables
-        }
+    def run_sync(self):
+        adapter = DatabaseAdapter()
 
-        # get the native query from the processor (without trailing semicolon)
-        self.native_query = processor.query.rstrip(';')
+        self.actual_query = adapter.build_sync_query(
+            self.native_query,
+            settings.QUERY_SYNC_TIMEOUT,
+            self.max_records
+        )
+
+        job_sources = get_job_sources(self)
+
+        # create a stats record for this job
+        Record.objects.create(
+            time=now(),
+            resource_type='QUERY',
+            resource={
+                'job_id': None,
+                'job_type': self.job_type,
+                'query': self.query,
+                'query_language': self.query_language,
+                'sources': job_sources
+            },
+            client_ip=self.client_ip,
+            user=self.owner
+        )
 
-        # set clean flag
-        self.is_clean = True
+        try:
+            download_adapter = DownloadAdapter()
 
-    def run(self, sync=False):
-        if not self.is_clean:
-            raise Exception('job.process() was not called.')
+            yield from generate_votable(adapter.fetchall(self.actual_query), get_job_columns(self),
+                                        table=download_adapter.get_table_name(self.schema_name, self.table_name),
+                                        infos=download_adapter.get_infos('OK', self.query, self.query_language, job_sources),
+                                        links=download_adapter.get_links(job_sources),
+                                        services=download_adapter.get_services())
+            self.drop_uploads()
 
+        except (OperationalError, ProgrammingError, InternalError, DataError):
+            raise StopIteration()
+
+    def ingest(self, file_path):
         if self.phase == self.PHASE_PENDING:
             self.phase = self.PHASE_QUEUED
             self.save()
 
-            # start the submit_query task in a syncronous or asuncronous way
-            job_id = str(self.id)
-            if not settings.ASYNC or sync:
-                logger.info('job %s submitted (sync)' % self.id)
-                run_query.apply((job_id, ), task_id=job_id, throw=True)
-
+            if not settings.ASYNC:
+                run_database_ingest_task.apply((self.id, file_path), throw=True)
             else:
-                logger.info('job %s submitted (async, queue=query, priority=%s)' % (self.id, self.priority))
-                run_query.apply_async((job_id, ), task_id=job_id, queue='query', priority=self.priority)
+                run_database_ingest_task.apply_async((self.id, file_path), queue='download')
 
         else:
             raise ValidationError({
                 'phase': ['Job is not PENDING.']
             })
 
     def abort(self):
-        if settings.ASYNC:
-            # first, revoke the task in celery, regardless the phase
-            revoke(str(self.id))
-
         current_phase = self.phase
-
         if current_phase in self.PHASE_ACTIVE:
             # next, set the phase to ABORTED
             self.phase = self.PHASE_ABORTED
             self.save()
 
             # finally, abort query, this will trigger OperationalError in the run_query task
             if current_phase == self.PHASE_EXECUTING:
                 self.abort_query()
 
     def archive(self):
         self.abort()
         self.drop_table()
+        self.drop_uploads()
         self.phase = self.PHASE_ARCHIVED
         self.nrows = None
         self.size = None
         self.save()
 
     def rename_table(self, new_table_name):
         if self.table_name != new_table_name:
-            DatabaseAdapter().rename_table(self.schema_name, self.table_name, new_table_name)
-
             self.metadata['name'] = new_table_name
             self.save()
 
+            task_args = (self.schema_name, self.table_name, new_table_name)
+
+            if not settings.ASYNC:
+                rename_database_table_task.apply(task_args, throw=True)
+            else:
+                rename_database_table_task.apply_async(task_args)
+
     def drop_table(self):
-        # drop the corresponding database table, but fail silently
-        try:
-            DatabaseAdapter().drop_table(self.schema_name, self.table_name)
-        except ProgrammingError:
-            pass
+        task_args = (self.schema_name, self.table_name)
+
+        if not settings.ASYNC:
+            drop_database_table_task.apply(task_args, throw=True)
+        else:
+            drop_database_table_task.apply_async(task_args)
+
+    def drop_uploads(self):
+        if self.uploads:
+            for table_name, file_path in self.uploads.items():
+                task_args = (settings.TAP_UPLOAD, table_name)
+
+                if not settings.ASYNC:
+                    drop_database_table_task.apply(task_args, throw=True)
+                else:
+                    drop_database_table_task.apply_async(task_args)
 
     def abort_query(self):
-        # abort the job on the database
-        try:
-            DatabaseAdapter().abort_query(self.pid)
-        except OperationalError:
-            # the query was probably killed before
-            pass
+        task_args = (self.pid, )
+
+        if not settings.ASYNC:
+            abort_databae_query_task.apply(task_args, throw=True)
+        else:
+            abort_databae_query_task.apply_async(task_args)
 
     def stream(self, format_key):
         if self.phase == self.PHASE_COMPLETED:
             return DownloadAdapter().generate(
                 format_key,
-                self.schema_name,
-                self.table_name,
-                self.metadata.get('columns'),
-                self.metadata.get('sources'),
-                self.result_status,
-                (self.nrows == 0)
+                self.metadata.get('columns', []),
+                sources=self.metadata.get('sources', []),
+                schema_name=self.schema_name,
+                table_name=self.table_name,
+                nrows=self.nrows,
+                query_status=self.result_status,
+                query=self.query,
+                query_language=self.query_language
             )
         else:
             raise ValidationError({
                 'phase': ['Job is not COMPLETED.']
             })
 
     def rows(self, column_names, ordering, page, page_size, search, filters):
@@ -416,16 +384,16 @@
             return []
 
 
 class DownloadJob(Job):
 
     objects = JobManager()
 
-    job = models.ForeignKey(
-        QueryJob, related_name='downloads',
+    query_job = models.ForeignKey(
+        QueryJob, related_name='downloads', on_delete=models.CASCADE,
         verbose_name=_('QueryJob'),
         help_text=_('QueryJob this DownloadJob belongs to.')
     )
     format_key = models.CharField(
         max_length=32,
         verbose_name=_('Format key'),
         help_text=_('Format key for this download.')
@@ -433,34 +401,32 @@
 
     class Meta:
         ordering = ('start_time', )
 
         verbose_name = _('DownloadJob')
         verbose_name_plural = _('DownloadJobs')
 
-        permissions = (('view_downloadjob', 'Can view DownloadJob'),)
-
     @property
     def file_path(self):
         if not self.owner:
             username = 'anonymous'
         else:
             username = self.owner.username
 
         format_config = get_format_config(self.format_key)
 
         if format_config:
             directory_name = os.path.join(settings.QUERY_DOWNLOAD_DIR, username)
-            return os.path.join(directory_name, '%s.%s' % (self.job.table_name, format_config['extension']))
+            return os.path.join(directory_name, '%s.%s' % (self.query_job.table_name, format_config['extension']))
         else:
             return None
 
     def process(self):
-        if self.job.phase == self.PHASE_COMPLETED:
-            self.owner = self.job.owner
+        if self.query_job.phase == self.PHASE_COMPLETED:
+            self.owner = self.query_job.owner
         else:
             raise ValidationError({
                 'phase': ['Job is not COMPLETED.']
             })
 
         # set clean flag
         self.is_clean = True
@@ -472,19 +438,19 @@
         if self.phase == self.PHASE_PENDING:
             self.phase = self.PHASE_QUEUED
             self.save()
 
             download_id = str(self.id)
             if not settings.ASYNC:
                 logger.info('download_job %s submitted (sync)' % download_id)
-                create_download_file.apply((download_id, ), task_id=download_id, throw=True)
+                create_download_table_task.apply((download_id, ), task_id=download_id, throw=True)
 
             else:
                 logger.info('download_job %s submitted (async, queue=download)' % download_id)
-                create_download_file.apply_async((download_id, ), task_id=download_id, queue='download')
+                create_download_table_task.apply_async((download_id, ), task_id=download_id, queue='download')
 
         else:
             raise ValidationError({
                 'phase': ['Job is not PENDING.']
             })
 
     def delete_file(self):
@@ -495,78 +461,70 @@
             pass
 
 
 class QueryArchiveJob(Job):
 
     objects = JobManager()
 
-    job = models.ForeignKey(
-        QueryJob, related_name='archives',
+    query_job = models.ForeignKey(
+        QueryJob, related_name='archives', on_delete=models.CASCADE,
         verbose_name=_('QueryJob'),
         help_text=_('QueryJob this ArchiveJob belongs to.')
     )
     column_name = models.CharField(
         max_length=32,
         verbose_name=_('Column name'),
         help_text=_('Column name for this download.')
     )
-    files = JSONField(
+    files = models.JSONField(
         verbose_name=_('Files'),
         help_text=_('List of files in the archive.')
     )
 
     class Meta:
         ordering = ('start_time', )
 
         verbose_name = _('QueryArchiveJob')
         verbose_name_plural = _('QueryArchiveJob')
 
-        permissions = (('view_queryarchivejob', 'Can view QueryArchiveJob'),)
-
     @property
     def file_path(self):
         if not self.owner:
             username = 'anonymous'
         else:
             username = self.owner.username
 
         directory_name = os.path.join(settings.QUERY_DOWNLOAD_DIR, username)
-        return os.path.join(directory_name, '%s.%s.zip' % (self.job.table_name, self.column_name))
+        return os.path.join(directory_name, '%s.%s.zip' % (self.query_job.table_name, self.column_name))
 
     def process(self):
-        try:
-            get_format_config(self.format_key)
-        except IndexError:
-            raise ValidationError({'format_key': "Not supported."})
-
-        if self.job.phase == self.PHASE_COMPLETED:
-            self.owner = self.job.owner
+        if self.query_job.phase == self.PHASE_COMPLETED:
+            self.owner = self.query_job.owner
         else:
             raise ValidationError({
                 'phase': ['Job is not COMPLETED.']
             })
 
         if not self.column_name:
             raise ValidationError({
                 'column_name': [_('This field may not be blank.')]
             })
 
-        if self.column_name not in self.job.column_names:
+        if self.column_name not in self.query_job.column_names:
             raise ValidationError({
                 'column_name': [_('Unknown column "%s".') % self.column_name]
             })
 
         # get database adapter and query the paginated rowset
-        rows = DatabaseAdapter().fetch_rows(self.job.schema_name, self.job.table_name, [self.column_name], page_size=0)
+        rows = DatabaseAdapter().fetch_rows(self.query_job.schema_name, self.query_job.table_name, [self.column_name], page_size=0)
 
         # prepare list of files for this job
         files = []
-
         for row in rows:
-            file_path = search_file(row[0])
+            file_path = row[0]
 
             # append the file to the list of files  if it exists
             if file_path and check_file(self.owner, file_path):
                 files.append(file_path)
             else:
                 raise ValidationError({
                     'files': [_('One or more of the files cannot be found.')]
@@ -585,33 +543,32 @@
         if self.phase == self.PHASE_PENDING:
             self.phase = self.PHASE_QUEUED
             self.save()
 
             archive_id = str(self.id)
             if not settings.ASYNC:
                 logger.info('archive_job %s submitted (sync)' % archive_id)
-                create_archive_file.apply((archive_id, ), task_id=archive_id, throw=True)
+                create_download_archive_task.apply((archive_id, ), task_id=archive_id, throw=True)
 
             else:
                 logger.info('archive_job %s submitted (async, queue=download)' % archive_id)
-                create_archive_file.apply_async((archive_id, ), task_id=archive_id, queue='download')
+                create_download_archive_task.apply_async((archive_id, ), task_id=archive_id, queue='download')
 
         else:
             raise ValidationError({
                 'phase': ['Job is not PENDING.']
             })
 
     def delete_file(self):
         try:
             os.remove(self.file_path)
         except OSError:
             pass
 
 
-@python_2_unicode_compatible
 class Example(models.Model):
 
     objects = ExampleManager()
 
     order = models.IntegerField(
         null=True, blank=True,
         verbose_name=_('Order'),
@@ -648,11 +605,9 @@
 
     class Meta:
         ordering = ('order',)
 
         verbose_name = _('Example')
         verbose_name_plural = _('Examples')
 
-        permissions = (('view_example', 'Can view Example'),)
-
     def __str__(self):
         return self.name
```

### Comparing `django-daiquiri-0.2/daiquiri/query/management/commands/fix_jobs.py` & `django-daiquiri-0.4.2/daiquiri/query/management/commands/fix_query_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from django.conf import settings
 from django.core.management.base import BaseCommand
 from django.db.utils import ProgrammingError
 
 from rest_framework.exceptions import ValidationError
 
 from daiquiri.core.adapter import DatabaseAdapter
 from daiquiri.query.models import QueryJob
 
 
 class Command(BaseCommand):
 
-
     def add_arguments(self, parser):
         parser.add_argument('--user', help='Only fix jobs for this user.')
         parser.add_argument('--queue', help='Name of the queue to use.')
         parser.add_argument('--dry', action='store_true', help='Perform a dryrun.')
 
     def handle(self, *args, **options):
         # look for completed jobs with no table
```

### Comparing `django-daiquiri-0.2/daiquiri/query/viewsets.py` & `django-daiquiri-0.4.2/daiquiri/query/viewsets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,80 @@
 import os
 
 from collections import OrderedDict
 
-from sendfile import sendfile
+from django_sendfile import sendfile
 
 from django.conf import settings
 from django.http import Http404, FileResponse
 
 from rest_framework import viewsets, mixins, filters
 from rest_framework.response import Response
 from rest_framework.exceptions import ValidationError, NotFound
-from rest_framework.decorators import list_route, detail_route
+from rest_framework.decorators import action
 from rest_framework.authentication import (
     SessionAuthentication,
     BasicAuthentication,
     TokenAuthentication
 )
 
 from daiquiri.core.viewsets import ChoicesViewSet, RowViewSetMixin
 from daiquiri.core.permissions import HasModelPermission
 from daiquiri.core.paginations import ListPagination
-from daiquiri.core.utils import get_client_ip, replace_nan
+from daiquiri.core.utils import (
+    get_client_ip,
+    fix_for_json,
+    filter_by_access_level,
+    handle_file_upload,
+    import_class
+)
 from daiquiri.jobs.viewsets import SyncJobViewSet, AsyncJobViewSet
 
-from .models import QueryJob, DownloadJob, QueryArchiveJob, Example
+from .models import QueryJob, DownloadJob, Example
 from .serializers import (
     FormSerializer,
     DropdownSerializer,
+    DownloadSerializer,
     QueryJobSerializer,
     QueryJobListSerializer,
     QueryJobRetrieveSerializer,
     QueryJobCreateSerializer,
     QueryJobUpdateSerializer,
+    QueryJobUploadSerializer,
     QueryLanguageSerializer,
     ExampleSerializer,
     UserExampleSerializer,
     SyncQueryJobSerializer,
     AsyncQueryJobSerializer
 )
 from .permissions import HasPermission
-from .utils import get_format_config, get_quota, fetch_user_schema_metadata
+from .utils import (
+    get_download_config,
+    get_format_config,
+    get_quota,
+    get_user_upload_directory,
+    fetch_user_schema_metadata,
+    handle_upload_param,
+    ingest_uploads
+)
+
 from .filters import JobFilterBackend
 
 
 class StatusViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
     permission_classes = (HasPermission, )
     queryset = []
 
     def list(self, request):
         return Response([{
-            'guest': not request.user.is_authenticated(),
+            'guest': not request.user.is_authenticated,
             'queued_jobs': None,
             'size': QueryJob.objects.get_size(request.user),
-            'quota': get_quota(request.user)
+            'quota': get_quota(request.user),
+            'upload_limit': get_quota(request.user, quota_settings='QUERY_UPLOAD_LIMIT')
         }])
 
 
 class FormViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
     permission_classes = (HasPermission, )
 
     serializer_class = FormSerializer
@@ -70,14 +88,23 @@
 
     serializer_class = DropdownSerializer
 
     def get_queryset(self):
         return settings.QUERY_DROPDOWNS
 
 
+class DownloadViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
+    permission_classes = (HasPermission, )
+
+    serializer_class = DownloadSerializer
+
+    def get_queryset(self):
+        return settings.QUERY_DOWNLOADS
+
+
 class QueryJobViewSet(RowViewSetMixin, viewsets.ModelViewSet):
     permission_classes = (HasPermission, )
     authentication_classes = (SessionAuthentication, BasicAuthentication, TokenAuthentication)
     pagination_class = ListPagination
 
     filter_backends = (
         filters.SearchFilter,
@@ -86,16 +113,16 @@
     )
     search_fields = ('id', 'run_id', 'table_name', 'phase')
     filter_fields = ('phase', )
 
     def get_queryset(self):
         queryset = QueryJob.objects.filter_by_owner(self.request.user).order_by('-creation_time')
 
-        # hide TAP jobs in the list for the anonymous user
-        if self.action == 'list' and self.request.user.is_anonymous:
+        # hide TAP queries for the anonymous user
+        if self.request.user.is_anonymous:
             queryset = queryset.filter(job_type=QueryJob.JOB_TYPE_INTERFACE)
 
         return queryset
 
     def get_serializer_class(self):
         if self.action == 'list':
             return QueryJobListSerializer
@@ -113,15 +140,15 @@
             self.throttle_scope = 'query.create'
 
         return super(QueryJobViewSet, self).get_throttles()
 
     def perform_create(self, serializer):
         job = QueryJob(
             job_type=QueryJob.JOB_TYPE_INTERFACE,
-            owner=(None if self.request.user.is_anonymous() else self.request.user),
+            owner=(None if self.request.user.is_anonymous else self.request.user),
             run_id=serializer.data.get('run_id'),
             table_name=serializer.data.get('table_name'),
             query_language=serializer.data.get('query_language'),
             query=serializer.data.get('query'),
             queue=serializer.data.get('queue'),
             client_ip=get_client_ip(self.request)
         )
@@ -134,196 +161,184 @@
 
     def perform_update(self, serializer):
         serializer.save()
 
     def perform_destroy(self, instance):
         instance.archive()
 
-    @list_route(methods=['get'])
+    @action(detail=False, methods=['get'])
     def tables(self, request):
-        return Response(fetch_user_schema_metadata(request.user, self.get_queryset()))
+        queryset = self.get_queryset().filter(phase=QueryJob.PHASE_COMPLETED)[:100]
+        return Response(fetch_user_schema_metadata(request.user, queryset))
 
-    @detail_route(methods=['put'])
+    @action(detail=False, methods=['post'], url_path='upload', url_name='upload')
+    def upload(self, request):
+
+        if not settings.QUERY_UPLOAD:
+            raise Http404
+
+        serializer = QueryJobUploadSerializer(data=request.data, context={
+            'request': request,
+            'view': self
+        })
+        serializer.is_valid(raise_exception=True)
+
+        file_name = handle_file_upload(get_user_upload_directory(self.request.user), serializer.validated_data['file'])
+
+        job = QueryJob(
+            job_type=QueryJob.JOB_TYPE_INTERFACE,
+            owner=(None if self.request.user.is_anonymous else self.request.user),
+            run_id=serializer.validated_data.get('run_id'),
+            table_name=serializer.validated_data.get('table_name'),
+            client_ip=get_client_ip(self.request)
+        )
+        job.process(upload=True)
+        job.save()
+        job.ingest(file_name)
+
+        serializer = QueryJobRetrieveSerializer(instance=job)
+        return Response(serializer.data)
+
+    @action(detail=True, methods=['put'])
     def abort(self, request, pk=None):
         try:
             job = self.get_queryset().get(pk=pk)
             job.abort()
 
             serializer = QueryJobRetrieveSerializer(instance=job)
             return Response(serializer.data)
         except QueryJob.DoesNotExist:
             raise Http404
 
-    @detail_route(methods=['get'])
+    @action(detail=True, methods=['get'])
     def rows(self, request, pk=None):
         try:
             job = self.get_queryset().get(pk=pk)
         except QueryJob.DoesNotExist:
             raise NotFound
 
+        # get the row query params from the request
+        ordering, page, page_size, search, filters = self._get_query_params(job.columns())
+
         # get column names from the request
         column_names = self.request.GET.getlist('column')
 
-        # get the row query params from the request
-        ordering, page, page_size, search, filters = self._get_query_params(column_names)
-
         # get the count and the rows from the job
         count, results = job.rows(column_names, ordering, page, page_size, search, filters)
 
-        replace_nan(results)
-
         # return ordered dict to be send as json
         return Response(OrderedDict((
             ('count', count),
-            ('results', results),
+            ('results', fix_for_json(results)),
             ('next', self._get_next_url(page, page_size, count)),
             ('previous', self._get_previous_url(page))
         )))
 
-    @detail_route(methods=['get'])
+    @action(detail=True, methods=['get'])
     def columns(self, request, pk=None, format_key=None):
         try:
             job = self.get_queryset().get(pk=pk)
         except QueryJob.DoesNotExist:
             raise NotFound
 
         return Response(job.columns())
 
-    @detail_route(methods=['get'], url_path='download/(?P<download_id>[A-Za-z0-9\-]+)', url_name='download')
-    def download(self, request, pk=None, download_id=None):
+    @action(detail=True, methods=['get'], url_name='download',
+            url_path=r'download/(?P<download_key>[a-z\-]+)/(?P<download_job_id>[A-Za-z0-9\-]+)')
+    def download(self, request, pk=None, download_key=None, download_job_id=None):
         try:
-            job = self.get_queryset().get(pk=pk)
+            self.get_queryset().get(pk=pk)
         except QueryJob.DoesNotExist:
             raise NotFound
 
+        download_config = get_download_config(download_key)
+        if download_config is None:
+            raise ValidationError({'download': 'Download key "{}" is not supported.'.format(download_key)})
+
+        download_job_model = import_class(download_config['model'])
+
         try:
-            download_job = job.downloads.get(pk=download_id)
-        except DownloadJob.DoesNotExist:
+            download_job = download_job_model.objects.get(query_job=pk, pk=download_job_id)
+        except download_job_model.DoesNotExist:
             raise NotFound
 
         if download_job.phase == download_job.PHASE_COMPLETED and request.GET.get('download', True):
             return sendfile(request, download_job.file_path, attachment=True)
         else:
             return Response(download_job.phase)
 
-    @detail_route(methods=['post'], url_path='download', url_name='create-download')
-    def create_download(self, request, pk=None):
+    @action(detail=True, methods=['post'], url_name='create-download',
+            url_path=r'download/(?P<download_key>[a-z\-]+)')
+    def create_download(self, request, pk=None, download_key=None):
         try:
             job = self.get_queryset().get(pk=pk)
         except QueryJob.DoesNotExist:
             raise NotFound
 
-        format_key = request.data.get('format_key')
+        download_config = get_download_config(download_key)
+        if download_config is None:
+            raise ValidationError({'download': 'Download key "{}" is not supported.'.format(download_key)})
+
+        download_job_model = import_class(download_config['model'])
+
+        params = {param: request.data.get(param) for param in download_config.get('params', [])}
 
         try:
-            download_job = DownloadJob.objects.get(job=job, format_key=format_key)
+            download_job = download_job_model.objects.get(query_job=job, **params)
 
             # check if the file was lost
             if download_job.phase == download_job.PHASE_COMPLETED and \
                     not os.path.isfile(download_job.file_path):
 
                 # set the phase back to pending so that the file is recreated
                 download_job.phase = download_job.PHASE_PENDING
                 download_job.process()
                 download_job.save()
                 download_job.run()
 
-        except DownloadJob.DoesNotExist:
-            download_job = DownloadJob(
+        except download_job_model.DoesNotExist:
+            download_job = download_job_model(
+                job_type=QueryJob.JOB_TYPE_INTERFACE,
+                owner=(None if self.request.user.is_anonymous else self.request.user),
                 client_ip=get_client_ip(self.request),
-                job=job,
-                format_key=format_key
+                query_job=job,
+                **params
             )
             download_job.process()
             download_job.save()
             download_job.run()
 
         return Response({
             'id': download_job.id
         })
 
-    @detail_route(methods=['get'], url_path='archive/(?P<archive_id>[A-Za-z0-9\-]+)', url_name='archive')
-    def archive(self, request, pk=None, archive_id=None):
-        try:
-            job = self.get_queryset().get(pk=pk)
-        except QueryJob.DoesNotExist:
-            raise NotFound
-
-        try:
-            archive_job = job.archives.get(pk=archive_id)
-        except QueryArchiveJob.DoesNotExist:
-            raise NotFound
-
-        if archive_job.phase == archive_job.PHASE_COMPLETED and request.GET.get('download', True):
-            return sendfile(request, archive_job.file_path, attachment=True)
-        else:
-            return Response(archive_job.phase)
-
-    @detail_route(methods=['post'], url_path='archive', url_name='create-archive')
-    def create_archive(self, request, pk=None):
-        try:
-            job = self.get_queryset().get(pk=pk)
-        except QueryJob.DoesNotExist:
-            raise NotFound
-
-        column_name = request.data.get('column_name')
-
-        try:
-            archive_job = QueryArchiveJob.objects.get(job=job, column_name=column_name)
-
-            # check if the file was lost
-            if archive_job.phase == archive_job.PHASE_COMPLETED and \
-                    not os.path.isfile(archive_job.file_path):
-
-                # set the phase back to pending so that the file is recreated
-                archive_job.phase = archive_job.PHASE_PENDING
-                archive_job.process()
-                archive_job.save()
-                archive_job.run()
-
-        except QueryArchiveJob.DoesNotExist:
-            archive_job = QueryArchiveJob(
-                client_ip=get_client_ip(self.request),
-                job=job,
-                column_name=column_name
-            )
-            archive_job.process()
-            archive_job.save()
-            archive_job.run()
-
-        return Response({
-            'id': archive_job.id
-        })
-
-    @detail_route(methods=['get'], url_path='stream/(?P<format_key>[A-Za-z0-9\-]+)', url_name='stream')
+    @action(detail=True, methods=['get'], url_path=r'stream/(?P<format_key>[A-Za-z0-9\-]+)', url_name='stream')
     def stream(self, request, pk=None, format_key=None):
         try:
             job = self.get_queryset().get(pk=pk)
         except QueryJob.DoesNotExist:
             raise NotFound
 
         try:
             format_config = get_format_config(format_key)
         except IndexError:
             raise ValidationError({'format': "Not supported."})
 
         try:
-            download_job = DownloadJob.objects.get(job=job, format_key=format_key)
+            download_job = DownloadJob.objects.get(query_job=job, format_key=format_key)
 
             # check if the file was lost
             if download_job.phase == download_job.PHASE_COMPLETED and os.path.isfile(download_job.file_path):
                 # stream the previously created file
-                return sendfile(request, download_job.file_path, attachment=True)
+                return sendfile(request, download_job.file_path)
         except DownloadJob.DoesNotExist:
             pass
 
         # stream the table directly from the database
-        file_name = '%s.%s' % (job.table_name, format_config['extension'])
         response = FileResponse(job.stream(format_key), content_type=format_config['content_type'])
-        response['Content-Disposition'] = "attachment; filename=%s" % file_name
         return response
 
 
 class ExampleViewSet(viewsets.ModelViewSet):
     permission_classes = (HasModelPermission, )
     serializer_class = ExampleSerializer
     pagination_class = ListPagination
@@ -331,30 +346,35 @@
 
     filter_backends = (
         filters.SearchFilter,
         filters.OrderingFilter
     )
     search_fields = ('name', 'description', 'query_string')
 
-    @list_route(methods=['get'], permission_classes=(HasPermission, ))
+    @action(detail=False, methods=['get'], permission_classes=(HasPermission, ))
     def user(self, request):
         examples = Example.objects.filter_by_access_level(self.request.user)
         serializer = UserExampleSerializer(examples, many=True)
         return Response(serializer.data)
 
 
 class QueueViewSet(ChoicesViewSet):
     permission_classes = (HasPermission, )
-    queryset = [(item['key'], item['label']) for item in settings.QUERY_QUEUES]
+
+    def get_queryset(self):
+        items = filter_by_access_level(self.request.user, settings.QUERY_QUEUES)
+        return [(item['key'], item['label']) for item in items]
 
 
 class QueryLanguageViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
     permission_classes = (HasPermission, )
     serializer_class = QueryLanguageSerializer
-    queryset = settings.QUERY_LANGUAGES
+
+    def get_queryset(self):
+        return filter_by_access_level(self.request.user, settings.QUERY_LANGUAGES)
 
 
 class PhaseViewSet(ChoicesViewSet):
     permission_classes = (HasPermission, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
     queryset = QueryJob.PHASE_CHOICES
 
@@ -369,14 +389,18 @@
         'LANG': 'query_language',
         'QUERY': 'query'
     }
 
     def get_queryset(self):
         return QueryJob.objects.filter_by_owner(self.request.user)
 
+    def handle_upload(self, job, upload_string):
+        job.uploads = handle_upload_param(self.request, upload_string)
+        ingest_uploads(job.uploads, job.owner)
+
 
 class AsyncQueryJobViewSet(AsyncJobViewSet):
     permission_classes = (HasPermission, )
     serializer_class = AsyncQueryJobSerializer
 
     parameter_map = {
         'FORMAT': 'response_format',
@@ -384,7 +408,10 @@
         'LANG': 'query_language',
         'QUEUE': 'queue',
         'QUERY': 'query'
     }
 
     def get_queryset(self):
         return QueryJob.objects.filter_by_owner(self.request.user)
+
+    def handle_upload(self, job, upload_string):
+        job.uploads = handle_upload_param(self.request, upload_string)
```

### Comparing `django-daiquiri-0.2/daiquiri/stats/views.py` & `django-daiquiri-0.4.2/daiquiri/stats/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/stats/migrations/0002_data_migration.py` & `django-daiquiri-0.4.2/daiquiri/stats/migrations/0002_data_migration.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,12 +21,13 @@
         )
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('daiquiri_stats', '0001_initial'),
         ('daiquiri_jobs', '0012_meta'),
+        ('daiquiri_query', '0013_refactoring')
     ]
 
     operations = [
         migrations.RunPython(migrate_jobs)
     ]
```

### Comparing `django-daiquiri-0.2/daiquiri/stats/migrations/0001_initial.py` & `django-daiquiri-0.4.2/daiquiri/stats/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/stats/templates/stats/management.html` & `django-daiquiri-0.4.2/daiquiri/stats/templates/stats/management.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/uws/urls.py` & `django-daiquiri-0.4.2/daiquiri/uws/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from django.conf import settings
-from django.conf.urls import url, include
-from django.views.generic import TemplateView
-
 from daiquiri.core.utils import import_class
 from daiquiri.jobs.routers import JobRouter
+from django.conf import settings
+from django.urls import include, re_path
+from django.views.generic import TemplateView
 
+app_name = 'uws'
 
 router = JobRouter(trailing_slash=False)
 
 '''
 add uws routes for the resources specified in the settings
 resources need to be of the form
 {
@@ -19,13 +19,13 @@
 '''
 try:
     resources = settings.UWS_RESOURCES
 except AttributeError:
     pass
 else:
     for resource in resources:
-        router.register(resource['prefix'], import_class(resource['viewset']), base_name=resource['base_name'])
+        router.register(resource['prefix'], import_class(resource['viewset']), basename=resource['base_name'])
 
 urlpatterns = [
-    url(r'^$', TemplateView.as_view(template_name='uws/root.html'), name='uws_root'),
-    url(r'', include(router.urls)),
+    re_path(r'^$', TemplateView.as_view(template_name='uws/root.html'), name='uws_root'),
+    re_path(r'', include(router.urls)),
 ]
```

### Comparing `django-daiquiri-0.2/daiquiri/cutout/viewsets.py` & `django-daiquiri-0.4.2/daiquiri/conesearch/viewsets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from django.utils.timezone import now
 
 from rest_framework.views import APIView
 from rest_framework.response import Response
+from rest_framework.renderers import JSONRenderer
 from rest_framework.authentication import SessionAuthentication, TokenAuthentication
 
 from daiquiri.core.utils import get_client_ip
 from daiquiri.stats.models import Record
 
-from .adapter import CutOutAdapter
-from .renderers import CutOutErrorRenderer
+from .adapter import ConeSearchAdapter
+from .renderers import ConeSearchErrorRenderer
 from .permissions import HasPermission
 
 
-class CutOutViewSet(APIView):
+class ConeSearchView(APIView):
 
     permission_classes = (HasPermission, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
-    renderer_classes = (CutOutErrorRenderer, )
+    renderer_classes = (ConeSearchErrorRenderer, JSONRenderer)
 
     def get(self, request, resource=None):
 
-        adapter = CutOutAdapter()
+        adapter = ConeSearchAdapter()
         adapter.clean(request, resource)
 
         if request.GET.get('download', True):
             # create a stats record for this cutout
             Record.objects.create(
                 time=now(),
-                resource_type='CUTOUT',
+                resource_type='CONESEARCH',
                 resource=adapter.args,
                 client_ip=get_client_ip(request),
                 user=request.user if request.user.is_authenticated else None
             )
 
             # stream the table
             return adapter.stream()
```

### Comparing `django-daiquiri-0.2/daiquiri/contact/serializers.py` & `django-daiquiri-0.4.2/daiquiri/contact/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/contact/utils.py` & `django-daiquiri-0.4.2/daiquiri/contact/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from django.urls import reverse
 
-from daiquiri.core.utils import send_mail, get_admin_emails
+from daiquiri.core.utils import send_mail, get_admin_emails, get_permission_emails
 
 
-def send_contact_message(request, message):
+def get_manager_emails():
+    return get_permission_emails((
+        'daiquiri_contact.view_contactmessage',
+    )) + get_admin_emails()
+
 
-    admin_emails = get_admin_emails()
+def send_contact_message(request, message):
+    # sends an email to the admins, managers and the user once a message was submitted.
     context = {
         'user': message.user,
         'author': message.author,
         'email': message.email,
         'subject': message.subject,
         'message': message.message,
         'url': request.build_absolute_uri(reverse('contact:messages'))
     }
-    send_mail(request, 'contact/email/new_message_admin', context, admin_emails)
+    send_mail(request, 'contact/email/new_message_admin', context, get_manager_emails())
     send_mail(request, 'contact/email/new_message_user', context, [message.email])
```

### Comparing `django-daiquiri-0.2/daiquiri/contact/views.py` & `django-daiquiri-0.4.2/daiquiri/contact/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+from django.contrib.auth.decorators import login_required
 from django.shortcuts import render
 from django.utils.timezone import now
 from django.views.generic import TemplateView
 
-from daiquiri.core.views import ModelPermissionMixin
+from daiquiri.core.views import CSRFViewMixin, ModelPermissionMixin
 
 from .forms import ContactForm
 from .utils import send_contact_message
 
 
+@login_required()
 def contact(request):
     contact_form = ContactForm(request.POST or None)
 
     if request.method == 'POST':
         if 'cancel' in request.POST:
             return render(request, 'core/home.html')
 
         if contact_form.is_valid():
 
             message = contact_form.save(commit=False)
             message.set_status_active()
             message.created = now()
 
-            if request.user.is_authenticated:
-                message.user = request.user
+            message.user = request.user
+            message.email = request.user.email
+            message.author = request.user.profile.full_name
 
             message.save()
 
             send_contact_message(request, message)
 
             return render(request, 'contact/thanks.html')
 
@@ -39,10 +42,10 @@
                 }
             except AttributeError:
                 pass
 
     return render(request, 'contact/contact.html', {'form': contact_form})
 
 
-class MessagesView(ModelPermissionMixin, TemplateView):
+class MessagesView(ModelPermissionMixin, CSRFViewMixin, TemplateView):
     template_name = 'contact/messages.html'
     permission_required = 'daiquiri_contact.view_contactmessage'
```

### Comparing `django-daiquiri-0.2/daiquiri/contact/migrations/0002_meta.py` & `django-daiquiri-0.4.2/daiquiri/contact/migrations/0002_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/contact/migrations/0004_meta.py` & `django-daiquiri-0.4.2/daiquiri/contact/migrations/0004_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/contact/migrations/0003_add_permissions.py` & `django-daiquiri-0.4.2/daiquiri/contact/migrations/0003_add_permissions.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/contact/migrations/0001_initial.py` & `django-daiquiri-0.4.2/daiquiri/contact/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/contact/static/contact/js/messages.js` & `django-daiquiri-0.4.2/daiquiri/contact/static/contact/js/messages.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/contact/templates/contact/messages_modal_show.html` & `django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_modal_show.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/contact/templates/contact/messages.html` & `django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core/wide.html' %}
-{% load staticfiles %}
+{% load static %}
 {% load i18n %}
 {% load compress %}
-{% load core_tags %}
+{% load vendor_tags %}
 
 {% block bodyargs %}ng-app="messages" ng-controller="MessagesController"{% endblock %}
 
 {% block headextra %}
     {% vendor 'angular' %}
     {% vendor 'ng-infinite-scroll' %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends 'core/wide.html' %} {% load staticfiles %} {% load i18n %} {% load
-compress %} {% load core_tags %} {% block bodyargs %}ng-app="messages" ng-
+{% extends 'core/wide.html' %} {% load static %} {% load i18n %} {% load
+compress %} {% load vendor_tags %} {% block bodyargs %}ng-app="messages" ng-
 controller="MessagesController"{% endblock %} {% block headextra %} {% vendor
 'angular' %} {% vendor 'ng-infinite-scroll' %} {% compress css %}
 
  {% endcompress css %} {% compress js %}
  {% endcompress js %} {% endblock %} {% block wide %}
 ****** Contact messages ******
 [                    ]
```

### Comparing `django-daiquiri-0.2/daiquiri/contact/templates/contact/messages_options.html` & `django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_options.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,24 @@
 {% load i18n %}
 {% load core_tags %}
 
     <a href="{% include 'contact/messages_mailto.html' %}" class="fa fa-reply"
         title="{% trans 'Reply to message' %}">
     </a>
-
     <a href="" class="fa fa-eye" title="{% trans 'Show message details' %}"
         ng-click="service.modal('show-message-modal', $index)">
     </a>
     <a href="" ng-show="row.status == 'ACTIVE'"
         class="fa fa-square-o" title="{% trans 'Close the thread' %} "
         ng-click="service.updateMessage(row, 'CLOSED')">
     </a>
     <a href="" ng-show="row.status == 'CLOSED'" class="fa fa-check" title="{% trans 'Open the thread' %}"
         ng-click="service.updateMessage(row, 'ACTIVE')">
     </a>
-
-    <div class="dropdown">
-        <a class="dropdown-toggle" type="button" id="messages-options"
-            data-toggle="dropdown" aria-haspopup="true" aria-expanded="true"
-            title="{% trans 'Show options' %}">
-            <span class="fa fa-ellipsis-h"></span>
-        </a>
-        <ul class="dropdown-menu dropdown-menu-right" aria-labelledby="messages-options">
-            <li>
-                <a href=""
-                    ng-hide="row.status == 'SPAM'"
-                    ng-click="service.updateMessage(row, 'SPAM')">
-                    <i class="fa fa-ban"></i>
-                    <span>{% trans 'Mark as spam' %}</span>
-                </a>
-            <li>
-            <li>
-                <a href=""
-                    ng-hide="row.status != 'SPAM'"
-                    ng-click="service.updateMessage(row, 'ACTIVE')">
-                    <i class="fa fa-check"></i>
-                    <span>{% trans 'Not spam' %}</span>
-                </a>
-            <li>
-        </ul>
-    </div>
+    <a href="" class="fa fa-ban" title="{% trans 'Mark as spam' %}"
+        ng-hide="row.status == 'SPAM'"
+        ng-click="service.updateMessage(row, 'SPAM')">
+    </a>
+    <a href="" class="fa fa-thumbs-o-up" title="{% trans 'Not spam' %}"
+        ng-hide="row.status != 'SPAM'"
+        ng-click="service.updateMessage(row, 'ACTIVE')">
+    </a>
```

#### html2text {}

```diff
@@ -1,3 +1 @@
 {% load i18n %} {% load core_tags %}
-    *  {% trans 'Mark as spam' %}
-    *  {% trans 'Not spam' %}
```

### Comparing `django-daiquiri-0.2/daiquiri/contact/models.py` & `django-daiquiri-0.4.2/daiquiri/contact/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from __future__ import unicode_literals
-
 from django.contrib.auth.models import User
 from django.db import models
-from django.utils.encoding import python_2_unicode_compatible
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
-@python_2_unicode_compatible
 class ContactMessage(models.Model):
 
     STATUS_ACTIVE = 'ACTIVE'
     STATUS_CLOSED = 'CLOSED'
     STATUS_SPAM = 'SPAM'
     STATUS_CHOICES = (
         (STATUS_ACTIVE, 'active'),
@@ -30,16 +26,14 @@
 
     class Meta:
         ordering = ('-created', 'author')
 
         verbose_name = _('Contact message')
         verbose_name_plural = _('Contact messages')
 
-        permissions = (('view_contactmessage', 'Can view ContactMessage'),)
-
     def __str__(self):
         return "created=%s; email=%s; subject=%s; status=%s" % (self.created, self.email, self.subject, self.status)
 
     def set_status_closed(self):
         self.status = self.STATUS_CLOSED
         self.save()
```

### Comparing `django-daiquiri-0.2/daiquiri/contact/viewsets.py` & `django-daiquiri-0.4.2/daiquiri/contact/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,13 +25,13 @@
     filter_backends = (
         filters.SearchFilter,
         filters.OrderingFilter,
         DjangoFilterBackend,
         SpamBackend
     )
     search_fields = ('author', 'email', 'subject', 'message', 'status')
-    filter_fields = ('status', )
+    filterset_fields = ('status', )
 
 
 class StatusViewSet(ChoicesViewSet):
     permission_classes = (IsAuthenticated, )
     queryset = ContactMessage.STATUS_CHOICES
```

### Comparing `django-daiquiri-0.2/daiquiri/meetings/migrations/0003_meta.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0016_rename_database_to_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 # -*- coding: utf-8 -*-
-# Generated by Django 1.11.9 on 2018-01-23 16:02
+# Generated by Django 1.11.10 on 2018-02-16 17:14
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('daiquiri_meetings', '0002_meeting_registration_done_message'),
+        ('daiquiri_metadata', '0015_change_doi_to_char'),
     ]
 
     operations = [
+        migrations.AlterModelOptions(
+            name='table',
+            options={'ordering': ('schema__order', 'order'), 'permissions': (('view_table', 'Can view Table'),), 'verbose_name': 'Table', 'verbose_name_plural': 'Tables'},
+        ),
+        migrations.RenameField(
+            model_name='table',
+            old_name='database',
+            new_name='schema',
+        ),
+        migrations.AlterField(
+            model_name='database',
+            name='attribution',
+            field=models.TextField(blank=True, help_text='The desired attribution for the schema.', null=True, verbose_name='Attribution'),
+        ),
         migrations.AlterField(
-            model_name='contribution',
-            name='abstract',
-            field=models.TextField(default='---', verbose_name='Abstract'),
-            preserve_default=False,
+            model_name='database',
+            name='description',
+            field=models.TextField(blank=True, help_text='A brief description of the schema to be displayed in the user interface.', null=True, verbose_name='Description'),
         ),
         migrations.AlterField(
-            model_name='meeting',
-            name='contributions_message',
-            field=models.TextField(blank=True, help_text='Message on contributions page, you can use Markdown here.', null=True, verbose_name='Contributions message'),
+            model_name='database',
+            name='groups',
+            field=models.ManyToManyField(blank=True, help_text='The groups which have access to the schema.', to='auth.Group', verbose_name='Groups'),
         ),
         migrations.AlterField(
-            model_name='meeting',
-            name='participants_message',
-            field=models.TextField(blank=True, help_text='Message on participants page, you can use Markdown here.', null=True, verbose_name='Participants message'),
+            model_name='database',
+            name='long_description',
+            field=models.TextField(blank=True, help_text='A more extensive description of the schema to be displayed on the public schema page.', null=True, verbose_name='Long description'),
         ),
         migrations.AlterField(
-            model_name='meeting',
-            name='registration_done_message',
-            field=models.TextField(blank=True, help_text='Message on the page displayed after registration, you can use Markdown here.', null=True, verbose_name='Registration done message'),
+            model_name='database',
+            name='name',
+            field=models.CharField(help_text='Name of the schema on the database server.', max_length=256, verbose_name='Name'),
         ),
         migrations.AlterField(
-            model_name='meeting',
-            name='registration_message',
-            field=models.TextField(blank=True, help_text='Message on registration page, you can use Markdown here.', null=True, verbose_name='Registration message'),
+            model_name='database',
+            name='title',
+            field=models.CharField(blank=True, help_text='Human readable title of the schema.', max_length=256, null=True, verbose_name='Title'),
         ),
     ]
```

### Comparing `django-daiquiri-0.2/daiquiri/meetings/forms.py` & `django-daiquiri-0.4.2/daiquiri/auth/forms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,107 @@
+
 from django import forms
 from django.conf import settings
-from django.utils.timezone import now
-from django.utils.translation import ugettext as _
-
-from daiquiri.core.utils import get_detail_fields
-
-from .models import Participant, Contribution
-
+from django.contrib.auth.models import User
+from django.core.exceptions import BadRequest
+from django.utils.translation import gettext as _
+
+from daiquiri.core.utils import get_detail_fields, sanitize_str
+
+from .models import Profile
+
+
+class HoneypotField(forms.CharField):
+    hpstyle = 'border: 1px dashed'
+    hplabel = settings.HONEYPOT_FIELD_NAME
+    if settings.HONEYPOT_FIELD_HIDDEN is True:
+        hpstyle = 'opacity: 0; position: absolute; top: 0; left: 0; height: 0; width: 0; z-index: -1;'
+        hplabel = ''
+    default_widget = forms.TextInput(
+        {'style': hpstyle, 'tabindex': '-1', 'autocomplete': 'off'}
+    )
 
-class ParticipantForm(forms.ModelForm):
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault('widget', HoneypotField.default_widget)
+        kwargs['required'] = False
+        kwargs['label'] = self.hplabel
+        super().__init__(*args, **kwargs)
+
+    def validate(self, value):
+        return value == settings.HONEYPOT_FIELD_VALUE
+
+    def clean(self, value):
+        cleaned_value = super().clean(value)
+        if self.validate(cleaned_value) is True:
+            return cleaned_value
+        else:
+            raise BadRequest('invalid request')
 
+class UserForm(forms.ModelForm):
     class Meta:
-        model = Participant
-        fields = ('first_name', 'last_name', 'email')
+        model = User
+        fields = ('first_name', 'last_name')
         widgets = {
             'first_name': forms.TextInput(attrs={'placeholder': _('First name')}),
             'last_name': forms.TextInput(attrs={'placeholder': _('Last name')}),
-            'email': forms.TextInput(attrs={'placeholder': _('Email')})
         }
 
+
+class ProfileForm(forms.ModelForm):
+
+    class Meta:
+        model = Profile
+        fields = ()
+
     def __init__(self, *args, **kwargs):
-        self.meeting = kwargs.pop('meeting')
-        super(ParticipantForm, self).__init__(*args, **kwargs)
+        super(ProfileForm, self).__init__(*args, **kwargs)
+
+        for key, field in get_detail_fields(settings.AUTH_DETAIL_KEYS):
+            if self.instance.details and key in self.instance.details:
+                field.initial = self.instance.details[key]
 
-        for key, field in get_detail_fields(settings.MEETINGS_PARTICIPANT_DETAIL_KEYS):
             self.fields[key] = field
 
     def save(self, *args, **kwargs):
-        # set the meeting and the current time
-        self.instance.meeting = self.meeting
-        self.instance.registered = now()
-
         # create an empty details dict if it does not exist
         if not self.instance.details:
             self.instance.details = {}
 
         # store the form date for each detail key
-        for detail_key in settings.MEETINGS_PARTICIPANT_DETAIL_KEYS:
+        for detail_key in settings.AUTH_DETAIL_KEYS:
             self.instance.details[detail_key['key']] = self.cleaned_data[detail_key['key']]
 
-        return super(ParticipantForm, self).save(*args, **kwargs)
-
-    def clean_email(self):
-        email = self.cleaned_data['email']
+        return super(ProfileForm, self).save(*args, **kwargs)
 
-        try:
-            self.meeting.participants.get(email=email)
-            self.add_error('email', _('You have already registred with this email address.'))
-        except Participant.DoesNotExist:
-            pass
 
-        return email
+class SignupForm(ProfileForm):
 
+    first_name = forms.CharField(max_length=30,
+        label=_('First name'), widget=forms.TextInput(attrs={'placeholder': _('First name')}))
+    last_name = forms.CharField(max_length=30,
+        label=_('Last name'), widget=forms.TextInput(attrs={'placeholder': _('Last name')}))
+    if settings.HONEYPOT_ENABLED is True:
+        locals()[sanitize_str(settings.HONEYPOT_FIELD_NAME)] = HoneypotField()
 
-class ContributionForm(forms.ModelForm):
+    field_order = ['username', 'email', 'password1', 'password2']
 
-    contribution_type = forms.ChoiceField(
-        choices=settings.MEETINGS_CONTRIBUTION_TYPES,
-        widget=forms.RadioSelect,
-        help_text=None,
-        required=None
-    )
-    title = forms.CharField(
-        widget=forms.TextInput(attrs={'placeholder': _('Title')}),
-        required=None
-    )
-    abstract = forms.CharField(
-        widget=forms.Textarea(attrs={'placeholder': _('Abstract')}),
-        required=None,
-        max_length=settings.MEETINGS_ABSTRACT_MAX_LENGTH,
-        help_text=_('The abstract needs to be shorter than %s characters.') % settings.MEETINGS_ABSTRACT_MAX_LENGTH
-    )
+    def __init__(self, *args, **kwargs):
+        super(SignupForm, self).__init__(*args, **kwargs)
 
-    class Meta:
-        model = Contribution
-        fields = ('contribution_type', 'title', 'abstract')
+        # add a consent field, the label is added in the template
+        if settings.AUTH_TERMS_OF_USE:
+            self.fields['consent'] = forms.BooleanField(required=True)
+
+    def signup(self, request, user):
+        # create an empty details dict
+        user.profile.details = {}
 
-    def clean(self):
-        cleaned_data = super(ContributionForm, self).clean()
+        # store the form date for each detail key
+        for detail_key in settings.AUTH_DETAIL_KEYS:
+            user.profile.details[detail_key['key']] = self.cleaned_data[detail_key['key']]
 
-        # if the contribution_type is set, title and abstract need to be provided
-        if 'contribution_type' in cleaned_data and cleaned_data['contribution_type']:
-            if not cleaned_data['title']:
-                self.add_error('title', _('This field is required.'))
+        # store the consent field
+        if settings.AUTH_TERMS_OF_USE:
+            user.profile.consent = self.cleaned_data['consent']
 
-            if not cleaned_data['abstract']:
-                self.add_error('abstract', _('This field is required.'))
-        else:
-            if cleaned_data['title'] or cleaned_data['abstract']:
-                self.add_error('contribution_type', _('This field is required.'))
+        # save the profile model
+        user.profile.save()
```

### Comparing `django-daiquiri-0.2/daiquiri/jobs/renderers.py` & `django-daiquiri-0.4.2/daiquiri/jobs/renderers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/serializers.py` & `django-daiquiri-0.4.2/daiquiri/jobs/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,52 +4,71 @@
 from daiquiri.jobs.models import Job
 
 from .utils import get_job_results
 
 
 class JobListSerializer(serializers.ModelSerializer):
 
+    creation_time = serializers.SerializerMethodField()
+
     class Meta:
         model = Job
         fields = ('id', 'phase', 'run_id', 'creation_time')
 
+    def get_creation_time(self, obj):
+        return obj.creation_time.strftime('%Y-%m-%dT%H:%M:%S.%fZ') if obj.creation_time else None
+
 
 class JobRetrieveSerializer(serializers.ModelSerializer):
 
     job_id = serializers.UUIDField(source='id')
     owner_id = serializers.SerializerMethodField()
     destruction = serializers.DateTimeField(source='destruction_time')
     results = serializers.SerializerMethodField()
 
+    creation_time = serializers.SerializerMethodField()
+    start_time = serializers.SerializerMethodField()
+    end_time = serializers.SerializerMethodField()
+
     class Meta:
         model = Job
         fields = (
             'job_id',
             'run_id',
             'owner_id',
             'phase',
             'quote',
             'creation_time',
             'start_time',
             'end_time',
             'execution_duration',
             'destruction',
+            'error_summary',
             'results',
             'parameters'
         )
 
     def get_owner_id(self, obj):
         if obj.owner:
             return obj.owner.username
         else:
             return None
 
     def get_results(self, obj):
         return get_job_results(self.context['request'], obj)
 
+    def get_creation_time(self, obj):
+        return obj.creation_time.strftime('%Y-%m-%dT%H:%M:%S.%fZ') if obj.creation_time else None
+
+    def get_start_time(self, obj):
+        return obj.start_time.strftime('%Y-%m-%dT%H:%M:%S.%fZ') if obj.start_time else None
+
+    def get_end_time(self, obj):
+        return obj.end_time.strftime('%Y-%m-%dT%H:%M:%S.%fZ') if obj.end_time else None
+
 
 class JobUpdateSerializer(CaseInsensitiveSerializer):
 
     ACTION = serializers.CharField(required=False)
     DESTRUCTION = serializers.DateTimeField(required=False)
     EXECUTIONDURATION = serializers.IntegerField(required=False)
     PHASE = serializers.CharField(required=False)
```

### Comparing `django-daiquiri-0.2/daiquiri/jobs/migrations/0012_meta.py` & `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0012_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/migrations/0005_owner_null_true.py` & `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0005_owner_null_true.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/migrations/0010_add_fields.py` & `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0010_add_fields.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/migrations/0001_job_model.py` & `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0001_job_model.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/migrations/0004_phases_to_char.py` & `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0004_phases_to_char.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/migrations/0003_owner_fk.py` & `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0003_owner_fk.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/migrations/0006_owner_blank_true.py` & `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0006_owner_blank_true.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/filters.py` & `django-daiquiri-0.4.2/daiquiri/jobs/filters.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/jobs/models.py` & `django-daiquiri-0.4.2/daiquiri/jobs/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from __future__ import unicode_literals
-
 import uuid
 
-from django.db import models
 from django.contrib.auth.models import User
-from django.utils.encoding import python_2_unicode_compatible
+from django.db import models
 from django.utils.timezone import now
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
-@python_2_unicode_compatible
 class Job(models.Model):
 
     PHASE_PENDING = 'PENDING'
     PHASE_QUEUED = 'QUEUED'
     PHASE_EXECUTING = 'EXECUTING'
     PHASE_COMPLETED = 'COMPLETED'
     PHASE_ERROR = 'ERROR'
@@ -48,25 +44,25 @@
         (JOB_TYPE_SYNC, _('Syncronous')),
         (JOB_TYPE_ASYNC, _('Asyncronous')),
         (JOB_TYPE_INTERFACE, _('Interface')),
     )
 
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
 
-    owner = models.ForeignKey(User, blank=True, null=True)
+    owner = models.ForeignKey(User, blank=True, null=True, on_delete=models.CASCADE)
 
     client_ip = models.GenericIPAddressField(blank=True, null=True)
 
     response_format = models.CharField(max_length=64, blank=True, null=True)
     max_records = models.IntegerField(blank=True, null=True)
-    run_id = models.CharField(max_length=64, blank=True, default='')
+    run_id = models.CharField(max_length=64, blank=True, default='', db_index=True)
 
-    phase = models.CharField(max_length=10, choices=PHASE_CHOICES)
+    phase = models.CharField(max_length=10, choices=PHASE_CHOICES, db_index=True)
 
-    creation_time = models.DateTimeField(blank=True, null=True)
+    creation_time = models.DateTimeField(blank=True, null=True, db_index=True)
     start_time = models.DateTimeField(blank=True, null=True)
     end_time = models.DateTimeField(blank=True, null=True)
     execution_duration = models.PositiveIntegerField(blank=True, default=0)
     destruction_time = models.DateTimeField(blank=True, null=True)
 
     error_summary = models.TextField(blank=True, null=True)
 
@@ -74,16 +70,14 @@
 
     class Meta:
         ordering = ('start_time', )
 
         verbose_name = _('Job')
         verbose_name_plural = _('Jobs')
 
-        permissions = (('view_job', 'Can view Job'),)
-
     def __str__(self):
         return str(self.id)
 
     def save(self, *args, **kwargs):
         if self.pk is None:
             self.phase = self.PHASE_PENDING
             self.creation_time = now()
@@ -108,14 +102,17 @@
 
     def process(self):
         raise NotImplementedError
 
     def run(self):
         raise NotImplementedError
 
+    def run_sync(self):
+        raise NotImplementedError
+
     def abort(self):
         raise NotImplementedError
 
     def archive(self):
         raise NotImplementedError
 
     def stream(self):
```

### Comparing `django-daiquiri-0.2/daiquiri/jobs/routers.py` & `django-daiquiri-0.4.2/daiquiri/jobs/routers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from rest_framework.routers import Route, DynamicRoute, SimpleRouter
 
 
 class JobRouter(SimpleRouter):
     '''
     A dedicated router for UWS services. The main difference is that a POST on an instance
-    maps to update, not PUT. Also list_routes are removed.
+    maps to update, not PUT. Also actions are removed.
     '''
 
     routes = [
         Route(
             url=r'^{prefix}$',
             mapping={
                 'get': 'list',
```

### Comparing `django-daiquiri-0.2/daiquiri/jobs/viewsets.py` & `django-daiquiri-0.4.2/daiquiri/jobs/viewsets.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,96 @@
 from django.http import HttpResponse, FileResponse
-from django.urls import reverse
-
 from rest_framework import viewsets
 from rest_framework.response import Response
-from rest_framework.parsers import FormParser
+from rest_framework.parsers import FormParser, MultiPartParser
 from rest_framework.exceptions import ValidationError
 from rest_framework.authentication import SessionAuthentication, BasicAuthentication, TokenAuthentication
-from rest_framework.decorators import detail_route
+from rest_framework.decorators import action
 
 from daiquiri.core.responses import HttpResponseSeeOther
 from daiquiri.core.utils import get_client_ip
 
 from .models import Job
 from .serializers import (
     JobListSerializer,
     JobRetrieveSerializer,
     JobUpdateSerializer,
     SyncJobSerializer,
     AsyncJobSerializer
 )
 from .renderers import UWSRenderer, UWSErrorRenderer
 from .filters import UWSFilterBackend
-from .utils import get_job_url, get_job_results
+from .utils import get_job_url, get_job_results, get_content_type
 
 
 class JobViewSet(viewsets.GenericViewSet):
 
     authentication_classes = (SessionAuthentication, BasicAuthentication, TokenAuthentication)
-    parser_classes = (FormParser, )
+    parser_classes = (FormParser, MultiPartParser)
 
     parameter_map = {}
 
     def rewrite_exception(self, exception):
         detail = {}
         for field, field_errors in exception.detail.items():
-            parameter = dict(map(reversed, self.parameter_map.items()))[field]
+            parameter = dict(map(reversed, self.parameter_map.items())).get(field, field.upper())
             detail[parameter] = field_errors
         return detail
 
+    def handle_upload(self, job, upload_string):
+        pass
+
 
 class SyncJobViewSet(JobViewSet):
 
     serializer_class = SyncJobSerializer
 
     renderer_classes = (UWSErrorRenderer, )
 
+    def list(self, request, *args, **kwargs):
+        serializer = self.get_serializer(data=request.GET)
+        serializer.is_valid(raise_exception=True)
+
+        return self.perform_sync_job(request, serializer.data)
+
     def create(self, request, *args, **kwargs):
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
+        return self.perform_sync_job(request, serializer.validated_data)
+
+    def perform_sync_job(self, request, data):
         # create the job objects
         job = self.get_queryset().model(
             job_type=Job.JOB_TYPE_SYNC,
-            owner=(None if self.request.user.is_anonymous() else self.request.user),
-            response_format=serializer.data.get('RESPONSEFORMAT'),
-            max_records=serializer.data.get('MAXREC'),
-            run_id=serializer.data.get('RUNID'),
+            owner=(None if self.request.user.is_anonymous else self.request.user),
+            response_format=data.get('RESPONSEFORMAT'),
+            max_records=data.get('MAXREC'),
+            run_id=data.get('RUNID'),
             client_ip=get_client_ip(self.request)
         )
 
         # add parameters to the job object
         for parameter, model_field in self.parameter_map.items():
-            value = serializer.data.get(parameter)
+            value = data.get(parameter)
             if value is not None:
                 setattr(job, model_field, value)
 
+        # handle possible uploads
+        try:
+            self.handle_upload(job, data.get('UPLOAD'))
+        except ValueError:
+            raise ValidationError('Could not parse VOTable')
+
         try:
             job.process()
         except ValidationError as e:
             raise ValidationError(self.rewrite_exception(e))
 
-        job.save()
-        job.run(sync=True)
-
-        # reload the job from the database since job.run() doesn't work on the same job object
-        job = self.get_queryset().get(pk=job.pk)
-
-        if job.phase == job.PHASE_COMPLETED:
-            return FileResponse(job.stream(job.response_format), content_type=job.formats[job.response_format])
-        else:
-            return Response(job.error_summary, content_type='application/xml')
+        return FileResponse(job.run_sync(), content_type=job.formats[job.response_format])
 
 
 class AsyncJobViewSet(JobViewSet):
 
     serializer_class = AsyncJobSerializer
     renderer_classes = (UWSErrorRenderer, )
     filter_backends = (UWSFilterBackend, )
@@ -96,50 +103,54 @@
 
         return get_job_url(self.request, kwargs=kwargs)
 
     def list(self, request, *args, **kwargs):
         queryset = self.filter_queryset(self.get_queryset())
         serializer = JobListSerializer(queryset, many=True)
         renderered_data = UWSRenderer().render(serializer.data, renderer_context=self.get_renderer_context())
-        return HttpResponse(renderered_data, content_type=UWSRenderer.media_type)
+        return HttpResponse(renderered_data, content_type=get_content_type(request, UWSRenderer))
 
     def retrieve(self, request, *args, **kwargs):
         job = self.get_object()
         serializer = JobRetrieveSerializer(job, context={'request': request})
         renderered_data = UWSRenderer().render(serializer.data, renderer_context=self.get_renderer_context())
-        return HttpResponse(renderered_data, content_type=UWSRenderer.media_type)
+        return HttpResponse(renderered_data, content_type=get_content_type(request, UWSRenderer))
 
     def create(self, request, *args, **kwargs):
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         # create the job objects
         job = self.get_queryset().model(
             job_type=Job.JOB_TYPE_ASYNC,
-            owner=(None if self.request.user.is_anonymous() else self.request.user),
-            response_format=serializer.data.get('RESPONSEFORMAT'),
-            max_records=serializer.data.get('MAXREC'),
-            run_id=serializer.data.get('RUNID'),
+            owner=(None if self.request.user.is_anonymous else self.request.user),
+            response_format=serializer.validated_data.get('RESPONSEFORMAT'),
+            max_records=serializer.validated_data.get('MAXREC'),
+            # uploads=handle_uploads(request, serializer.validated_data.get('UPLOAD'), self.get_upload_directory()),
+            run_id=serializer.validated_data.get('RUNID'),
             client_ip=get_client_ip(self.request)
         )
 
         # add parameters to the job object
         for parameter, model_field in self.parameter_map.items():
-            value = serializer.data.get(parameter)
+            value = serializer.validated_data.get(parameter)
             if value is not None:
                 setattr(job, model_field, value)
 
+        # handle possible uploads
+        self.handle_upload(job, serializer.validated_data.get('UPLOAD'))
+
         try:
             job.process()
         except ValidationError as e:
             raise ValidationError(self.rewrite_exception(e))
 
         job.save()
 
-        if serializer.data.get('PHASE') == job.PHASE_RUN:
+        if serializer.validated_data.get('PHASE') == job.PHASE_RUN:
             job.run()
 
         return HttpResponseSeeOther(self.get_success_url(job))
 
     def update(self, request, *args, **kwargs):
         self.get_object()  # necessary to check permissions
 
@@ -159,44 +170,44 @@
             })
 
     def destroy(self, request, *args, **kwargs):
         job = self.get_object()
         job.archive()
         return HttpResponseSeeOther(self.get_success_url())
 
-    @detail_route(methods=['get'])
+    @action(detail=True, methods=['get'])
     def results(self, request, pk, key=None):
         job = self.get_object()
 
         renderered_data = UWSRenderer().render({
             'results': get_job_results(request, job)
         }, renderer_context=self.get_renderer_context())
-        return HttpResponse(renderered_data, content_type=UWSRenderer.media_type)
+        return HttpResponse(renderered_data, content_type=get_content_type(request, UWSRenderer))
 
-    @detail_route(methods=['get'], url_path='results/(?P<result>[A-Za-z0-9\-]+)', url_name='result')
+    @action(detail=True, methods=['get'], url_path=r'results/(?P<result>[A-Za-z0-9\-]+)', url_name='result')
     def result(self, request, pk, result):
         job = self.get_object()
 
         if result == 'result':
             return FileResponse(job.stream(job.response_format), content_type=job.formats[job.response_format])
         elif result in job.formats:
             return FileResponse(job.stream(result), content_type=job.formats[result])
         else:
             raise ValidationError({
                 'result': 'Unsupported value.'
             })
 
-    @detail_route(methods=['get'])
+    @action(detail=True, methods=['get'])
     def parameters(self, request, pk):
         renderered_data = UWSRenderer().render({
             'parameters': self.get_object().parameters
         }, renderer_context=self.get_renderer_context())
-        return HttpResponse(renderered_data, content_type=UWSRenderer.media_type)
+        return HttpResponse(renderered_data, content_type=get_content_type(request, UWSRenderer))
 
-    @detail_route(methods=['get', 'post'])
+    @action(detail=True, methods=['get', 'post'])
     def destruction(self, request, pk):
         job = self.get_object()
 
         if request.method == 'GET':
             if job.destruction_time:
                 # use the JobUpdateSerializer to create timestamp
                 serializer = JobUpdateSerializer({
@@ -215,15 +226,15 @@
                 job.save()
                 return HttpResponseSeeOther(self.get_success_url(), status=303)
             else:
                 raise ValidationError({
                     'DESTRUCTION': 'Parameter not found.'
                 })
 
-    @detail_route(methods=['get', 'post'])
+    @action(detail=True, methods=['get', 'post'])
     def executionduration(self, request, pk):
         job = self.get_object()
 
         if request.method == 'GET':
             return HttpResponse(job.execution_duration)
         else:
             serializer = JobUpdateSerializer(data=request.data)
@@ -234,15 +245,15 @@
                 job.save()
                 return HttpResponseSeeOther(self.get_success_url())
             else:
                 raise ValidationError({
                     'EXECUTIONDURATION': 'Parameter not found.'
                 })
 
-    @detail_route(methods=['get', 'post'])
+    @action(detail=True, methods=['get', 'post'])
     def phase(self, request, pk):
         job = self.get_object()
 
         if request.method == 'GET':
             return HttpResponse(job.phase)
         else:
             serializer = JobUpdateSerializer(data=request.data)
@@ -268,21 +279,21 @@
                         'PHASE': 'Unsupported value.'
                     })
             else:
                 raise ValidationError({
                     'PHASE': 'Parameter not found.'
                 })
 
-    @detail_route(methods=['get'])
+    @action(detail=True, methods=['get'])
     def error(self, request, pk):
         job = self.get_object()
         return Response(job.error_summary, content_type='application/xml') if job.error_summary else HttpResponse()
 
-    @detail_route(methods=['get'])
+    @action(detail=True, methods=['get'])
     def quote(self, request, pk):
         job = self.get_object()
         return HttpResponse(job.quote) if job.quote else HttpResponse()
 
-    @detail_route(methods=['get'])
+    @action(detail=True, methods=['get'])
     def owner(self, request, pk):
         job = self.get_object()
         return HttpResponse(job.owner) if job.owner else HttpResponse()
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templatetags/metadata_tags.py` & `django-daiquiri-0.4.2/daiquiri/metadata/templatetags/metadata_tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 from django import template
-from django.utils.translation import ugettext_lazy as _
+from django.conf import settings
+from django.utils.html import format_html
+from django.utils.translation import gettext_lazy as _
 
-from daiquiri.core.constants import LICENSE_CHOICES, LICENSE_URLS
 from daiquiri.core.utils import get_doi_url
 
 from ..models import Schema
 
 register = template.Library()
 
 
 @register.inclusion_tag('metadata/tags/schemas_menu.html', takes_context=True)
-def schemas_menu(context):
+def schemas_menu(context, tables=True):
 
     schemas = Schema.objects.filter_by_metadata_access_level(context.request.user)
 
     context['schemas'] = []
     for schema in schemas:
         context['schemas'].append({
             'name': schema.name,
             'label': schema.title or schema.name,
             'tables': [{
                 'name': table.name,
                 'label': '%s.%s' % (schema.name, table.name)
                 } for table in schema.tables.filter_by_metadata_access_level(context.request.user)
-            ]
+            ] if tables else []
         })
 
     return context
 
 
 @register.inclusion_tag('metadata/tags/access_panel.html')
 def access_panel(doi, dataset=_('dataset')):
     return {
         'dataset': dataset
     }
 
 
+@register.simple_tag()
+def doi_link(doi):
+    url = get_doi_url(doi)
+    return format_html('<a class="break" href="{}">{}</a>', url, url)
+
+
 @register.inclusion_tag('metadata/tags/doi_panel.html')
 def doi_panel(doi, dataset=_('dataset')):
     return {
         'doi_url': get_doi_url(doi),
         'dataset': dataset
     }
 
 
 @register.inclusion_tag('metadata/tags/license_panel.html')
-def license_panel(license):
+def license_panel(license, dataset=_('dataset')):
     return {
         'license': license,
-        'license_url': LICENSE_URLS[license],
-        'license_label': dict(LICENSE_CHOICES)[license]
+        'license_url': settings.LICENSE_URLS[license],
+        'license_label': dict(settings.LICENSE_CHOICES)[license],
+        'dataset': dataset
     }
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/serializers/__init__.py` & `django-daiquiri-0.4.2/daiquiri/metadata/serializers/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from django.conf import settings
 from django.contrib.auth.models import Group
 
+from daiquiri.core.serializers import JSONListField
+
 from rest_framework import serializers
 
 from ..models import Schema, Table, Column, Function
 
 
 class GroupSerializer(serializers.ModelSerializer):
 
@@ -53,19 +55,29 @@
             )
 
 
 class TableSerializer(serializers.ModelSerializer):
 
     label = serializers.CharField(source='__str__', read_only=True)
 
+    related_identifiers = JSONListField(required=False)
+    creators = JSONListField(required=False)
+    contributors = JSONListField(required=False)
+    license = serializers.ChoiceField(choices=settings.LICENSE_CHOICES, default='')
+
     class Meta:
         model = Table
         fields = '__all__'
 
 
 class SchemaSerializer(serializers.ModelSerializer):
 
     label = serializers.CharField(source='__str__', read_only=True)
 
+    related_identifiers = JSONListField(required=False)
+    creators = JSONListField(required=False)
+    contributors = JSONListField(required=False)
+    license = serializers.ChoiceField(choices=settings.LICENSE_CHOICES, default='', initial='')
+
     class Meta:
         model = Schema
         fields = '__all__'
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/serializers/export.py` & `django-daiquiri-0.4.2/daiquiri/metadata/serializers/export.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/serializers/management.py` & `django-daiquiri-0.4.2/daiquiri/metadata/serializers/management.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/serializers/user.py` & `django-daiquiri-0.4.2/daiquiri/metadata/serializers/dublincore.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,74 @@
 from django.conf import settings
 
 from rest_framework import serializers
 
-from ..models import Schema, Table, Column, Function
+from daiquiri.core.serializers import JSONListField
+from daiquiri.metadata.models import Schema, Table
 
 
-class ColumnSerializer(serializers.ModelSerializer):
+class DublincoreSerializer(serializers.ModelSerializer):
 
-    class Meta:
-        model = Column
-        fields = (
-            'id',
-            'order',
-            'name',
-            'query_strings',
-            'description',
-            'unit',
-            'ucd',
-            'utype',
-            'datatype',
-            'arraysize',
-            'principal',
-            'indexed',
-            'std'
-        )
+    title = serializers.SerializerMethodField()
+    description = serializers.SerializerMethodField()
+    creators = JSONListField(default=[])
+    contributors = JSONListField(default=[])
+    subjects = serializers.ReadOnlyField(default=settings.SITE_SUBJECTS)
+    publisher = serializers.ReadOnlyField(default=settings.SITE_PUBLISHER)
+    date = serializers.ReadOnlyField(source='published')
+    type = serializers.SerializerMethodField()
+    identifier = serializers.SerializerMethodField()
+    rights = serializers.ReadOnlyField(source='license')
 
+    def get_title(self, obj):
+        return obj.title or obj.name
 
-class TableSerializer(serializers.ModelSerializer):
+    def get_description(self, obj):
+        return obj.long_description or obj.description
 
-    columns = serializers.SerializerMethodField()
+    def get_type(self, obj):
+        return 'Dataset'
 
-    class Meta:
-        model = Table
-        fields = (
-            'id',
-            'order',
-            'name',
-            'query_strings',
-            'description',
-            'type',
-            'utype',
-            'columns'
-        )
-
-    def get_columns(self, obj):
-        # filter the columns which are published for the groups of the user
-        if not settings.METADATA_COLUMN_PERMISSIONS:
-            queryset = obj.columns.all()
-        else:
-            queryset = obj.columns.filter_by_access_level(self.context['request'].user)
-        return ColumnSerializer(queryset, context=self.context, many=True).data
+    def get_identifier(self, obj):
+        raise NotImplementedError()
 
 
-class SchemaSerializer(serializers.ModelSerializer):
-
-    tables = serializers.SerializerMethodField()
+class DublincoreSchemaSerializer(DublincoreSerializer):
 
     class Meta:
         model = Schema
         fields = (
-            'id',
-            'order',
-            'name',
-            'query_strings',
+            'title',
             'description',
-            'utype',
-            'tables'
+            'creators',
+            'contributors',
+            'subjects',
+            'publisher',
+            'date',
+            'type',
+            'identifier',
+            'rights'
         )
 
-    def get_tables(self, obj):
-        # filter the tables which are published for the groups of the user
-        queryset = obj.tables.filter_by_access_level(self.context['request'].user)
-        return TableSerializer(queryset, context=self.context, many=True).data
+    def get_identifier(self, obj):
+        return obj.doi or 'schemas/%i' % obj.pk
 
 
-class FunctionSerializer(serializers.ModelSerializer):
+class DublincoreTableSerializer(DublincoreSerializer):
 
     class Meta:
-        model = Function
+        model = Table
         fields = (
-            'id',
-            'order',
-            'name',
-            'query_string'
+            'title',
+            'description',
+            'creators',
+            'contributors',
+            'subjects',
+            'publisher',
+            'date',
+            'type',
+            'identifier',
+            'rights'
         )
+
+    def get_identifier(self, obj):
+        return obj.doi or 'tables/%i' % obj.pk
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/views.py` & `django-daiquiri-0.4.2/daiquiri/metadata/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from django.http import Http404
 from django.views.generic import TemplateView
 
-from daiquiri.core.views import ModelPermissionMixin
+from daiquiri.core.views import CSRFViewMixin, ModelPermissionMixin
 from daiquiri.core.utils import get_model_field_meta
 
 from .models import Schema, Table, Column, Function
 
 
-class ManagementView(ModelPermissionMixin, TemplateView):
+class ManagementView(ModelPermissionMixin, CSRFViewMixin, TemplateView):
     template_name = 'metadata/management.html'
     permission_required = 'daiquiri_metadata.view_schema'
 
     def get_context_data(self, **kwargs):
         context = super(ManagementView, self).get_context_data(**kwargs)
         context['meta'] = {
             'Schema': get_model_field_meta(Schema),
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0014_rename_pid_to_doi.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0014_rename_pid_to_doi.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0007_access_level.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0007_access_level.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0015_change_doi_to_char.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0015_change_doi_to_char.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0003_groups.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0003_groups.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0018_meta.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0018_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0021_table_nrows.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0021_table_nrows.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0020_blank_index_for.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0020_blank_index_for.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0005_more_fields.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0005_more_fields.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0019_column_index_for.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0019_column_index_for.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0001_initial.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0006_meta.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0006_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0010_meta.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0010_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0017_rename_database_to_schema.py` & `django-daiquiri-0.4.2/daiquiri/auth/migrations/0014_use_django_jsonfield.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# -*- coding: utf-8 -*-
-# Generated by Django 1.11.10 on 2018-02-16 17:22
-from __future__ import unicode_literals
+# Generated by Django 3.2.12 on 2022-02-04 14:57
 
-from django.db import migrations
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('daiquiri_metadata', '0016_rename_database_to_schema'),
+        ('daiquiri_auth', '0013_alter_profile_id'),
     ]
 
     operations = [
-        migrations.RenameModel(
-            old_name='Database',
-            new_name='Schema',
+        migrations.AlterField(
+            model_name='profile',
+            name='attributes',
+            field=models.JSONField(blank=True, null=True),
         ),
-        migrations.AlterModelOptions(
-            name='schema',
-            options={'ordering': ('order',), 'permissions': (('view_schema', 'Can view Schema'),), 'verbose_name': 'Schema', 'verbose_name_plural': 'Schemas'},
+        migrations.AlterField(
+            model_name='profile',
+            name='details',
+            field=models.JSONField(blank=True, null=True),
         ),
     ]
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0008_refactoring.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0008_refactoring.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0002_published_for.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0002_published_for.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/migrations/0011_directory.py` & `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0011_directory.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/pd.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/pd.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_nc_sa.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc_sa.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_nd.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nd.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_sa.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_sa.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_nc.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/cc0.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/cc0.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/nc.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/nc.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/sa.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/sa.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/by_nc_nd.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc_nd.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/img/nd.png` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/nd.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/static/metadata/css/metadata.scss` & `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/css/metadata.scss`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+@import 'core/css/variables';
+
 .daiquiri-metadata-browser .daiquiri-browser-body {
     height: 400px;
 }
 
 .daiquiri-metadata-display {
 
     margin-bottom: 20px;
@@ -25,10 +27,15 @@
 
     .daiquiri-metadata-display-title {
         height: 20px;
         margin-bottom: 10px;
     }
 }
 
+.daiquiri-metadata-modal-person {
+    border-bottom: 1px solid $modal-border-color;
+    margin-bottom: 15px;
+}
+
 .CodeMirror {
     height: 600px;
 }
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <div class="modal-dialog modal-lg">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Schema' %}
+                        {% trans 'Update schema attribution' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <formgroup
                         data-id="schema-attribution"
                         data-type="codemirror"
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_delete_columns.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_columns.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <div class="modal-dialog modal-lg">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Tables' %}
+                        {% trans 'Update table description' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <formgroup
                         data-id="tables-long_description"
                         data-type="codemirror"
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_delete_functions.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_tables.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 {% load i18n %}
 
-    <div class="modal" id="functions-delete-modal" tabindex="-1">
+    <div class="modal" id="tables-delete-modal" tabindex="-1">
         <div class="modal-dialog">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Delete function' %}
+                        {% trans 'Delete table' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <p>
                         {% blocktrans trimmed %}
-                        You are about to permanently delete the metadata for the function <strong>{$ service.values.name $}</strong>.
+                        You are about to permanently delete the metadata for the table <strong>{$ service.values.name $}</strong>.
+                        {% endblocktrans %}
+                    </p>
+                    <p>
+                        {% blocktrans trimmed %}
+                        This will also delete the metadata for all its columns.
                         {% endblocktrans %}
                     </p>
                     <p class="text-danger">
                         {% trans 'This action cannot be undone!' %}
                     </p>
                 </div>
 
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">
                         {% trans 'Close' %}
                     </button>
                     <button type="button" class="btn btn-danger"
-                            ng-click="service.submitDeleteModal('functions')">
+                            ng-click="service.submitDeleteModal('tables')">
                         {% trans 'Delete' %}
                     </button>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 {% extends 'core/wide.html' %}
-{% load staticfiles %}
+{% load static %}
 {% load compress %}
 {% load i18n %}
-{% load core_tags %}
+{% load vendor_tags %}
 
 {% block bodyargs %}ng-app="metadata" ng-controller="MetadataController"{% endblock %}
 
 {% block headextra %}
     {% vendor 'angular' %}
     {% vendor 'ng-infinite-scroll' %}
     {% vendor 'codemirror' %}
+    {% vendor 'moment' %}
 
     {% compress css %}
     <link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/browser.scss' %}" />
     <link rel="stylesheet" type="text/x-scss" href="{% static 'core/css/codemirror.scss' %}" />
     <link rel="stylesheet" type="text/x-scss" href="{% static 'metadata/css/metadata.scss' %}" />
     {% endcompress css %}
 
@@ -58,17 +59,21 @@
             </div>
         </div>
     </div>
 
     {% include 'metadata/management_modal_form_schemas.html' %}
     {% include 'metadata/management_modal_form_schemas_description.html' %}
     {% include 'metadata/management_modal_form_schemas_attribution.html' %}
+    {% include 'metadata/management_modal_form_schemas_creators.html' %}
+    {% include 'metadata/management_modal_form_schemas_contributors.html' %}
     {% include 'metadata/management_modal_form_tables.html' %}
     {% include 'metadata/management_modal_form_tables_description.html' %}
     {% include 'metadata/management_modal_form_tables_attribution.html' %}
+    {% include 'metadata/management_modal_form_tables_creators.html' %}
+    {% include 'metadata/management_modal_form_tables_contributors.html' %}
     {% include 'metadata/management_modal_form_columns.html' %}
     {% include 'metadata/management_modal_form_functions.html' %}
 
     {% include 'metadata/management_modal_delete_schemas.html' %}
     {% include 'metadata/management_modal_delete_tables.html' %}
     {% include 'metadata/management_modal_delete_columns.html' %}
     {% include 'metadata/management_modal_delete_functions.html' %}
```

#### html2text {}

```diff
@@ -1,26 +1,30 @@
-{% extends 'core/wide.html' %} {% load staticfiles %} {% load compress %} {%
-load i18n %} {% load core_tags %} {% block bodyargs %}ng-app="metadata" ng-
+{% extends 'core/wide.html' %} {% load static %} {% load compress %} {% load
+i18n %} {% load vendor_tags %} {% block bodyargs %}ng-app="metadata" ng-
 controller="MetadataController"{% endblock %} {% block headextra %} {% vendor
 'angular' %} {% vendor 'ng-infinite-scroll' %} {% vendor 'codemirror' %} {%
-compress css %}
+vendor 'moment' %} {% compress css %}
 
 
  {% endcompress css %} {% compress js %}
  {% endcompress js %} {% endblock %} {% block wide %}
 ****** {% trans 'Metadata management' %} ******
 {% trans 'Please click on a schema, a table, a column or a function to show or
 edit its metadata.' %}
 {% include 'metadata/management_display.html' %}
 {% include 'metadata/management_options.html' %}
 {% include 'metadata/management_modal_form_schemas.html' %} {% include
 'metadata/management_modal_form_schemas_description.html' %} {% include
 'metadata/management_modal_form_schemas_attribution.html' %} {% include
-'metadata/management_modal_form_tables.html' %} {% include 'metadata/
+'metadata/management_modal_form_schemas_creators.html' %} {% include 'metadata/
+management_modal_form_schemas_contributors.html' %} {% include 'metadata/
+management_modal_form_tables.html' %} {% include 'metadata/
 management_modal_form_tables_description.html' %} {% include 'metadata/
 management_modal_form_tables_attribution.html' %} {% include 'metadata/
+management_modal_form_tables_creators.html' %} {% include 'metadata/
+management_modal_form_tables_contributors.html' %} {% include 'metadata/
 management_modal_form_columns.html' %} {% include 'metadata/
 management_modal_form_functions.html' %} {% include 'metadata/
 management_modal_delete_schemas.html' %} {% include 'metadata/
 management_modal_delete_tables.html' %} {% include 'metadata/
 management_modal_delete_columns.html' %} {% include 'metadata/
 management_modal_delete_functions.html' %} {% endblock %}
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/table.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/table.html`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,19 @@
         {% if table.title %}
         {{ table.title }} ({{ table }})
         {% else %}
         {{ table }}
         {% endif %}
     </h1>
 
+    {% if table.nrows %}
+
+    <p>The table has {{ table.nrows }} rows, {{ table.columns.all | length }} columns.</p>
+    {% endif %}
+
     {% if table.long_description %}
 
     <h2>Description</h2>
 
     {{ table.long_description | markdown }}
 
     {% elif table.description %}
@@ -57,15 +62,15 @@
                     <td>
                         {{ column.ucd|default_if_none:''|semicolonbr }}
                     </td>
                     <td>
                         {{ column.unit|default_if_none:'' }}
                     </td>
                     <td>
-                        {{ column.description|default_if_none:'' }}
+                        {{ column.description | markdown }}
                     </td>
                 </tr>
                 {% endfor %}
             </tbody>
         </table>
     </div>
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
 {% extends 'core/page.html' %} {% load i18n %} {% load static %} {% load
 core_tags %} {% load metadata_tags %} {% block page %}
 ****** {% if table.title %} {{ table.title }} ({{ table }}) {% else %} {{ table
 }} {% endif %} ******
-{% if table.long_description %}
+{% if table.nrows %}
+The table has {{ table.nrows }} rows, {{ table.columns.all | length }} columns.
+{% endif %} {% if table.long_description %}
 ***** Description *****
 {{ table.long_description | markdown }} {% elif table.description %}
 ***** Description *****
 {{ table.description | markdown }} {% endif %} {% if table.attribution %}
 ***** Attribution *****
 {{ table.attribution | markdown }} {% endif %}
 ***** {% trans 'Columns' %} *****
 {           {               {                           {                            {
 {           {               {                           {                            {
-column.name column.datatype column.ucd|default_if_none: column.unit|default_if_none: column.description|default_if_none:
-}}          }}              ''|semicolonbr }}           '' }}                        '' }}
+column.name column.datatype column.ucd|default_if_none: column.unit|default_if_none: column.description
+}}          }}              ''|semicolonbr }}           '' }}                        | markdown }}
 {% endblock %} {% block sidebar %} {% access_panel table _('table') %} {% if
 table.doi %} {% doi_panel table.doi _('table') %} {% endif %} {% if
 table.license %} {% license_panel table.license %} {% endif %} {% endblock %}
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <div class="modal-dialog modal-lg">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Tables' %}
+                        {% trans 'Update table attribution' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <formgroup
                         data-id="tables-attribution"
                         data-type="codemirror"
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas.html`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <div class="modal-dialog modal-lg">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Schema' %}
+                        {% trans 'Update schema' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <div class="row">
                         <formgroup
                             class="col-md-8"
@@ -55,16 +55,15 @@
                             data-id="license"
                             data-type="select"
                             data-label="{{ meta.Schema.license.verbose_name }}"
                             data-help="{{ meta.Schema.license.help_text }}"
                             data-model="service.values.license"
                             data-errors="service.errors.license"
                             data-options="service.licenses"
-                            data-options-label="text"
-                            data-options-null="1">
+                            data-options-label="text">
                         </formgroup>
                         <formgroup
                             class="col-md-4"
                             data-id="doi"
                             data-type="text"
                             data-label="{{ meta.Schema.doi.verbose_name }}"
                             data-help="{{ meta.Schema.doi.help_text }}"
@@ -80,14 +79,34 @@
                             data-model="service.values.utype"
                             data-errors="service.errors.utype">
                         </formgroup>
                     </div>
                     <div class="row">
                         <formgroup
                             class="col-md-6"
+                            data-id="published"
+                            data-type="date"
+                            data-label="{{ meta.Schema.published.verbose_name }}"
+                            data-help="{{ meta.Schema.published.help_text }}"
+                            data-model="service.values.published"
+                            data-errors="service.errors.published">
+                        </formgroup>
+                        <formgroup
+                            class="col-md-6"
+                            data-id="updated"
+                            data-type="date"
+                            data-label="{{ meta.Schema.updated.verbose_name }}"
+                            data-help="{{ meta.Schema.updated.help_text }}"
+                            data-model="service.values.updated"
+                            data-errors="service.errors.updated">
+                        </formgroup>
+                    </div>
+                    <div class="row">
+                        <formgroup
+                            class="col-md-6"
                             data-id="access_level"
                             data-type="select"
                             data-label="{{ meta.Schema.access_level.verbose_name }}"
                             data-help="{{ meta.Schema.access_level.help_text }}"
                             data-model="service.values.access_level"
                             data-errors="service.errors.access_level"
                             data-options="service.accesslevels"
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_options.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_options.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/schema.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/schema.html`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     {% else %}
                     {{ table }}
                     {% endif %}
                 </a>
             </h4>
 
             {% if table.description %}
-            {{ table.description }}
+            {{ table.description | markdown }}
             {% endif %}
         </li>
         {% endfor %}
     </ul>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -11,12 +11,12 @@
 {% endif %} {% if schema.attribution %}
 ***** Attribution *****
 {{ schema.attribution | markdown }} {% endif %}
 ***** {% trans 'Tables' %} *****
     * {% for table in tables %}
     * *** {%_if_table.title_%}_{{_table.title_}}_({{_table_}})_{%_else_%}_{
       {_table_}}_{%_endif_%} ***
-      {% if table.description %} {{ table.description }} {% endif %}
+      {% if table.description %} {{ table.description | markdown }} {% endif %}
     * {% endfor %}
 {% endblock %} {% block sidebar %} {% access_panel schema _('schema') %} {% if
 schema.doi %} {% doi_panel schema.doi _('schema') %} {% endif %} {% if
 schema.license %} {% license_panel schema.license %} {% endif %} {% endblock %}
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_functions.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_functions.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <div class="modal-dialog modal-lg">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Function' %}
+                        {% trans 'Update function' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <div class="row">
                         <formgroup
                             class="col-md-10"
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_delete_tables.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 {% load i18n %}
 
-    <div class="modal" id="tables-delete-modal" tabindex="-1">
-        <div class="modal-dialog">
+    <div class="modal" id="schemas-description-form-modal" tabindex="-1">
+        <div class="modal-dialog modal-lg">
             <div class="modal-content">
                 <div class="modal-header">
-                    <button type="button" class="close" data-dismiss="modal">
+                    <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Delete table' %}
+                        {% trans 'Update schema description' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
-                    <p>
-                        {% blocktrans trimmed %}
-                        You are about to permanently delete the metadata for the table <strong>{$ service.values.name $}</strong>.
-                        {% endblocktrans %}
-                    </p>
-                    <p>
-                        {% blocktrans trimmed %}
-                        This will also delete the metadata for all its columns.
-                        {% endblocktrans %}
-                    </p>
-                    <p class="text-danger">
-                        {% trans 'This action cannot be undone!' %}
-                    </p>
+                    <formgroup
+                        data-id="schema-long_description"
+                        data-type="codemirror"
+                        data-label="{{ meta.Schema.long_description.verbose_name }}"
+                        data-help="{{ meta.Schema.long_description.help_text }}"
+                        data-model="service.values.long_description"
+                        data-errors="service.errors.long_description"
+                        data-mode="markdown">
+                    </formgroup>
                 </div>
 
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">
                         {% trans 'Close' %}
                     </button>
-                    <button type="button" class="btn btn-danger"
-                            ng-click="service.submitDeleteModal('tables')">
-                        {% trans 'Delete' %}
+                    <button type="button" class="btn btn-default"
+                            ng-click="service.submitFormModal('schemas', false)">
+                        {% trans 'Save' %}
+                    </button>
+                    <button type="button" class="btn btn-primary"
+                            ng-click="service.submitFormModal('schemas')">
+                        {% trans 'Save and close' %}
                     </button>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_tables.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <div class="modal-dialog modal-lg">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Tables' %}
+                        {% trans 'Update table' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <div class="row">
                         <formgroup
                             class="col-md-4"
@@ -31,15 +31,15 @@
                             data-type="text"
                             data-label="{{ meta.Table.name.verbose_name }}"
                             data-help="{{ meta.Table.name.help_text }}"
                             data-model="service.values.name"
                             data-errors="service.errors.name">
                         </formgroup>
                         <formgroup
-                             class="col-md-2"
+                            class="col-md-2"
                             data-id="order"
                             data-type="number"
                             data-label="{{ meta.Table.order.verbose_name }}"
                             data-help="{{ meta.Table.order.help_text }}"
                             data-model="service.values.order"
                             data-errors="service.errors.order">
                         </formgroup>
@@ -95,16 +95,15 @@
                             data-id="license"
                             data-type="select"
                             data-label="{{ meta.Table.license.verbose_name }}"
                             data-help="{{ meta.Table.license.help_text }}"
                             data-model="service.values.license"
                             data-errors="service.errors.license"
                             data-options="service.licenses"
-                            data-options-label="text"
-                            data-options-null="1">
+                            data-options-label="text">
                         </formgroup>
                         <formgroup
                             class="col-md-4"
                             data-id="doi"
                             data-type="text"
                             data-label="{{ meta.Table.doi.verbose_name }}"
                             data-help="{{ meta.Table.doi.help_text }}"
@@ -120,14 +119,34 @@
                             data-model="service.values.utype"
                             data-errors="service.errors.utype">
                         </formgroup>
                     </div>
                     <div class="row">
                         <formgroup
                             class="col-md-6"
+                            data-id="published"
+                            data-type="date"
+                            data-label="{{ meta.Table.published.verbose_name }}"
+                            data-help="{{ meta.Table.published.help_text }}"
+                            data-model="service.values.published"
+                            data-errors="service.errors.published">
+                        </formgroup>
+                        <formgroup
+                            class="col-md-6"
+                            data-id="updated"
+                            data-type="date"
+                            data-label="{{ meta.Table.updated.verbose_name }}"
+                            data-help="{{ meta.Table.updated.help_text }}"
+                            data-model="service.values.updated"
+                            data-errors="service.errors.updated">
+                        </formgroup>
+                    </div>
+                    <div class="row">
+                        <formgroup
+                            class="col-md-6"
                             data-id="access_level"
                             data-type="select"
                             data-label="{{ meta.Table.access_level.verbose_name }}"
                             data-help="{{ meta.Table.access_level.help_text }}"
                             data-model="service.values.access_level"
                             data-errors="service.errors.access_level"
                             data-options="service.accesslevels"
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_columns.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_columns.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <div class="modal-dialog">
             <div class="modal-content modal-lg">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Column' %}
+                        {% trans 'Update column' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <div class="row">
                         <formgroup
                             class="col-md-4"
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_display.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_display.html`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,22 @@
                     ng-show="service.active.resource === 'schemas' || service.active.resource === 'tables'"
                     ng-click="service.openFormModal(service.active.resource, false, 'description')">
                 </a>
                 <a href="" class="fa fa-graduation-cap" title="{% trans 'Update attribution' %}"
                     ng-show="service.active.resource === 'schemas' || service.active.resource === 'tables'"
                     ng-click="service.openFormModal(service.active.resource, false, 'attribution')">
                 </a>
+                <a href="" class="fa fa-user" title="{% trans 'Update creators' %}"
+                    ng-show="service.active.resource === 'schemas' || service.active.resource === 'tables'"
+                    ng-click="service.openFormModal(service.active.resource, false, 'creators')">
+                </a>
+                <a href="" class="fa fa-user-plus" title="{% trans 'Update contributors' %}"
+                    ng-show="service.active.resource === 'schemas' || service.active.resource === 'tables'"
+                    ng-click="service.openFormModal(service.active.resource, false, 'contributors')">
+                </a>
                 <a href="" class="fa fa-trash" title="{% trans 'Delete' %}"
                     ng-click="service.openDeleteModal(service.active.resource, false)">
                 </a>
             </div>
 
             <div class="daiquiri-metadata-display-title">
                 <strong ng-show="service.active.resource === 'schemas'">{% trans 'Schema' %}</strong>
@@ -28,15 +36,15 @@
                 <strong ng-show="service.active.resource === 'columns'">{% trans 'Column' %}</strong>
                 <strong ng-show="service.active.resource === 'functions'">{% trans 'Function' %}</strong>
                 <span>{$ service.active.label $}</span>
             </div>
 
             <dl class="dl-horizontal">
                 <div ng-repeat="(key, value) in service.active"
-                    ng-hide="['resource', 'groups', 'schema', 'table'].indexOf(key) != -1">
+                    ng-hide="['resource', 'groups', 'schema', 'table', 'creators', 'contributors'].indexOf(key) != -1">
 
                     <dt>{$ key | ucfirst | removeUnderscores $}</dt>
                     <dd>{$ value $}&nbsp;</dd>
 
                 </div>
             </dl>
         </div>
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html` & `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html` & `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_logout.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 {% load i18n %}
 
-    <div class="modal" id="schemas-description-form-modal" tabindex="-1">
-        <div class="modal-dialog modal-lg">
-            <div class="modal-content">
-                <div class="modal-header">
-                    <button type="button" class="close" data-dismiss="modal" tabindex="-1">
-                        <span aria-hidden="true">&times;</span>
-                    </button>
-                    <h4 class="modal-title">
-                        {% trans 'Schema' %}
-                    </h4>
-                </div>
+<div class="modal" id="logout-modal" tabindex="-1" data-backdrop="static" data-keyboard="false">
+    <div class="modal-dialog">
+        <div class="modal-content">
+            <div class="modal-header">
+                <h4 class="modal-title">
+                    {% trans 'Logout' %}
+                </h4>
+            </div>
 
-                <div class="modal-body">
-                    <formgroup
-                        data-id="schema-long_description"
-                        data-type="codemirror"
-                        data-label="{{ meta.Schema.long_description.verbose_name }}"
-                        data-help="{{ meta.Schema.long_description.help_text }}"
-                        data-model="service.values.long_description"
-                        data-errors="service.errors.long_description"
-                        data-mode="markdown">
-                    </formgroup>
-                </div>
+            <div class="modal-body">
+                <p>
+                    {% blocktrans trimmed with table_name='{$ service.values.table_name $}' %}
+                    You have been logged out. This happens after a certain time or when you have logged out in another window.
+                    {% endblocktrans %}
+                </p>
+            </div>
 
-                <div class="modal-footer">
-                    <button type="button" class="btn btn-default" data-dismiss="modal">
-                        {% trans 'Close' %}
-                    </button>
-                    <button type="button" class="btn btn-default"
-                            ng-click="service.submitFormModal('schemas', false)">
-                        {% trans 'Save' %}
-                    </button>
-                    <button type="button" class="btn btn-primary"
-                            ng-click="service.submitFormModal('schemas')">
-                        {% trans 'Save and close' %}
-                    </button>
-                </div>
+            <div class="modal-footer">
+                <a type="button" href="{% url 'query:query' %}" class="btn btn-default">
+                    {% trans 'Continue as guest' %}
+                </a>
+                <a type="button" href="{% url 'account_login' %}?next={% url 'query:query' %}" class="btn btn-primary">
+                    {% trans 'Login' %}
+                </a>
             </div>
         </div>
     </div>
+</div>
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/models.py` & `django-daiquiri-0.4.2/daiquiri/metadata/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from django.db import models
+from django.conf import settings
 from django.contrib.auth.models import Group
-from django.utils.encoding import python_2_unicode_compatible
-from django.utils.translation import ugettext_lazy as _
+from django.db import models
+from django.utils.translation import gettext_lazy as _
 
-from daiquiri.core.constants import LICENSE_CHOICES, LICENSE_URLS, ACCESS_LEVEL_CHOICES
+from daiquiri.core.constants import ACCESS_LEVEL_CHOICES, ACCESS_LEVEL_PRIVATE
 from daiquiri.core.managers import AccessLevelManager
 
 
-@python_2_unicode_compatible
 class Schema(models.Model):
 
     objects = AccessLevelManager()
 
     order = models.IntegerField(
         default=0, null=True, blank=True,
         verbose_name=_('Order'),
@@ -19,230 +18,264 @@
     )
     name = models.CharField(
         max_length=256,
         verbose_name=_('Name'),
         help_text=_('Name of the schema on the database server.')
     )
     title = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('Title'),
         help_text=_('Human readable title of the schema.')
     )
     description = models.TextField(
-        null=True, blank=True,
+        blank=True, default='',
         verbose_name=_('Description'),
         help_text=_('A brief description of the schema to be displayed in the user interface.')
     )
     long_description = models.TextField(
-        null=True, blank=True,
+        blank=True, default='',
         verbose_name=_('Long description'),
         help_text=_('A more extensive description of the schema to be displayed on the public schema page.')
     )
     attribution = models.TextField(
-        null=True, blank=True,
+        blank=True, default='',
         verbose_name=_('Attribution'),
         help_text=_('The desired attribution for the schema.')
     )
     license = models.CharField(
-        max_length=8, choices=LICENSE_CHOICES, null=True, blank=True,
+        max_length=8, blank=True, default='',
         verbose_name=_('License')
     )
     doi = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('Digital object identifier')
     )
+    related_identifiers = models.JSONField(
+        blank=True, default=list,
+        verbose_name=_('Related Identifiers'),
+    )
     utype = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('IVOA Utype'),
     )
+    creators = models.JSONField(
+        blank=True, default=list,
+        verbose_name=_('Creators'),
+    )
+    contributors = models.JSONField(
+        blank=True, default=list,
+        verbose_name=_('Contributors'),
+    )
+    published = models.DateField(
+        null=True, blank=True,
+        verbose_name=_('Published'),
+    )
+    updated = models.DateField(
+        null=True, blank=True,
+        verbose_name=_('Updated'),
+    )
     access_level = models.CharField(
-        max_length=8, choices=ACCESS_LEVEL_CHOICES,
+        max_length=8, choices=ACCESS_LEVEL_CHOICES, default=ACCESS_LEVEL_PRIVATE,
         verbose_name=_('Access level')
     )
     metadata_access_level = models.CharField(
-        max_length=8, choices=ACCESS_LEVEL_CHOICES,
+        max_length=8, choices=ACCESS_LEVEL_CHOICES, default=ACCESS_LEVEL_PRIVATE,
         verbose_name=_('Metadata access level')
     )
     groups = models.ManyToManyField(
         Group, blank=True,
         verbose_name=_('Groups'),
         help_text=_('The groups which have access to the schema.')
     )
 
     class Meta:
-        ordering = ('order', )
+        ordering = ('order', 'name')
 
         verbose_name = _('Schema')
         verbose_name_plural = _('Schemas')
 
-        permissions = (('view_schema', 'Can view Schema'),)
-
     def __str__(self):
         return self.name
 
     @property
     def query_strings(self):
         return [self.name]
 
     @property
     def license_label(self):
-        return dict(LICENSE_CHOICES)[self.license]
+        return dict(settings.LICENSE_CHOICES)[self.license]
 
     @property
     def license_url(self):
-        return LICENSE_URLS[self.license]
+        return settings.LICENSE_URLS[self.license]
 
 
-@python_2_unicode_compatible
 class Table(models.Model):
 
     TYPE_TABLE = 'table'
     TYPE_VIEW = 'view'
     TYPE_CHOICES = (
-        (TYPE_TABLE, _('Table')),
-        (TYPE_VIEW, _('View'))
+        (TYPE_TABLE, _('table')),
+        (TYPE_VIEW, _('view'))
     )
 
     objects = AccessLevelManager()
 
     schema = models.ForeignKey(
-        Schema, related_name='tables',
+        Schema, related_name='tables', on_delete=models.CASCADE,
         verbose_name=_('Database'),
         help_text=_('Database the table belongs to.')
     )
     order = models.IntegerField(
         null=True, blank=True,
         verbose_name=_('Order'),
         help_text=_('Position in lists.')
     )
     name = models.CharField(
         max_length=256,
         verbose_name=_('Name'),
         help_text=_('Identifier of the table on the database server.')
     )
     title = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('Title'),
         help_text=_('Human readable title of the table.')
     )
     description = models.TextField(
-        null=True, blank=True,
+        blank=True, default='',
         verbose_name=_('Description'),
         help_text=_('A brief description of the table to be displayed in the user interface.')
     )
     long_description = models.TextField(
-        null=True, blank=True,
+        blank=True, default='',
         verbose_name=_('Long description'),
         help_text=_('A more extensive description of the table to be displayed on the public database page.')
     )
     attribution = models.TextField(
-        null=True, blank=True,
+        blank=True, default='',
         verbose_name=_('Attribution'),
         help_text=_('The desired attribution for the table.')
     )
     license = models.CharField(
-        max_length=8, choices=LICENSE_CHOICES, null=True, blank=True,
+        max_length=8, blank=True, default='',
         verbose_name=_('License')
     )
     doi = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('Digital object identifier')
     )
+    related_identifiers = models.JSONField(
+        blank=True, default=list,
+        verbose_name=_('Related Identifiers'),
+    )
     type = models.CharField(
-        max_length=8, choices=TYPE_CHOICES,
+        max_length=8, choices=TYPE_CHOICES, default=TYPE_TABLE,
         verbose_name=_('Type of table')
     )
     nrows = models.BigIntegerField(
         null=True, blank=True,
         verbose_name=_('Number of rows in the table')
     )
     size = models.BigIntegerField(
         null=True, blank=True,
         verbose_name=_('Size of the table in bytes')
     )
     utype = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('IVOA Utype')
     )
+    creators = models.JSONField(
+        blank=True, default=list,
+        verbose_name=_('Creators'),
+    )
+    contributors = models.JSONField(
+        blank=True, default=list,
+        verbose_name=_('Contributors'),
+    )
+    published = models.DateField(
+        null=True, blank=True,
+        verbose_name=_('Published'),
+    )
+    updated = models.DateField(
+        null=True, blank=True,
+        verbose_name=_('Updated'),
+    )
     access_level = models.CharField(
-        max_length=8, choices=ACCESS_LEVEL_CHOICES,
+        max_length=8, choices=ACCESS_LEVEL_CHOICES, default=ACCESS_LEVEL_PRIVATE,
         verbose_name=_('Access level')
     )
     metadata_access_level = models.CharField(
-        max_length=8, choices=ACCESS_LEVEL_CHOICES,
+        max_length=8, choices=ACCESS_LEVEL_CHOICES, default=ACCESS_LEVEL_PRIVATE,
         verbose_name=_('Metadata access level')
     )
     groups = models.ManyToManyField(
         Group, blank=True,
         verbose_name=_('Groups'),
         help_text=_('The groups which have access to the table.')
     )
 
     class Meta:
-        ordering = ('schema__order', 'order', )
+        ordering = ('schema__order', 'order', 'name')
 
         verbose_name = _('Table')
         verbose_name_plural = _('Tables')
 
-        permissions = (('view_table', 'Can view Table'),)
-
     def __str__(self):
         return self.schema.name + '.' + self.name
 
     @property
     def query_strings(self):
         return [self.schema.name, self.name]
 
     @property
     def license_label(self):
-        return dict(LICENSE_CHOICES)[self.license]
+        return dict(settings.LICENSE_CHOICES)[self.license]
 
     @property
     def license_url(self):
-        return LICENSE_URLS[self.license]
+        return settings.LICENSE_URLS[self.license]
 
 
-@python_2_unicode_compatible
 class Column(models.Model):
 
     objects = AccessLevelManager()
 
     table = models.ForeignKey(
-        Table, related_name='columns',
+        Table, related_name='columns', on_delete=models.CASCADE,
         help_text=_('Table the column belongs to.')
     )
     order = models.IntegerField(
         null=True, blank=True,
         verbose_name=_('Order'),
         help_text=_('Position in lists.')
     )
     name = models.CharField(
         max_length=256,
         verbose_name=_('Name'),
         help_text=_('Identifier of the column on the database server.')
     )
     description = models.TextField(
-        null=True, blank=True,
+        blank=True, default='',
         verbose_name=_('Description'),
         help_text=_('A brief description of the column to be displayed in the user interface.')
     )
     unit = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('Unit')
     )
     ucd = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('IVOA UCDs')
     )
     utype = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('IVOA Utype')
     )
     datatype = models.CharField(
-        max_length=256, null=True, blank=True,
+        max_length=256, blank=True, default='',
         verbose_name=_('Datatype'),
         help_text=_('The datatype of the column on the database server.')
     )
     arraysize = models.IntegerField(
         null=True, blank=True,
         verbose_name=_('Arraysize'),
         help_text=_('The length of variable length datatypes, e.g. varchar(256).')
@@ -264,35 +297,33 @@
     )
     index_for = models.CharField(
         max_length=256, blank=True, default='',
         verbose_name=_('Index for'),
         help_text=_('The columns which this column is an index for (e.g. for pgSphere).')
     )
     access_level = models.CharField(
-        max_length=8, choices=ACCESS_LEVEL_CHOICES,
+        max_length=8, choices=ACCESS_LEVEL_CHOICES, default=ACCESS_LEVEL_PRIVATE,
         verbose_name=_('Access level')
     )
     metadata_access_level = models.CharField(
-        max_length=8, choices=ACCESS_LEVEL_CHOICES,
+        max_length=8, choices=ACCESS_LEVEL_CHOICES, default=ACCESS_LEVEL_PRIVATE,
         verbose_name=_('Metadata access level')
     )
     groups = models.ManyToManyField(
         Group, blank=True,
         verbose_name=_('Groups'),
         help_text=_('The groups which have access to the column.')
     )
 
     class Meta:
-        ordering = ('table__schema__order', 'table__order', 'order', )
+        ordering = ('table__schema__order', 'table__order', 'order', 'name')
 
         verbose_name = _('Column')
         verbose_name_plural = _('Columns')
 
-        permissions = (('view_column', 'Can view Column'),)
-
     def __str__(self):
         return self.table.schema.name + '.' + self.table.name + '.' + self.name
 
     @property
     def query_strings(self):
         return [self.name]
 
@@ -300,15 +331,14 @@
     def indexed_columns(self):
         if self.index_for:
             return [(self.table.schema.name, self.table.name, name.strip()) for name in self.index_for.split(',')] + [self.name]
         else:
             return None
 
 
-@python_2_unicode_compatible
 class Function(models.Model):
 
     objects = AccessLevelManager()
 
     order = models.IntegerField(
         null=True, blank=True,
         verbose_name=_('Order'),
@@ -316,40 +346,38 @@
     )
     name = models.CharField(
         max_length=256,
         verbose_name=_('Name'),
         help_text=_('Identifier of the function on the server.')
     )
     description = models.TextField(
-        null=True, blank=True,
+        blank=True, default='',
         verbose_name=_('Description'),
         help_text=_('A brief description of the function to be displayed in the user interface.')
     )
     query_string = models.CharField(
         max_length=256,
         verbose_name=_('Query string'),
         help_text=_('Prototype of this function in a SQL query.')
     )
     access_level = models.CharField(
-        max_length=8, choices=ACCESS_LEVEL_CHOICES,
+        max_length=8, choices=ACCESS_LEVEL_CHOICES, default=ACCESS_LEVEL_PRIVATE,
         verbose_name=_('Access level')
     )
     metadata_access_level = models.CharField(
-        max_length=8, choices=ACCESS_LEVEL_CHOICES,
+        max_length=8, choices=ACCESS_LEVEL_CHOICES, default=ACCESS_LEVEL_PRIVATE,
         verbose_name=_('Metadata access level')
     )
     groups = models.ManyToManyField(
         Group, blank=True,
         verbose_name=_('Groups'),
         help_text=_('The groups which have access to this function.')
     )
 
     class Meta:
-        ordering = ('order', )
+        ordering = ('order', 'name')
 
         verbose_name = _('Function')
         verbose_name_plural = _('Functions')
 
-        permissions = (('view_function', 'Can view Function'),)
-
     def __str__(self):
         return self.name
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/management/commands/update_access_level.py` & `django-daiquiri-0.4.2/daiquiri/metadata/management/commands/update_access_level.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from django.core.management.base import BaseCommand,CommandError
-from django.utils.translation import ugettext_lazy as _
+from django.core.management.base import BaseCommand, CommandError
+from django.utils.translation import gettext_lazy as _
 
 from daiquiri.core.constants import ACCESS_LEVEL_CHOICES
 from daiquiri.metadata.models import Schema
 
 
 class Command(BaseCommand):
```

### Comparing `django-daiquiri-0.2/daiquiri/metadata/management/commands/dump_table.py` & `django-daiquiri-0.4.2/daiquiri/metadata/management/commands/dump_table.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/metadata/viewsets.py` & `django-daiquiri-0.4.2/daiquiri/metadata/viewsets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from rest_framework import viewsets, filters, status
 from rest_framework.response import Response
-from rest_framework.decorators import list_route, detail_route
+from rest_framework.decorators import action
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.authentication import SessionAuthentication, TokenAuthentication
 
 from django_filters.rest_framework import DjangoFilterBackend
 
 from daiquiri.core.adapter import DatabaseAdapter
 from daiquiri.core.viewsets import ChoicesViewSet
 from daiquiri.core.permissions import HasModelPermission
-from daiquiri.core.constants import LICENSE_CHOICES, ACCESS_LEVEL_CHOICES
+from daiquiri.core.constants import ACCESS_LEVEL_CHOICES
+
+from django.conf import settings
 
 from .models import Schema, Table, Column, Function
 from .serializers import (
     SchemaSerializer,
     TableSerializer,
     ColumnSerializer,
     FunctionSerializer
@@ -36,15 +38,15 @@
     permission_classes = (HasModelPermission, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
 
     queryset = Schema.objects.all()
     serializer_class = SchemaSerializer
 
     filter_backends = (DjangoFilterBackend, filters.SearchFilter, filters.OrderingFilter)
-    filter_fields = ('name', 'access_level', 'metadata_access_level')
+    filterset_fields = ('name', 'access_level', 'metadata_access_level')
     search_fields = ('name', 'description')
     ordering_fields = ('name', 'access_level', 'metadata_access_level')
 
     def create(self, request, *args, **kwargs):
 
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
@@ -73,49 +75,49 @@
                         column_serializer = ColumnSerializer(data=column_metadata)
                         if column_serializer.is_valid():
                             column_serializer.save()
 
         headers = self.get_success_headers(serializer.data)
         return Response(serializer.data, status=status.HTTP_201_CREATED, headers=headers)
 
-    @list_route()
+    @action(detail=False)
     def management(self, request):
         queryset = Schema.objects.all()
         serializer = ManagementSchemaSerializer(queryset, many=True)
         return Response(serializer.data)
 
-    @list_route(methods=['get'], permission_classes=[])
+    @action(detail=False, methods=['get'], permission_classes=[])
     def user(self, request):
         # filter the schemas which are published for the groups of the user
         queryset = Schema.objects.filter_by_access_level(self.request.user)
         serializer = UserSchemaSerializer(queryset, context={'request': request}, many=True)
         return Response(serializer.data)
 
-    @list_route(methods=['get'], url_path='export', url_name='export-detail')
+    @action(detail=False, methods=['get'], url_path='export', url_name='export-detail')
     def export_list(self, request):
         queryset = Schema.objects.all()
         serializer = ExportSchemaSerializer(queryset, many=True)
         return Response(serializer.data)
 
-    @detail_route(methods=['get'], url_path='export', url_name='export-detail')
+    @action(detail=True, methods=['get'], url_path='export', url_name='export-detail')
     def export_detail(self, request, pk=None):
         queryset = Schema.objects.get(pk=pk)
         serializer = ExportSchemaSerializer(queryset)
         return Response(serializer.data)
 
 
 class TableViewSet(viewsets.ModelViewSet):
     permission_classes = (HasModelPermission, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
 
     queryset = Table.objects.all()
     serializer_class = TableSerializer
 
     filter_backends = (DjangoFilterBackend, filters.SearchFilter, filters.OrderingFilter)
-    filter_fields = ('name', 'access_level', 'metadata_access_level')
+    filterset_fields = ('name', 'access_level', 'metadata_access_level')
     search_fields = ('name', 'description')
     ordering_fields = ('name', 'access_level', 'metadata_access_level')
 
     def create(self, request, *args, **kwargs):
 
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
@@ -134,15 +136,15 @@
                 column_serializer = ColumnSerializer(data=column_metadata)
                 if column_serializer.is_valid():
                     column_serializer.save()
 
         headers = self.get_success_headers(serializer.data)
         return Response(serializer.data, status=status.HTTP_201_CREATED, headers=headers)
 
-    @list_route(methods=['get'])
+    @action(detail=False, methods=['get'])
     def discover(self, request):
         schema_name = request.GET.get('schema')
         table_name = request.GET.get('table')
 
         if schema_name and table_name:
             adapter = DatabaseAdapter()
             table_metadata = adapter.fetch_table(schema_name, table_name)
@@ -157,19 +159,19 @@
     permission_classes = (HasModelPermission, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
 
     queryset = Column.objects.all()
     serializer_class = ColumnSerializer
 
     filter_backends = (DjangoFilterBackend, filters.SearchFilter, filters.OrderingFilter)
-    filter_fields = ('name', 'access_level', 'metadata_access_level')
+    filterset_fields = ('name', 'access_level', 'metadata_access_level')
     search_fields = ('name', 'description')
     ordering_fields = ('name', 'access_level', 'metadata_access_level')
 
-    @list_route(methods=['get'])
+    @action(detail=False, methods=['get'])
     def discover(self, request):
         schema_name = request.GET.get('schema')
         table_name = request.GET.get('table')
         column_name = request.GET.get('column')
 
         if schema_name and table_name and column_name:
             return Response([DatabaseAdapter().fetch_column(schema_name, table_name, column_name)])
@@ -181,31 +183,31 @@
     permission_classes = (HasModelPermission, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
 
     queryset = Function.objects.all()
     serializer_class = FunctionSerializer
 
     filter_backends = (DjangoFilterBackend, filters.SearchFilter, filters.OrderingFilter)
-    filter_fields = ('name', 'access_level', 'metadata_access_level')
+    filterset_fields = ('name', 'access_level', 'metadata_access_level')
     search_fields = ('name', 'description')
     ordering_fields = ('name', 'access_level', 'metadata_access_level')
 
-    @list_route(methods=['get'])
+    @action(detail=False, methods=['get'])
     def management(self, request):
         queryset = Function.objects.all()
         serializer = ManagementFunctionSerializer(queryset, many=True)
         return Response(serializer.data)
 
-    @list_route(methods=['get'])
+    @action(detail=False, methods=['get'])
     def export(self, request):
         queryset = Function.objects.all()
         serializer = ExportFunctionSerializer(queryset, many=True)
         return Response(serializer.data)
 
-    @list_route(methods=['get'], permission_classes=[])
+    @action(detail=False, methods=['get'], permission_classes=[])
     def user(self, request):
         queryset = Function.objects.filter_by_access_level(self.request.user)
         serializer = UserFunctionSerializer(queryset, many=True)
         return Response(serializer.data)
 
 
 class TableTypeViewSet(ChoicesViewSet):
@@ -215,15 +217,15 @@
     queryset = Table.TYPE_CHOICES
 
 
 class LicenseViewSet(ChoicesViewSet):
     permission_classes = (IsAuthenticated, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
 
-    queryset = LICENSE_CHOICES
+    queryset = settings.LICENSE_CHOICES
 
 
 class AccessLevelViewSet(ChoicesViewSet):
     permission_classes = (IsAuthenticated, )
     authentication_classes = (SessionAuthentication, TokenAuthentication)
 
     queryset = ACCESS_LEVEL_CHOICES
```

### Comparing `django-daiquiri-0.2/daiquiri/files/utils.py` & `django-daiquiri-0.4.2/daiquiri/files/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,73 @@
-import logging
 import os
-
-from sendfile import sendfile
+import logging
 
 from django.conf import settings
-from django.utils.timezone import now
+from django.contrib.auth.views import redirect_to_login
+from django.core.exceptions import PermissionDenied
+from django.core.paginator import Paginator
+from django.http import Http404
+from django.shortcuts import render
+from django.views.generic import View
+
+from .search import Searcher
+from .utils import (
+        get_directory,
+        get_file_path,
+        render_with_layout,
+        send_file
+)
 
-from daiquiri.core.utils import get_client_ip
-from daiquiri.stats.models import Record
-
-from .models import Directory
 
 logger = logging.getLogger(__name__)
 
 
-def check_file(user, file_path):
-    # loop over all directories beginning with the hights depth and return as soon as a directory matches
-    for directory in Directory.objects.order_by('-depth'):
-        if os.path.normpath(file_path).startswith(directory.path):
-            return Directory.objects.filter_by_access_level(user).filter(pk=directory.pk).exists()
-
-
-def search_file(search_path):
-    base_path = os.path.normpath(settings.FILES_BASE_PATH)
-
-    # look for the file in all directory below the base path
-    results = set()
-    for directory_path, _, _ in os.walk(base_path):
-        normalized_file_path = normalize_file_path(directory_path, search_path)
-        absolute_file_path = os.path.join(directory_path, normalized_file_path)
-
-        if os.path.isfile(absolute_file_path):
-            results.add(absolute_file_path)
-
-    if len(results) == 1:
-        # subtract the base path and return
-        file_path = results.pop().split(base_path, 1)[1].lstrip('/')
-
-        logger.debug('%s => %s', search_path, file_path)
-        return file_path
-    elif len(results) > 1:
-        logger.debug('search_path = %s found more than once', search_path)
-        return None
-    else:
-        logger.debug('search_path = %s not found', search_path)
-        return None
-
-
-def send_file(request, file_path, search=None):
-    # create a stats record for this download
-    resource = {
-        'file_path': file_path
-    }
-    if search:
-        resource['search'] = search
-
-    Record.objects.create(
-        time=now(),
-        resource_type='FILE',
-        resource=resource,
-        client_ip=get_client_ip(request),
-        user=request.user if request.user.is_authenticated else None
-    )
-
-    # send the file to the client
-    absolute_file_path = os.path.join(settings.FILES_BASE_PATH, file_path)
-    return sendfile(request, absolute_file_path, attachment=True)
-
-
-def normalize_file_path(directory_path, file_path):
-
-    directory_path_tokens = os.path.normpath(directory_path).split(os.path.sep)
-    file_path_tokens = os.path.normpath(file_path).split(os.path.sep)
-
-    match = 0
-    for i in range(len(file_path_tokens)):
-        if file_path_tokens[:i] == directory_path_tokens[-i:]:
-            match = i
+class FileView(View):
+
+    root = None
+
+    def get(self, request, file_path, **kwargs):
+        if self.root:
+            logger.debug('root=%s', self.root)
+            file_path = os.path.join(self.root, file_path)
+
+        file_path = get_file_path(file_path)
+        if file_path is None:
+            logger.debug('%s not found', file_path)
+            raise Http404
+
+        directory = get_directory(request.user, file_path)
+        if directory is None:
+            logger.debug('%s is forbidden', file_path)
+            if request.user.is_authenticated:
+                raise PermissionDenied
+            else:
+                return redirect_to_login(request.path_info)
+
+        if file_path.endswith('.html') or file_path.endswith('.md') and directory.layout:
+            return render_with_layout(request, file_path)
+        else:
+            return send_file(request, file_path)
+
+
+class SearchView(View):
+
+    root = None
+
+    def get(self, request, **kwargs):
+
+        search_string = request.GET.get("q", "")
+
+        results = Searcher.search_for_string(string_query=search_string)
+
+        paginator = Paginator(results, settings.FILES_SEARCH_RESULTS_PER_PAGE)
+        page_number = request.GET.get('page')
+        search_results = paginator.get_page(page_number)
+
+        context = {
+                "search_results": search_results,
+                "search_string": search_string,
+                "num_of_search_results": len(results)
+                }
+
+        return render(request, "files/search-results.html", context)
 
-    return os.path.join(*file_path_tokens[match:])
```

### Comparing `django-daiquiri-0.2/daiquiri/files/migrations/0002_depth.py` & `django-daiquiri-0.4.2/daiquiri/files/migrations/0002_depth.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.2/daiquiri/files/models.py` & `django-daiquiri-0.4.2/daiquiri/files/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os
 
-from django.db import models
 from django.conf import settings
 from django.contrib.auth.models import Group
-from django.utils.encoding import python_2_unicode_compatible
-from django.utils.translation import ugettext_lazy as _
+from django.db import models
+from django.utils.translation import gettext_lazy as _
 
 from daiquiri.core.constants import ACCESS_LEVEL_CHOICES
 from daiquiri.core.managers import AccessLevelManager
 
 
-@python_2_unicode_compatible
 class Directory(models.Model):
 
     objects = AccessLevelManager()
 
     path = models.CharField(
         max_length=256, blank=True,
         verbose_name=_('Path'),
         help_text=_('Path of the directory.')
     )
+    layout = models.BooleanField(
+        verbose_name=_('Layout'), default=True,
+        help_text=_('Use the page layout with the content.')
+    )
     access_level = models.CharField(
         max_length=8, choices=ACCESS_LEVEL_CHOICES,
         verbose_name=_('Access level')
     )
     groups = models.ManyToManyField(
         Group, blank=True,
         verbose_name=_('Groups'),
@@ -33,16 +35,14 @@
 
     class Meta:
         ordering = ('path', )
 
         verbose_name = _('Directory')
         verbose_name_plural = _('Directory')
 
-        permissions = (('view_function', 'Can view Directory'),)
-
     def __str__(self):
         return self.absolute_path
 
     def save(self):
         self.depth = len(os.path.normpath(self.path).split(os.path.sep))
         super(Directory, self).save()
```

