# Comparing `tmp/vstutils-5.6.1.tar.gz` & `tmp/vstutils-5.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.6.1.tar", last modified: Thu Jul 20 03:28:42 2023, max compression
+gzip compressed data, was "vstutils-5.6.2.tar", last modified: Thu Jul 20 08:32:38 2023, max compression
```

## Comparing `vstutils-5.6.1.tar` & `vstutils-5.6.2.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.008897 vstutils-5.6.1/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.6.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.6.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.6.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4427 2023-07-20 03:28:42.008897 vstutils-5.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2389 2023-06-22 02:12:27.000000 vstutils-5.6.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-30 04:31:13.000000 vstutils-5.6.1/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.6.1/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.6.1/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-30 04:31:13.000000 vstutils-5.6.1/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-30 04:31:13.000000 vstutils-5.6.1/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-28 03:44:06.000000 vstutils-5.6.1/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-14 22:04:13.000000 vstutils-5.6.1/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-17 01:55:56.000000 vstutils-5.6.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-07-20 03:28:42.012897 vstutils-5.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.956896 vstutils-5.6.1/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-20 02:32:17.000000 vstutils-5.6.1/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.960896 vstutils-5.6.1/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-14 22:04:13.000000 vstutils-5.6.1/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.6.1/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-17 22:32:27.000000 vstutils-5.6.1/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:54.000000 vstutils-5.6.1/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    29458 2023-07-14 07:52:42.000000 vstutils-5.6.1/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:43.000000 vstutils-5.6.1/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.6.1/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-14 22:04:13.000000 vstutils-5.6.1/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:43.000000 vstutils-5.6.1/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    13794 2023-07-14 07:52:42.000000 vstutils-5.6.1/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.6.1/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-27 04:42:54.000000 vstutils-5.6.1/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.964896 vstutils-5.6.1/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-14 22:04:13.000000 vstutils-5.6.1/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-14 07:52:42.000000 vstutils-5.6.1/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.6.1/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.6.1/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.964896 vstutils-5.6.1/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.6.1/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-07-08 04:27:47.000000 vstutils-5.6.1/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    29661 2023-07-14 07:52:42.000000 vstutils-5.6.1/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)    11905 2023-07-14 07:52:42.000000 vstutils-5.6.1/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-14 22:04:13.000000 vstutils-5.6.1/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:17:53.000000 vstutils-5.6.1/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5667 2023-06-27 04:42:54.000000 vstutils-5.6.1/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3554 2023-06-30 04:31:13.000000 vstutils-5.6.1/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-06-28 03:44:06.000000 vstutils-5.6.1/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:04.000000 vstutils-5.6.1/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.6.1/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.6.1/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.940896 vstutils-5.6.1/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.964896 vstutils-5.6.1/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.964896 vstutils-5.6.1/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.6.1/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.968896 vstutils-5.6.1/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3487 2023-06-23 05:26:08.000000 vstutils-5.6.1/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.6.1/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.6.1/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.968896 vstutils-5.6.1/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.968896 vstutils-5.6.1/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:54.000000 vstutils-5.6.1/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.6.1/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     3661 2023-07-08 04:27:47.000000 vstutils-5.6.1/vstutils/management/commands/rpc_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-17 22:32:27.000000 vstutils-5.6.1/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.6.1/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.6.1/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10594 2023-06-30 04:31:13.000000 vstutils-5.6.1/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.972896 vstutils-5.6.1/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.6.1/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25952 2023-07-14 05:18:37.000000 vstutils-5.6.1/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4528 2023-07-20 02:32:17.000000 vstutils-5.6.1/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.6.1/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.6.1/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:17:53.000000 vstutils-5.6.1/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    55656 2023-07-08 04:27:47.000000 vstutils-5.6.1/vstutils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.6.1/vstutils/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.944896 vstutils-5.6.1/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.980896 vstutils-5.6.1/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126391 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      170 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1099741 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/505.js
--rw-r--r--   0 root         (0) root         (0)     2180 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/505.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38355 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    73740 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536116 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    87131 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      218 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355745 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)   113317 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/app_loader.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   317669 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3621 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   513414 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.984896 vstutils-5.6.1/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.984896 vstutils-5.6.1/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5580 2023-07-20 02:32:17.000000 vstutils-5.6.1/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.984896 vstutils-5.6.1/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.6.1/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.6.1/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.6.1/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.6.1/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.988896 vstutils-5.6.1/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.6.1/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.6.1/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.988896 vstutils-5.6.1/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.988896 vstutils-5.6.1/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.6.1/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.992896 vstutils-5.6.1/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.996897 vstutils-5.6.1/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.996897 vstutils-5.6.1/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.000897 vstutils-5.6.1/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.000897 vstutils-5.6.1/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.000897 vstutils-5.6.1/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.6.1/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.004897 vstutils-5.6.1/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.6.1/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.004897 vstutils-5.6.1/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.008897 vstutils-5.6.1/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.008897 vstutils-5.6.1/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.008897 vstutils-5.6.1/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.6.1/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.6.1/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    18312 2023-07-08 04:27:47.000000 vstutils-5.6.1/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:42.008897 vstutils-5.6.1/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16335 2023-07-14 02:01:10.000000 vstutils-5.6.1/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    24130 2023-07-14 02:01:10.000000 vstutils-5.6.1/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    19158 2023-07-14 02:01:10.000000 vstutils-5.6.1/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.6.1/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-14 22:04:13.000000 vstutils-5.6.1/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.6.1/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.6.1/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:28:41.956896 vstutils-5.6.1/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4427 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7756 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1835 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 03:28:41.000000 vstutils-5.6.1/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.141970 vstutils-5.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.6.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.6.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.6.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-07-20 08:32:38.141970 vstutils-5.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2023-06-22 02:12:27.000000 vstutils-5.6.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-30 04:31:13.000000 vstutils-5.6.2/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.6.2/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.6.2/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-30 04:31:13.000000 vstutils-5.6.2/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-30 04:31:13.000000 vstutils-5.6.2/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-28 03:44:06.000000 vstutils-5.6.2/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-14 22:04:13.000000 vstutils-5.6.2/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-17 01:55:56.000000 vstutils-5.6.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-07-20 08:32:38.141970 vstutils-5.6.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.097970 vstutils-5.6.2/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-20 08:09:36.000000 vstutils-5.6.2/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.105970 vstutils-5.6.2/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-14 22:04:13.000000 vstutils-5.6.2/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.6.2/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-17 22:32:27.000000 vstutils-5.6.2/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:54.000000 vstutils-5.6.2/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    29458 2023-07-14 07:52:42.000000 vstutils-5.6.2/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:43.000000 vstutils-5.6.2/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.6.2/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-14 22:04:13.000000 vstutils-5.6.2/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:43.000000 vstutils-5.6.2/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    13849 2023-07-20 08:09:36.000000 vstutils-5.6.2/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.6.2/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-27 04:42:54.000000 vstutils-5.6.2/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.105970 vstutils-5.6.2/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-14 22:04:13.000000 vstutils-5.6.2/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-14 07:52:42.000000 vstutils-5.6.2/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.6.2/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.6.2/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.109970 vstutils-5.6.2/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.6.2/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-07-08 04:27:47.000000 vstutils-5.6.2/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    29661 2023-07-14 07:52:42.000000 vstutils-5.6.2/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)    11905 2023-07-14 07:52:42.000000 vstutils-5.6.2/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-14 22:04:13.000000 vstutils-5.6.2/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:17:53.000000 vstutils-5.6.2/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2023-06-27 04:42:54.000000 vstutils-5.6.2/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3554 2023-06-30 04:31:13.000000 vstutils-5.6.2/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2023-06-28 03:44:06.000000 vstutils-5.6.2/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:04.000000 vstutils-5.6.2/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.6.2/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.6.2/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.089969 vstutils-5.6.2/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.109970 vstutils-5.6.2/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.109970 vstutils-5.6.2/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.6.2/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.109970 vstutils-5.6.2/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3487 2023-06-23 05:26:08.000000 vstutils-5.6.2/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.6.2/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.6.2/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.109970 vstutils-5.6.2/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.109970 vstutils-5.6.2/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:54.000000 vstutils-5.6.2/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.6.2/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     3661 2023-07-08 04:27:47.000000 vstutils-5.6.2/vstutils/management/commands/rpc_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-17 22:32:27.000000 vstutils-5.6.2/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.6.2/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.6.2/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10594 2023-06-30 04:31:13.000000 vstutils-5.6.2/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.113970 vstutils-5.6.2/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.6.2/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25952 2023-07-14 05:18:37.000000 vstutils-5.6.2/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2023-07-20 08:09:36.000000 vstutils-5.6.2/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.6.2/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.6.2/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:17:53.000000 vstutils-5.6.2/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    55656 2023-07-08 04:27:47.000000 vstutils-5.6.2/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.6.2/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.089969 vstutils-5.6.2/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.121970 vstutils-5.6.2/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126391 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      170 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1099741 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/505.js
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/505.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38355 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    73740 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536116 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    87131 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355745 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)   113317 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/app_loader.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   317669 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   513414 2023-07-20 08:32:37.000000 vstutils-5.6.2/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.121970 vstutils-5.6.2/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.125970 vstutils-5.6.2/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5592 2023-07-20 08:09:36.000000 vstutils-5.6.2/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.125970 vstutils-5.6.2/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.6.2/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.6.2/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.6.2/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.6.2/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.125970 vstutils-5.6.2/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.6.2/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.6.2/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.125970 vstutils-5.6.2/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.125970 vstutils-5.6.2/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.6.2/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.129970 vstutils-5.6.2/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.129970 vstutils-5.6.2/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.133970 vstutils-5.6.2/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.133970 vstutils-5.6.2/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.133970 vstutils-5.6.2/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.133970 vstutils-5.6.2/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.6.2/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.137970 vstutils-5.6.2/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.6.2/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.137970 vstutils-5.6.2/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.137970 vstutils-5.6.2/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.137970 vstutils-5.6.2/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.137970 vstutils-5.6.2/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.6.2/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.6.2/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18312 2023-07-08 04:27:47.000000 vstutils-5.6.2/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.141970 vstutils-5.6.2/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16335 2023-07-14 02:01:10.000000 vstutils-5.6.2/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    24130 2023-07-14 02:01:10.000000 vstutils-5.6.2/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    19158 2023-07-14 02:01:10.000000 vstutils-5.6.2/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.6.2/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    47150 2023-07-20 08:09:36.000000 vstutils-5.6.2/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.6.2/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.6.2/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:32:38.097970 vstutils-5.6.2/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-07-20 08:32:38.000000 vstutils-5.6.2/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7756 2023-07-20 08:32:38.000000 vstutils-5.6.2/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-20 08:32:38.000000 vstutils-5.6.2/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-20 08:32:38.000000 vstutils-5.6.2/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 08:32:38.000000 vstutils-5.6.2/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-07-20 08:32:38.000000 vstutils-5.6.2/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 08:32:38.000000 vstutils-5.6.2/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.6.1/LICENSE` & `vstutils-5.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/MANIFEST.in` & `vstutils-5.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/NOTICE` & `vstutils-5.6.2/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/PKG-INFO` & `vstutils-5.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.6.1
+Version: 5.6.2
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.6.1/README.rst` & `vstutils-5.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/setup.cfg` & `vstutils-5.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/setup.py` & `vstutils-5.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/actions.py` & `vstutils-5.6.2/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/admin.py` & `vstutils-5.6.2/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/auth.py` & `vstutils-5.6.2/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/base.py` & `vstutils-5.6.2/vstutils/api/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/decorators.py` & `vstutils-5.6.2/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/decorators.pyi` & `vstutils-5.6.2/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/doc_generator.py` & `vstutils-5.6.2/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/endpoint.py` & `vstutils-5.6.2/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/fields.py` & `vstutils-5.6.2/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/filter_backends.py` & `vstutils-5.6.2/vstutils/api/filter_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         if isinstance(field, filters.NumberFilter):
             field_type = openapi.TYPE_NUMBER
         elif isinstance(field, filters.BooleanFilter):
             field_type = openapi.TYPE_BOOLEAN
         elif isinstance(field, filters.ChoiceFilter):
             kwargs['enum'] = tuple(dict(field.field.choices).keys())
         elif field_name in {'id', 'id__not'}:
-            m_field = next((f for f in queryset.model._meta.fields if f.name == field_name), None)
+            search_field = field_name.split('__')[0]
+            m_field = next((f for f in queryset.model._meta.fields if f.name == search_field), None)
             field_type, kwargs_update = get_field_type_from_queryset(m_field)
 
         if field.method == extra_filter:
             kwargs = {
                 'items': {
                     'type': field_type,
                     **kwargs,
```

### Comparing `vstutils-5.6.1/vstutils/api/filters.py` & `vstutils-5.6.2/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/health.py` & `vstutils-5.6.2/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/meta.py` & `vstutils-5.6.2/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/metrics.py` & `vstutils-5.6.2/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/migrations/0001_initial.py` & `vstutils-5.6.2/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.6.2/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.6.2/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.6.2/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.6.2/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.6.2/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/models.py` & `vstutils-5.6.2/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/pagination.py` & `vstutils-5.6.2/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/parsers.py` & `vstutils-5.6.2/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/permissions.py` & `vstutils-5.6.2/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/renderers.py` & `vstutils-5.6.2/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/responses.py` & `vstutils-5.6.2/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/responses.pyi` & `vstutils-5.6.2/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/routers.py` & `vstutils-5.6.2/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/routers.pyi` & `vstutils-5.6.2/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/schema/generators.py` & `vstutils-5.6.2/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/schema/info.py` & `vstutils-5.6.2/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/schema/inspectors.py` & `vstutils-5.6.2/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/schema/schema.py` & `vstutils-5.6.2/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/serializers.py` & `vstutils-5.6.2/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/throttling.py` & `vstutils-5.6.2/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/validators.py` & `vstutils-5.6.2/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/api/views.py` & `vstutils-5.6.2/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/asgi.py` & `vstutils-5.6.2/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/asgi_worker.py` & `vstutils-5.6.2/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/auth.py` & `vstutils-5.6.2/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/auth.pyi` & `vstutils-5.6.2/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/celery_beat_scheduler.py` & `vstutils-5.6.2/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.6.2/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/environment.py` & `vstutils-5.6.2/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/exceptions.py` & `vstutils-5.6.2/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/gui/context.py` & `vstutils-5.6.2/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/gui/forms.py` & `vstutils-5.6.2/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/gui/pwa_manifest.py` & `vstutils-5.6.2/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/gui/views.py` & `vstutils-5.6.2/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/ldap_utils.py` & `vstutils-5.6.2/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/_base.py` & `vstutils-5.6.2/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/celery_inspect.py` & `vstutils-5.6.2/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/dockerrun.py` & `vstutils-5.6.2/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/newproject.py` & `vstutils-5.6.2/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/rpc_worker.py` & `vstutils-5.6.2/vstutils/management/commands/rpc_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/run_task.py` & `vstutils-5.6.2/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/runrpc.py` & `vstutils-5.6.2/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/runserver.py` & `vstutils-5.6.2/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/management/commands/web.py` & `vstutils-5.6.2/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/middleware.py` & `vstutils-5.6.2/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/models/__init__.py` & `vstutils-5.6.2/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/models/base.py` & `vstutils-5.6.2/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/models/cent_notify.py` & `vstutils-5.6.2/vstutils/models/cent_notify.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,34 +29,35 @@
 
     queue: _t.List[_t.Tuple[_t.Sequence[_t.Text], _t.Any]]
     cent_client: CentrifugoClient
     label: _t.Text
 
     _json_renderer = ORJSONRenderer()
 
-    def __init__(self, queue=None, client=None, label=None):
+    def __init__(self, queue=None, client=None, label=None, autoconnect=True):
         self.queue = queue or []
         self.cent_client = client
         self.label = label
         self._signals: _t.List[signals.ModelSignal] = []
-        if self.is_usable():
+        if autoconnect and self.is_usable():
             self.connect_signal(signals.post_save)
             self.connect_signal(signals.post_delete)
 
     def is_usable(self):
         return bool(settings.CENTRIFUGO_CLIENT_KWARGS) or self.cent_client  # nocv
 
     def connect_signal(self, signal: signals.ModelSignal):
         if signal not in self._signals:
             signal.connect(self.signal_handler)
             self._signals.append(signal)
 
     def disconnect_signal(self, signal: signals.ModelSignal):
         if signal in self._signals:
             signal.disconnect(self.signal_handler)
+            self._signals.remove(signal)
 
     def signal_handler(self, instance, *args, **kwargs):
         if isinstance(instance, (BaseModel, get_user_model())) and getattr(instance, '_notify_update', True):
             self.create_notification_from_instance(instance)
 
     def get_openapi_secret(self):
         return settings.CENTRIFUGO_CLIENT_KWARGS.get('token_hmac_secret_key', '')
@@ -67,20 +68,24 @@
         centrifugo_client_kwargs.pop('token_hmac_secret_key', None)
         if 'json_encoder' not in centrifugo_client_kwargs:
             centrifugo_client_kwargs['json_encoder'] = JsonEncoder
         logger.debug(f"Getting Centrifugo client with kwargs: {centrifugo_client_kwargs}")
         return self.client_class(**centrifugo_client_kwargs)
 
     def create_notification_from_instance(self, instance):  # pylint: disable=invalid-name
+        if not self.is_usable():
+            return  # nocv
         model = instance.__class__
         self.queue.append(
             ((model._meta.label, *get_proxy_labels(model)), {'pk': instance.pk})
         )
 
     def create_notification(self, labels, data):
+        if not self.is_usable():
+            return  # nocv
         if isinstance(labels, str):
             labels = (labels,)
         data = orjson.loads(self._json_renderer.render(data) or '{}')
         self.queue.append(
             (labels, data)
         )
 
@@ -102,29 +107,29 @@
                 for obj_label in obj_labels:
                     channel = self.get_subscription_channel(provided_label or obj_label)
                     self.cent_client.add("publish", self.cent_client.get_publish_params(
                         channel=channel,
                         data=data,
                     ))
                     sent_channels.add(channel)
-        if objects:
+        if objects and sent_channels:
             logger.debug(f'Send notifications about {len(objects)} updates to channel(s) {sent_channels}.')
             return self.cent_client.send()
 
     def disconnect_all(self):
         for signal in self._signals:
             self.disconnect_signal(signal)
 
     def get_subscription_channel(self, label: str):
         return f'{settings.SUBSCRIPTIONS_PREFIX}.{label}'
 
     def __del__(self):
-        logger.debug('Disconnect all notification signals.')
+        logger.log(logging.NOTSET, 'Disconnect all notification signals.')
         self.disconnect_all()
-        logger.debug('Disconnected all notification signals.')
+        logger.log(logging.NOTSET, 'Disconnected all notification signals.')
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.is_usable():
             self.send()
```

### Comparing `vstutils-5.6.1/vstutils/models/custom_model.py` & `vstutils-5.6.2/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/models/custom_model.pyi` & `vstutils-5.6.2/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/models/decorators.py` & `vstutils-5.6.2/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/models/fields.py` & `vstutils-5.6.2/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/models/queryset.py` & `vstutils-5.6.2/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/settings.ini` & `vstutils-5.6.2/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/settings.py` & `vstutils-5.6.2/vstutils/settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/281.chunk.js` & `vstutils-5.6.2/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/296.chunk.js` & `vstutils-5.6.2/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/345.chunk.js` & `vstutils-5.6.2/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/368.chunk.js` & `vstutils-5.6.2/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/421.js` & `vstutils-5.6.2/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.6.2/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/505.js` & `vstutils-5.6.2/vstutils/static/bundle/505.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/505.js.LICENSE.txt` & `vstutils-5.6.2/vstutils/static/bundle/505.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/618.js` & `vstutils-5.6.2/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/683.chunk.js` & `vstutils-5.6.2/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/686.js` & `vstutils-5.6.2/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/742.chunk.js` & `vstutils-5.6.2/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.6.2/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/755.js` & `vstutils-5.6.2/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/826.chunk.js` & `vstutils-5.6.2/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.6.2/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/844.js` & `vstutils-5.6.2/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/app_loader.js` & `vstutils-5.6.2/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/base.js` & `vstutils-5.6.2/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.6.2/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.6.2/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/output.json` & `vstutils-5.6.2/vstutils/static/bundle/output.json`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/spa.js` & `vstutils-5.6.2/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/bundle/vstutils.js` & `vstutils-5.6.2/vstutils/static/bundle/vstutils.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static/img/anonymous.png` & `vstutils-5.6.2/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/static_files.py` & `vstutils-5.6.2/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/tasks.py` & `vstutils-5.6.2/vstutils/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 from django.apps import apps
 
 from .utils import import_class, send_template_email_handler, Lock, translate as _
 
 celery_app: Celery = import_class(
     settings.WORKER_OPTIONS['app'].replace(':', '.')  # type: ignore
 )
-notificator_class = apps.get_app_config('vstutils_api').module.notificator_class
 notificator = None
 
 
+def get_notificator():
+    return apps.get_app_config('vstutils_api').module.notificator_class([])
+
+
 @worker_process_init.connect
 def init_notificator(*_, **__):
     # pylint: disable=global-statement
     global notificator
-    notificator = notificator_class([])  # nocv
+    notificator = get_notificator()  # nocv
 
 
 @worker_process_shutdown.connect
 def destruct_notificator(*_, **__):
     # pylint: disable=global-statement
     global notificator
     if notificator is not None:  # nocv
@@ -50,15 +53,15 @@
     @staticmethod
     def get_notificator_decorator(func):
         if getattr(func, '__notify_wrapped__', False):
             return func
 
         @wraps(func, assigned=WRAPPER_ASSIGNMENTS+('__notify_wrapped__',))
         def wrapper(self, *args, **kwargs):
-            with notificator or notificator_class([]):
+            with notificator or get_notificator():
                 self.__notifier__ = notificator
                 result = func(self, *args, **kwargs)
             self.__notifier__ = None
             return result
 
         wrapper.__notify_wrapped__ = True
         return wrapper
```

### Comparing `vstutils-5.6.1/vstutils/templates/auth/base.html` & `vstutils-5.6.2/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/auth/language_selector.html` & `vstutils-5.6.2/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/auth/tfa.html` & `vstutils-5.6.2/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/base.html` & `vstutils-5.6.2/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/gui/base.html` & `vstutils-5.6.2/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/gui/offline.html` & `vstutils-5.6.2/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/gui/service-worker.js` & `vstutils-5.6.2/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.6.2/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.6.2/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/package.json.template` & `vstutils-5.6.2/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.6.2/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.6.2/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/setup.py.template` & `vstutils-5.6.2/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/test.py.template` & `vstutils-5.6.2/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.6.2/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.6.2/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.6.2/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/registration/confirm_email.html` & `vstutils-5.6.2/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.6.2/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.6.2/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/registration/user_registration.html` & `vstutils-5.6.2/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/rest_framework/admin.html` & `vstutils-5.6.2/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.6.2/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.6.2/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templatetags/request_static.py` & `vstutils-5.6.2/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templatetags/translation.py` & `vstutils-5.6.2/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.6.2/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.6.2/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/templatetags/vstconfigs.py` & `vstutils-5.6.2/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/tests.py` & `vstutils-5.6.2/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/tools.py` & `vstutils-5.6.2/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/translations/cn.py` & `vstutils-5.6.2/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/translations/ru.py` & `vstutils-5.6.2/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/translations/vi.py` & `vstutils-5.6.2/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/urls.py` & `vstutils-5.6.2/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/utils.py` & `vstutils-5.6.2/vstutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import typing as tp
 import uuid
 import warnings
 from functools import lru_cache, wraps
 from pathlib import Path
 from enum import Enum, EnumMeta
 
-from asgiref.sync import sync_to_async
+from asgiref.sync import sync_to_async, async_to_sync
 from django.conf import settings
 from django.middleware.gzip import GZipMiddleware
 from django.urls import re_path, path, include
 from django.core.mail import get_connection, EmailMultiAlternatives
 from django.core.cache import caches, InvalidCacheBackendError
 from django.core.paginator import Paginator as BasePaginator
 from django.template import loader
@@ -909,16 +909,15 @@
         Executes commands and outputs its result.
 
         :param cmd: -- list of cmd command and arguments
         :param cwd: -- workdir for executions
         :param env: -- extra environment variables which overrides defaults
         :return: -- string with full output
         """
-        asyncio.run(self.aexecute(cmd, cwd, env))
-        return self.output
+        return async_to_sync(self.aexecute)(cmd, cwd, env)
 
 
 class UnhandledExecutor(Executor):
     """
     Class based on :class:`.Executor` but disables `working_handler`.
     """
     __slots__ = ()
```

### Comparing `vstutils-5.6.1/vstutils/web.ini` & `vstutils-5.6.2/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils/wsgi.py` & `vstutils-5.6.2/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils.egg-info/PKG-INFO` & `vstutils-5.6.2/vstutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.6.1
+Version: 5.6.2
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.6.1/vstutils.egg-info/SOURCES.txt` & `vstutils-5.6.2/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.1/vstutils.egg-info/requires.txt` & `vstutils-5.6.2/vstutils.egg-info/requires.txt`

 * *Files identical despite different names*

