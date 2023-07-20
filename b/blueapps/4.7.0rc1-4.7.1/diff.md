# Comparing `tmp/blueapps-4.7.0rc1.tar.gz` & `tmp/blueapps-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blueapps-4.7.0rc1.tar", last modified: Mon May  8 11:22:04 2023, max compression
+gzip compressed data, was "dist/blueapps-4.7.1.tar", last modified: Thu Jul 20 13:34:54 2023, max compression
```

## Comparing `blueapps-4.7.0rc1.tar` & `blueapps-4.7.1.tar`

### file list

```diff
@@ -1,249 +1,221 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/middleware/
--rw-r--r--   0 root         (0) root         (0)      842 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/request_provider.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/middleware/bkui/
--rw-r--r--   0 root         (0) root         (0)     1296 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/bkui/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/bkui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/
--rw-r--r--   0 root         (0) root         (0)     2516 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/decorators.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7918 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/pxfilter.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/utils.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/
--rw-r--r--   0 root         (0) root         (0)     1873 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/base.py
--rw-r--r--   0 root         (0) root         (0)     3778 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/lock.py
--rw-r--r--   0 root         (0) root         (0)     5547 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/request_provider.py
--rw-r--r--   0 root         (0) root         (0)      884 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2887 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/jwt_client.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/time.py
--rw-r--r--   0 root         (0) root         (0)     8333 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/esbclient.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/fancy_dict.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/json.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/unique.py
--rw-r--r--   0 root         (0) root         (0)     3694 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/db.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/local.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)     1432 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/sites/open/
--rw-r--r--   0 root         (0) root         (0)     1337 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/sites/open/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)     1427 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/sites/tencent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/
--rw-r--r--   0 root         (0) root         (0)     1420 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/metric.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/assets/
--rw-r--r--   0 root         (0) root         (0)   169851 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/assets/local_jaeger.png
--rw-r--r--   0 root         (0) root         (0)     3491 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/trace.md
--rw-r--r--   0 root         (0) root         (0)     1859 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/export.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/
--rw-r--r--   0 root         (0) root         (0)     2658 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/instrumentor.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/server.py
--rw-r--r--   0 root         (0) root         (0)     1109 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/celery.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrumentor.py
--rw-r--r--   0 root         (0) root         (0)     4919 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/setup.py
--rw-r--r--   0 root         (0) root         (0)      671 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/README.md
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/apps.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/celery.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/utils.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/metrics.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/
--rw-r--r--   0 root         (0) root         (0)     1409 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/exceptions/
--rw-r--r--   0 root         (0) root         (0)     5628 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/exceptions/base.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/exceptions/middleware.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/handler/
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/handler/wsgi.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/handler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/celery/
--rw-r--r--   0 root         (0) root         (0)      835 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/celery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/celery/celery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/sites/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/sites/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/sites/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/
--rw-r--r--   0 root         (0) root         (0)     5600 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/log.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/database.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/environ.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/validators.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/default_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)      942 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/sites/open/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/sites/open/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)      986 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/sites/tencent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/
--rw-r--r--   0 root         (0) root         (0)     5954 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/base.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/app.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/
--rw-r--r--   0 root         (0) root         (0)     6356 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/
--rw-r--r--   0 root         (0) root         (0)     2489 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/celerybeat.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/celery.py
--rw-r--r--   0 root         (0) root         (0)     7158 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/templates.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      833 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/test.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/test/
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/test/override_middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/dummy/
--rw-r--r--   0 root         (0) root         (0)     1005 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/dummy/dummy_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/dummy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4323 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/serializer_fields.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/filters.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1080 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/authentication.py
--rw-r--r--   0 root         (0) root         (0)     2039 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/pagination.py
--rw-r--r--   0 root         (0) root         (0)     5453 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/serializers.py
--rw-r--r--   0 root         (0) root         (0)     3234 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/viewset_mixin.py
--rw-r--r--   0 root         (0) root         (0)     3505 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/viewsets.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/README.md
--rw-r--r--   0 root         (0) root         (0)     2763 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/renderers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/swagger/
--rw-r--r--   0 root         (0) root         (0)     7127 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/swagger/schemas.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/patch/
--rw-r--r--   0 root         (0) root         (0)     3773 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/patch/log.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/patch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/patch/settings_paas_services.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/patch/settings_open_saas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/
--rw-r--r--   0 root         (0) root         (0)     1046 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/decorators.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/middlewares.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/management/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/management/commands/
--rw-r--r--   0 root         (0) root         (0)     1079 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/management/commands/apigw_clean_cache.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/apps.py
--rw-r--r--   0 root         (0) root         (0)     1287 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/utils/
--rw-r--r--   0 root         (0) root         (0)      940 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/utils/sms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/handlers/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6562 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/handlers/response.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/views.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/static/account/
--rw-r--r--   0 root         (0) root         (0)     2049 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/static/account/login.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/
--rw-r--r--   0 root         (0) root         (0)     3176 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7830 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/models.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/null/
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/null/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/
--rw-r--r--   0 root         (0) root         (0)     3634 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/models.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/forms.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/
--rw-r--r--   0 root         (0) root         (0)     4669 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/backends.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/
--rw-r--r--   0 root         (0) root         (0)     3337 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/backends.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5752 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/
--rw-r--r--   0 root         (0) root         (0)     3668 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4030 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/models.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/forms.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/templates/account/
--rw-r--r--   0 root         (0) root         (0)     1905 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/templates/account/login_page.html
--rw-r--r--   0 root         (0) root         (0)     1355 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/templates/account/login_success.html
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/readme.md
--rw-r--r--   0 root         (0) root         (0)     1249 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/backends.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/conf.py
--rw-r--r--   0 root         (0) root         (0)     8875 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/models.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/migrations/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/0003_verifyinfo.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/0002_init_superuser.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/0004_create_cache_table.py
--rw-r--r--   0 root         (0) root         (0)     7369 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/0001_initial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/ieod/conf.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/sites/open/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/open/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/open/conf.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/tencent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/tencent/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/template/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/template/backends/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/template/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4226 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/template/backends/mako.py
--rw-r--r--   0 root         (0) root         (0)     3260 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/template/context_processors.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     6948 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     4156 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      833 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/test.py
--rw-r--r--   0 root         (0) root         (0)     4038 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/setup.py
--rw-r--r--   0 root         (0) root         (0)     3383 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/README.md
--rw-r--r--   0 root         (0) root         (0)     4156 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7810 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/
+-rw-r--r--   0 root         (0) root         (0)     3383 2023-07-20 13:32:05.000000 blueapps-4.7.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      833 2023-07-20 13:32:05.000000 blueapps-4.7.1/test.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-20 13:32:05.000000 blueapps-4.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4013 2023-07-20 13:32:05.000000 blueapps-4.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/
+-rw-r--r--   0 root         (0) root         (0)      833 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/celerybeat.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/celery.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
+-rw-r--r--   0 root         (0) root         (0)     7158 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/templates.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/handlers/
+-rw-r--r--   0 root         (0) root         (0)     6356 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/bk_commands/management/base.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/middleware/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/middleware/bkui/
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/bkui/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/bkui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/request_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/middleware/xss/
+-rw-r--r--   0 root         (0) root         (0)     7918 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/xss/pxfilter.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/xss/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/xss/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/xss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/middleware/xss/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/opentelemetry/
+-rw-r--r--   0 root         (0) root         (0)     4566 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/instrumentor.py
+-rw-r--r--   0 root         (0) root         (0)      671 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/README.md
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/opentelemetry/docs/
+-rw-r--r--   0 root         (0) root         (0)     3491 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/docs/trace.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/opentelemetry/docs/assets/
+-rw-r--r--   0 root         (0) root         (0)   169851 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/docs/assets/local_jaeger.png
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/docs/metric.md
+-rw-r--r--   0 root         (0) root         (0)     5064 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/setup.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/opentelemetry/instrument_app/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/instrument_app/apps.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/instrument_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/instrument_app/celery.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/opentelemetry/metrics/
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/metrics/instrumentor.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/metrics/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/metrics/server.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/metrics/celery.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/opentelemetry/export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/
+-rw-r--r--   0 root         (0) root         (0)     8875 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/models.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/components/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/components/bk_jwt/
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_jwt/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_jwt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_jwt/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/components/ptlogin/
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/ptlogin/models.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/ptlogin/forms.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/ptlogin/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/ptlogin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/ptlogin/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/components/bk_token/
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_token/models.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_token/forms.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_token/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9552 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_token/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/components/rio/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/rio/forms.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/rio/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/rio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/rio/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/components/weixin/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/weixin/forms.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/weixin/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/weixin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/weixin/backends.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/components/bk_ticket/
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_ticket/models.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_ticket/forms.py
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_ticket/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_ticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/bk_ticket/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/components/null/
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/components/null/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/views.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/admin.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/migrations/
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/migrations/0002_init_superuser.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/migrations/0003_verifyinfo.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/migrations/0004_create_cache_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/templates/account/
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/templates/account/login_page.html
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/templates/account/login_forbidden.html
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/templates/account/login_success.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/utils/
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/utils/sms.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/management/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/management/commands/apigw_clean_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/sites/open/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/sites/open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/sites/open/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/sites/default.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/sites/tencent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/sites/tencent/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/sites/ieod/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/static/account/
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/static/account/login.js
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/account/handlers/
+-rw-r--r--   0 root         (0) root         (0)     6812 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/handlers/response.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/account/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/dummy/
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/dummy/dummy_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/dummy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/patch/
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/patch/settings_open_saas.py
+-rw-r--r--   0 root         (0) root         (0)     3773 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/patch/log.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/patch/settings_paas_services.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/conf/
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/database.py
+-rw-r--r--   0 root         (0) root         (0)     5600 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/log.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/conf/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/conf/sites/open/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/sites/open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/conf/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)      986 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/sites/tencent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/conf/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)      942 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/environ.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/validators.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/conf/default_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/utils/
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/jwt_client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/esbclient.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/unique.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      884 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/utils/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/utils/sites/open/
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/sites/open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/utils/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/sites/tencent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/utils/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/fancy_dict.py
+-rw-r--r--   0 root         (0) root         (0)     4673 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/request_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/core/celery/
+-rw-r--r--   0 root         (0) root         (0)      835 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/celery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/celery/celery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/core/exceptions/
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/exceptions/base.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/exceptions/middleware.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/core/sites/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/sites/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/sites/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/core/handler/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/core/handler/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/template/
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/template/context_processors.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/template/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps/template/backends/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/template/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-07-20 13:32:05.000000 blueapps-4.7.1/blueapps/template/backends/mako.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      933 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     6162 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-07-20 13:34:54.000000 blueapps-4.7.1/blueapps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7810 2023-07-20 13:32:05.000000 blueapps-4.7.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-20 13:34:54.000000 blueapps-4.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-07-20 13:34:54.000000 blueapps-4.7.1/PKG-INFO
```

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/request_provider.py` & `blueapps-4.7.1/blueapps/middleware/request_provider.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/__init__.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/bkui/middlewares.py` & `blueapps-4.7.1/blueapps/middleware/bkui/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/bkui/__init__.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/xss/decorators.py` & `blueapps-4.7.1/blueapps/middleware/xss/decorators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/xss/middlewares.py` & `blueapps-4.7.1/blueapps/middleware/xss/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/xss/__init__.py` & `blueapps-4.7.1/blueapps/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/xss/pxfilter.py` & `blueapps-4.7.1/blueapps/middleware/xss/pxfilter.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/middleware/xss/utils.py` & `blueapps-4.7.1/blueapps/middleware/xss/utils.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/__init__.py` & `blueapps-4.7.1/blueapps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-VERSION = "4.7.0rc1"
+VERSION = "4.7.1"
 __version__ = VERSION
 
 
 RUN_VER = ""
 
 
 def get_run_ver():
```

### Comparing `blueapps-4.7.0rc1/blueapps/utils/base.py` & `blueapps-4.7.1/blueapps/account/utils/sms.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,61 +6,44 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
-import hashlib
-import traceback
-from collections import namedtuple
-from contextlib import contextmanager
 
-from blueapps.utils.logger import logger
+from blueapps.account.conf import ConfFixture
+from blueapps.utils import client
+from blueapps.utils.esbclient import CustomComponentAPI
 
 
-@contextmanager
-def ignored(*exceptions, **kwargs):
-    """
-    在忽略某异常下执行
-    example:
-        with ignored(Exception):
-            # 不会抛出异常
-            print(1/0)
-    """
-    try:
-        yield
-    except exceptions:
-        if kwargs.get("log_exception", True):
-            logger.warning(traceback.format_exc())
+"""
+发送短信工具文件，开发者可以直接调用此处的send_sms函数，屏蔽环境之间的差异
+"""
 
 
-def dict_to_namedtuple(dic):
+def send_sms(user_list, content):
     """
-    从dict转换到namedtuple
+    发送短信给指定的用户，
+    :param user_list: 用户列表，list
+    :param content: 消息内容
+    :return: True | raise Exception
     """
-    return namedtuple("AttrStore", list(dic.keys()))(**dic)
 
+    # 1. 获取发送短信的函数实际句柄
+    sms_module = client.__getattr__(ConfFixture.SMS_CLIENT_MODULE)
+    sms_func = sms_module.__getattr__(ConfFixture.SMS_CLIENT_FUNC)
 
-def choices_to_namedtuple(choices):
-    """
-    从django-model的choices转换到namedtuple
-    """
-    return dict_to_namedtuple(dict(choices))
+    # 2. 拼接发送函数的内容
+    request_args = {
+        ConfFixture.SMS_CLIENT_USER_ARGS_NAME: ",".join(user_list),
+        ConfFixture.SMS_CLIENT_CONTENT_ARGS_NAME: content,
+    }
 
+    # 3. 发送短信
+    if type(sms_func) == CustomComponentAPI:
+        result = sms_func.post(request_args)
 
-def tuple_choices(tupl):
-    """
-    从django-model的choices转换到namedtuple
-    """
-    return [(t, t) for t in tupl]
-
+    else:
+        result = sms_func(request_args)
 
-def md5_sum(src_str: str):
-    """
-    计算md5_sum值
-    @param src_str {str} 源字符串
-    """
-    md5 = hashlib.md5()
-    md5.update(src_str.encode("utf-8"))
-    md5_key = md5.hexdigest()
-    return md5_key
+    return result
```

### Comparing `blueapps-4.7.0rc1/blueapps/utils/request_provider.py` & `blueapps-4.7.1/blueapps/utils/request_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,20 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
-import sys
-import uuid
 
 from django.dispatch import Signal
 from django.utils.deprecation import MiddlewareMixin
 
 from blueapps.conf import settings
 from blueapps.core.exceptions import AccessForbidden, ServerBlueException
-from blueapps.settings import blueapps_settings
-from blueapps.utils.local import inject_request_id, release_request_local, request_local
 
 # since each thread has its own greenlet we can just use those as identifiers
 # for the context.  If greenlets are not available we fall back to the
 # current thread ident depending on where it is.
 try:
     from greenlet import getcurrent as get_ident
 except ImportError:
@@ -36,15 +32,17 @@
 class AccessorSignal(Signal):
     allowed_receiver = "blueapps.utils.request_provider.RequestProvider"
 
     def __init__(self, providing_args=None):
         Signal.__init__(self, providing_args)
 
     def connect(self, receiver, sender=None, weak=True, dispatch_uid=None):
-        receiver_name = ".".join([receiver.__class__.__module__, receiver.__class__.__name__])
+        receiver_name = ".".join(
+            [receiver.__class__.__module__, receiver.__class__.__name__]
+        )
         if receiver_name != self.allowed_receiver:
             raise AccessForbidden(u"%s is not allowed to connect" % receiver_name)
         Signal.connect(self, receiver, sender, weak, dispatch_uid)
 
 
 request_accessor = AccessorSignal()
 
@@ -63,15 +61,17 @@
 
     def __init__(self, get_response):
         super(RequestProvider, self).__init__(get_response)
         self._request_pool = {}
         request_accessor.connect(self)
 
     def process_request(self, request):
-        request.is_mobile = lambda: bool(settings.RE_MOBILE.search(request.META.get("HTTP_USER_AGENT", "")))
+        request.is_mobile = lambda: bool(
+            settings.RE_MOBILE.search(request.META.get("HTTP_USER_AGENT", ""))
+        )
 
         # 是否为合法的RIO请求
         request.is_rio = lambda: bool(
             request.META.get("HTTP_STAFFNAME", "")
             and getattr(settings, "RIO_TOKEN", None)
             and settings.RE_WECHAT.search(request.META.get("HTTP_USER_AGENT", ""))
         )
@@ -84,21 +84,18 @@
             and not request.is_rio()
         )
 
         # JWT请求
         request.is_bk_jwt = lambda: bool(request.META.get("HTTP_X_BKAPI_JWT", ""))
 
         self._request_pool[get_ident()] = request
-        request_local.request = request
-        inject_request_id(request_local, request)
         return None
 
     def process_response(self, request, response):
         assert request is self._request_pool.pop(get_ident())
-        release_request_local()
         return response
 
     def __call__(self, *args, **kwargs):
         """
         1）接受 signal 请求响应，
         2）继承 MiddlewareMixin.__call__ 兼容 djagno 1.10 之前中间件
         """
@@ -122,34 +119,11 @@
 
 
 def get_x_request_id():
     x_request_id = ""
     http_request = get_request()
     if hasattr(http_request, "META"):
         meta = http_request.META
-        x_request_id = meta.get("HTTP_X_REQUEST_ID", "") if isinstance(meta, dict) else ""
+        x_request_id = (
+            meta.get("HTTP_X_REQUEST_ID", "") if isinstance(meta, dict) else ""
+        )
     return x_request_id
-
-
-def get_local_request():
-    return getattr(request_local, "request", None)
-
-
-def get_local_request_id():
-    return getattr(request_local, "request_id", str(uuid.uuid4()))
-
-
-def get_or_create_local_request_id():
-    if not hasattr(request_local, "request_id"):
-        request_local.request_id = str(uuid.uuid4())
-    return request_local.request_id
-
-
-def get_request_username():
-    operator = None
-    try:
-        operator = get_local_request().user.username
-    except (IndexError, AttributeError):
-        if blueapps_settings.NON_REQUEST_USERNAME_PROVIDER:
-            operator = blueapps_settings.NON_REQUEST_USERNAME_PROVIDER()
-
-    return operator
```

### Comparing `blueapps-4.7.0rc1/blueapps/utils/logger.py` & `blueapps-4.7.1/blueapps/utils/logger.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/__init__.py` & `blueapps-4.7.1/blueapps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/jwt_client.py` & `blueapps-4.7.1/blueapps/utils/jwt_client.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/tools.py` & `blueapps-4.7.1/blueapps/utils/tools.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/esbclient.py` & `blueapps-4.7.1/blueapps/utils/esbclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
 
 try:
     client = SDKClient()
     backend_client = SDKClient  # pylint: disable=invalid-name
     client.patch_sdk_component_api_class()
 except ImportError as err:
-    from blueapps.contrib.dummy.dummy_client import DummyClient
+    from blueapps.dummy.dummy_client import DummyClient
 
     client = DummyClient(err)
     backend_client = DummyClient  # pylint: disable=invalid-name
 
 
 def get_client_by_user(user_or_username):
     user_model = get_user_model()
```

### Comparing `blueapps-4.7.0rc1/blueapps/utils/fancy_dict.py` & `blueapps-4.7.1/blueapps/utils/fancy_dict.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/unique.py` & `blueapps-4.7.1/blueapps/utils/unique.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/sites/ieod/__init__.py` & `blueapps-4.7.1/blueapps/utils/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/sites/__init__.py` & `blueapps-4.7.1/blueapps/middleware/bkui/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/sites/open/__init__.py` & `blueapps-4.7.1/blueapps/utils/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/utils/sites/tencent/__init__.py` & `blueapps-4.7.1/blueapps/utils/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/docs/metric.md` & `blueapps-4.7.1/blueapps/opentelemetry/docs/metric.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/docs/assets/local_jaeger.png` & `blueapps-4.7.1/blueapps/opentelemetry/docs/assets/local_jaeger.png`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/docs/trace.md` & `blueapps-4.7.1/blueapps/opentelemetry/docs/trace.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/export.py` & `blueapps-4.7.1/blueapps/opentelemetry/export.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/middlewares.py` & `blueapps-4.7.1/blueapps/opentelemetry/metrics/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/__init__.py` & `blueapps-4.7.1/blueapps/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/instrumentor.py` & `blueapps-4.7.1/blueapps/opentelemetry/metrics/instrumentor.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/server.py` & `blueapps-4.7.1/blueapps/opentelemetry/metrics/server.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/celery.py` & `blueapps-4.7.1/blueapps/opentelemetry/metrics/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/__init__.py` & `blueapps-4.7.1/blueapps/middleware/xss/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/instrumentor.py` & `blueapps-4.7.1/blueapps/opentelemetry/instrumentor.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 import json
+
 from typing import Collection
 
+from django.conf import settings
+
+from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation import dbapi
+from opentelemetry.trace import Span, Status, StatusCode, format_trace_id
 from opentelemetry.instrumentation.celery import CeleryInstrumentor
 from opentelemetry.instrumentation.django import DjangoInstrumentor
-from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 from opentelemetry.instrumentation.redis import RedisInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
-from opentelemetry.trace import Span, Status, StatusCode, format_trace_id
-from requests import Response
-
-from blueapps.settings import blueapps_settings
 
 
-def requests_callback(span: Span, response: Response):
+def requests_callback(span: Span, response):
     """
     处理蓝鲸标准协议响应
     """
     try:
         json_result = response.json()
     except Exception:  # pylint: disable=broad-except
         return
@@ -59,15 +59,18 @@
         or response.headers.get("x-request-id")
         # old esb
         or json_result.get("request_id", "")
     )
     if request_id:
         span.set_attribute("request_id", request_id)
 
-    span.set_status(Status(StatusCode.OK if response.ok else StatusCode.ERROR))
+    if code in [0, "0", "00"]:
+        span.set_status(Status(StatusCode.OK))
+    else:
+        span.set_status(Status(StatusCode.ERROR))
 
 
 def django_request_hook(span, request):
     """
     在request注入trace_id，方便获取
     """
     trace_id = span.get_span_context().trace_id
@@ -104,22 +107,18 @@
     def _instrument(self, **kwargs):
         LoggingInstrumentor().instrument()
         RequestsInstrumentor().instrument(span_callback=requests_callback)
         DjangoInstrumentor().instrument(request_hook=django_request_hook, response_hook=django_response_hook)
         CeleryInstrumentor().instrument()
         RedisInstrumentor().instrument()
 
-        for instrumentor in blueapps_settings.BK_APP_OTEL_ADDTIONAL_INSTRUMENTORS or getattr(
-            blueapps_settings, "BK_APP_OTEL_ADDTIONAL_INSTRUMENTORS", []
-        ):
+        for instrumentor in getattr(settings, "BK_APP_OTEL_ADDTIONAL_INSTRUMENTORS", []):
             instrumentor.instrument()
 
-        if blueapps_settings.BKAPP_OTEL_INSTRUMENT_DB_API or getattr(
-            blueapps_settings, "BK_APP_OTEL_INSTRUMENT_DB_API", False
-        ):
+        if getattr(settings, "BK_APP_OTEL_INSTRUMENT_DB_API", False):
             import MySQLdb  # noqa
 
             dbapi.wrap_connect(
                 __name__,
                 MySQLdb,
                 "connect",
                 "mysql",
```

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/setup.py` & `blueapps-4.7.1/blueapps/opentelemetry/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,46 +11,42 @@
 specific language governing permissions and limitations under the License.
 """
 
 import os
 
 from django.conf import settings
 from django.utils.log import configure_logging
+
 from opentelemetry import trace
-from opentelemetry.exporter.jaeger.thrift import JaegerExporter
-from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
-from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import TracerProvider
+from opentelemetry.sdk.resources import Resource, SERVICE_NAME
 from opentelemetry.sdk.trace.sampling import _KNOWN_SAMPLERS
+from opentelemetry.exporter.jaeger.thrift import JaegerExporter
+from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 
 from blueapps.core.celery import celery_app
-from blueapps.opentelemetry.constants import DEFAULT_LOGGING_TRACE_FORMAT
 from blueapps.opentelemetry.instrumentor import BKAppInstrumentor
 from blueapps.opentelemetry.metrics.celery import MetricsServerStep
 from blueapps.opentelemetry.metrics.instrumentor import SaaSMetricsInstrumentor
+from blueapps.opentelemetry.constants import DEFAULT_LOGGING_TRACE_FORMAT
 from blueapps.opentelemetry.utils import inject_logging_trace_info
-from blueapps.settings import blueapps_settings
 from blueapps.opentelemetry.export import LazyBatchSpanProcessor
 
 
 def setup_trace_config(
-    service_name: str,
-    bk_data_id: int,
-    otel_sampler: str,
-    otel_grpc_host: str,
-    bk_data_token: str = "",
+    service_name: str, bk_data_id: int, otel_sampler: str, otel_grpc_host: str, bk_data_token: str = "",
 ):
     span_processor = getattr(settings, "BLUEAPPS_BKAPP_OTEL_SPAN_PROCESSOR", LazyBatchSpanProcessor)
-    service_name_handler = blueapps_settings.BKAPP_OTEL_SERVICE_NAME_HANDLER
-    service_name = service_name_handler(service_name).get_service_name()
     if settings.ENVIRONMENT == "dev":
         # local environment, use jaeger as trace service
         # docker run -p 16686:16686 -p 6831:6831/udp jaegertracing/all-in-one
         trace.set_tracer_provider(TracerProvider(resource=Resource.create({SERVICE_NAME: service_name})))
-        jaeger_exporter = JaegerExporter(agent_host_name="localhost", agent_port=6831, udp_split_oversized_batches=True)
+        jaeger_exporter = JaegerExporter(
+            agent_host_name="localhost", agent_port=6831, udp_split_oversized_batches=True,
+        )
         trace.get_tracer_provider().add_span_processor(span_processor(jaeger_exporter))
     else:
         # stage and prod environment, use bk_log as trace service
         trace.set_tracer_provider(
             tracer_provider=TracerProvider(
                 resource=Resource.create(
                     {"service.name": service_name, "bk_data_id": bk_data_id, "bk.data.token": bk_data_token},
@@ -61,32 +57,47 @@
         otlp_exporter = OTLPSpanExporter(endpoint=otel_grpc_host)
         span_processor = span_processor(otlp_exporter)
         trace.get_tracer_provider().add_span_processor(span_processor)
 
 
 def setup_by_settings():
     enable_paas_otel = True if getattr(settings, "OTEL_BK_DATA_TOKEN", "") else False
-    enable_trace = os.getenv("ENABLE_TRACE", enable_paas_otel) or blueapps_settings.ENABLE_OTEL_TRACE
+    enable_trace = os.getenv("ENABLE_TRACE", enable_paas_otel) or getattr(
+        settings, "ENABLE_OTEL_TRACE", enable_paas_otel
+    )
     if enable_trace:
         app_module_name = getattr(settings, "APP_MODULE_NAME", "")
         service_name = (
             os.getenv("BKAPP_OTEL_SERVICE_NAME")
             or getattr(settings, "BKAPP_OTEL_SERVICE_NAME", None)
             or (settings.APP_CODE + f"-{app_module_name}" if app_module_name else "")
         )
-        bk_data_id = int(os.getenv("BKAPP_OTEL_BK_DATA_ID") or blueapps_settings.BKAPP_OTEL_BK_DATA_ID)
-        otel_sampler = os.getenv("BKAPP_OTEL_SAMPLER") or blueapps_settings.BKAPP_OTEL_SAMPLER
-        otel_grpc_host = os.getenv("BKAPP_OTEL_GRPC_HOST") or blueapps_settings.BKAPP_OTEL_GRPC_HOST
-        otel_bk_data_token = os.getenv("BKAPP_OTEL_BK_DATA_TOKEN") or blueapps_settings.BKAPP_OTEL_BK_DATA_TOKEN
-        setup_trace_config(service_name, bk_data_id, otel_sampler, otel_grpc_host, bk_data_token=otel_bk_data_token)
+        bk_data_id = int(os.getenv("BKAPP_OTEL_BK_DATA_ID") or getattr(settings, "BKAPP_OTEL_BK_DATA_ID", -1))
+        otel_sampler = (
+            os.getenv("BKAPP_OTEL_SAMPLER")
+            or getattr(settings, "BKAPP_OTEL_SAMPLER", None)
+            or getattr(settings, "OTEL_SAMPLER", None)
+            or "parentbased_always_off"
+        )
+        otel_grpc_host = (
+            os.getenv("BKAPP_OTEL_GRPC_HOST")
+            or getattr(settings, "BKAPP_OTEL_GRPC_HOST", None)
+            or getattr(settings, "OTEL_GRPC_HOST", None)
+        )
+        otel_bk_data_token = (
+            os.getenv("BKAPP_OTEL_BK_DATA_TOKEN")
+            or getattr(settings, "BKAPP_OTEL_BK_DATA_TOKEN", "")
+            or getattr(settings, "OTEL_BK_DATA_TOKEN", "")
+        )
+        setup_trace_config(
+            service_name, bk_data_id, otel_sampler, otel_grpc_host, bk_data_token=otel_bk_data_token,
+        )
         BKAppInstrumentor().instrument()
         # 将Trace信息配置到项目日志中
-        trace_format = blueapps_settings.BKAPP_OTEL_LOGGING_TRACE_FORMAT or getattr(
-            blueapps_settings, "OTEL_LOGGING_TRACE_FORMAT", DEFAULT_LOGGING_TRACE_FORMAT
-        )
+        trace_format = getattr(settings, "OTEL_LOGGING_TRACE_FORMAT", DEFAULT_LOGGING_TRACE_FORMAT)
         inject_logging_trace_info(settings.LOGGING, ("verbose",), trace_format)
         configure_logging(settings.LOGGING_CONFIG, settings.LOGGING)
     # metrics
-    enable_metrics = os.getenv("ENABLE_METRICS") or blueapps_settings.ENABLE_OTEL_METRICS
+    enable_metrics = os.getenv("ENABLE_METRICS") or getattr(settings, "ENABLE_OTEL_METRICS", False)
     if enable_metrics:
         SaaSMetricsInstrumentor().instrument()
         celery_app.steps["worker"].add(MetricsServerStep)
```

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/README.md` & `blueapps-4.7.1/blueapps/opentelemetry/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/constants.py` & `blueapps-4.7.1/blueapps/opentelemetry/constants.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/apps.py` & `blueapps-4.7.1/blueapps/opentelemetry/instrument_app/apps.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/__init__.py` & `blueapps-4.7.1/blueapps/opentelemetry/instrument_app/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/celery.py` & `blueapps-4.7.1/blueapps/opentelemetry/instrument_app/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/metrics.py` & `blueapps-4.7.1/blueapps/metrics.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/wsgi.py` & `blueapps-4.7.1/blueapps/core/wsgi.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/exceptions/__init__.py` & `blueapps-4.7.1/blueapps/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/exceptions/middleware.py` & `blueapps-4.7.1/blueapps/core/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/__init__.py` & `blueapps-4.7.1/blueapps/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/handler/wsgi.py` & `blueapps-4.7.1/blueapps/core/handler/wsgi.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/handler/__init__.py` & `blueapps-4.7.1/blueapps/opentelemetry/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/celery/__init__.py` & `blueapps-4.7.1/blueapps/core/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/celery/celery.py` & `blueapps-4.7.1/blueapps/core/celery/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/sites/__init__.py` & `blueapps-4.7.1/blueapps/account/components/bk_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/core/sites/middleware.py` & `blueapps-4.7.1/blueapps/core/sites/middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/log.py` & `blueapps-4.7.1/blueapps/conf/log.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/__init__.py` & `blueapps-4.7.1/blueapps/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/database.py` & `blueapps-4.7.1/blueapps/conf/database.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/environ.py` & `blueapps-4.7.1/blueapps/conf/environ.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/validators.py` & `blueapps-4.7.1/blueapps/conf/validators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/default_settings.py` & `blueapps-4.7.1/blueapps/conf/default_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     "whitenoise.middleware.WhiteNoiseMiddleware",
     # Auth middleware
     "blueapps.account.middlewares.RioLoginRequiredMiddleware",
     "blueapps.account.middlewares.WeixinLoginRequiredMiddleware",
     "blueapps.account.middlewares.LoginRequiredMiddleware",
     # exception middleware
     "blueapps.core.exceptions.middleware.AppExceptionMiddleware",
+    # django国际化中间件
     "django.middleware.locale.LocaleMiddleware",
 )
 
 DATABASES = {"default": get_default_database_config_dict(locals())}
 
 # Cache
```

### Comparing `blueapps-4.7.0rc1/blueapps/conf/sites/ieod/__init__.py` & `blueapps-4.7.1/blueapps/conf/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/sites/__init__.py` & `blueapps-4.7.1/blueapps/account/components/ptlogin/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/sites/open/__init__.py` & `blueapps-4.7.1/blueapps/account/components/bk_token/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/conf/sites/tencent/__init__.py` & `blueapps-4.7.1/blueapps/conf/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/base.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/base.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/app.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/app.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/__init__.py` & `blueapps-4.7.1/blueapps/account/components/rio/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/__init__.py` & `blueapps-4.7.1/blueapps/account/components/weixin/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/__init__.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/celerybeat.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/celerybeat.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/celery.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/templates.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/management/templates.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/__init__.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/test.py` & `blueapps-4.7.1/test.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/__init__.py` & `blueapps-4.7.1/blueapps/account/components/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/test/override_middleware.py` & `blueapps-4.7.1/blueapps/account/components/null/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 Tencent is pleased to support the open source community by making 蓝鲸智云PaaS平台社区版 (BlueKing PaaS Community
 Edition) available.
-Copyright (C) 2017-2022 THL A29 Limited, a Tencent company. All rights reserved.
+Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
-from django.utils.deprecation import MiddlewareMixin
-
 
-class OverrideMiddleware(MiddlewareMixin):
-    """
-    用于跳过登录验证的中间件
-    """
+from django.utils.deprecation import MiddlewareMixin
 
-    def process_request(self, request):
-        class Base(object):
-            pass
 
-        request.user = Base()
-        request.source = "WEB"
-        request.user.username = "admin"
-        request.user.is_superuser = True
-        request.user.is_authenticated = True
-        request.user.is_active = True
+class NullMiddleware(MiddlewareMixin):
+    pass
 
-        request.session = {"bluking_timezone": "Asia/Shanghai"}
 
-        request.permission_exempt = True
-        request.META.update({"HTTP_X_REQUESTED_WITH": "XMLHttpRequest"})
+class NullBackend(object):
+    def authenticate(self, **kwargs):
+        return None
```

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/dummy/dummy_client.py` & `blueapps-4.7.1/blueapps/dummy/dummy_client.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/drf/__init__.py` & `blueapps-4.7.1/blueapps/account/components/bk_ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/__init__.py` & `blueapps-4.7.1/blueapps/account/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/authentication.py` & `blueapps-4.7.1/blueapps/account/migrations/0004_create_cache_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,26 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
-from rest_framework.authentication import SessionAuthentication
 
+from django.core.management import call_command
+from django.db import migrations
 
-class CsrfExemptSessionAuthentication(SessionAuthentication):
+
+def create_cache_table(apps, schema_editor):
     """
-    免除csrf认证
+    创建 cache table
     """
+    call_command("createcachetable", "account_cache")
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ("account", "0003_verifyinfo"),
+    ]
 
-    def enforce_csrf(self, request):  # pylint: disable=no-self-use,unused-argument
-        """To not perform the csrf check previously happening"""
-        return
+    operations = [migrations.RunPython(create_cache_table)]
```

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/drf/renderers.py` & `blueapps-4.7.1/blueapps/account/apps.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,66 +6,65 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
-from rest_framework import status
-from rest_framework.renderers import JSONRenderer
-from rest_framework.status import is_success
-
-from blueapps.utils.request_provider import get_or_create_local_request_id
-
-
-class APIRenderer(JSONRenderer):
-    """
-    统一的结构封装返回内容
-    """
-
-    SUCCESS_CODE = 0
-
-    def render(self, data, accepted_media_type=None, renderer_context=None):
-        """
-        统一处理返回数据
-        """
-        response = renderer_context["response"]
-        req_id = get_or_create_local_request_id()
-
-        res_data = {
-            "result": True,
-            "code": self.SUCCESS_CODE,
-            "data": None,
-            "message": None,
-            "request_id": req_id,
-            "trace_id": getattr(renderer_context.get("request"), "otel_trace_id", None),
-        }
-
-        if is_success(response.status_code):
-            response.status_code = status.HTTP_200_OK
-            res_data["data"] = data
-            res_data["code"] = self.SUCCESS_CODE
-            return super(APIRenderer, self).render(res_data, accepted_media_type, renderer_context)
-
-        code = response.status_code
-        message = response.data
-        errors = response.data
-        if isinstance(response.data, dict) and "code" in response.data:
-            code = response.data["code"]
-            message = self.pretty_dict(response.data["message"])
-            errors = response.data["data"]
-
-        res_data.update({"result": False, "code": code, "message": message, "errors": errors})
-
-        return super(APIRenderer, self).render(res_data, accepted_media_type, renderer_context)
-
-    def pretty_dict(self, dict_data):  # pylint: disable=no-self-use
-        """
-        将字典转为字符串返回
-        格式: {key}: {value}
-        """
-        if not isinstance(dict_data, dict) or not dict_data:
-            return dict_data
-        res = []
-        for key, value in dict_data.items():
-            res.append(f"{key}: {value}")
-        return "; ".join(res)
+
+from django.apps import AppConfig
+from django.utils.translation import ugettext_lazy as _
+from django.conf import settings
+from django.core.cache import caches
+
+from blueapps.account.conf import APIGW_CACHE_KEY, APIGW_CACHE_EXPIRES
+
+cache = caches["login_db"]
+
+
+class AccountConfig(AppConfig):
+    default_auto_field = "django.db.models.AutoField"
+    name = "blueapps.account"
+    verbose_name = _("account")
+
+    def ready(self):
+        self.get_api_public_key()
+        return True
+
+    @staticmethod
+    def get_api_public_key():
+        # return if APIGW_ENABLED is not set
+        if not hasattr(settings, "APIGW_ENABLED") or not bool(settings.APIGW_ENABLED):
+            return
+
+        # return if public key is configured
+        if hasattr(settings, "APIGW_PUBLIC_KEY"):
+            return
+
+        # get api key by cache
+        from blueapps.utils.logger import logger  # noqa
+
+        api_public_key = cache.get(APIGW_CACHE_KEY)
+        if api_public_key:
+            message = "[ESB][JWT]get esb api public key success (from cache)"
+            print(message, flush=True)
+            logger.info(message)
+            settings.APIGW_PUBLIC_KEY = api_public_key
+            return api_public_key
+
+        # get api key by api
+        from blueapps.utils import get_client_by_user  # noqa
+
+        client = get_client_by_user(getattr(settings, "APIGW_API_ACCOUNT", "admin"))
+        esb_result = client.esb.get_api_public_key()
+        if esb_result["result"]:
+            api_public_key = esb_result["data"]["public_key"]
+            settings.APIGW_PUBLIC_KEY = api_public_key
+            cache.set(APIGW_CACHE_KEY, api_public_key, APIGW_CACHE_EXPIRES)
+            message = "[ESB][JWT]get esb api public key success (from realtime api)"
+            print(message, flush=True)
+            logger.info(message)
+        else:
+            message = f'[ESB][JWT]get esb api public key error:{esb_result["message"]}'
+            print(message, flush=True)
+            logger.warning(message)
+            raise Exception(message)
```

### Comparing `blueapps-4.7.0rc1/blueapps/contrib/drf/exception.py` & `blueapps-4.7.1/blueapps/account/components/bk_jwt/middlewares.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,60 +6,56 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
-import json
-from json.decoder import JSONDecodeError
 
-from rest_framework import status
-from rest_framework.response import Response
-from rest_framework.views import exception_handler
-
-from blueapps.core.exceptions import BlueException
-from blueapps.utils.logger import logger
-
-
-def custom_exception_handler(exc, context):
-    """
-    分类：
-        APIException及子类异常
-        app自定义异常和未处理异常
-    """
-    response = exception_handler(exc, context)
-    if response:
-        return Response(
-            response.data["detail"] if "detail" in response.data else response.data, status=response.status_code,
-        )
-
-    exc_message = str(exc)
-    exc_data = None
-    if hasattr(exc, "data") and exc.data:
-        try:
-            exc_data = json.loads(exc.data)
-        except JSONDecodeError:
-            exc_data = exc.data
-        except TypeError:
-            # 其它内容不能被json解析 忽略
-            pass
-
-    if hasattr(exc, "message") and exc.message:
-        try:
-            exc_message = json.loads(str(exc.message))
-        except JSONDecodeError:
-            exc_message = str(exc.message)
-
-    code = status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
-    if isinstance(exc, BlueException):
-        code = exc.code
-        status_code = exc.STATUS_CODE
-
-    data = {
-        "code":  code,
-        "message": exc_message,
-        "data": exc_data,
-    }
-    # 使用json方便提取
-    logger.exception(json.dumps({"code": data["code"], "message": data["message"], "data": data["data"]}))
-    return Response(data, status=status_code)
+import logging
+
+from django.conf import settings
+from django.contrib import auth
+from django.utils.deprecation import MiddlewareMixin
+
+from blueapps.account.conf import ConfFixture
+from blueapps.account.handlers.response import ResponseHandler
+
+logger = logging.getLogger("component")
+
+
+class BkJwtLoginRequiredMiddleware(MiddlewareMixin):
+    def process_view(self, request, view, args, kwargs):
+        """
+        可通过登录认证的请求：
+        1. 带有BK JWT HEADER
+        2. JWT签名正确
+        """
+        # 框架前置中间件，已将识别的客户端信息填充进 request
+        if not hasattr(request, "is_bk_jwt") or not request.is_bk_jwt():
+            return None
+
+        logger.debug("当前请求是否经过JWT转发")
+        login_exempt = getattr(view, "login_exempt", False)
+
+        if login_exempt or request.user.is_authenticated:
+            return None
+
+        # 每次请求都需要做校验
+        user = self.authenticate(request)
+        if user:
+            return None
+
+        handler = ResponseHandler(ConfFixture, settings)
+        return handler.build_bk_jwt_401_response(request)
+
+    def process_response(self, request, response):
+        return response
+
+    def authenticate(self, request):
+        user = auth.authenticate(request=request)
+        if user and user.username != request.user.username:
+            auth.login(request, user)
+        if request.user.is_authenticated:
+            # 登录成功，确认登陆正常后退出
+            return request.user
+        return user
```

### Comparing `blueapps-4.7.0rc1/blueapps/patch/log.py` & `blueapps-4.7.1/blueapps/patch/log.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/patch/__init__.py` & `blueapps-4.7.1/blueapps/account/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/patch/settings_paas_services.py` & `blueapps-4.7.1/blueapps/patch/settings_paas_services.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/patch/settings_open_saas.py` & `blueapps-4.7.1/blueapps/patch/settings_open_saas.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/decorators.py` & `blueapps-4.7.1/blueapps/account/decorators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/middlewares.py` & `blueapps-4.7.1/blueapps/account/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/management/__init__.py` & `blueapps-4.7.1/blueapps/account/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/management/commands/apigw_clean_cache.py` & `blueapps-4.7.1/blueapps/account/management/commands/apigw_clean_cache.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/management/commands/__init__.py` & `blueapps-4.7.1/blueapps/account/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/__init__.py` & `blueapps-4.7.1/blueapps/account/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/utils/__init__.py` & `blueapps-4.7.1/blueapps/account/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/utils/http.py` & `blueapps-4.7.1/blueapps/account/utils/http.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/utils/sms.py` & `blueapps-4.7.1/blueapps/account/migrations/0002_init_superuser.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,43 +7,26 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-from blueapps.account.conf import ConfFixture
-from blueapps.utils import client
-from blueapps.utils.esbclient import CustomComponentAPI
+from django.conf import settings
+from django.db import migrations
 
 
-"""
-发送短信工具文件，开发者可以直接调用此处的send_sms函数，屏蔽环境之间的差异
-"""
-
-
-def send_sms(user_list, content):
+def load_data(apps, schema_editor):
     """
-    发送短信给指定的用户，
-    :param user_list: 用户列表，list
-    :param content: 消息内容
-    :return: True | raise Exception
+    添加用户为管理员
     """
+    User = apps.get_model("account", "User")
+    for name in settings.INIT_SUPERUSER:
+        User.objects.update_or_create(
+            username=name,
+            defaults={"is_staff": True, "is_active": True, "is_superuser": True},
+        )
 
-    # 1. 获取发送短信的函数实际句柄
-    sms_module = client.__getattr__(ConfFixture.SMS_CLIENT_MODULE)
-    sms_func = sms_module.__getattr__(ConfFixture.SMS_CLIENT_FUNC)
-
-    # 2. 拼接发送函数的内容
-    request_args = {
-        ConfFixture.SMS_CLIENT_USER_ARGS_NAME: ",".join(user_list),
-        ConfFixture.SMS_CLIENT_CONTENT_ARGS_NAME: content,
-    }
-
-    # 3. 发送短信
-    if type(sms_func) == CustomComponentAPI:
-        result = sms_func.post(request_args)
-
-    else:
-        result = sms_func(request_args)
 
-    return result
+class Migration(migrations.Migration):
+    dependencies = [("account", "0001_initial")]
+    operations = [migrations.RunPython(load_data)]
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/handlers/__init__.py` & `blueapps-4.7.1/blueapps/account/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/handlers/response.py` & `blueapps-4.7.1/blueapps/account/handlers/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
+from urllib.parse import urlencode
 
+from django.conf import settings
 from django.http import HttpResponseRedirect, JsonResponse
 from django.utils.translation import ugettext_lazy as _
 
 from blueapps.account.utils.http import build_redirect_url
 from blueapps.core.exceptions import BkJwtVerifyError, RioVerifyError
-from blueapps.settings import blueapps_settings
 from blueapps.utils.tools import resolve_login_url
 
 try:
     from django.urls import reverse
 except Exception:  # pylint: disable=broad-except
     from django.core.urlresolvers import reverse
 
@@ -30,18 +31,21 @@
         """
         @param {object} confFixture Account Package Settings
         @param {object} settings Django User Settings
         """
         self._conf = _confFixture
         self._settings = _settings
 
+    def build_403_response(self, msg):
+        return HttpResponseRedirect(f'{reverse("account:login_forbidden")}?{urlencode({"hint_msg": msg})}')
+
     def build_401_response(self, request):
 
         # 强制要求进行跳转的方式
-        if blueapps_settings.IS_AJAX_PLAIN_MODE and request.is_ajax():
+        if getattr(settings, "IS_AJAX_PLAIN_MODE", False) and request.is_ajax():
             return self._build_ajax_401_response(request)
 
         # Just redirect to PAAS-LOGIN-PLATRORM no matter whether request.is_ajax
         if self._conf.HAS_PLAIN:
             if request.is_ajax():
                 return self._build_ajax_401_response(request)
             else:
@@ -55,16 +59,16 @@
 
     def _build_ajax_401_response(self, request):
         """
         Return 401 info, inlclude login_url to PAAS-LOGIN-PLATFORM,
         width & height for adjusting iframe window, login_url as
         http://xxx/login/?c_url=http%3A//xxx/t/data/&app_id=data
         """
-        if blueapps_settings.AJAX_401_RESPONSE_FUNC:
-            return blueapps_settings.AJAX_401_RESPONSE_FUNC(request)
+        if hasattr(settings, "BLUEAPPS_AJAX_401_RESPONSE_FUNC"):
+            return settings.BLUEAPPS_AJAX_401_RESPONSE_FUNC(request)
         _next = request.build_absolute_uri(reverse("account:login_success"))
 
         if self._conf.ADD_CROSS_PREFIX:
             _next = self._conf.CROSS_PREFIX + _next
 
         _login_url = build_redirect_url(
             _next,
@@ -83,36 +87,36 @@
         return JsonResponse(context, status=401)
 
     def _build_page_401_response(self, request):
         """
         Redirect to login page in self app, redirect url format as
         http://xxx:8000/account/login_page/?refer_url=http%3A//xxx%3A8000/
         """
-        if blueapps_settings.PAGE_401_RESPONSE_FUNC:
-            return blueapps_settings.PAGE_401_RESPONSE_FUNC(request)
+        if hasattr(settings, "BLUEAPPS_PAGE_401_RESPONSE_FUNC"):
+            return settings.BLUEAPPS_PAGE_401_RESPONSE_FUNC(request)
         _next = request.build_absolute_uri()
-        if request.method == "GET" and blueapps_settings.SPECIFIC_REDIRECT_KEY:
-            _next = request.GET.get(blueapps_settings.SPECIFIC_REDIRECT_KEY) or _next
+        if request.method == "GET" and hasattr(settings, "BLUEAPPS_SPECIFIC_REDIRECT_KEY"):
+            _next = request.GET.get(settings.BLUEAPPS_SPECIFIC_REDIRECT_KEY) or _next
         _redirect = build_redirect_url(
             _next,
             resolve_login_url(self._conf.LOGIN_PLAIN_URL, request),
             self._conf.C_URL,
             extra_args=self._build_extra_args(),
         )
         return HttpResponseRedirect(_redirect)
 
     def _build_page_401_response_platform(self, request):
         """
         Directly redirect to PAAS-LOGIN-PLATFORM
         """
-        if blueapps_settings.PAGE_401_RESPONSE_PLATFORM_FUNC:
-            return blueapps_settings.PAGE_401_RESPONSE_PLATFORM_FUNC(request)
+        if hasattr(settings, "BLUEAPPS_PAGE_401_RESPONSE_PLATFORM_FUNC"):
+            return settings.BLUEAPPS_PAGE_401_RESPONSE_PLATFORM_FUNC(request)
         _next = request.build_absolute_uri()
-        if request.method == "GET" and blueapps_settings.SPECIFIC_REDIRECT_KEY:
-            _next = request.GET.get(blueapps_settings.SPECIFIC_REDIRECT_KEY) or _next
+        if request.method == "GET" and hasattr(settings, "BLUEAPPS_SPECIFIC_REDIRECT_KEY"):
+            _next = request.GET.get(settings.BLUEAPPS_SPECIFIC_REDIRECT_KEY) or _next
         if self._conf.ADD_CROSS_PREFIX:
             _next = self._conf.CROSS_PREFIX + _next
 
         _login_url = build_redirect_url(
             _next,
             resolve_login_url(self._conf.LOGIN_URL, request),
             self._conf.C_URL,
@@ -128,16 +132,16 @@
 
     def build_weixin_401_response(self, request):
         """
         todo，说明 url 格式
         """
         _login_url = self._conf.WEIXIN_OAUTH_URL
         _next = request.build_absolute_uri()
-        if request.method == "GET" and blueapps_settings.SPECIFIC_REDIRECT_KEY:
-            _next = request.GET.get(blueapps_settings.SPECIFIC_REDIRECT_KEY) or _next
+        if request.method == "GET" and hasattr(settings, "BLUEAPPS_SPECIFIC_REDIRECT_KEY"):
+            _next = request.GET.get(settings.BLUEAPPS_SPECIFIC_REDIRECT_KEY) or _next
 
         extra_args = {
             "appid": self._conf.WEIXIN_APP_ID,
             "response_type": "code",
             "scope": "snsapi_base",
             "state": request.session["WEIXIN_OAUTH_STATE"],
         }
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/views.py` & `blueapps-4.7.1/blueapps/account/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import time
 
 from django.http import JsonResponse
 from django.middleware import csrf
 from django.shortcuts import render
 
 from blueapps.account.decorators import login_exempt
+from blueapps.middleware.xss.decorators import escape_exempt
 
 
 @login_exempt
 def login_success(request):
     """
     弹框登录成功返回页面
     """
@@ -35,29 +36,36 @@
     """
     refer_url = request.GET.get("refer_url")
 
     context = {"refer_url": refer_url}
     return render(request, "account/login_page.html", context)
 
 
+@login_exempt
+@escape_exempt
+def login_forbidden(request):
+    """
+    跳转至固定页面，拦截登录
+    """
+    hint_msg = request.GET.get("hint_msg")
+    context = {"hint_msg": hint_msg}
+    return render(request, "account/login_forbidden.html", context)
+
+
 def send_code_view(request):
     ret = request.user.send_code()
     return JsonResponse(ret)
 
 
 def get_user_info(request):
 
     return JsonResponse(
         {
             "code": 0,
-            "data": {
-                "id": request.user.id,
-                "username": request.user.username,
-                "timestamp": time.time(),
-            },
+            "data": {"id": request.user.id, "username": request.user.username, "timestamp": time.time()},
             "message": "ok",
         }
     )
 
 
 def get_csrf_token(request):
     """
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/urls.py` & `blueapps-4.7.1/blueapps/account/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 from blueapps.account import views
 
 app_name = "account"  # pylint: disable=invalid-name
 
 urlpatterns = [
     url(r"^login_success/$", views.login_success, name="login_success"),
     url(r"^login_page/$", views.login_page, name="login_page"),
+    url(r"^login_forbidden/$", views.login_forbidden, name="login_forbidden"),
     url(r"^send_code/$", views.send_code_view, name="send_code"),
     url(r"^get_user_info/$", views.get_user_info, name="get_user_info"),
     url(r"^get_csrf_token/$", views.get_csrf_token, name="get_csrf_token"),
 ]
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/static/account/login.js` & `blueapps-4.7.1/blueapps/account/static/account/login.js`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_token/middlewares.py` & `blueapps-4.7.1/blueapps/account/components/ptlogin/middlewares.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,74 +12,80 @@
 """
 
 import logging
 
 from django.conf import settings
 from django.contrib import auth
 from django.core.cache import caches
+from django.utils.deprecation import MiddlewareMixin
 
-from blueapps.account.components.bk_token.forms import AuthenticationForm
+from blueapps.account.components.ptlogin.forms import AuthenticationForm
 from blueapps.account.conf import ConfFixture
 from blueapps.account.handlers.response import ResponseHandler
 
-try:
-    from django.utils.deprecation import MiddlewareMixin
-except Exception:  # pylint: disable=broad-except
-    MiddlewareMixin = object
-
-
 logger = logging.getLogger("component")
 cache = caches["login_db"]
 
 
 class LoginRequiredMiddleware(MiddlewareMixin):
     def process_view(self, request, view, args, kwargs):
         """
-        Login paas by two ways
-        1. views decorated with 'login_exempt' keyword
-        2. User has logged in calling auth.login
+        可通过登录认证的方式，仅有两种
+        1. 带有 login_exemp 标识的 view 函数
+        2. 需要进行验证逻辑：
+        # 先获得 cookie 并校验，失败进入 401 页面进行登录，其他情况继续执行
+        # 在 session 和 cookie 中的 p_uin,p_skey 是否相同且用户有效
+        直接 None 放行页面
+        # 不满足上面的条件，则需要对 p_uin,p_skey 进行校验，并返回 user ，
+        如果 user 对象存在，进行将 p_uin,p_skey 写入 session
+        # 其他情况返回 401 页面 进行登录
         """
-        if hasattr(request, "is_wechat") and request.is_wechat():
+        if request.is_wechat():
             return None
 
         if hasattr(request, "is_bk_jwt") and request.is_bk_jwt():
             return None
 
-        if hasattr(request, "is_rio") and request.is_rio():
-            return None
-
+        # 登录豁免
         if getattr(view, "login_exempt", False):
             return None
 
         user = self.authenticate(request)
         if user:
             return None
 
+        # 验证不通过，需要跳转至统一登录平台
         handler = ResponseHandler(ConfFixture, settings)
         return handler.build_401_response(request)
 
     def process_response(self, request, response):
         return response
 
     def authenticate(self, request):
         form = AuthenticationForm(request.COOKIES)
         if not form.is_valid():
             return None
-
-        bk_token = form.cleaned_data["bk_token"]
+        uin = form.cleaned_data["p_uin"]
+        skey = form.cleaned_data["p_skey"]
         session_key = request.session.session_key
         if session_key:
-            # 确认 cookie 中的 ticket 和 cache 中的是否一致
             cache_session = cache.get(session_key)
-            is_match = cache_session and bk_token == cache_session.get("bk_token")
+            # 确认 cookie 中的 uin sky 和 cache 中的是否一致
+            is_match = (
+                cache_session
+                and uin == cache_session.get("p_uin")
+                and skey == cache_session.get("p_skey")
+            )
             if is_match and request.user.is_authenticated:
                 return request.user
-
-        user = auth.authenticate(request=request, bk_token=bk_token)
-        if user is not None and user.username != request.user.username:
+        user = auth.authenticate(request=request, uin=uin, skey=skey)
+        if user and user.username != request.user.username:
             auth.login(request, user)
-
-        if user is not None and request.user.is_authenticated:
+        if request.user.is_authenticated:
             # 登录成功，重新调用自身函数，即可退出
-            cache.set(session_key, {"bk_token": bk_token}, settings.LOGIN_CACHE_EXPIRED)
+            cache.set(
+                session_key,
+                {"p_uin": uin, "p_skey": skey},
+                settings.LOGIN_CACHE_EXPIRED,
+            )
             return self.authenticate(request)
         return user
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_token/__init__.py` & `blueapps-4.7.1/blueapps/account/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_token/backends.py` & `blueapps-4.7.1/blueapps/account/components/bk_token/backends.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
 import logging
 import traceback
 
+from blueapps.core.exceptions.base import MethodError
 from django.conf import settings
 from django.contrib.auth.backends import ModelBackend
 from django.db import IntegrityError
 
 from blueapps import metrics
 from blueapps.account import get_user_model
 from blueapps.account.conf import ConfFixture
@@ -135,34 +136,69 @@
             return True, user_info
         else:
             error_msg = response.get("message", "")
             error_data = response.get("data", "")
             logger.error("Failed to Get User Info: error=%(err)s, ret=%(ret)s" % {"err": error_msg, "ret": error_data})
             return False, {}
 
-    @staticmethod
-    def verify_bk_token(bk_token, request=None):
+    def verify_bk_token(self, bk_token, request=None):
         """
         请求VERIFY_URL,认证bk_token是否正确
         @param bk_token: "_FrcQiMNevOD05f8AY0tCynWmubZbWz86HslzmOqnhk"
         @type bk_token: str
         @return: False,None True,username
         @rtype: bool,None/str
         """
+        try:
+            return self.verify_bk_token_through_esb(bk_token)
+        except (NotImplementedError, MethodError, AttributeError):
+            # 对应版本 esb 不支持 client.bk_login.is_login 接口的情况
+            return self.verify_bk_token_through_verify_url(bk_token, request)
+
+    @staticmethod
+    def verify_bk_token_through_esb(bk_token):
+        api_params = {"bk_token": bk_token}
+
+        try:
+            with metrics.observe(
+                metrics.BLUEAPPS_USER_TOKEN_VERIFY_DURATION, hostname=metrics.HOSTNAME, token_type=TOKEN_TYPE,
+            ):
+                response = client.bk_login.is_login(api_params)
+        except (NotImplementedError, MethodError, AttributeError):
+            raise
+        except Exception:  # pylint: disable=broad-except
+            metrics.BLUEAPPS_USER_TOKEN_VERIFY_FAILED_TOTAL.labels(
+                hostname=metrics.HOSTNAME, token_type=TOKEN_TYPE, err="unknow_execption_raise",
+            ).inc()
+            logger.exception("Abnormal error in verify_bk_token...")
+            return False, None
+
+        if response.get("result"):
+            data = response.get("data")
+            username = data.get("bk_username")
+            return True, username
+        else:
+            metrics.BLUEAPPS_USER_TOKEN_VERIFY_FAILED_TOTAL.labels(
+                hostname=metrics.HOSTNAME, token_type=TOKEN_TYPE, err="verify_fail"
+            ).inc()
+            error_msg = response.get("message", "")
+            error_data = response.get("data", "")
+            logger.error("Fail to verify bk_token, error={}, ret={}".format(error_msg, error_data))
+            return False, None
+
+    @staticmethod
+    def verify_bk_token_through_verify_url(bk_token, request=None):
         api_params = {"bk_token": bk_token}
 
         try:
             with metrics.observe(
                 metrics.BLUEAPPS_USER_TOKEN_VERIFY_DURATION, hostname=metrics.HOSTNAME, token_type=TOKEN_TYPE
             ):
                 response = send(
-                    resolve_login_url(ConfFixture.VERIFY_URL, request, "http"),
-                    "GET",
-                    api_params,
-                    verify=False,
+                    resolve_login_url(ConfFixture.VERIFY_URL, request, "http"), "GET", api_params, verify=False,
                 )
         except Exception:  # pylint: disable=broad-except
             metrics.BLUEAPPS_USER_TOKEN_VERIFY_FAILED_TOTAL.labels(
                 hostname=metrics.HOSTNAME, token_type=TOKEN_TYPE, err="unknow_execption_raise"
             ).inc()
             logger.exception("Abnormal error in verify_bk_token...")
             return False, None
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_token/models.py` & `blueapps-4.7.1/blueapps/account/components/ptlogin/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_token/forms.py` & `blueapps-4.7.1/blueapps/account/components/bk_token/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/null/__init__.py` & `blueapps-4.7.1/blueapps/account/sites/ieod/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,7 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
-
-from django.utils.deprecation import MiddlewareMixin
-
-
-class NullMiddleware(MiddlewareMixin):
-    pass
-
-
-class NullBackend(object):
-    def authenticate(self, **kwargs):
-        return None
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/middlewares.py` & `blueapps-4.7.1/blueapps/account/components/bk_ticket/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/__init__.py` & `blueapps-4.7.1/blueapps/account/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/backends.py` & `blueapps-4.7.1/blueapps/account/components/bk_ticket/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/models.py` & `blueapps-4.7.1/blueapps/account/components/bk_token/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/forms.py` & `blueapps-4.7.1/blueapps/account/components/bk_ticket/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/__init__.py` & `blueapps-4.7.1/blueapps/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/weixin/middlewares.py` & `blueapps-4.7.1/blueapps/account/components/weixin/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/weixin/__init__.py` & `blueapps-4.7.1/blueapps/conf/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/weixin/backends.py` & `blueapps-4.7.1/blueapps/account/components/weixin/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/weixin/forms.py` & `blueapps-4.7.1/blueapps/account/components/weixin/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/rio/middlewares.py` & `blueapps-4.7.1/blueapps/account/components/rio/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/rio/__init__.py` & `blueapps-4.7.1/blueapps/conf/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/rio/backends.py` & `blueapps-4.7.1/blueapps/account/components/rio/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/rio/forms.py` & `blueapps-4.7.1/blueapps/account/components/rio/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/__init__.py` & `blueapps-4.7.1/blueapps/utils/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/backends.py` & `blueapps-4.7.1/blueapps/account/components/bk_jwt/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/middlewares.py` & `blueapps-4.7.1/blueapps/account/components/bk_token/middlewares.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,80 +12,100 @@
 """
 
 import logging
 
 from django.conf import settings
 from django.contrib import auth
 from django.core.cache import caches
-from django.utils.deprecation import MiddlewareMixin
 
-from blueapps.account.components.ptlogin.forms import AuthenticationForm
+from blueapps.account.components.bk_token.forms import AuthenticationForm
 from blueapps.account.conf import ConfFixture
 from blueapps.account.handlers.response import ResponseHandler
+from blueapps.utils import client
+
+try:
+    from django.utils.deprecation import MiddlewareMixin
+except Exception:  # pylint: disable=broad-except
+    MiddlewareMixin = object
+
 
 logger = logging.getLogger("component")
 cache = caches["login_db"]
 
 
 class LoginRequiredMiddleware(MiddlewareMixin):
     def process_view(self, request, view, args, kwargs):
         """
-        可通过登录认证的方式，仅有两种
-        1. 带有 login_exemp 标识的 view 函数
-        2. 需要进行验证逻辑：
-        # 先获得 cookie 并校验，失败进入 401 页面进行登录，其他情况继续执行
-        # 在 session 和 cookie 中的 p_uin,p_skey 是否相同且用户有效
-        直接 None 放行页面
-        # 不满足上面的条件，则需要对 p_uin,p_skey 进行校验，并返回 user ，
-        如果 user 对象存在，进行将 p_uin,p_skey 写入 session
-        # 其他情况返回 401 页面 进行登录
+        Login paas by two ways
+        1. views decorated with 'login_exempt' keyword
+        2. User has logged in calling auth.login
         """
-        if request.is_wechat():
+        if hasattr(request, "is_wechat") and request.is_wechat():
             return None
 
         if hasattr(request, "is_bk_jwt") and request.is_bk_jwt():
             return None
 
-        # 登录豁免
+        if hasattr(request, "is_rio") and request.is_rio():
+            return None
+
         if getattr(view, "login_exempt", False):
             return None
 
         user = self.authenticate(request)
         if user:
             return None
 
-        # 验证不通过，需要跳转至统一登录平台
         handler = ResponseHandler(ConfFixture, settings)
+
+        # check if the user is forbidden
+        user_forbidden, msg = self.is_user_forbidden(request)
+        if user_forbidden:
+            return handler.build_403_response(msg)
+
         return handler.build_401_response(request)
 
     def process_response(self, request, response):
         return response
 
     def authenticate(self, request):
         form = AuthenticationForm(request.COOKIES)
         if not form.is_valid():
             return None
-        uin = form.cleaned_data["p_uin"]
-        skey = form.cleaned_data["p_skey"]
+
+        bk_token = form.cleaned_data["bk_token"]
         session_key = request.session.session_key
         if session_key:
+            # 确认 cookie 中的 ticket 和 cache 中的是否一致
             cache_session = cache.get(session_key)
-            # 确认 cookie 中的 uin sky 和 cache 中的是否一致
-            is_match = (
-                cache_session
-                and uin == cache_session.get("p_uin")
-                and skey == cache_session.get("p_skey")
-            )
+            is_match = cache_session and bk_token == cache_session.get("bk_token")
             if is_match and request.user.is_authenticated:
                 return request.user
-        user = auth.authenticate(request=request, uin=uin, skey=skey)
-        if user and user.username != request.user.username:
+
+        user = auth.authenticate(request=request, bk_token=bk_token)
+        if user is not None and user.username != request.user.username:
             auth.login(request, user)
-        if request.user.is_authenticated:
+
+        if user is not None and request.user.is_authenticated:
             # 登录成功，重新调用自身函数，即可退出
-            cache.set(
-                session_key,
-                {"p_uin": uin, "p_skey": skey},
-                settings.LOGIN_CACHE_EXPIRED,
-            )
+            cache.set(session_key, {"bk_token": bk_token}, settings.LOGIN_CACHE_EXPIRED)
             return self.authenticate(request)
         return user
+
+    @staticmethod
+    def is_user_forbidden(request) -> (bool, str):
+        """
+        check if the user is forbidden
+        """
+        USER_FORBIDDEN_CODE = "1302403"
+        form = AuthenticationForm(request.COOKIES)
+        if not form.is_valid():
+            return False, ""
+
+        bk_token = form.cleaned_data["bk_token"]
+        try:
+            response = client.bk_login.is_login({"bk_token": bk_token})
+            if response["result"] is False and str(response["code"]) == USER_FORBIDDEN_CODE:
+                return True, response["message"]
+        except Exception as e:
+            logger.debug(f"check user forbidden error: {e}")
+        return False, ""
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/__init__.py` & `blueapps-4.7.1/blueapps/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/backends.py` & `blueapps-4.7.1/blueapps/account/components/ptlogin/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/models.py` & `blueapps-4.7.1/blueapps/account/components/bk_ticket/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/forms.py` & `blueapps-4.7.1/blueapps/account/components/ptlogin/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/admin.py` & `blueapps-4.7.1/blueapps/account/admin.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/templates/account/login_page.html` & `blueapps-4.7.1/blueapps/account/templates/account/login_page.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/templates/account/login_success.html` & `blueapps-4.7.1/blueapps/account/templates/account/login_success.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/readme.md` & `blueapps-4.7.1/blueapps/account/readme.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/backends.py` & `blueapps-4.7.1/blueapps/account/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/conf.py` & `blueapps-4.7.1/blueapps/account/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,28 @@
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 
 from blueapps.account.sites.default import ConfFixture as default_fixture
-from blueapps.settings import blueapps_settings
 
 
 class _ConfFixture:
-    ACCOUNT_CONF_PREFIX = "ACCOUNT"
+    ACCOUNT_CONF_PREFIX = "BLUEAPPS_ACCOUNT"
 
     def __init__(self, fixture_module):
         # store the module
         self._fixture = import_string(fixture_module)
 
     def __getattr__(self, name):
         # settings fixture, 优先返回开发者配置
         account_conf_key = f"{self.ACCOUNT_CONF_PREFIX}_{name}"
-        if hasattr(blueapps_settings, account_conf_key):
-            return getattr(blueapps_settings, account_conf_key)
+        if hasattr(settings, account_conf_key):
+            return getattr(settings, account_conf_key)
 
         # site fixture, 对应环境配置
         if hasattr(self._fixture, name):
             return getattr(self._fixture, name)
 
         # default fixture, 默认配置
         if hasattr(default_fixture, name):
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/models.py` & `blueapps-4.7.1/blueapps/account/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/forms.py` & `blueapps-4.7.1/blueapps/account/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/migrations/0003_verifyinfo.py` & `blueapps-4.7.1/blueapps/account/migrations/0003_verifyinfo.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/migrations/__init__.py` & `blueapps-4.7.1/blueapps/core/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/migrations/0001_initial.py` & `blueapps-4.7.1/blueapps/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/sites/ieod/__init__.py` & `blueapps-4.7.1/blueapps/core/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/sites/ieod/conf.py` & `blueapps-4.7.1/blueapps/account/sites/ieod/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/sites/__init__.py` & `blueapps-4.7.1/blueapps/template/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/sites/open/__init__.py` & `blueapps-4.7.1/blueapps/template/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/sites/open/conf.py` & `blueapps-4.7.1/blueapps/account/sites/open/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/sites/default.py` & `blueapps-4.7.1/blueapps/account/sites/default.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/account/sites/tencent/__init__.py` & `blueapps-4.7.1/blueapps/contrib/bk_commands/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,7 +6,13 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
+
+import sys
+
+from blueapps.contrib.bk_commands import bk_admin
+
+bk_admin(sys.argv)
```

### Comparing `blueapps-4.7.0rc1/blueapps/account/sites/tencent/conf.py` & `blueapps-4.7.1/blueapps/account/sites/tencent/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/template/backends/mako.py` & `blueapps-4.7.1/blueapps/template/backends/mako.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps/template/context_processors.py` & `blueapps-4.7.1/blueapps/template/context_processors.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/blueapps.egg-info/SOURCES.txt` & `blueapps-4.7.1/blueapps.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 test.py
 blueapps/__init__.py
 blueapps/metrics.py
-blueapps/settings.py
 blueapps.egg-info/PKG-INFO
 blueapps.egg-info/SOURCES.txt
 blueapps.egg-info/dependency_links.txt
 blueapps.egg-info/entry_points.txt
 blueapps.egg-info/not-zip-safe
 blueapps.egg-info/requires.txt
 blueapps.egg-info/top_level.txt
@@ -69,14 +68,15 @@
 blueapps/account/sites/ieod/__init__.py
 blueapps/account/sites/ieod/conf.py
 blueapps/account/sites/open/__init__.py
 blueapps/account/sites/open/conf.py
 blueapps/account/sites/tencent/__init__.py
 blueapps/account/sites/tencent/conf.py
 blueapps/account/static/account/login.js
+blueapps/account/templates/account/login_forbidden.html
 blueapps/account/templates/account/login_page.html
 blueapps/account/templates/account/login_success.html
 blueapps/account/utils/__init__.py
 blueapps/account/utils/http.py
 blueapps/account/utils/sms.py
 blueapps/conf/__init__.py
 blueapps/conf/database.py
@@ -97,43 +97,27 @@
 blueapps/contrib/bk_commands/management/templates.py
 blueapps/contrib/bk_commands/management/commands/__init__.py
 blueapps/contrib/bk_commands/management/commands/celery.py
 blueapps/contrib/bk_commands/management/commands/celerybeat.py
 blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
 blueapps/contrib/bk_commands/management/handlers/__init__.py
 blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
-blueapps/contrib/drf/README.md
-blueapps/contrib/drf/__init__.py
-blueapps/contrib/drf/exception.py
-blueapps/contrib/drf/renderers.py
-blueapps/contrib/drf/serializer.py
-blueapps/contrib/drf/viewsets.py
-blueapps/contrib/drf/swagger/schemas.py
-blueapps/contrib/drf/utils/__init__.py
-blueapps/contrib/drf/utils/authentication.py
-blueapps/contrib/drf/utils/filters.py
-blueapps/contrib/drf/utils/pagination.py
-blueapps/contrib/drf/utils/serializer_fields.py
-blueapps/contrib/drf/utils/serializers.py
-blueapps/contrib/drf/utils/viewset_mixin.py
-blueapps/contrib/dummy/__init__.py
-blueapps/contrib/dummy/dummy_client.py
-blueapps/contrib/test/__init__.py
-blueapps/contrib/test/override_middleware.py
 blueapps/core/__init__.py
 blueapps/core/wsgi.py
 blueapps/core/celery/__init__.py
 blueapps/core/celery/celery.py
 blueapps/core/exceptions/__init__.py
 blueapps/core/exceptions/base.py
 blueapps/core/exceptions/middleware.py
 blueapps/core/handler/__init__.py
 blueapps/core/handler/wsgi.py
 blueapps/core/sites/__init__.py
 blueapps/core/sites/middleware.py
+blueapps/dummy/__init__.py
+blueapps/dummy/dummy_client.py
 blueapps/middleware/__init__.py
 blueapps/middleware/request_provider.py
 blueapps/middleware/bkui/__init__.py
 blueapps/middleware/bkui/middlewares.py
 blueapps/middleware/xss/__init__.py
 blueapps/middleware/xss/decorators.py
 blueapps/middleware/xss/middlewares.py
@@ -162,26 +146,18 @@
 blueapps/patch/settings_open_saas.py
 blueapps/patch/settings_paas_services.py
 blueapps/template/__init__.py
 blueapps/template/context_processors.py
 blueapps/template/backends/__init__.py
 blueapps/template/backends/mako.py
 blueapps/utils/__init__.py
-blueapps/utils/base.py
-blueapps/utils/cache.py
-blueapps/utils/constants.py
-blueapps/utils/db.py
 blueapps/utils/esbclient.py
 blueapps/utils/fancy_dict.py
-blueapps/utils/json.py
 blueapps/utils/jwt_client.py
-blueapps/utils/local.py
-blueapps/utils/lock.py
 blueapps/utils/logger.py
 blueapps/utils/request_provider.py
-blueapps/utils/time.py
 blueapps/utils/tools.py
 blueapps/utils/unique.py
 blueapps/utils/sites/__init__.py
 blueapps/utils/sites/ieod/__init__.py
 blueapps/utils/sites/open/__init__.py
 blueapps/utils/sites/tencent/__init__.py
```

### Comparing `blueapps-4.7.0rc1/blueapps.egg-info/PKG-INFO` & `blueapps-4.7.1/blueapps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapps
-Version: 4.7.0rc1
+Version: 4.7.1
 Summary: development framework for blueking
 Home-page: https://github.com/TencentBlueKing/blueapps
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # 蓝鲸Python开发框架Blueapps
```

### Comparing `blueapps-4.7.0rc1/blueapps.egg-info/requires.txt` & `blueapps-4.7.1/blueapps.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Django<4.0.0,>=2.2.6
-mysqlclient<=2.1.1,>=1.4.4
+mysqlclient<=2.0.3,>=1.4.4
 bkoauth>=0.0.12
 MarkupSafe<2.0.0,>=1.1.1
 Mako<2.0,>=1.0.6
 requests<3.0.0,>=2.22.0
 python-json-logger>=0.1.7
 whitenoise<=5.2.0,>=3.3.0
-Werkzeug<2.0.0,>=1.0.0
 pyCryptodome>=3.9.7
 PyJWT<2.0,>=1.6.1
-cryptography<3.4,>=2.7
+cryptography>=2.7
 
 [opentelemetry]
 opentelemetry-api<2.0.0,>=1.6.2
 opentelemetry-sdk<2.0.0,>=1.6.2
 opentelemetry-exporter-otlp<2.0.0,>=1.6.2
 opentelemetry-exporter-jaeger<2.0.0,>=1.6.2
 opentelemetry-exporter-jaeger-proto-grpc<2.0.0,>=1.6.2
```

### Comparing `blueapps-4.7.0rc1/setup.py` & `blueapps-4.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,26 +48,25 @@
     #   py_modules=["my_module"],
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
         "Django>=2.2.6,<4.0.0",
-        "mysqlclient>=1.4.4,<=2.1.1",
+        "mysqlclient>=1.4.4,<=2.0.3",
         "bkoauth>=0.0.12",
         "MarkupSafe>=1.1.1,<2.0.0",
         "Mako>=1.0.6,<2.0",
         "requests>=2.22.0,<3.0.0",
         "python-json-logger>=0.1.7",
         "whitenoise>=3.3.0,<=5.2.0",
-        "Werkzeug>=1.0.0,<2.0.0",
         # jwt
         "pyCryptodome>=3.9.7",
         "PyJWT>=1.6.1,<2.0",
-        "cryptography>=2.7,<3.4",
+        "cryptography>=2.7",
     ],
     extras_require={
         "opentelemetry": [
             "opentelemetry-api>=1.6.2,<2.0.0",
             "opentelemetry-sdk>=1.6.2,<2.0.0",
             "opentelemetry-exporter-otlp>=1.6.2,<2.0.0",
             "opentelemetry-exporter-jaeger>=1.6.2,<2.0.0",
@@ -84,9 +83,11 @@
             "django-prometheus>=2.1.0,<3.0.0",
         ]
     },
     zip_safe=False,
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
-    entry_points={"console_scripts": ["bk-admin=blueapps.contrib.bk_commands:bk_admin"],},
+    entry_points={
+        "console_scripts": ["bk-admin=blueapps.contrib.bk_commands:bk_admin"],
+    },
 )
```

### Comparing `blueapps-4.7.0rc1/README.md` & `blueapps-4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc1/PKG-INFO` & `blueapps-4.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapps
-Version: 4.7.0rc1
+Version: 4.7.1
 Summary: development framework for blueking
 Home-page: https://github.com/TencentBlueKing/blueapps
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # 蓝鲸Python开发框架Blueapps
```

### Comparing `blueapps-4.7.0rc1/LICENSE.txt` & `blueapps-4.7.1/LICENSE.txt`

 * *Files identical despite different names*

