# Comparing `tmp/django-map-widgets-0.4.1.tar.gz` & `tmp/django-map-widgets-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-map-widgets-0.4.1.tar", last modified: Wed Dec 21 15:45:23 2022, max compression
+gzip compressed data, was "django-map-widgets-0.4.2.tar", last modified: Thu Jul 20 16:51:19 2023, max compression
```

## Comparing `django-map-widgets-0.4.1.tar` & `django-map-widgets-0.4.2.tar`

### file list

```diff
@@ -1,126 +1,130 @@
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.180791 django-map-widgets-0.4.1/
--rw-r--r--   0 erdem      (501) staff       (20)     1078 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/LICENSE
--rw-r--r--   0 erdem      (501) staff       (20)      191 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/MANIFEST.in
--rw-r--r--   0 erdem      (501) staff       (20)      761 2022-12-21 15:45:23.180894 django-map-widgets-0.4.1/PKG-INFO
--rw-r--r--   0 erdem      (501) staff       (20)     4625 2022-12-21 15:44:08.000000 django-map-widgets-0.4.1/README.md
--rw-r--r--   0 erdem      (501) staff       (20)     3659 2022-12-21 15:44:28.000000 django-map-widgets-0.4.1/README.rst
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.165243 django-map-widgets-0.4.1/django_map_widgets.egg-info/
--rw-r--r--   0 erdem      (501) staff       (20)      761 2022-12-21 15:45:23.000000 django-map-widgets-0.4.1/django_map_widgets.egg-info/PKG-INFO
--rw-r--r--   0 erdem      (501) staff       (20)     3587 2022-12-21 15:45:23.000000 django-map-widgets-0.4.1/django_map_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 erdem      (501) staff       (20)        1 2022-12-21 15:45:23.000000 django-map-widgets-0.4.1/django_map_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 erdem      (501) staff       (20)       17 2022-12-21 15:45:23.000000 django-map-widgets-0.4.1/django_map_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.166386 django-map-widgets-0.4.1/mapwidgets/
--rw-r--r--   0 erdem      (501) staff       (20)      220 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/__init__.py
--rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/admin.py
--rw-r--r--   0 erdem      (501) staff       (20)    15648 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/constants.py
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.159366 django-map-widgets-0.4.1/mapwidgets/locale/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.158289 django-map-widgets-0.4.1/mapwidgets/locale/de/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.166841 django-map-widgets-0.4.1/mapwidgets/locale/de/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)      761 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     1536 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.158407 django-map-widgets-0.4.1/mapwidgets/locale/en/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.167264 django-map-widgets-0.4.1/mapwidgets/locale/en/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)      337 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     1397 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.158527 django-map-widgets-0.4.1/mapwidgets/locale/es/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.167666 django-map-widgets-0.4.1/mapwidgets/locale/es/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)      802 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     1810 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.158638 django-map-widgets-0.4.1/mapwidgets/locale/et/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.168018 django-map-widgets-0.4.1/mapwidgets/locale/et/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)      732 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     1507 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.158749 django-map-widgets-0.4.1/mapwidgets/locale/it/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.168321 django-map-widgets-0.4.1/mapwidgets/locale/it/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)      738 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     1513 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.158862 django-map-widgets-0.4.1/mapwidgets/locale/ja/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.168623 django-map-widgets-0.4.1/mapwidgets/locale/ja/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)      762 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     1541 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.158995 django-map-widgets-0.4.1/mapwidgets/locale/pt_BR/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.168965 django-map-widgets-0.4.1/mapwidgets/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)      783 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     1562 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.159132 django-map-widgets-0.4.1/mapwidgets/locale/ru/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.169286 django-map-widgets-0.4.1/mapwidgets/locale/ru/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)     1010 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     1795 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.159276 django-map-widgets-0.4.1/mapwidgets/locale/sk/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.169600 django-map-widgets-0.4.1/mapwidgets/locale/sk/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)     1235 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     2008 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.169778 django-map-widgets-0.4.1/mapwidgets/locale/zh/
--rw-r--r--   0 erdem      (501) staff       (20)     6148 2022-12-21 15:23:21.000000 django-map-widgets-0.4.1/mapwidgets/locale/zh/.DS_Store
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.170307 django-map-widgets-0.4.1/mapwidgets/locale/zh/LC_MESSAGES/
--rw-r--r--   0 erdem      (501) staff       (20)      778 2022-12-21 15:23:12.000000 django-map-widgets-0.4.1/mapwidgets/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 erdem      (501) staff       (20)     2421 2022-12-21 15:21:50.000000 django-map-widgets-0.4.1/mapwidgets/locale/zh/LC_MESSAGES/django.po
--rw-r--r--   0 erdem      (501) staff       (20)     5248 2022-12-21 14:52:28.000000 django-map-widgets-0.4.1/mapwidgets/settings.py
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.159589 django-map-widgets-0.4.1/mapwidgets/static/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.170544 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/
--rw-r--r--   0 erdem      (501) staff       (20)     6148 2022-05-15 23:27:30.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/.DS_Store
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.171576 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/
--rw-r--r--   0 erdem      (501) staff       (20)     7014 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/magnific-popup.css
--rw-r--r--   0 erdem      (501) staff       (20)     5388 2022-05-15 23:25:02.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/magnific-popup.min.css
--rw-r--r--   0 erdem      (501) staff       (20)    17302 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/map_widgets.css
--rw-r--r--   0 erdem      (501) staff       (20)    14031 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/map_widgets.min.css
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.172695 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/
--rwxr-xr-x   0 erdem      (501) staff       (20)     5952 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.eot
--rwxr-xr-x   0 erdem      (501) staff       (20)     2086 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.svg
--rwxr-xr-x   0 erdem      (501) staff       (20)     5784 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.ttf
--rwxr-xr-x   0 erdem      (501) staff       (20)     3396 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.woff
--rwxr-xr-x   0 erdem      (501) staff       (20)     2788 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.woff2
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.173003 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/images/
--rw-r--r--   0 erdem      (501) staff       (20)     8261 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/images/no-map-image.png
--rw-r--r--   0 erdem      (501) staff       (20)    94267 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/images/ripple.gif
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.175204 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/
--rw-r--r--   0 erdem      (501) staff       (20)     7050 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/django_mw_base.js
--rw-r--r--   0 erdem      (501) staff       (20)    66974 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/jquery.custom.magnific-popup.js
--rw-r--r--   0 erdem      (501) staff       (20)    28305 2022-05-15 23:24:55.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/jquery.custom.magnific-popup.min.js
--rw-r--r--   0 erdem      (501) staff       (20)     1882 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/jquery_class.js
--rw-r--r--   0 erdem      (501) staff       (20)      302 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/jquery_init.js
--rw-r--r--   0 erdem      (501) staff       (20)     4227 2022-12-21 14:48:48.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_google_point_field.js
--rw-r--r--   0 erdem      (501) staff       (20)     9549 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_google_point_field.min.js
--rw-r--r--   0 erdem      (501) staff       (20)     2828 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_google_point_field_generater.js
--rw-r--r--   0 erdem      (501) staff       (20)    11609 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_google_point_inline_field.min.js
--rw-r--r--   0 erdem      (501) staff       (20)     6812 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_mapbox_point_field.js
--rw-r--r--   0 erdem      (501) staff       (20)    11190 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_mapbox_point_field.min.js
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.159971 django-map-widgets-0.4.1/mapwidgets/templates/
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.176125 django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/
--rw-r--r--   0 erdem      (501) staff       (20)     3028 2022-12-21 15:06:10.000000 django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/google-point-field-inline-widget.html
--rw-r--r--   0 erdem      (501) staff       (20)     5129 2022-12-21 15:06:18.000000 django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/google-point-field-widget.html
--rw-r--r--   0 erdem      (501) staff       (20)      254 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/google-static-map.html
--rw-r--r--   0 erdem      (501) staff       (20)      249 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/google-static-overlay-map.html
--rw-r--r--   0 erdem      (501) staff       (20)     4506 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/mapbox-point-field-widget.html
--rw-r--r--   0 erdem      (501) staff       (20)    14543 2022-05-16 00:43:41.000000 django-map-widgets-0.4.1/mapwidgets/widgets.py
--rw-r--r--   0 erdem      (501) staff       (20)      102 2022-12-21 15:45:23.181143 django-map-widgets-0.4.1/setup.cfg
--rw-r--r--   0 erdem      (501) staff       (20)     1079 2022-12-21 15:42:55.000000 django-map-widgets-0.4.1/setup.py
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.176285 django-map-widgets-0.4.1/tests/
--rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/__init__.py
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.176477 django-map-widgets-0.4.1/tests/testapp/
--rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/__init__.py
--rwxr-xr-x   0 erdem      (501) staff       (20)      805 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/manage.py
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.177219 django-map-widgets-0.4.1/tests/testapp/testapp/
--rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/testapp/__init__.py
--rw-r--r--   0 erdem      (501) staff       (20)     4501 2021-06-26 15:34:06.000000 django-map-widgets-0.4.1/tests/testapp/testapp/settings.py
--rw-r--r--   0 erdem      (501) staff       (20)     1141 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/testapp/urls.py
--rw-r--r--   0 erdem      (501) staff       (20)      392 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/testapp/wsgi.py
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.178435 django-map-widgets-0.4.1/tests/testapp/widgets/
--rw-r--r--   0 erdem      (501) staff       (20)      142 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/__init__.py
--rw-r--r--   0 erdem      (501) staff       (20)      756 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/admin.py
--rw-r--r--   0 erdem      (501) staff       (20)      130 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/apps.py
--rw-r--r--   0 erdem      (501) staff       (20)      423 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/forms.py
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.178885 django-map-widgets-0.4.1/tests/testapp/widgets/migrations/
--rw-r--r--   0 erdem      (501) staff       (20)      795 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/migrations/0001_initial.py
--rw-r--r--   0 erdem      (501) staff       (20)      806 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/migrations/0002_street.py
--rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/migrations/__init__.py
--rw-r--r--   0 erdem      (501) staff       (20)      528 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/models.py
-drwxr-xr-x   0 erdem      (501) staff       (20)        0 2022-12-21 15:45:23.180621 django-map-widgets-0.4.1/tests/testapp/widgets/tests/
--rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/tests/__init__.py
--rw-r--r--   0 erdem      (501) staff       (20)      120 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/tests/constants.py
--rw-r--r--   0 erdem      (501) staff       (20)      764 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/tests/mixins.py
--rw-r--r--   0 erdem      (501) staff       (20)     3170 2021-04-11 21:11:06.000000 django-map-widgets-0.4.1/tests/testapp/widgets/tests/test_settings.py
--rw-r--r--   0 erdem      (501) staff       (20)    17925 2021-04-11 21:11:06.000000 django-map-widgets-0.4.1/tests/testapp/widgets/tests/test_widgets.py
--rw-r--r--   0 erdem      (501) staff       (20)      748 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/tests/utils.py
--rw-r--r--   0 erdem      (501) staff       (20)      673 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/urls.py
--rw-r--r--   0 erdem      (501) staff       (20)      600 2021-01-03 13:10:31.000000 django-map-widgets-0.4.1/tests/testapp/widgets/views.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.916426 django-map-widgets-0.4.2/
+-rw-r--r--   0 erdem      (501) staff       (20)     1078 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/LICENSE
+-rw-r--r--   0 erdem      (501) staff       (20)      191 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/MANIFEST.in
+-rw-r--r--   0 erdem      (501) staff       (20)      759 2023-07-20 16:51:19.916480 django-map-widgets-0.4.2/PKG-INFO
+-rw-r--r--   0 erdem      (501) staff       (20)     4803 2023-07-20 16:50:49.000000 django-map-widgets-0.4.2/README.md
+-rw-r--r--   0 erdem      (501) staff       (20)     3814 2023-07-20 16:51:03.000000 django-map-widgets-0.4.2/README.rst
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.902583 django-map-widgets-0.4.2/django_map_widgets.egg-info/
+-rw-r--r--   0 erdem      (501) staff       (20)      759 2023-07-20 16:51:19.000000 django-map-widgets-0.4.2/django_map_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 erdem      (501) staff       (20)     3673 2023-07-20 16:51:19.000000 django-map-widgets-0.4.2/django_map_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 erdem      (501) staff       (20)        1 2023-07-20 16:51:19.000000 django-map-widgets-0.4.2/django_map_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 erdem      (501) staff       (20)       17 2023-07-20 16:51:19.000000 django-map-widgets-0.4.2/django_map_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.903611 django-map-widgets-0.4.2/mapwidgets/
+-rw-r--r--   0 erdem      (501) staff       (20)      220 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/__init__.py
+-rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/admin.py
+-rw-r--r--   0 erdem      (501) staff       (20)    15648 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/constants.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.900148 django-map-widgets-0.4.2/mapwidgets/locale/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899165 django-map-widgets-0.4.2/mapwidgets/locale/de/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.903904 django-map-widgets-0.4.2/mapwidgets/locale/de/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)      761 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     1536 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899269 django-map-widgets-0.4.2/mapwidgets/locale/en/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.904171 django-map-widgets-0.4.2/mapwidgets/locale/en/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)      337 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     1397 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899369 django-map-widgets-0.4.2/mapwidgets/locale/es/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.904443 django-map-widgets-0.4.2/mapwidgets/locale/es/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)      802 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     1810 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899469 django-map-widgets-0.4.2/mapwidgets/locale/et/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.904716 django-map-widgets-0.4.2/mapwidgets/locale/et/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)      732 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     1507 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899567 django-map-widgets-0.4.2/mapwidgets/locale/it/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.904977 django-map-widgets-0.4.2/mapwidgets/locale/it/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)      738 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     1513 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899666 django-map-widgets-0.4.2/mapwidgets/locale/ja/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.905240 django-map-widgets-0.4.2/mapwidgets/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)      762 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     1541 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899769 django-map-widgets-0.4.2/mapwidgets/locale/pl/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.905565 django-map-widgets-0.4.2/mapwidgets/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)     1010 2023-07-20 15:45:55.000000 django-map-widgets-0.4.2/mapwidgets/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     2640 2023-07-20 15:45:55.000000 django-map-widgets-0.4.2/mapwidgets/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899880 django-map-widgets-0.4.2/mapwidgets/locale/pt_BR/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.905872 django-map-widgets-0.4.2/mapwidgets/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)      783 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     1562 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.899980 django-map-widgets-0.4.2/mapwidgets/locale/ru/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.906133 django-map-widgets-0.4.2/mapwidgets/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)     1010 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     1795 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.900087 django-map-widgets-0.4.2/mapwidgets/locale/sk/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.906398 django-map-widgets-0.4.2/mapwidgets/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)     1235 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     2008 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.906549 django-map-widgets-0.4.2/mapwidgets/locale/zh/
+-rw-r--r--   0 erdem      (501) staff       (20)     6148 2022-12-21 15:23:21.000000 django-map-widgets-0.4.2/mapwidgets/locale/zh/.DS_Store
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.906980 django-map-widgets-0.4.2/mapwidgets/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 erdem      (501) staff       (20)      778 2022-12-21 20:25:18.000000 django-map-widgets-0.4.2/mapwidgets/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 erdem      (501) staff       (20)     2421 2022-12-21 20:25:18.000000 django-map-widgets-0.4.2/mapwidgets/locale/zh/LC_MESSAGES/django.po
+-rw-r--r--   0 erdem      (501) staff       (20)     5248 2022-12-21 20:25:18.000000 django-map-widgets-0.4.2/mapwidgets/settings.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.900325 django-map-widgets-0.4.2/mapwidgets/static/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.907158 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/
+-rw-r--r--   0 erdem      (501) staff       (20)     6148 2022-05-15 23:27:30.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/.DS_Store
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.908155 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/
+-rw-r--r--   0 erdem      (501) staff       (20)     7014 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/magnific-popup.css
+-rw-r--r--   0 erdem      (501) staff       (20)     5388 2023-07-20 16:33:59.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/magnific-popup.min.css
+-rw-r--r--   0 erdem      (501) staff       (20)    17302 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/map_widgets.css
+-rw-r--r--   0 erdem      (501) staff       (20)    14031 2023-07-20 16:33:45.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/map_widgets.min.css
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.909145 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/
+-rwxr-xr-x   0 erdem      (501) staff       (20)     5952 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.eot
+-rwxr-xr-x   0 erdem      (501) staff       (20)     2086 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.svg
+-rwxr-xr-x   0 erdem      (501) staff       (20)     5784 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.ttf
+-rwxr-xr-x   0 erdem      (501) staff       (20)     3396 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.woff
+-rwxr-xr-x   0 erdem      (501) staff       (20)     2788 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.woff2
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.909432 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/images/
+-rw-r--r--   0 erdem      (501) staff       (20)     8261 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/images/no-map-image.png
+-rw-r--r--   0 erdem      (501) staff       (20)    94267 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/images/ripple.gif
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.911778 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/
+-rw-r--r--   0 erdem      (501) staff       (20)     7050 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/django_mw_base.js
+-rw-r--r--   0 erdem      (501) staff       (20)    66974 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/jquery.custom.magnific-popup.js
+-rw-r--r--   0 erdem      (501) staff       (20)    28305 2023-07-20 16:33:37.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/jquery.custom.magnific-popup.min.js
+-rw-r--r--   0 erdem      (501) staff       (20)     1882 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/jquery_class.js
+-rw-r--r--   0 erdem      (501) staff       (20)      302 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/jquery_init.js
+-rw-r--r--   0 erdem      (501) staff       (20)     4227 2022-12-21 20:25:18.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_google_point_field.js
+-rw-r--r--   0 erdem      (501) staff       (20)     9571 2023-07-20 16:38:44.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_google_point_field.min.js
+-rw-r--r--   0 erdem      (501) staff       (20)     2932 2023-07-20 16:38:30.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_google_point_field_generater.js
+-rw-r--r--   0 erdem      (501) staff       (20)    11701 2023-07-20 16:38:44.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_google_point_inline_field.min.js
+-rw-r--r--   0 erdem      (501) staff       (20)     6812 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_mapbox_point_field.js
+-rw-r--r--   0 erdem      (501) staff       (20)    11190 2023-07-20 16:33:26.000000 django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_mapbox_point_field.min.js
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.900814 django-map-widgets-0.4.2/mapwidgets/templates/
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.912532 django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/
+-rw-r--r--   0 erdem      (501) staff       (20)     3028 2022-12-21 20:25:18.000000 django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/google-point-field-inline-widget.html
+-rw-r--r--   0 erdem      (501) staff       (20)     5147 2023-07-20 15:45:55.000000 django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/google-point-field-widget.html
+-rw-r--r--   0 erdem      (501) staff       (20)      254 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/google-static-map.html
+-rw-r--r--   0 erdem      (501) staff       (20)      249 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/google-static-overlay-map.html
+-rw-r--r--   0 erdem      (501) staff       (20)     4506 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/mapbox-point-field-widget.html
+-rw-r--r--   0 erdem      (501) staff       (20)    14543 2022-05-16 00:43:41.000000 django-map-widgets-0.4.2/mapwidgets/widgets.py
+-rw-r--r--   0 erdem      (501) staff       (20)      102 2023-07-20 16:51:19.916678 django-map-widgets-0.4.2/setup.cfg
+-rw-r--r--   0 erdem      (501) staff       (20)     1079 2023-07-20 16:49:12.000000 django-map-widgets-0.4.2/setup.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.912755 django-map-widgets-0.4.2/tests/
+-rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/__init__.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.912949 django-map-widgets-0.4.2/tests/testapp/
+-rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/__init__.py
+-rwxr-xr-x   0 erdem      (501) staff       (20)      805 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/manage.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.913591 django-map-widgets-0.4.2/tests/testapp/testapp/
+-rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/testapp/__init__.py
+-rw-r--r--   0 erdem      (501) staff       (20)     4501 2021-06-26 15:34:06.000000 django-map-widgets-0.4.2/tests/testapp/testapp/settings.py
+-rw-r--r--   0 erdem      (501) staff       (20)     1141 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/testapp/urls.py
+-rw-r--r--   0 erdem      (501) staff       (20)      392 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/testapp/wsgi.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.914723 django-map-widgets-0.4.2/tests/testapp/widgets/
+-rw-r--r--   0 erdem      (501) staff       (20)      142 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/__init__.py
+-rw-r--r--   0 erdem      (501) staff       (20)      756 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/admin.py
+-rw-r--r--   0 erdem      (501) staff       (20)      130 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/apps.py
+-rw-r--r--   0 erdem      (501) staff       (20)      423 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/forms.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.915118 django-map-widgets-0.4.2/tests/testapp/widgets/migrations/
+-rw-r--r--   0 erdem      (501) staff       (20)      795 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/migrations/0001_initial.py
+-rw-r--r--   0 erdem      (501) staff       (20)      806 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/migrations/0002_street.py
+-rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/migrations/__init__.py
+-rw-r--r--   0 erdem      (501) staff       (20)      528 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/models.py
+drwxr-xr-x   0 erdem      (501) staff       (20)        0 2023-07-20 16:51:19.916294 django-map-widgets-0.4.2/tests/testapp/widgets/tests/
+-rw-r--r--   0 erdem      (501) staff       (20)        0 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/tests/__init__.py
+-rw-r--r--   0 erdem      (501) staff       (20)      120 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/tests/constants.py
+-rw-r--r--   0 erdem      (501) staff       (20)      764 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/tests/mixins.py
+-rw-r--r--   0 erdem      (501) staff       (20)     3170 2021-04-11 21:11:06.000000 django-map-widgets-0.4.2/tests/testapp/widgets/tests/test_settings.py
+-rw-r--r--   0 erdem      (501) staff       (20)    17925 2021-04-11 21:11:06.000000 django-map-widgets-0.4.2/tests/testapp/widgets/tests/test_widgets.py
+-rw-r--r--   0 erdem      (501) staff       (20)      748 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/tests/utils.py
+-rw-r--r--   0 erdem      (501) staff       (20)      673 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/urls.py
+-rw-r--r--   0 erdem      (501) staff       (20)      600 2021-01-03 13:10:31.000000 django-map-widgets-0.4.2/tests/testapp/widgets/views.py
```

### Comparing `django-map-widgets-0.4.1/LICENSE` & `django-map-widgets-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/PKG-INFO` & `django-map-widgets-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-map-widgets
-Version: 0.4.1
+Version: 0.4.2
 Summary: Map widgets for Django PostGIS fields
 Home-page: https://github.com/erdem/django-map-widgets
 Author: Erdem Ozkol
 Author-email: erdemozkol@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -15,9 +15,7 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 Configurable, pluggable and more user friendly map widgets for Django PostGIS fields. 
 Please check the `project home page <https://github.com/erdem/django-map-widgets/>`_ for latest updates.
-
-
```

### Comparing `django-map-widgets-0.4.1/README.md` & `django-map-widgets-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,20 @@
 This widget is working with <a href="http://dimsemenov.com/plugins/magnific-popup/" target="_blank">Magnific Popup</a> jQuery plugin.
 
 ![](https://cloud.githubusercontent.com/assets/1518272/18732296/18f1813e-805a-11e6-8801-f1f48ed02a9c.png)
 
 
 ### Release Notes
 
+
+#### 0.4.2
+> -   GooglePointFieldInlineWidget bug fixes for Django 4.2.x (#142), thanks for @isarota.
+> -   Added `.readthedocs.yaml` to cover new **Read the Docs** updates. 
+
+
 #### 0.4.1
 > -   Added scroll wheel zooming functionality switch to Google Point Map Settings. (#134)
 > -   Added Chinese(ZH) localisation support. (#133)
 
 #### 0.4.0
 > -   Supported MapBox Map for Django Geo Point Field.
 > -   Fixed undefined place object binding issue in javascript triggers. (#125)
```

### Comparing `django-map-widgets-0.4.1/README.rst` & `django-map-widgets-0.4.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,21 @@
    :width: 100 %
 
 
 Release Notes
 ^^^^^^^^^^^^^
 
 =====
+0.4.2
+=====
+
+ * GooglePointFieldInlineWidget bug fixes for Django 4.2.x (#142)
+ * Added `.readthedocs.yaml` to cover new **Read the Docs** updates.
+
+=====
 0.4.1
 =====
 
  * Added scroll wheel zooming functionality switch to Google Point Map Settings. (#134)
  * Added Chinese(ZH) localisation support. (#133)
 
 =====
```

### Comparing `django-map-widgets-0.4.1/django_map_widgets.egg-info/PKG-INFO` & `django-map-widgets-0.4.2/django_map_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-map-widgets
-Version: 0.4.1
+Version: 0.4.2
 Summary: Map widgets for Django PostGIS fields
 Home-page: https://github.com/erdem/django-map-widgets
 Author: Erdem Ozkol
 Author-email: erdemozkol@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -15,9 +15,7 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 Configurable, pluggable and more user friendly map widgets for Django PostGIS fields. 
 Please check the `project home page <https://github.com/erdem/django-map-widgets/>`_ for latest updates.
-
-
```

### Comparing `django-map-widgets-0.4.1/django_map_widgets.egg-info/SOURCES.txt` & `django-map-widgets-0.4.2/django_map_widgets.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 mapwidgets/locale/es/LC_MESSAGES/django.po
 mapwidgets/locale/et/LC_MESSAGES/django.mo
 mapwidgets/locale/et/LC_MESSAGES/django.po
 mapwidgets/locale/it/LC_MESSAGES/django.mo
 mapwidgets/locale/it/LC_MESSAGES/django.po
 mapwidgets/locale/ja/LC_MESSAGES/django.mo
 mapwidgets/locale/ja/LC_MESSAGES/django.po
+mapwidgets/locale/pl/LC_MESSAGES/django.mo
+mapwidgets/locale/pl/LC_MESSAGES/django.po
 mapwidgets/locale/pt_BR/LC_MESSAGES/django.mo
 mapwidgets/locale/pt_BR/LC_MESSAGES/django.po
 mapwidgets/locale/ru/LC_MESSAGES/django.mo
 mapwidgets/locale/ru/LC_MESSAGES/django.po
 mapwidgets/locale/sk/LC_MESSAGES/django.mo
 mapwidgets/locale/sk/LC_MESSAGES/django.po
 mapwidgets/locale/zh/.DS_Store
```

### Comparing `django-map-widgets-0.4.1/mapwidgets/constants.py` & `django-map-widgets-0.4.2/mapwidgets/constants.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/de/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/de/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/en/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/es/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/es/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/et/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/et/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/it/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/it/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/ja/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/ja/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/pt_BR/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/pt_BR/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/ru/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/ru/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/sk/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/sk/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/zh/.DS_Store` & `django-map-widgets-0.4.2/mapwidgets/locale/zh/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/zh/LC_MESSAGES/django.mo` & `django-map-widgets-0.4.2/mapwidgets/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/locale/zh/LC_MESSAGES/django.po` & `django-map-widgets-0.4.2/mapwidgets/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/settings.py` & `django-map-widgets-0.4.2/mapwidgets/settings.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/.DS_Store` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/magnific-popup.css` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/magnific-popup.css`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/magnific-popup.min.css` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/magnific-popup.min.css`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/map_widgets.css` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/map_widgets.css`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/css/map_widgets.min.css` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/css/map_widgets.min.css`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.eot` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.eot`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.svg` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.svg`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.ttf` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.ttf`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.woff` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.woff`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/font/fontello.woff2` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/font/fontello.woff2`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/images/no-map-image.png` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/images/no-map-image.png`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/images/ripple.gif` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/images/ripple.gif`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/django_mw_base.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/django_mw_base.js`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/jquery.custom.magnific-popup.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/jquery.custom.magnific-popup.js`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/jquery.custom.magnific-popup.min.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/jquery.custom.magnific-popup.min.js`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/jquery_class.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/jquery_class.js`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_google_point_field.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_google_point_field.js`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_google_point_field.min.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_google_point_field.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -238,30 +238,30 @@
                 }, function(results, status) {
                     if (status === google.maps.GeocoderStatus.OK) {
                         var geo_location = results[0].geometry.location;
                         mapCenter = [geo_location.lat(), geo_location.lng()]
                     }
                     this.map = new google.maps.Map(this.mapElement, {
                         center: new google.maps.LatLng(mapCenter[0], mapCenter[1]),
-                        scrollwheel: false,
+                        scrollwheel: this.scrollWheel,
                         zoomControlOptions: {
                             position: google.maps.ControlPosition.RIGHT
                         },
                         zoom: this.zoom,
                         streetViewControl: this.streetViewControl
                     });
                     if (!$.isEmptyObject(this.locationFieldValue)) {
                         this.updateLocationInput(this.locationFieldValue.lat, this.locationFieldValue.lng);
                         this.fitBoundMarker()
                     }
                 }.bind(this))
             } else {
                 this.map = new google.maps.Map(this.mapElement, {
                     center: new google.maps.LatLng(mapCenter[0], mapCenter[1]),
-                    scrollwheel: false,
+                    scrollwheel: this.scrollWheel,
                     zoomControlOptions: {
                         position: google.maps.ControlPosition.RIGHT
                     },
                     zoom: this.zoom,
                     streetViewControl: this.streetViewControl
                 });
                 if (!$.isEmptyObject(this.locationFieldValue)) {
```

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_google_point_field_generater.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_google_point_field_generater.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -6,16 +6,18 @@
             $(document).on('formset:added', this.handle_added_formset_row.bind(this));
         },
 
         handle_added_formset_row: function(e, row, prefix) {
             var mapOptions = this.mapOptions;
             var widgetData = {};
 
+            prefix = prefix || $(e.target).attr("id").split("-")[0];
             var id_regex = new RegExp("(" + prefix + "-(\\d+|__prefix__))");
 
+            row = row || e.target;
             var numberPattern = /\d+/g;
             var row_index = $(row).attr("id").match(numberPattern);
             var replacement = prefix + "-" + row_index;
             $.each(this.widgetDataTemplate, function(key, value) {
                 widgetData[key] = value.replace(id_regex, replacement)
             });
```

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_google_point_inline_field.min.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_google_point_inline_field.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -238,30 +238,30 @@
                 }, function(results, status) {
                     if (status === google.maps.GeocoderStatus.OK) {
                         var geo_location = results[0].geometry.location;
                         mapCenter = [geo_location.lat(), geo_location.lng()]
                     }
                     this.map = new google.maps.Map(this.mapElement, {
                         center: new google.maps.LatLng(mapCenter[0], mapCenter[1]),
-                        scrollwheel: false,
+                        scrollwheel: this.scrollWheel,
                         zoomControlOptions: {
                             position: google.maps.ControlPosition.RIGHT
                         },
                         zoom: this.zoom,
                         streetViewControl: this.streetViewControl
                     });
                     if (!$.isEmptyObject(this.locationFieldValue)) {
                         this.updateLocationInput(this.locationFieldValue.lat, this.locationFieldValue.lng);
                         this.fitBoundMarker()
                     }
                 }.bind(this))
             } else {
                 this.map = new google.maps.Map(this.mapElement, {
                     center: new google.maps.LatLng(mapCenter[0], mapCenter[1]),
-                    scrollwheel: false,
+                    scrollwheel: this.scrollWheel,
                     zoomControlOptions: {
                         position: google.maps.ControlPosition.RIGHT
                     },
                     zoom: this.zoom,
                     streetViewControl: this.streetViewControl
                 });
                 if (!$.isEmptyObject(this.locationFieldValue)) {
@@ -329,15 +329,17 @@
         init: function(options) {
             $.extend(this, options);
             $(document).on("formset:added", this.handle_added_formset_row.bind(this))
         },
         handle_added_formset_row: function(e, row, prefix) {
             var mapOptions = this.mapOptions;
             var widgetData = {};
+            prefix = prefix || $(e.target).attr("id").split("-")[0];
             var id_regex = new RegExp("(" + prefix + "-(\\d+|__prefix__))");
+            row = row || e.target;
             var numberPattern = /\d+/g;
             var row_index = $(row).attr("id").match(numberPattern);
             var replacement = prefix + "-" + row_index;
             $.each(this.widgetDataTemplate, function(key, value) {
                 widgetData[key] = value.replace(id_regex, replacement)
             });
             var wrapElemSelector = widgetData.wrapElemSelector;
```

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_mapbox_point_field.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_mapbox_point_field.js`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/static/mapwidgets/js/mw_mapbox_point_field.min.js` & `django-map-widgets-0.4.2/mapwidgets/static/mapwidgets/js/mw_mapbox_point_field.min.js`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/google-point-field-inline-widget.html` & `django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/google-point-field-inline-widget.html`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/google-point-field-widget.html` & `django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/google-point-field-widget.html`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,14 @@
                 GooglePlaceAutocompleteOptions: mapOptions.GooglePlaceAutocompleteOptions,
                 streetViewControl: mapOptions.streetViewControl,
                 markerCreateTriggerNameSpace: "google_point_map_widget:marker_create",
                 markerChangeTriggerNameSpace: "google_point_map_widget:marker_change",
                 markerDeleteTriggerNameSpace: "google_point_map_widget:marker_delete",
                 placeChangedTriggerNameSpace: "google_point_map_widget:place_changed"
             };
-            new DjangoGooglePointFieldWidget(mapWidgetOptions);
+            const mapWidget = new DjangoGooglePointFieldWidget(mapWidgetOptions);
             {% block extra_javascript %}
 
             {% endblock %}
         })(mapWidgets.jQuery);
     </script>
 {% endblock javascript %}
```

### Comparing `django-map-widgets-0.4.1/mapwidgets/templates/mapwidgets/mapbox-point-field-widget.html` & `django-map-widgets-0.4.2/mapwidgets/templates/mapwidgets/mapbox-point-field-widget.html`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/mapwidgets/widgets.py` & `django-map-widgets-0.4.2/mapwidgets/widgets.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/setup.py` & `django-map-widgets-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = (0, 4, 1)
+VERSION = (0, 4, 2)
 __version__ = '.'.join(map(str, VERSION))
 
 
 LONG_DESCRIPTION = """
 Configurable, pluggable and more user friendly map widgets for Django PostGIS fields. 
 Please check the `project home page <https://github.com/erdem/django-map-widgets/>`_ for latest updates.
 """
```

### Comparing `django-map-widgets-0.4.1/tests/testapp/manage.py` & `django-map-widgets-0.4.2/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/testapp/settings.py` & `django-map-widgets-0.4.2/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/testapp/urls.py` & `django-map-widgets-0.4.2/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/admin.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/admin.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/migrations/0001_initial.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/migrations/0002_street.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/migrations/0002_street.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/models.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/models.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/tests/mixins.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/tests/test_settings.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/tests/test_widgets.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/tests/utils.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/urls.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/urls.py`

 * *Files identical despite different names*

### Comparing `django-map-widgets-0.4.1/tests/testapp/widgets/views.py` & `django-map-widgets-0.4.2/tests/testapp/widgets/views.py`

 * *Files identical despite different names*

