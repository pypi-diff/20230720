# Comparing `tmp/django-data-browser-4.2.4.tar.gz` & `tmp/django-data-browser-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-data-browser-4.2.4.tar", last modified: Sun Jul  2 18:09:50 2023, max compression
+gzip compressed data, was "django-data-browser-4.2.5.tar", last modified: Thu Jul 20 11:18:29 2023, max compression
```

## Comparing `django-data-browser-4.2.4.tar` & `django-data-browser-4.2.5.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.445522 django-data-browser-4.2.4/
--rw-rw-rw-   0        0        0     1885 2023-03-30 21:24:18.000000 django-data-browser-4.2.4/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0    14913 2021-12-12 20:01:39.000000 django-data-browser-4.2.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1522 2020-03-29 21:09:45.000000 django-data-browser-4.2.4/LICENSE
--rw-rw-rw-   0        0        0      605 2022-01-04 07:58:07.000000 django-data-browser-4.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0    65961 2023-07-02 18:09:50.443529 django-data-browser-4.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    64745 2023-07-02 18:09:04.000000 django-data-browser-4.2.4/README.rst
--rw-rw-rw-   0        0        0      508 2021-09-26 12:42:44.000000 django-data-browser-4.2.4/build.sh
--rw-rw-rw-   0        0        0      243 2020-10-18 11:05:29.000000 django-data-browser-4.2.4/build_fe.sh
--rw-rw-rw-   0        0        0      209 2020-11-28 10:32:50.000000 django-data-browser-4.2.4/build_whl.sh
--rw-rw-rw-   0        0        0      105 2020-10-18 11:05:29.000000 django-data-browser-4.2.4/clean.sh
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.281941 django-data-browser-4.2.4/data_browser/
--rw-rw-rw-   0        0        0       18 2023-07-02 18:09:11.000000 django-data-browser-4.2.4/data_browser/__init__.py
--rw-rw-rw-   0        0        0     2009 2023-06-08 21:24:56.000000 django-data-browser-4.2.4/data_browser/admin.py
--rw-rw-rw-   0        0        0     4818 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/api.py
--rw-rw-rw-   0        0        0      206 2022-02-07 19:45:31.000000 django-data-browser-4.2.4/data_browser/apps.py
--rw-rw-rw-   0        0        0     5599 2023-06-15 07:06:33.000000 django-data-browser-4.2.4/data_browser/common.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.283935 django-data-browser-4.2.4/data_browser/fe_build/
--rw-rw-rw-   0        0        0      374 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/asset-manifest.json
--rw-rw-rw-   0        0        0     2400 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.215101 django-data-browser-4.2.4/data_browser/fe_build/static/
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.289437 django-data-browser-4.2.4/data_browser/fe_build/static/css/
--rw-rw-rw-   0        0        0     7170 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/css/main.a2cd42f2.css
--rw-rw-rw-   0        0        0    10320 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/css/main.a2cd42f2.css.map
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.294417 django-data-browser-4.2.4/data_browser/fe_build/static/js/
--rw-rw-rw-   0        0        0   328249 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js
--rw-rw-rw-   0        0        0     1447 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1220644 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js.map
--rw-rw-rw-   0        0        0     1741 2021-03-13 16:54:43.000000 django-data-browser-4.2.4/data_browser/format_csv.py
--rw-rw-rw-   0        0        0     5819 2023-05-28 08:26:29.000000 django-data-browser-4.2.4/data_browser/helpers.py
--rw-rw-rw-   0        0        0     2566 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/migration_helpers.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.314871 django-data-browser-4.2.4/data_browser/migrations/
--rw-rw-rw-   0        0        0     1629 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      536 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0002_auto_20200331_1842.py
--rw-rw-rw-   0        0        0      263 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0003_remove_view_app.py
--rw-rw-rw-   0        0        0      325 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0004_auto_20200501_0903.py
--rw-rw-rw-   0        0        0      463 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0005_auto_20200516_1726.py
--rw-rw-rw-   0        0        0      592 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0006_auto_20200531_1450.py
--rw-rw-rw-   0        0        0      440 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0007_view_public_slug.py
--rw-rw-rw-   0        0        0      344 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0008_view_limit.py
--rw-rw-rw-   0        0        0      469 2020-12-01 19:24:08.000000 django-data-browser-4.2.4/data_browser/migrations/0009_migrate_saved_views.py
--rw-rw-rw-   0        0        0      350 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/data_browser/migrations/0010_shared.py
--rw-rw-rw-   0        0        0      502 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/data_browser/migrations/0011_folder.py
--rw-rw-rw-   0        0        0      529 2023-05-01 18:51:44.000000 django-data-browser-4.2.4/data_browser/migrations/0012_can_share.py
--rw-rw-rw-   0        0        0        0 2020-03-31 16:35:44.000000 django-data-browser-4.2.4/data_browser/migrations/__init__.py
--rw-rw-rw-   0        0        0     2646 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/models.py
--rw-rw-rw-   0        0        0    15460 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/orm_admin.py
--rw-rw-rw-   0        0        0     3482 2023-07-01 15:54:32.000000 django-data-browser-4.2.4/data_browser/orm_aggregates.py
--rw-rw-rw-   0        0        0     2471 2021-12-31 10:44:42.000000 django-data-browser-4.2.4/data_browser/orm_debug.py
--rw-rw-rw-   0        0        0     8339 2023-07-01 15:18:54.000000 django-data-browser-4.2.4/data_browser/orm_fields.py
--rw-rw-rw-   0        0        0     4885 2023-07-01 15:59:41.000000 django-data-browser-4.2.4/data_browser/orm_functions.py
--rw-rw-rw-   0        0        0     1729 2022-01-03 10:46:07.000000 django-data-browser-4.2.4/data_browser/orm_lookups.py
--rw-rw-rw-   0        0        0     9234 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/orm_results.py
--rw-rw-rw-   0        0        0     3525 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/data_browser/orm_types.py
--rw-rw-rw-   0        0        0     9969 2023-06-04 16:30:52.000000 django-data-browser-4.2.4/data_browser/query.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.215101 django-data-browser-4.2.4/data_browser/templates/
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.314871 django-data-browser-4.2.4/data_browser/templates/data_browser/
--rw-rw-rw-   0        0        0     2400 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/templates/data_browser/index.html
--rw-rw-rw-   0        0        0    17004 2023-07-01 14:24:41.000000 django-data-browser-4.2.4/data_browser/types.py
--rw-rw-rw-   0        0        0     1684 2021-12-31 10:46:26.000000 django-data-browser-4.2.4/data_browser/urls.py
--rw-rw-rw-   0        0        0      349 2023-05-01 18:51:44.000000 django-data-browser-4.2.4/data_browser/util.py
--rw-rw-rw-   0        0        0    12967 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/views.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.330830 django-data-browser-4.2.4/data_browser/web_root/
--rw-rw-rw-   0        0        0     5221 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    17683 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     4613 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/apple-touch-icon.png
--rw-rw-rw-   0        0        0      333 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/favicon-16x16.png
--rw-rw-rw-   0        0        0      648 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/favicon-32x32.png
--rw-rw-rw-   0        0        0    15406 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/favicon.ico
--rw-rw-rw-   0        0        0      424 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/data_browser/web_root/site.webmanifest
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.344792 django-data-browser-4.2.4/django_data_browser.egg-info/
--rw-rw-rw-   0        0        0    65961 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3438 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.349779 django-data-browser-4.2.4/frontend/
--rw-rw-rw-   0        0        0     2891 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/README.md
--rw-rw-rw-   0        0        0  1009738 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/package-lock.json
--rw-rw-rw-   0        0        0     1000 2022-04-10 12:41:54.000000 django-data-browser-4.2.4/frontend/package.json
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.349779 django-data-browser-4.2.4/frontend/public/
--rw-rw-rw-   0        0        0     3304 2023-03-06 21:38:15.000000 django-data-browser-4.2.4/frontend/public/index.html
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.395656 django-data-browser-4.2.4/frontend/src/
--rw-rw-rw-   0        0        0     1298 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/src/App.js
--rw-rw-rw-   0        0        0     7342 2023-05-21 17:10:18.000000 django-data-browser-4.2.4/frontend/src/App.scss
--rw-rw-rw-   0        0        0      280 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/src/App.test.js
--rw-rw-rw-   0        0        0       85 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/src/Config.js
--rw-rw-rw-   0        0        0     2678 2021-12-29 21:35:30.000000 django-data-browser-4.2.4/frontend/src/ContextMenu.js
--rw-rw-rw-   0        0        0      551 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/src/CurrentSavedView.js
--rw-rw-rw-   0        0        0     4278 2023-05-01 19:00:44.000000 django-data-browser-4.2.4/frontend/src/HomePage.js
--rw-rw-rw-   0        0        0     9603 2023-05-21 17:07:43.000000 django-data-browser-4.2.4/frontend/src/Query.js
--rw-rw-rw-   0        0        0      144 2020-06-27 10:10:01.000000 django-data-browser-4.2.4/frontend/src/Query.test.js
--rw-rw-rw-   0        0        0    14930 2023-05-21 17:09:38.000000 django-data-browser-4.2.4/frontend/src/QueryPage.js
--rw-rw-rw-   0        0        0     9360 2023-05-21 16:43:53.000000 django-data-browser-4.2.4/frontend/src/Results.js
--rw-rw-rw-   0        0        0     6645 2023-05-01 19:01:07.000000 django-data-browser-4.2.4/frontend/src/SavedViewPage.js
--rw-rw-rw-   0        0        0     1649 2021-12-30 00:35:29.000000 django-data-browser-4.2.4/frontend/src/Tooltip.js
--rw-rw-rw-   0        0        0    12431 2023-05-21 14:02:17.000000 django-data-browser-4.2.4/frontend/src/Util.js
--rw-rw-rw-   0        0        0      591 2021-12-12 20:01:39.000000 django-data-browser-4.2.4/frontend/src/WindowDimensions.js
--rw-rw-rw-   0        0        0      733 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/src/index.js
--rw-rw-rw-   0        0        0      366 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/src/index.scss
--rw-rw-rw-   0        0        0     2671 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/src/logo.svg
--rw-rw-rw-   0        0        0      255 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/src/setupTests.js
--rw-rw-rw-   0        0        0     2864 2023-07-01 15:58:55.000000 django-data-browser-4.2.4/pyproject.toml
--rw-rw-rw-   0        0        0      260 2023-03-06 20:00:37.000000 django-data-browser-4.2.4/requirements.txt
--rw-rw-rw-   0        0        0   112598 2021-03-13 16:54:43.000000 django-data-browser-4.2.4/screenshot.png
--rw-rw-rw-   0        0        0       42 2023-07-02 18:09:50.445522 django-data-browser-4.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1092 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/setup.py
--rw-rw-rw-   0        0        0    35837 2020-06-27 10:10:01.000000 django-data-browser-4.2.4/structure.svg
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.422584 django-data-browser-4.2.4/tests/
--rw-rw-rw-   0        0        0        0 2019-07-20 09:57:44.000000 django-data-browser-4.2.4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.427570 django-data-browser-4.2.4/tests/array/
--rw-rw-rw-   0        0        0        0 2020-10-24 10:26:31.000000 django-data-browser-4.2.4/tests/array/__init__.py
--rw-rw-rw-   0        0        0      617 2021-12-31 10:07:16.000000 django-data-browser-4.2.4/tests/array/models.py
--rw-rw-rw-   0        0        0     2600 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.430562 django-data-browser-4.2.4/tests/core/
--rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.4/tests/core/__init__.py
--rw-rw-rw-   0        0        0     4422 2021-12-31 10:49:19.000000 django-data-browser-4.2.4/tests/core/admin.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.432557 django-data-browser-4.2.4/tests/core/migrations/
--rw-rw-rw-   0        0        0    10069 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/tests/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2021-12-29 23:58:51.000000 django-data-browser-4.2.4/tests/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     4303 2021-12-31 10:48:59.000000 django-data-browser-4.2.4/tests/core/models.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.433554 django-data-browser-4.2.4/tests/json/
--rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.4/tests/json/__init__.py
--rw-rw-rw-   0        0        0       98 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/tests/json/models.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.438541 django-data-browser-4.2.4/tests/snapshots/
--rw-rw-rw-   0        0        0        0 2020-06-27 10:10:01.000000 django-data-browser-4.2.4/tests/snapshots/__init__.py
--rw-rw-rw-   0        0        0   439282 2023-07-01 13:49:30.000000 django-data-browser-4.2.4/tests/snapshots/snap_test_views.py
--rw-rw-rw-   0        0        0     6618 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_admin.py
--rw-rw-rw-   0        0        0    20582 2023-06-04 21:17:05.000000 django-data-browser-4.2.4/tests/test_api.py
--rw-rw-rw-   0        0        0     7227 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_array_field.py
--rw-rw-rw-   0        0        0      919 2020-09-09 18:29:41.000000 django-data-browser-4.2.4/tests/test_common.py
--rw-rw-rw-   0        0        0     3744 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_helpers.py
--rw-rw-rw-   0        0        0     6156 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_json_field.py
--rw-rw-rw-   0        0        0     4472 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_migrations.py
--rw-rw-rw-   0        0        0     1392 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_models.py
--rw-rw-rw-   0        0        0    35257 2023-07-01 07:55:19.000000 django-data-browser-4.2.4/tests/test_orm.py
--rw-rw-rw-   0        0        0      878 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/tests/test_orm_debug.py
--rw-rw-rw-   0        0        0    25645 2023-05-21 16:31:25.000000 django-data-browser-4.2.4/tests/test_query.py
--rw-rw-rw-   0        0        0      165 2020-10-22 20:32:07.000000 django-data-browser-4.2.4/tests/test_tests.py
--rw-rw-rw-   0        0        0    18706 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_views.py
--rw-rw-rw-   0        0        0      184 2020-10-22 18:16:38.000000 django-data-browser-4.2.4/tests/urls.py
--rw-rw-rw-   0        0        0      366 2023-03-30 21:24:18.000000 django-data-browser-4.2.4/tests/util.py
--rw-rw-rw-   0        0        0      574 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.978565 django-data-browser-4.2.5/
+-rw-rw-rw-   0        0        0     1885 2023-03-30 21:24:18.000000 django-data-browser-4.2.5/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0    14913 2021-12-12 20:01:39.000000 django-data-browser-4.2.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1522 2020-03-29 21:09:45.000000 django-data-browser-4.2.5/LICENSE
+-rw-rw-rw-   0        0        0      605 2022-01-04 07:58:07.000000 django-data-browser-4.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    66372 2023-07-20 11:18:29.977567 django-data-browser-4.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    65153 2023-07-20 11:17:39.000000 django-data-browser-4.2.5/README.rst
+-rw-rw-rw-   0        0        0      508 2021-09-26 12:42:44.000000 django-data-browser-4.2.5/build.sh
+-rw-rw-rw-   0        0        0      243 2020-10-18 11:05:29.000000 django-data-browser-4.2.5/build_fe.sh
+-rw-rw-rw-   0        0        0      209 2020-11-28 10:32:50.000000 django-data-browser-4.2.5/build_whl.sh
+-rw-rw-rw-   0        0        0      105 2020-10-18 11:05:29.000000 django-data-browser-4.2.5/clean.sh
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.869855 django-data-browser-4.2.5/data_browser/
+-rw-rw-rw-   0        0        0       18 2023-07-20 11:17:45.000000 django-data-browser-4.2.5/data_browser/__init__.py
+-rw-rw-rw-   0        0        0     2009 2023-06-08 21:24:56.000000 django-data-browser-4.2.5/data_browser/admin.py
+-rw-rw-rw-   0        0        0     4818 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/data_browser/api.py
+-rw-rw-rw-   0        0        0      206 2022-02-07 19:45:31.000000 django-data-browser-4.2.5/data_browser/apps.py
+-rw-rw-rw-   0        0        0     5599 2023-06-15 07:06:33.000000 django-data-browser-4.2.5/data_browser/common.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.872847 django-data-browser-4.2.5/data_browser/fe_build/
+-rw-rw-rw-   0        0        0      374 2023-07-20 11:18:19.000000 django-data-browser-4.2.5/data_browser/fe_build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2400 2023-07-20 11:18:19.000000 django-data-browser-4.2.5/data_browser/fe_build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.820986 django-data-browser-4.2.5/data_browser/fe_build/static/
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.875839 django-data-browser-4.2.5/data_browser/fe_build/static/css/
+-rw-rw-rw-   0        0        0     7170 2023-07-20 11:18:19.000000 django-data-browser-4.2.5/data_browser/fe_build/static/css/main.a2cd42f2.css
+-rw-rw-rw-   0        0        0    10320 2023-07-20 11:18:19.000000 django-data-browser-4.2.5/data_browser/fe_build/static/css/main.a2cd42f2.css.map
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.878832 django-data-browser-4.2.5/data_browser/fe_build/static/js/
+-rw-rw-rw-   0        0        0   328249 2023-07-20 11:18:19.000000 django-data-browser-4.2.5/data_browser/fe_build/static/js/main.c57e8af0.js
+-rw-rw-rw-   0        0        0     1447 2023-07-20 11:18:19.000000 django-data-browser-4.2.5/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1220644 2023-07-20 11:18:19.000000 django-data-browser-4.2.5/data_browser/fe_build/static/js/main.c57e8af0.js.map
+-rw-rw-rw-   0        0        0     1741 2021-03-13 16:54:43.000000 django-data-browser-4.2.5/data_browser/format_csv.py
+-rw-rw-rw-   0        0        0     5819 2023-05-28 08:26:29.000000 django-data-browser-4.2.5/data_browser/helpers.py
+-rw-rw-rw-   0        0        0     2566 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/data_browser/migration_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.893792 django-data-browser-4.2.5/data_browser/migrations/
+-rw-rw-rw-   0        0        0     1629 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/data_browser/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      536 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/data_browser/migrations/0002_auto_20200331_1842.py
+-rw-rw-rw-   0        0        0      263 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/data_browser/migrations/0003_remove_view_app.py
+-rw-rw-rw-   0        0        0      325 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/data_browser/migrations/0004_auto_20200501_0903.py
+-rw-rw-rw-   0        0        0      463 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/data_browser/migrations/0005_auto_20200516_1726.py
+-rw-rw-rw-   0        0        0      592 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/data_browser/migrations/0006_auto_20200531_1450.py
+-rw-rw-rw-   0        0        0      440 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/data_browser/migrations/0007_view_public_slug.py
+-rw-rw-rw-   0        0        0      344 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/data_browser/migrations/0008_view_limit.py
+-rw-rw-rw-   0        0        0      469 2020-12-01 19:24:08.000000 django-data-browser-4.2.5/data_browser/migrations/0009_migrate_saved_views.py
+-rw-rw-rw-   0        0        0      350 2023-04-25 17:09:12.000000 django-data-browser-4.2.5/data_browser/migrations/0010_shared.py
+-rw-rw-rw-   0        0        0      502 2023-04-25 17:09:12.000000 django-data-browser-4.2.5/data_browser/migrations/0011_folder.py
+-rw-rw-rw-   0        0        0      529 2023-05-01 18:51:44.000000 django-data-browser-4.2.5/data_browser/migrations/0012_can_share.py
+-rw-rw-rw-   0        0        0        0 2020-03-31 16:35:44.000000 django-data-browser-4.2.5/data_browser/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2646 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/data_browser/models.py
+-rw-rw-rw-   0        0        0    15460 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/data_browser/orm_admin.py
+-rw-rw-rw-   0        0        0     3482 2023-07-01 15:54:32.000000 django-data-browser-4.2.5/data_browser/orm_aggregates.py
+-rw-rw-rw-   0        0        0     2471 2021-12-31 10:44:42.000000 django-data-browser-4.2.5/data_browser/orm_debug.py
+-rw-rw-rw-   0        0        0     8339 2023-07-01 15:18:54.000000 django-data-browser-4.2.5/data_browser/orm_fields.py
+-rw-rw-rw-   0        0        0     4885 2023-07-01 15:59:41.000000 django-data-browser-4.2.5/data_browser/orm_functions.py
+-rw-rw-rw-   0        0        0     1729 2022-01-03 10:46:07.000000 django-data-browser-4.2.5/data_browser/orm_lookups.py
+-rw-rw-rw-   0        0        0     9234 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/data_browser/orm_results.py
+-rw-rw-rw-   0        0        0     3525 2023-03-30 22:40:08.000000 django-data-browser-4.2.5/data_browser/orm_types.py
+-rw-rw-rw-   0        0        0     9969 2023-06-04 16:30:52.000000 django-data-browser-4.2.5/data_browser/query.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.821983 django-data-browser-4.2.5/data_browser/templates/
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.896784 django-data-browser-4.2.5/data_browser/templates/data_browser/
+-rw-rw-rw-   0        0        0     2400 2023-07-20 11:18:19.000000 django-data-browser-4.2.5/data_browser/templates/data_browser/index.html
+-rw-rw-rw-   0        0        0    17024 2023-07-19 14:24:57.000000 django-data-browser-4.2.5/data_browser/types.py
+-rw-rw-rw-   0        0        0     1684 2021-12-31 10:46:26.000000 django-data-browser-4.2.5/data_browser/urls.py
+-rw-rw-rw-   0        0        0      349 2023-05-01 18:51:44.000000 django-data-browser-4.2.5/data_browser/util.py
+-rw-rw-rw-   0        0        0    13449 2023-07-09 10:24:44.000000 django-data-browser-4.2.5/data_browser/views.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.903765 django-data-browser-4.2.5/data_browser/web_root/
+-rw-rw-rw-   0        0        0     5221 2020-07-01 20:11:06.000000 django-data-browser-4.2.5/data_browser/web_root/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    17683 2020-07-01 20:11:06.000000 django-data-browser-4.2.5/data_browser/web_root/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     4613 2020-07-01 20:11:06.000000 django-data-browser-4.2.5/data_browser/web_root/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      333 2020-07-01 20:11:06.000000 django-data-browser-4.2.5/data_browser/web_root/favicon-16x16.png
+-rw-rw-rw-   0        0        0      648 2020-07-01 20:11:06.000000 django-data-browser-4.2.5/data_browser/web_root/favicon-32x32.png
+-rw-rw-rw-   0        0        0    15406 2020-07-01 20:11:06.000000 django-data-browser-4.2.5/data_browser/web_root/favicon.ico
+-rw-rw-rw-   0        0        0      424 2023-04-25 17:09:12.000000 django-data-browser-4.2.5/data_browser/web_root/site.webmanifest
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.912742 django-data-browser-4.2.5/django_data_browser.egg-info/
+-rw-rw-rw-   0        0        0    66372 2023-07-20 11:18:29.000000 django-data-browser-4.2.5/django_data_browser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3438 2023-07-20 11:18:29.000000 django-data-browser-4.2.5/django_data_browser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 11:18:29.000000 django-data-browser-4.2.5/django_data_browser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-20 11:18:29.000000 django-data-browser-4.2.5/django_data_browser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-20 11:18:29.000000 django-data-browser-4.2.5/django_data_browser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.916730 django-data-browser-4.2.5/frontend/
+-rw-rw-rw-   0        0        0     2891 2020-04-22 19:19:40.000000 django-data-browser-4.2.5/frontend/README.md
+-rw-rw-rw-   0        0        0  1009738 2023-04-25 17:09:12.000000 django-data-browser-4.2.5/frontend/package-lock.json
+-rw-rw-rw-   0        0        0     1000 2022-04-10 12:41:54.000000 django-data-browser-4.2.5/frontend/package.json
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.917728 django-data-browser-4.2.5/frontend/public/
+-rw-rw-rw-   0        0        0     3304 2023-03-06 21:38:15.000000 django-data-browser-4.2.5/frontend/public/index.html
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.940666 django-data-browser-4.2.5/frontend/src/
+-rw-rw-rw-   0        0        0     1298 2023-04-25 17:09:12.000000 django-data-browser-4.2.5/frontend/src/App.js
+-rw-rw-rw-   0        0        0     7342 2023-05-21 17:10:18.000000 django-data-browser-4.2.5/frontend/src/App.scss
+-rw-rw-rw-   0        0        0      280 2020-04-22 19:19:40.000000 django-data-browser-4.2.5/frontend/src/App.test.js
+-rw-rw-rw-   0        0        0       85 2023-04-25 17:09:12.000000 django-data-browser-4.2.5/frontend/src/Config.js
+-rw-rw-rw-   0        0        0     2678 2021-12-29 21:35:30.000000 django-data-browser-4.2.5/frontend/src/ContextMenu.js
+-rw-rw-rw-   0        0        0      551 2023-04-25 17:09:12.000000 django-data-browser-4.2.5/frontend/src/CurrentSavedView.js
+-rw-rw-rw-   0        0        0     4278 2023-05-01 19:00:44.000000 django-data-browser-4.2.5/frontend/src/HomePage.js
+-rw-rw-rw-   0        0        0     9603 2023-05-21 17:07:43.000000 django-data-browser-4.2.5/frontend/src/Query.js
+-rw-rw-rw-   0        0        0      144 2020-06-27 10:10:01.000000 django-data-browser-4.2.5/frontend/src/Query.test.js
+-rw-rw-rw-   0        0        0    14930 2023-05-21 17:09:38.000000 django-data-browser-4.2.5/frontend/src/QueryPage.js
+-rw-rw-rw-   0        0        0     9360 2023-05-21 16:43:53.000000 django-data-browser-4.2.5/frontend/src/Results.js
+-rw-rw-rw-   0        0        0     6645 2023-05-01 19:01:07.000000 django-data-browser-4.2.5/frontend/src/SavedViewPage.js
+-rw-rw-rw-   0        0        0     1649 2021-12-30 00:35:29.000000 django-data-browser-4.2.5/frontend/src/Tooltip.js
+-rw-rw-rw-   0        0        0    12431 2023-05-21 14:02:17.000000 django-data-browser-4.2.5/frontend/src/Util.js
+-rw-rw-rw-   0        0        0      591 2021-12-12 20:01:39.000000 django-data-browser-4.2.5/frontend/src/WindowDimensions.js
+-rw-rw-rw-   0        0        0      733 2023-04-25 17:09:12.000000 django-data-browser-4.2.5/frontend/src/index.js
+-rw-rw-rw-   0        0        0      366 2020-04-22 19:19:40.000000 django-data-browser-4.2.5/frontend/src/index.scss
+-rw-rw-rw-   0        0        0     2671 2020-04-22 19:19:40.000000 django-data-browser-4.2.5/frontend/src/logo.svg
+-rw-rw-rw-   0        0        0      255 2020-04-22 19:19:40.000000 django-data-browser-4.2.5/frontend/src/setupTests.js
+-rw-rw-rw-   0        0        0     2864 2023-07-01 15:58:55.000000 django-data-browser-4.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      260 2023-03-06 20:00:37.000000 django-data-browser-4.2.5/requirements.txt
+-rw-rw-rw-   0        0        0   112598 2021-03-13 16:54:43.000000 django-data-browser-4.2.5/screenshot.png
+-rw-rw-rw-   0        0        0       42 2023-07-20 11:18:29.978565 django-data-browser-4.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2023-03-30 22:40:08.000000 django-data-browser-4.2.5/setup.py
+-rw-rw-rw-   0        0        0    35837 2020-06-27 10:10:01.000000 django-data-browser-4.2.5/structure.svg
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.963605 django-data-browser-4.2.5/tests/
+-rw-rw-rw-   0        0        0        0 2019-07-20 09:57:44.000000 django-data-browser-4.2.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.965599 django-data-browser-4.2.5/tests/array/
+-rw-rw-rw-   0        0        0        0 2020-10-24 10:26:31.000000 django-data-browser-4.2.5/tests/array/__init__.py
+-rw-rw-rw-   0        0        0      617 2021-12-31 10:07:16.000000 django-data-browser-4.2.5/tests/array/models.py
+-rw-rw-rw-   0        0        0     2600 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.970586 django-data-browser-4.2.5/tests/core/
+-rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.5/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     4422 2021-12-31 10:49:19.000000 django-data-browser-4.2.5/tests/core/admin.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.972581 django-data-browser-4.2.5/tests/core/migrations/
+-rw-rw-rw-   0        0        0    10069 2023-03-06 08:08:57.000000 django-data-browser-4.2.5/tests/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2021-12-29 23:58:51.000000 django-data-browser-4.2.5/tests/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4303 2021-12-31 10:48:59.000000 django-data-browser-4.2.5/tests/core/models.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.973578 django-data-browser-4.2.5/tests/json/
+-rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.5/tests/json/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-03-30 22:40:08.000000 django-data-browser-4.2.5/tests/json/models.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:18:29.975573 django-data-browser-4.2.5/tests/snapshots/
+-rw-rw-rw-   0        0        0        0 2020-06-27 10:10:01.000000 django-data-browser-4.2.5/tests/snapshots/__init__.py
+-rw-rw-rw-   0        0        0   439290 2023-07-09 10:46:29.000000 django-data-browser-4.2.5/tests/snapshots/snap_test_views.py
+-rw-rw-rw-   0        0        0     6618 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/tests/test_admin.py
+-rw-rw-rw-   0        0        0    20582 2023-06-04 21:17:05.000000 django-data-browser-4.2.5/tests/test_api.py
+-rw-rw-rw-   0        0        0     7227 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/tests/test_array_field.py
+-rw-rw-rw-   0        0        0      919 2020-09-09 18:29:41.000000 django-data-browser-4.2.5/tests/test_common.py
+-rw-rw-rw-   0        0        0     3744 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     6156 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/tests/test_json_field.py
+-rw-rw-rw-   0        0        0     4472 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/tests/test_migrations.py
+-rw-rw-rw-   0        0        0     1392 2023-06-08 07:10:28.000000 django-data-browser-4.2.5/tests/test_models.py
+-rw-rw-rw-   0        0        0    35257 2023-07-01 07:55:19.000000 django-data-browser-4.2.5/tests/test_orm.py
+-rw-rw-rw-   0        0        0      878 2023-03-30 22:40:08.000000 django-data-browser-4.2.5/tests/test_orm_debug.py
+-rw-rw-rw-   0        0        0    25625 2023-07-19 14:15:50.000000 django-data-browser-4.2.5/tests/test_query.py
+-rw-rw-rw-   0        0        0      165 2020-10-22 20:32:07.000000 django-data-browser-4.2.5/tests/test_tests.py
+-rw-rw-rw-   0        0        0    18982 2023-07-09 12:36:02.000000 django-data-browser-4.2.5/tests/test_views.py
+-rw-rw-rw-   0        0        0      184 2020-10-22 18:16:38.000000 django-data-browser-4.2.5/tests/urls.py
+-rw-rw-rw-   0        0        0      366 2023-03-30 21:24:18.000000 django-data-browser-4.2.5/tests/util.py
+-rw-rw-rw-   0        0        0      574 2023-03-30 22:40:08.000000 django-data-browser-4.2.5/tox.ini
```

### Comparing `django-data-browser-4.2.4/.pre-commit-config.yaml` & `django-data-browser-4.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/CONTRIBUTING.rst` & `django-data-browser-4.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/LICENSE` & `django-data-browser-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/MANIFEST.in` & `django-data-browser-4.2.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/PKG-INFO` & `django-data-browser-4.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-browser
-Version: 4.2.4
+Version: 4.2.5
 Summary: Interactive user-friendly database explorer.
 Home-page: https://github.com/tolomea/django-data-browser
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -279,15 +279,15 @@
         "author__number_of_books",
         "publisher__name",
     )
     AuthorAdmin.get_queryset().in_bulk(pks=...)
 
 Where the ``pks`` passed to in_bulk in the second query came from ``author__id`` in the first.
 
-You can view an approximation of the main queryset by changing the `.html` in the URL to `.qs`. In a similar manner `.sql` and `.explain` are also available.
+You can view an approximation of the main queryset by changing the `.html` in the URL to `.qs`. In a similar manner `.sql`, `.explain` and `.analyze` are also available.
 
 When the Data Browser calls the admin ``get_queryset()`` functions it will put some context in ``request.data_browser``. This allows you to test to see if the Data Browser is making the call as follows:
 
 .. code-block:: python
 
     if hasattr(request, "data_browser"):
         # Data Browser specific customization
@@ -445,16 +445,19 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
-| 4.2.4   | 2023-07-02 | Provisional support for adding custom functions and aggregations.                                        |
-|         |            | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                         |
+| 4.2.5   | 2023-07-20 | | Fix parsing of date/datetime strings like ``mon-1``.                                                   |
+|         |            | | Add support for DB query analyze via ``.analyze`` url, similar to the existing ``.explain``.           |
++---------+------------+----------------------------------------------------------------------------------------------------------+
+| 4.2.4   | 2023-07-02 | | Provisional support for adding custom functions and aggregations.                                      |
+|         |            | | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                       |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.3   | 2023-06-15 | Fix ASGI compatibility issue.                                                                            |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
```

### Comparing `django-data-browser-4.2.4/README.rst` & `django-data-browser-4.2.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         "author__number_of_books",
         "publisher__name",
     )
     AuthorAdmin.get_queryset().in_bulk(pks=...)
 
 Where the ``pks`` passed to in_bulk in the second query came from ``author__id`` in the first.
 
-You can view an approximation of the main queryset by changing the `.html` in the URL to `.qs`. In a similar manner `.sql` and `.explain` are also available.
+You can view an approximation of the main queryset by changing the `.html` in the URL to `.qs`. In a similar manner `.sql`, `.explain` and `.analyze` are also available.
 
 When the Data Browser calls the admin ``get_queryset()`` functions it will put some context in ``request.data_browser``. This allows you to test to see if the Data Browser is making the call as follows:
 
 .. code-block:: python
 
     if hasattr(request, "data_browser"):
         # Data Browser specific customization
@@ -431,16 +431,19 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
-| 4.2.4   | 2023-07-02 | Provisional support for adding custom functions and aggregations.                                        |
-|         |            | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                         |
+| 4.2.5   | 2023-07-20 | | Fix parsing of date/datetime strings like ``mon-1``.                                                   |
+|         |            | | Add support for DB query analyze via ``.analyze`` url, similar to the existing ``.explain``.           |
++---------+------------+----------------------------------------------------------------------------------------------------------+
+| 4.2.4   | 2023-07-02 | | Provisional support for adding custom functions and aggregations.                                      |
+|         |            | | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                       |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.3   | 2023-06-15 | Fix ASGI compatibility issue.                                                                            |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
```

### Comparing `django-data-browser-4.2.4/data_browser/admin.py` & `django-data-browser-4.2.5/data_browser/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/api.py` & `django-data-browser-4.2.5/data_browser/api.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/common.py` & `django-data-browser-4.2.5/data_browser/common.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/fe_build/index.html` & `django-data-browser-4.2.5/data_browser/fe_build/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/fe_build/static/css/main.a2cd42f2.css` & `django-data-browser-4.2.5/data_browser/fe_build/static/css/main.a2cd42f2.css`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/fe_build/static/css/main.a2cd42f2.css.map` & `django-data-browser-4.2.5/data_browser/fe_build/static/css/main.a2cd42f2.css.map`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js` & `django-data-browser-4.2.5/data_browser/fe_build/static/js/main.c57e8af0.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt` & `django-data-browser-4.2.5/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js.map` & `django-data-browser-4.2.5/data_browser/fe_build/static/js/main.c57e8af0.js.map`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/format_csv.py` & `django-data-browser-4.2.5/data_browser/format_csv.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/helpers.py` & `django-data-browser-4.2.5/data_browser/helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/migration_helpers.py` & `django-data-browser-4.2.5/data_browser/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/migrations/0001_initial.py` & `django-data-browser-4.2.5/data_browser/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/migrations/0002_auto_20200331_1842.py` & `django-data-browser-4.2.5/data_browser/migrations/0002_auto_20200331_1842.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/migrations/0006_auto_20200531_1450.py` & `django-data-browser-4.2.5/data_browser/migrations/0006_auto_20200531_1450.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/migrations/0012_can_share.py` & `django-data-browser-4.2.5/data_browser/migrations/0012_can_share.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/models.py` & `django-data-browser-4.2.5/data_browser/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/orm_admin.py` & `django-data-browser-4.2.5/data_browser/orm_admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/orm_aggregates.py` & `django-data-browser-4.2.5/data_browser/orm_aggregates.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/orm_debug.py` & `django-data-browser-4.2.5/data_browser/orm_debug.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/orm_fields.py` & `django-data-browser-4.2.5/data_browser/orm_fields.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/orm_functions.py` & `django-data-browser-4.2.5/data_browser/orm_functions.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/orm_lookups.py` & `django-data-browser-4.2.5/data_browser/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/orm_results.py` & `django-data-browser-4.2.5/data_browser/orm_results.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/orm_types.py` & `django-data-browser-4.2.5/data_browser/orm_types.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/query.py` & `django-data-browser-4.2.5/data_browser/query.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/templates/data_browser/index.html` & `django-data-browser-4.2.5/data_browser/templates/data_browser/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/types.py` & `django-data-browser-4.2.5/data_browser/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,17 @@
 
     for c1 in _clause_types:
         for c2 in _clause_types:
             assert c1 == c2 or not c1.startswith(c2), c2
 
     @staticmethod
     def _unambiguous_date_parse(value, **kwargs):
+        if not any(c.isdigit() for c in value):
+            return None
+
         try:
             res = {
                 dateutil.parser.parse(value, dayfirst=False, yearfirst=False, **kwargs),
                 dateutil.parser.parse(value, dayfirst=True, yearfirst=False, **kwargs),
                 dateutil.parser.parse(value, dayfirst=False, yearfirst=True, **kwargs),
                 dateutil.parser.parse(value, dayfirst=True, yearfirst=True, **kwargs),
             }
@@ -284,35 +287,26 @@
         d422 = r"(\d{4}[^\d]+\d{1,2}[^\d]+\d{1,2}([^\d]|$))"
 
         res = timezone.now()
 
         # iterate the clauses in the expression
         for clause_str in value.split():
             clause_str = clause_str.lower()
+            match = cls._clause.fullmatch(clause_str)
 
             if clause_str == "now":
                 res = timezone.now()
             elif clause_str == "today":
                 res = cls._truncate_dt(timezone.now())
             elif re.match(rf"[^\d]*({d8}|{d422})", clause_str):
                 # looks like some kinda iso date, roll with the defaults
                 # includes T delimited like 2018-03-20T22:31:23
                 res = dateutil.parser.parse(clause_str, default=cls._truncate_dt(res))
-            elif cls._unambiguous_date_parse(clause_str, default=cls._truncate_dt(res)):
-                # TODO could walrus the duplicate call once we drop support for py3.7
-                res = cls._unambiguous_date_parse(
-                    clause_str, default=cls._truncate_dt(res)
-                )
-            else:
-                # failing that must be relative delta stuff
-                match = cls._clause.fullmatch(clause_str)
-                if not match:
-                    raise Exception(f"Unrecognized clause '{clause_str}'")
-
-                # cut up the clause
+            elif match:
+                # relative delta stuff, cut up the clause
                 field, op, val = match.groups()
                 val = int(val)
                 human_op = {"+": "add", "-": "subtract", "=": "set"}[op]
 
                 # find the field
                 for prefix, arg in cls._clause_types.items():
                     if field.startswith(prefix):
@@ -345,14 +339,21 @@
                             raise Exception(f"Can't {human_op} '{val}' '{field}'s")
                         if op == "+":
                             kwargs = {"weekday": arg(val)}
                         else:  # op == "-"
                             kwargs = {"weekday": arg(-val)}
 
                 res += relativedelta.relativedelta(**kwargs)
+            elif cls._unambiguous_date_parse(clause_str, default=cls._truncate_dt(res)):
+                # TODO could walrus the duplicate call once we drop support for py3.7
+                res = cls._unambiguous_date_parse(
+                    clause_str, default=cls._truncate_dt(res)
+                )
+            else:
+                raise Exception(f"Unrecognized clause '{clause_str}'")
 
         return res
 
 
 class DateTimeType(DateTimeParseMixin, SequenceTypeMixin, BaseType):
     default_value = "now"
```

### Comparing `django-data-browser-4.2.4/data_browser/urls.py` & `django-data-browser-4.2.5/data_browser/urls.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/views.py` & `django-data-browser-4.2.5/data_browser/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -319,37 +319,52 @@
         results = get_results(bound_query, orm_models, True)
         resp = _get_query_data(bound_query) if privileged else {}
         resp.update(results)
         return JsonResponse(resp)
     elif privileged and media == "query":
         resp = _get_query_data(bound_query)
         return JsonResponse(resp)
-    elif privileged and media in ["sql", "explain", "qs"]:
+    elif privileged and media in ["sql", "explain", "analyze", "qs"]:
         query_set = get_result_queryset(bound_query, media == "qs")
         if isinstance(query_set, list):
             res = "Not available for pure aggregates"
         else:
-            if media == "sql":
+            # disclaimer
+            if media in ["sql", "explain", "analyze"]:
                 res = (
                     "/* This is an approximation of the main query.\nPages with pivoted"
-                    " or calculated data may do additional queries. */\n\n"
-                )
-                res += sqlparse.format(
-                    str(query_set.query), reindent=True, keyword_case="upper"
+                    " or calculated data may do additional queries. */\n\n\n"
                 )
-            elif media == "explain":
-                res = query_set.explain()
             elif media == "qs":
                 res = (
                     "# This is an approximation of the main queryset.\n# Pages with"
-                    " pivoted or calculated data may do additional queries.\n\n"
+                    " pivoted or calculated data may do additional queries.\n\n\n"
                 )
+            else:
+                assert False
+
+            # main part
+            if media == "sql":
+                pass  # actual SQL is handled below
+            elif media == "explain":
+                res += query_set.explain()
+                res += "\n\n\n"
+            elif media == "analyze":
+                res += query_set.explain(analyze=True)
+                res += "\n\n\n"
+            elif media == "qs":
                 res += str(query_set)
             else:
                 assert False
+
+            # sql
+            if media in ["sql", "explain", "analyze"]:
+                res += sqlparse.format(
+                    str(query_set.query), reindent=True, keyword_case="upper"
+                )
         return HttpResponse(res, content_type="text/plain")
     else:
         raise http.Http404(f"Bad file format {media} requested")
 
 
 def _get_from_js_dev_server(request, method=None):  # pragma: no cover
     import requests
```

### Comparing `django-data-browser-4.2.4/data_browser/web_root/android-chrome-192x192.png` & `django-data-browser-4.2.5/data_browser/web_root/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/web_root/android-chrome-512x512.png` & `django-data-browser-4.2.5/data_browser/web_root/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/web_root/apple-touch-icon.png` & `django-data-browser-4.2.5/data_browser/web_root/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/web_root/favicon-32x32.png` & `django-data-browser-4.2.5/data_browser/web_root/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/data_browser/web_root/favicon.ico` & `django-data-browser-4.2.5/data_browser/web_root/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/django_data_browser.egg-info/PKG-INFO` & `django-data-browser-4.2.5/django_data_browser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-browser
-Version: 4.2.4
+Version: 4.2.5
 Summary: Interactive user-friendly database explorer.
 Home-page: https://github.com/tolomea/django-data-browser
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -279,15 +279,15 @@
         "author__number_of_books",
         "publisher__name",
     )
     AuthorAdmin.get_queryset().in_bulk(pks=...)
 
 Where the ``pks`` passed to in_bulk in the second query came from ``author__id`` in the first.
 
-You can view an approximation of the main queryset by changing the `.html` in the URL to `.qs`. In a similar manner `.sql` and `.explain` are also available.
+You can view an approximation of the main queryset by changing the `.html` in the URL to `.qs`. In a similar manner `.sql`, `.explain` and `.analyze` are also available.
 
 When the Data Browser calls the admin ``get_queryset()`` functions it will put some context in ``request.data_browser``. This allows you to test to see if the Data Browser is making the call as follows:
 
 .. code-block:: python
 
     if hasattr(request, "data_browser"):
         # Data Browser specific customization
@@ -445,16 +445,19 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
-| 4.2.4   | 2023-07-02 | Provisional support for adding custom functions and aggregations.                                        |
-|         |            | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                         |
+| 4.2.5   | 2023-07-20 | | Fix parsing of date/datetime strings like ``mon-1``.                                                   |
+|         |            | | Add support for DB query analyze via ``.analyze`` url, similar to the existing ``.explain``.           |
++---------+------------+----------------------------------------------------------------------------------------------------------+
+| 4.2.4   | 2023-07-02 | | Provisional support for adding custom functions and aggregations.                                      |
+|         |            | | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                       |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.3   | 2023-06-15 | Fix ASGI compatibility issue.                                                                            |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
```

### Comparing `django-data-browser-4.2.4/django_data_browser.egg-info/SOURCES.txt` & `django-data-browser-4.2.5/django_data_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/README.md` & `django-data-browser-4.2.5/frontend/README.md`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/package-lock.json` & `django-data-browser-4.2.5/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/package.json` & `django-data-browser-4.2.5/frontend/package.json`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/public/index.html` & `django-data-browser-4.2.5/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/App.js` & `django-data-browser-4.2.5/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/App.scss` & `django-data-browser-4.2.5/frontend/src/App.scss`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/ContextMenu.js` & `django-data-browser-4.2.5/frontend/src/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/CurrentSavedView.js` & `django-data-browser-4.2.5/frontend/src/CurrentSavedView.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/HomePage.js` & `django-data-browser-4.2.5/frontend/src/HomePage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/Query.js` & `django-data-browser-4.2.5/frontend/src/Query.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/QueryPage.js` & `django-data-browser-4.2.5/frontend/src/QueryPage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/Results.js` & `django-data-browser-4.2.5/frontend/src/Results.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/SavedViewPage.js` & `django-data-browser-4.2.5/frontend/src/SavedViewPage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/Tooltip.js` & `django-data-browser-4.2.5/frontend/src/Tooltip.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/Util.js` & `django-data-browser-4.2.5/frontend/src/Util.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/WindowDimensions.js` & `django-data-browser-4.2.5/frontend/src/WindowDimensions.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/index.js` & `django-data-browser-4.2.5/frontend/src/index.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/frontend/src/logo.svg` & `django-data-browser-4.2.5/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/pyproject.toml` & `django-data-browser-4.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/screenshot.png` & `django-data-browser-4.2.5/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/setup.py` & `django-data-browser-4.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/structure.svg` & `django-data-browser-4.2.5/structure.svg`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/array/models.py` & `django-data-browser-4.2.5/tests/array/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/conftest.py` & `django-data-browser-4.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/core/admin.py` & `django-data-browser-4.2.5/tests/core/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/core/migrations/0001_initial.py` & `django-data-browser-4.2.5/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/core/models.py` & `django-data-browser-4.2.5/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/snapshots/snap_test_views.py` & `django-data-browser-4.2.5/tests/snapshots/snap_test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -12315,14 +12315,15 @@
     "rows": [{"created_time__year": 2020.0}, {"created_time__year": 2021.0}],
 }
 
 snapshots["test_query_qs_variants content"] = [
     "# This is an approximation of the main queryset.",
     "# Pages with pivoted or calculated data may do additional queries.",
     "",
+    "",
     "tests.core.admin.ProductAdmin(model, admin_site).get_queryset(request).annotate(",
     "    ddb_size_is_null=ExpressionWrapper(",
     "        Q(size=None),",
     "        output_field=BooleanField(),",
     "    ),",
     ").annotate(",
     "    ddb_annotated=Subquery(",
```

### Comparing `django-data-browser-4.2.4/tests/test_admin.py` & `django-data-browser-4.2.5/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_api.py` & `django-data-browser-4.2.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_array_field.py` & `django-data-browser-4.2.5/tests/test_array_field.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_common.py` & `django-data-browser-4.2.5/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_helpers.py` & `django-data-browser-4.2.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_json_field.py` & `django-data-browser-4.2.5/tests/test_json_field.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_migrations.py` & `django-data-browser-4.2.5/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_models.py` & `django-data-browser-4.2.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_orm.py` & `django-data-browser-4.2.5/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_orm_debug.py` & `django-data-browser-4.2.5/tests/test_orm_debug.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.4/tests/test_query.py` & `django-data-browser-4.2.5/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -449,20 +449,20 @@
             ("hour=0", dt(2020, 12, 13, 0, 42, 53), None),
             ("month+1", dt(2021, 1, 13, 9, 42, 53), None),
             ("month-1", dt(2020, 11, 13, 9, 42, 53), None),
             ("month=1", dt(2020, 1, 13, 9, 42, 53), None),
             ("month 1", None, "Unrecognized clause 'month'"),
             ("month+0", dt(2020, 12, 13, 9, 42, 53), None),
             ("month=0", None, "Can't set 'month' to '0'"),
-            ("thurs+1", dt(2020, 12, 17, 9, 42, 53), None),
-            ("thurs-1", dt(2020, 12, 10, 9, 42, 53), None),
-            ("thurs=1", None, "'=' not supported for 'thurs'"),
-            ("thurs 1", None, "Unrecognized clause 'thurs'"),
-            ("thurs+0", None, "Can't add '0' 'thurs's"),
-            ("thurs=0", None, "'=' not supported for 'thurs'"),
+            ("thu+1", dt(2020, 12, 17, 9, 42, 53), None),
+            ("thu-1", dt(2020, 12, 10, 9, 42, 53), None),
+            ("thu=1", None, "'=' not supported for 'thu'"),
+            ("thu 1", None, "Unrecognized clause 'thu'"),
+            ("thu+0", None, "Can't add '0' 'thu's"),
+            ("thu=0", None, "'=' not supported for 'thu'"),
             ("month+1 month=1", dt(2021, 1, 13, 9, 42, 53), None),
             ("month=1 month+1", dt(2020, 2, 13, 9, 42, 53), None),
             ("bobit+1", None, "Unrecognized field 'bobit'"),
             ("week=1", None, "'=' not supported for 'week'"),
         ],
     )
     def test_parse(self, value, expected, err):
```

### Comparing `django-data-browser-4.2.4/tests/test_views.py` & `django-data-browser-4.2.5/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,23 @@
     res = admin_client.get(
         "/data_browser/query/core.Product/size-0,name+1,size_unit.explain"
         "?size__lt=2&id__gt=0"
     )
     assert res.status_code == 200
 
 
+@pytest.mark.skipif(SQLITE, reason="Not supported by SQLITE")
+def test_query_analyze(admin_client):
+    res = admin_client.get(
+        "/data_browser/query/core.Product/size-0,name+1,size_unit.analyze"
+        "?size__lt=2&id__gt=0"
+    )
+    assert res.status_code == 200
+
+
 def test_query_sql_aggregate(admin_client):
     res = admin_client.get("/data_browser/query/core.Product/size__count.sql")
     assert res.status_code == 200
 
 
 def test_query_qs_variants(admin_client, snapshot):
     res = admin_client.get(
```

### Comparing `django-data-browser-4.2.4/tox.ini` & `django-data-browser-4.2.5/tox.ini`

 * *Files identical despite different names*

