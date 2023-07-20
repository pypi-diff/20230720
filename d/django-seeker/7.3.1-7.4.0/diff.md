# Comparing `tmp/django-seeker-7.3.1.tar.gz` & `tmp/django-seeker-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-seeker-7.3.1.tar", last modified: Fri Apr 21 13:48:16 2023, max compression
+gzip compressed data, was "django-seeker-7.4.0.tar", last modified: Thu Jul 20 19:55:47 2023, max compression
```

## Comparing `django-seeker-7.3.1.tar` & `django-seeker-7.4.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.218403 django-seeker-7.3.1/
--rw-rw----   0 ruttenb   (1328) ims        (100)     1316 2018-10-01 19:52:22.000000 django-seeker-7.3.1/LICENSE
--rw-rw----   0 ruttenb   (1328) ims        (100)       38 2018-10-01 19:52:22.000000 django-seeker-7.3.1/MANIFEST.in
--rw-r--r--   0 ruttenb   (1328) ims        (100)      589 2023-04-21 13:48:16.219405 django-seeker-7.3.1/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)      249 2018-10-01 19:52:22.000000 django-seeker-7.3.1/README.md
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.756385 django-seeker-7.3.1/django_seeker.egg-info/
--rw-rw----   0 ruttenb   (1328) ims        (100)      589 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)     2086 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/SOURCES.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)        1 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/dependency_links.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)       70 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/requires.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)        7 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/top_level.txt
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.917385 django-seeker-7.3.1/seeker/
--rw-r--r--   0 ruttenb   (1328) ims        (100)      599 2023-04-21 13:46:11.000000 django-seeker-7.3.1/seeker/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      564 2019-04-26 17:33:41.000000 django-seeker-7.3.1/seeker/admin.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     2945 2019-06-18 15:37:07.000000 django-seeker-7.3.1/seeker/apps.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     1024 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/dsl.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)    25148 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/facets.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1630 2019-02-08 19:43:15.000000 django-seeker-7.3.1/seeker/forms.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     2078 2019-10-10 15:12:29.000000 django-seeker-7.3.1/seeker/indexer.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.975391 django-seeker-7.3.1/seeker/management/
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/management/__init__.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.998383 django-seeker-7.3.1/seeker/management/commands/
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/management/commands/__init__.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     2295 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/management/commands/dropindex.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     1188 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/management/commands/dumpindex.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     1275 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/management/commands/loadindex.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     4026 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/management/commands/reindex.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)    11740 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/mapping.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1016 2019-06-18 15:37:07.000000 django-seeker-7.3.1/seeker/middleware.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.063384 django-seeker-7.3.1/seeker/migrations/
--rw-rw----   0 ruttenb   (1328) ims        (100)     1193 2019-06-18 15:37:07.000000 django-seeker-7.3.1/seeker/migrations/0001_initial.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      499 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/migrations/0002_auto_20150507_0134.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      838 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/migrations/0003_auto_20180214_1501.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      971 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/migrations/0004_auto_20180322_1412.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      457 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/migrations/0005_auto_20180330_1708.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      714 2019-06-25 20:26:14.000000 django-seeker-7.3.1/seeker/migrations/0006_auto_20190625_1139.py
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/migrations/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1602 2020-10-14 20:36:41.000000 django-seeker-7.3.1/seeker/models.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      877 2021-09-01 20:33:51.000000 django-seeker-7.3.1/seeker/registry.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)      823 2022-12-15 21:11:12.000000 django-seeker-7.3.1/seeker/signals.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.680394 django-seeker-7.3.1/seeker/templates/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.092401 django-seeker-7.3.1/seeker/templates/advanced_seeker/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.119386 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/
--rw-rw----   0 ruttenb   (1328) ims        (100)      628 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/date_range.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      444 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/range.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      218 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/terms.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      306 2019-03-14 18:04:52.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/text.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      218 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/year_histogram.html
--rw-r--r--   0 ruttenb   (1328) ims        (100)     2561 2022-12-15 21:11:12.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/footer.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      243 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/header.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      854 2019-10-17 18:45:08.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/pager.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     2428 2019-09-23 17:53:11.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/results.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      465 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/save_form.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1341 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/seeker.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.183393 django-seeker-7.3.1/seeker/templates/seeker/
--rw-rw----   0 ruttenb   (1328) ims        (100)      267 2019-09-23 17:53:11.000000 django-seeker-7.3.1/seeker/templates/seeker/column.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.204383 django-seeker-7.3.1/seeker/templates/seeker/facets/
--rw-rw----   0 ruttenb   (1328) ims        (100)      476 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/facets/range.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      477 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/facets/terms.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      184 2019-03-14 18:04:52.000000 django-seeker-7.3.1/seeker/templates/seeker/facets/text.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      508 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/facets/year_histogram.html
--rw-r--r--   0 ruttenb   (1328) ims        (100)      832 2022-12-15 21:11:12.000000 django-seeker-7.3.1/seeker/templates/seeker/footer.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     2059 2019-08-29 20:00:08.000000 django-seeker-7.3.1/seeker/templates/seeker/form.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1185 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/seeker/header.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      768 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/pager.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1867 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/results.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1556 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/save.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      228 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/score.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1299 2019-08-29 20:00:08.000000 django-seeker-7.3.1/seeker/templates/seeker/seeker.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.213406 django-seeker-7.3.1/seeker/templatetags/
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templatetags/__init__.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     4044 2022-12-15 21:11:12.000000 django-seeker-7.3.1/seeker/templatetags/seeker.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7197 2023-04-21 13:46:11.000000 django-seeker-7.3.1/seeker/utils.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)    86043 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/views.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      418 2023-04-21 13:48:16.227386 django-seeker-7.3.1/setup.cfg
--rw-r--r--   0 ruttenb   (1328) ims        (100)     1048 2023-02-08 16:06:40.000000 django-seeker-7.3.1/setup.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.228937 django-seeker-7.4.0/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1316 2018-10-01 19:52:22.000000 django-seeker-7.4.0/LICENSE
+-rw-rw----   0 ruttenb   (1328) ims        (100)       38 2018-10-01 19:52:22.000000 django-seeker-7.4.0/MANIFEST.in
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      589 2023-07-20 19:55:47.229935 django-seeker-7.4.0/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)      249 2018-10-01 19:52:22.000000 django-seeker-7.4.0/README.md
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.010948 django-seeker-7.4.0/django_seeker.egg-info/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      589 2023-07-20 19:55:42.000000 django-seeker-7.4.0/django_seeker.egg-info/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2086 2023-07-20 19:55:42.000000 django-seeker-7.4.0/django_seeker.egg-info/SOURCES.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)        1 2023-07-20 19:55:42.000000 django-seeker-7.4.0/django_seeker.egg-info/dependency_links.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)       70 2023-07-20 19:55:42.000000 django-seeker-7.4.0/django_seeker.egg-info/requires.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)        7 2023-07-20 19:55:42.000000 django-seeker-7.4.0/django_seeker.egg-info/top_level.txt
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.070931 django-seeker-7.4.0/seeker/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      599 2023-07-20 19:54:33.000000 django-seeker-7.4.0/seeker/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      564 2019-04-26 17:33:41.000000 django-seeker-7.4.0/seeker/admin.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2945 2019-06-18 15:37:07.000000 django-seeker-7.4.0/seeker/apps.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     1024 2023-02-08 16:06:40.000000 django-seeker-7.4.0/seeker/dsl.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    25148 2023-02-08 16:06:40.000000 django-seeker-7.4.0/seeker/facets.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1630 2019-02-08 19:43:15.000000 django-seeker-7.4.0/seeker/forms.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     2585 2023-07-20 19:54:33.000000 django-seeker-7.4.0/seeker/indexer.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.074946 django-seeker-7.4.0/seeker/management/
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/management/__init__.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.095930 django-seeker-7.4.0/seeker/management/commands/
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/management/commands/__init__.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     2295 2023-02-08 16:06:40.000000 django-seeker-7.4.0/seeker/management/commands/dropindex.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     1188 2023-02-08 16:06:40.000000 django-seeker-7.4.0/seeker/management/commands/dumpindex.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     1275 2023-02-08 16:06:40.000000 django-seeker-7.4.0/seeker/management/commands/loadindex.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     4026 2023-02-08 16:06:40.000000 django-seeker-7.4.0/seeker/management/commands/reindex.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    11740 2023-02-08 16:06:40.000000 django-seeker-7.4.0/seeker/mapping.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1016 2019-06-18 15:37:07.000000 django-seeker-7.4.0/seeker/middleware.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.125930 django-seeker-7.4.0/seeker/migrations/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1193 2019-06-18 15:37:07.000000 django-seeker-7.4.0/seeker/migrations/0001_initial.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      499 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/migrations/0002_auto_20150507_0134.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      838 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/migrations/0003_auto_20180214_1501.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      971 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/migrations/0004_auto_20180322_1412.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      457 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/migrations/0005_auto_20180330_1708.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      714 2019-06-25 20:26:14.000000 django-seeker-7.4.0/seeker/migrations/0006_auto_20190625_1139.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/migrations/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1602 2020-10-14 20:36:41.000000 django-seeker-7.4.0/seeker/models.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      877 2021-09-01 20:33:51.000000 django-seeker-7.4.0/seeker/registry.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      823 2022-12-15 21:11:12.000000 django-seeker-7.4.0/seeker/signals.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:46.949929 django-seeker-7.4.0/seeker/templates/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.147938 django-seeker-7.4.0/seeker/templates/advanced_seeker/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.169932 django-seeker-7.4.0/seeker/templates/advanced_seeker/facets/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      628 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/facets/date_range.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      444 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/facets/range.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      218 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/facets/terms.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      306 2019-03-14 18:04:52.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/facets/text.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      218 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/facets/year_histogram.html
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     2561 2022-12-15 21:11:12.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/footer.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      243 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/header.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      854 2019-10-17 18:45:08.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/pager.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2428 2019-09-23 17:53:11.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/results.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      465 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/save_form.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1341 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/templates/advanced_seeker/seeker.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.202933 django-seeker-7.4.0/seeker/templates/seeker/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      451 2023-07-20 19:54:33.000000 django-seeker-7.4.0/seeker/templates/seeker/column.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.217939 django-seeker-7.4.0/seeker/templates/seeker/facets/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      476 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/templates/seeker/facets/range.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      477 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/templates/seeker/facets/terms.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      184 2019-03-14 18:04:52.000000 django-seeker-7.4.0/seeker/templates/seeker/facets/text.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      508 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/templates/seeker/facets/year_histogram.html
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      832 2022-12-15 21:11:12.000000 django-seeker-7.4.0/seeker/templates/seeker/footer.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2059 2019-08-29 20:00:08.000000 django-seeker-7.4.0/seeker/templates/seeker/form.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1185 2018-10-01 19:52:32.000000 django-seeker-7.4.0/seeker/templates/seeker/header.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      768 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/templates/seeker/pager.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1867 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/templates/seeker/results.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1556 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/templates/seeker/save.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      228 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/templates/seeker/score.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1299 2019-08-29 20:00:08.000000 django-seeker-7.4.0/seeker/templates/seeker/seeker.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-07-20 19:55:47.225941 django-seeker-7.4.0/seeker/templatetags/
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.4.0/seeker/templatetags/__init__.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     4044 2022-12-15 21:11:12.000000 django-seeker-7.4.0/seeker/templatetags/seeker.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7197 2023-04-21 13:46:11.000000 django-seeker-7.4.0/seeker/utils.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    88012 2023-07-20 19:54:33.000000 django-seeker-7.4.0/seeker/views.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      418 2023-07-20 19:55:47.231937 django-seeker-7.4.0/setup.cfg
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     1048 2023-02-08 16:06:40.000000 django-seeker-7.4.0/setup.py
```

### Comparing `django-seeker-7.3.1/LICENSE` & `django-seeker-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/PKG-INFO` & `django-seeker-7.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeker
-Version: 7.3.1
+Version: 7.4.0
 Summary: A python package for mapping and querying Django models in Elasticsearch/OpenSearch.
 Home-page: https://github.com/imsweb/django-seeker
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-seeker-7.3.1/django_seeker.egg-info/PKG-INFO` & `django-seeker-7.4.0/django_seeker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeker
-Version: 7.3.1
+Version: 7.4.0
 Summary: A python package for mapping and querying Django models in Elasticsearch/OpenSearch.
 Home-page: https://github.com/imsweb/django-seeker
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-seeker-7.3.1/django_seeker.egg-info/SOURCES.txt` & `django-seeker-7.4.0/django_seeker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/__init__.py` & `django-seeker-7.4.0/seeker/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '7.3.1'
+__version__ = '7.4.0'
 
 from .facets import DateRangeFacet, DateTermsFacet, Facet, GlobalTermsFacet, RangeFilter, TermsFacet, YearHistogram, TextFacet
 from .mapping import (
     build_mapping, deep_field_factory, DEFAULT_ANALYZER, document_field, document_from_model, Indexable, index_factory, ModelIndex,
     RawMultiString, RawString)
 from .registry import app_documents, documents, model_documents, register
 from .utils import delete, index, search
```

### Comparing `django-seeker-7.3.1/seeker/admin.py` & `django-seeker-7.4.0/seeker/admin.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/apps.py` & `django-seeker-7.4.0/seeker/apps.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/dsl.py` & `django-seeker-7.4.0/seeker/dsl.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/facets.py` & `django-seeker-7.4.0/seeker/facets.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/forms.py` & `django-seeker-7.4.0/seeker/forms.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/indexer.py` & `django-seeker-7.4.0/seeker/indexer.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,40 @@
     """
 
     def connect_signal_handlers(self):
         """
         Connects save and delete signal handler for mapped models. Also checks each ModelIndex for any additional signal handling that may be needed. 
         """
 
+        through = set()
+
         for model_class, document_classes in model_documents.items():
             signals.post_save.connect(self.handle_save, sender=model_class)
+            through.update([m2m.remote_field.through for m2m in model_class._meta.many_to_many])
             signals.post_delete.connect(self.handle_delete, sender=model_class)
 
             for document_class in document_classes:
                 document_class.connect_additional_signal_handlers(self)
+        
+        for model_class in through:
+            signals.m2m_changed.connect(self.handle_m2m_changed, sender=model_class)
 
     def disconnect_signal_handlers(self):
+        through = set()
+
         for model_class, document_classes in model_documents.items():
             signals.post_save.disconnect(self.handle_save, sender=model_class)
+            through.update([m2m.remote_field.through for m2m in model_class._meta.many_to_many])
             signals.post_delete.disconnect(self.handle_delete, sender=model_class)
 
             for document_class in document_classes:
                 document_class.disconnect_additional_signal_handlers(self)
+        
+        for model_class in through:
+            signals.m2m_changed.disconnect(self.handle_m2m_changed, sender=model_class)
 
     def handle_save(self, sender, instance, **kwargs):
         try:
             index(instance)
         except Exception as e:
             logger.exception('Error indexing %s instance: %s. Exception raised: %s', sender, instance, e)
```

### Comparing `django-seeker-7.3.1/seeker/management/commands/dropindex.py` & `django-seeker-7.4.0/seeker/management/commands/dropindex.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/management/commands/dumpindex.py` & `django-seeker-7.4.0/seeker/management/commands/dumpindex.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/management/commands/loadindex.py` & `django-seeker-7.4.0/seeker/management/commands/loadindex.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/management/commands/reindex.py` & `django-seeker-7.4.0/seeker/management/commands/reindex.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/mapping.py` & `django-seeker-7.4.0/seeker/mapping.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/middleware.py` & `django-seeker-7.4.0/seeker/middleware.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/migrations/0001_initial.py` & `django-seeker-7.4.0/seeker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/migrations/0003_auto_20180214_1501.py` & `django-seeker-7.4.0/seeker/migrations/0003_auto_20180214_1501.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/migrations/0004_auto_20180322_1412.py` & `django-seeker-7.4.0/seeker/migrations/0004_auto_20180322_1412.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/migrations/0006_auto_20190625_1139.py` & `django-seeker-7.4.0/seeker/migrations/0006_auto_20190625_1139.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/models.py` & `django-seeker-7.4.0/seeker/models.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/registry.py` & `django-seeker-7.4.0/seeker/registry.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/signals.py` & `django-seeker-7.4.0/seeker/signals.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/date_range.html` & `django-seeker-7.4.0/seeker/templates/advanced_seeker/facets/date_range.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/advanced_seeker/footer.html` & `django-seeker-7.4.0/seeker/templates/advanced_seeker/footer.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/advanced_seeker/pager.html` & `django-seeker-7.4.0/seeker/templates/advanced_seeker/pager.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/advanced_seeker/results.html` & `django-seeker-7.4.0/seeker/templates/advanced_seeker/results.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/advanced_seeker/seeker.html` & `django-seeker-7.4.0/seeker/templates/advanced_seeker/seeker.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/seeker/footer.html` & `django-seeker-7.4.0/seeker/templates/seeker/footer.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/seeker/form.html` & `django-seeker-7.4.0/seeker/templates/seeker/form.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/seeker/header.html` & `django-seeker-7.4.0/seeker/templates/seeker/header.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/seeker/pager.html` & `django-seeker-7.4.0/seeker/templates/seeker/pager.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/seeker/results.html` & `django-seeker-7.4.0/seeker/templates/seeker/results.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/seeker/save.html` & `django-seeker-7.4.0/seeker/templates/seeker/save.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templates/seeker/seeker.html` & `django-seeker-7.4.0/seeker/templates/seeker/seeker.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/templatetags/seeker.py` & `django-seeker-7.4.0/seeker/templatetags/seeker.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/utils.py` & `django-seeker-7.4.0/seeker/utils.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.1/seeker/views.py` & `django-seeker-7.4.0/seeker/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 from django.conf import settings
 from django.contrib import messages
 from django.forms.forms import Form
 from django.http import Http404, JsonResponse, QueryDict, StreamingHttpResponse
 from django.http.response import HttpResponseBadRequest, HttpResponseForbidden
 from django.shortcuts import redirect, render
 from django.template import Context, RequestContext, TemplateDoesNotExist, loader
+from django.template.defaultfilters import truncatewords_html, truncatechars_html
 from django.utils import timezone
 from django.utils.encoding import force_str
 from django.utils.html import escape, format_html
 from django.utils.http import urlencode
+from django.utils.safestring import mark_safe
 from django.views.generic import View
 from django.views.generic.edit import CreateView, FormView
 
 from .facets import TermsFacet, RangeFilter, TextFacet
 from .mapping import DEFAULT_ANALYZER
 from .signals import advanced_search_performed, search_complete
 from .templatetags.seeker import seeker_format
@@ -33,14 +35,28 @@
 seekerview_field_templates = {}
 
 
 class Column(object):
     """
     """
 
+    """
+    If enabled, large fields will be truncated in a "..." format
+    """
+    seeker_enable_truncation = getattr(settings, 'SEEKER_ENABLE_TRUNCATION', False)
+
+    """
+    The value of SEEKER_TRUNCATION_TYPE can be either "words" or 'chars".
+    """
+    seeker_truncation_type = getattr(settings, 'SEEKER_TRUNCATION_TYPE', 'words')
+
+    """
+    The desired number of words/chars to be truncated.
+    """
+    seeker_truncation_amount = getattr(settings, 'SEEKER_TRUNCATION_AMOUNT', 5)
     view = None
     visible = False
 
     def __init__(self, field, label=None, sort=None, value_format=None, template=None, header=None, export=True, highlight=None, field_definition=None):
         self.field = field
         self.label = label if label is not None else field.replace('_', ' ').replace('.raw', '').capitalize()
         self.sort = sort
@@ -151,18 +167,40 @@
             highlight = modified_values
 
         if self.value_format:
             value = self.value_format(value)
             if highlight:
                 highlight = self.value_format(highlight)
 
+        truncated_value = None
+        if self.seeker_enable_truncation and isinstance(value, str):
+            truncate_func = None
+            if self.seeker_truncation_type == 'words' and len(value.split()) > self.seeker_truncation_amount:
+                truncate_func = truncatewords_html
+            elif self.seeker_truncation_type == 'chars' and len(value) > self.seeker_truncation_amount:
+                truncate_func = truncatechars_html
+            if truncate_func:
+                if highlight:
+                    highlight_str = highlight[0] if isinstance(highlight, AttrList) else highlight
+                    highlight_str = highlight_str.lstrip("['").rstrip("']")
+                    start = highlight_str.find('<em>')
+                    end = highlight_str.find('</em>') + 5
+                    prefix = '…' if start > 0 else ''
+                    highlighted_value = highlight_str[start:end]
+                    trunc_value = truncate_func(highlight_str[end:], self.seeker_truncation_amount)
+                    truncated_value = mark_safe(f"{prefix}{highlighted_value}{trunc_value}".replace(' …', '…'))
+                else:
+                    truncated_value = truncate_func(value, self.seeker_truncation_amount).replace(' …', '…')
+
         params = {
             'result': result,
             'field': self.field,
+            'label': self.label,
             'value': value,
+            'truncated_value': truncated_value,
             'highlight': highlight,
             'model_lower': self.model_lower,
             'doc_class_name': result.__class__.__name__.lower(),
             'view': self.view,
             'user': self.view.request.user,
             'query': self.view.get_keywords(self.view.request.GET),
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-seeker-7.3.1/setup.py` & `django-seeker-7.4.0/setup.py`

 * *Files identical despite different names*

