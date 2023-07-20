# Comparing `tmp/skip-django-pymess-0.7.6.1.tar.gz` & `tmp/skip-django-pymess-0.7.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-pymess-0.7.6.1.tar", last modified: Mon Jan 30 01:41:52 2023, max compression
+gzip compressed data, was "skip-django-pymess-0.7.6.2.tar", last modified: Thu Jul 20 13:15:49 2023, max compression
```

## Comparing `skip-django-pymess-0.7.6.1.tar` & `skip-django-pymess-0.7.6.2.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.527156 skip-django-pymess-0.7.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-01-30 01:41:52.527156 skip-django-pymess-0.7.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.515155 skip-django-pymess-0.7.6.1/pymess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.515155 skip-django-pymess-0.7.6.1/pymess/backend/
--rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/controlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.515155 skip-django-pymess-0.7.6.1/pymess/backend/dialer/
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/dialer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/dialer/daktela.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/dialer/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.515155 skip-django-pymess-0.7.6.1/pymess/backend/emails/
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/emails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/emails/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/emails/mandrill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/emails/smtp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.515155 skip-django-pymess-0.7.6.1/pymess/backend/push/
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/push/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/push/onesignal.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/routers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.519156 skip-django-pymess-0.7.6.1/pymess/backend/sms/
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/sms/ats_sms_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/sms/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/sms/sms_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/sms/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/backend/sms/twilio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.511155 skip-django-pymess-0.7.6.1/pymess/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.511155 skip-django-pymess-0.7.6.1/pymess/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.519156 skip-django-pymess-0.7.6.1/pymess/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.519156 skip-django-pymess-0.7.6.1/pymess/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.519156 skip-django-pymess-0.7.6.1/pymess/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/management/commands/check_dialer_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/management/commands/check_sms_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/management/commands/dump_emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/management/commands/pull_emails_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/management/commands/send_messages_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/management/commands/sync_emails.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.523156 skip-django-pymess-0.7.6.1/pymess/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0002_emailmessage_number_of_send_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0003_dialer.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0004_dialermessage_is_final_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0005_push_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0006_auto_20190322_1712.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0007_auto_20190401_1145.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0008_auto_20190726_1459.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0009_20191108_2007.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0010_20191120_1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0011_auto_20191210_1749.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0012_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0013_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0014_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0015_auto_20200110_0904.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0016_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0017_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0018_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0019_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0020_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0021_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0022_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0023_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0024_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0025_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0026_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/0027_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.523156 skip-django-pymess-0.7.6.1/pymess/models/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/models/dialer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/models/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/models/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/models/sms.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.511155 skip-django-pymess-0.7.6.1/pymess/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.511155 skip-django-pymess-0.7.6.1/pymess/templates/pymess/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.511155 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.523156 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/ats/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/ats/base.xml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/ats/delivery_request.xml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/ats/sms.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.527156 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/sms_operator/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/sms_operator/base.xml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/sms_operator/delivery_request.xml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/templates/pymess/sms/sms_operator/sms.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.527156 skip-django-pymess-0.7.6.1/pymess/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/templatetags/pymess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.527156 skip-django-pymess-0.7.6.1/pymess/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/utils/logged_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/utils/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.527156 skip-django-pymess-0.7.6.1/pymess/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/pymess/webhooks/mandrill.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 01:41:52.527156 skip-django-pymess-0.7.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-01-30 01:41:43.000000 skip-django-pymess-0.7.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:41:52.527156 skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-01-30 01:41:52.000000 skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-01-30 01:41:52.000000 skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 01:41:52.000000 skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 01:41:52.000000 skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-30 01:41:52.000000 skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-30 01:41:52.000000 skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.361600 skip-django-pymess-0.7.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-20 13:15:49.361600 skip-django-pymess-0.7.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/controlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/backend/dialer/
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/dialer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/dialer/daktela.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/dialer/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/backend/emails/
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/emails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/emails/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/emails/mandrill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/emails/smtp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/backend/push/
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/push/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/push/onesignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/routers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.349599 skip-django-pymess-0.7.6.2/pymess/backend/sms/
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/ats_sms_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/sms_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.349599 skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.349599 skip-django-pymess-0.7.6.2/pymess/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.349599 skip-django-pymess-0.7.6.2/pymess/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/check_dialer_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/check_sms_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/dump_emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/pull_emails_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/send_messages_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/sync_emails.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.353599 skip-django-pymess-0.7.6.2/pymess/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0002_emailmessage_number_of_send_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0003_dialer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0004_dialermessage_is_final_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0005_push_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0006_auto_20190322_1712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0007_auto_20190401_1145.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0008_auto_20190726_1459.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0009_20191108_2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0010_20191120_1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0011_auto_20191210_1749.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0012_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0013_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0014_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0015_auto_20200110_0904.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0016_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0017_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0018_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0019_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0020_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0021_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0022_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0023_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0024_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0025_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0026_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0027_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0028_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/dialer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/templates/pymess/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/ats/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/ats/base.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/ats/delivery_request.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/ats/sms.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/sms_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/sms_operator/base.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/sms_operator/delivery_request.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/sms_operator/sms.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templatetags/pymess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/utils/logged_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/utils/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/webhooks/mandrill.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:15:49.361600 skip-django-pymess-0.7.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/top_level.txt
```

### Comparing `skip-django-pymess-0.7.6.1/LICENSE` & `skip-django-pymess-0.7.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/PKG-INFO` & `skip-django-pymess-0.7.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pymess
-Version: 0.7.6.1
+Version: 0.7.6.2
 Summary: Pymess is a Django framework for sending messages
 Home-page: https://github.com/skip-pay/django-pymess
 Author: Lubos Matl,Oskar Hollman
 Author-email: matllubos@gmail.com
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/__init__.py` & `skip-django-pymess-0.7.6.2/pymess/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/dialer/__init__.py` & `skip-django-pymess-0.7.6.2/pymess/backend/dialer/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/dialer/daktela.py` & `skip-django-pymess-0.7.6.2/pymess/backend/dialer/daktela.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/emails/__init__.py` & `skip-django-pymess-0.7.6.2/pymess/backend/emails/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/emails/dummy.py` & `skip-django-pymess-0.7.6.2/pymess/backend/emails/dummy.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/emails/mandrill.py` & `skip-django-pymess-0.7.6.2/pymess/backend/emails/mandrill.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/emails/smtp.py` & `skip-django-pymess-0.7.6.2/pymess/backend/emails/smtp.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/push/__init__.py` & `skip-django-pymess-0.7.6.2/pymess/backend/push/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/push/onesignal.py` & `skip-django-pymess-0.7.6.2/pymess/backend/push/onesignal.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/sms/__init__.py` & `skip-django-pymess-0.7.6.2/pymess/backend/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/sms/ats_sms_operator.py` & `skip-django-pymess-0.7.6.2/pymess/backend/sms/ats_sms_operator.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/sms/sms_operator.py` & `skip-django-pymess-0.7.6.2/pymess/backend/sms/sms_operator.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/sms/sns.py` & `skip-django-pymess-0.7.6.2/pymess/backend/sms/sns.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/backend/sms/twilio.py` & `skip-django-pymess-0.7.6.2/pymess/backend/sms/twilio.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/config.py` & `skip-django-pymess-0.7.6.2/pymess/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/enums.py` & `skip-django-pymess-0.7.6.2/pymess/enums.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/locale/cs/LC_MESSAGES/django.mo` & `skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/locale/cs/LC_MESSAGES/django.po` & `skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,214 +3,214 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-03-07 11:45+0100\n"
+"POT-Creation-Date: 2023-07-18 20:51-0500\n"
 "PO-Revision-Date: 2022-01-07 16:10+0100\n"
 "Last-Translator: Lukáš Říha <lukas.riha@mallpay.cz>\n"
 "Language-Team: \n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 2.2.1\n"
 
-#: backend/emails/mandrill.py:101
+#: backend/emails/mandrill.py:100
 msgid "invalid"
 msgstr "špatný formát"
 
-#: backend/emails/mandrill.py:103
+#: backend/emails/mandrill.py:102
 msgid "rejected, mandrill message: \"{}\""
 msgstr "zamítnuto, zpráva mandrillu \"{}\""
 
-#: backend/sms/__init__.py:91 backend/sms/sms_operator.py:33
+#: backend/sms/__init__.py:91 backend/sms/sms_operator.py:32
 msgid "timeouted"
 msgstr "vypršel čas na zpracování dotazu"
 
-#: backend/sms/ats_sms_operator.py:29 backend/sms/sms_operator.py:46
+#: backend/sms/ats_sms_operator.py:28 backend/sms/sms_operator.py:45
 msgid "not found"
 msgstr "nenalezeno"
 
-#: backend/sms/ats_sms_operator.py:30
+#: backend/sms/ats_sms_operator.py:29
 msgid "not sent yet"
 msgstr "zatím neodeslána"
 
-#: backend/sms/ats_sms_operator.py:31 enums.py:34 enums.py:43 enums.py:54
+#: backend/sms/ats_sms_operator.py:30 enums.py:34 enums.py:43 enums.py:54
 msgid "sent"
 msgstr "odeslána"
 
-#: backend/sms/ats_sms_operator.py:32 backend/sms/sms_operator.py:28
+#: backend/sms/ats_sms_operator.py:31 backend/sms/sms_operator.py:27
 #: enums.py:57
 msgid "delivered"
 msgstr "doručena"
 
-#: backend/sms/ats_sms_operator.py:33 backend/sms/sms_operator.py:29
+#: backend/sms/ats_sms_operator.py:32 backend/sms/sms_operator.py:28
 msgid "not delivered"
 msgstr "nedoručena"
 
-#: backend/sms/ats_sms_operator.py:34
+#: backend/sms/ats_sms_operator.py:33
 msgid "not able to determine the state"
 msgstr "není možné zjistit stav"
 
-#: backend/sms/ats_sms_operator.py:36
+#: backend/sms/ats_sms_operator.py:35
 msgid "authentication failed"
 msgstr "ověření se nezdařilo"
 
-#: backend/sms/ats_sms_operator.py:38
+#: backend/sms/ats_sms_operator.py:37
 msgid "DB error"
 msgstr "chyba databáze"
 
-#: backend/sms/ats_sms_operator.py:40
+#: backend/sms/ats_sms_operator.py:39
 msgid "SMS is OK and ready to be sent"
 msgstr "SMS je připravena k odeslání"
 
-#: backend/sms/ats_sms_operator.py:41
+#: backend/sms/ats_sms_operator.py:40
 msgid "unspecified error"
 msgstr "nespecifikovaná chyba"
 
-#: backend/sms/ats_sms_operator.py:42
+#: backend/sms/ats_sms_operator.py:41
 msgid "one of the requests has not unique \"uniq\""
 msgstr "jeden z požadavků nemá unikátní hodnotu \"uniq\""
 
-#: backend/sms/ats_sms_operator.py:43
+#: backend/sms/ats_sms_operator.py:42
 msgid "SMS has not unique \"uniq\""
 msgstr "SMS nemá unikátní hodnotu \"uniq\""
 
-#: backend/sms/ats_sms_operator.py:44
+#: backend/sms/ats_sms_operator.py:43
 msgid "SMS lacks keyword"
 msgstr "SMS postrádá klíčové slovo"
 
-#: backend/sms/ats_sms_operator.py:45
+#: backend/sms/ats_sms_operator.py:44
 msgid "keyword not valid"
 msgstr "neplatné klíčové slovo"
 
-#: backend/sms/ats_sms_operator.py:46
+#: backend/sms/ats_sms_operator.py:45
 msgid "no sender specified"
 msgstr "není specifikován odesílatel"
 
-#: backend/sms/ats_sms_operator.py:47
+#: backend/sms/ats_sms_operator.py:46
 msgid "sender not valid"
 msgstr "číslo odesílatele je neplatné"
 
-#: backend/sms/ats_sms_operator.py:48
+#: backend/sms/ats_sms_operator.py:47
 msgid "MO PR SMS not allowed"
 msgstr "SMS typu MO PR není povolena"
 
-#: backend/sms/ats_sms_operator.py:49
+#: backend/sms/ats_sms_operator.py:48
 msgid "MT PR SMS not allowed"
 msgstr "SMS typu MT PR není povolena"
 
-#: backend/sms/ats_sms_operator.py:50
+#: backend/sms/ats_sms_operator.py:49
 msgid "MT PR SMS daily limit exceeded"
 msgstr "počet SMS typu MT PR překročen denní limit"
 
-#: backend/sms/ats_sms_operator.py:51
+#: backend/sms/ats_sms_operator.py:50
 msgid "MT PR SMS total limit exceeded"
 msgstr "počet SMS typu MT PR překročen celkový limit"
 
-#: backend/sms/ats_sms_operator.py:52
+#: backend/sms/ats_sms_operator.py:51
 msgid "geographic number is not allowed"
 msgstr "geografické číslo není povoleno"
 
-#: backend/sms/ats_sms_operator.py:53
+#: backend/sms/ats_sms_operator.py:52
 msgid "MT SMS to Slovakia not allowed"
 msgstr "SMS typu MT na Slovensko není povolena"
 
-#: backend/sms/ats_sms_operator.py:54
+#: backend/sms/ats_sms_operator.py:53
 msgid "shortcodes not allowed"
 msgstr "zkratky nejsou povoleny"
 
-#: backend/sms/ats_sms_operator.py:55
+#: backend/sms/ats_sms_operator.py:54
 msgid "sender is unknown"
 msgstr "odesílatel je neznámý"
 
-#: backend/sms/ats_sms_operator.py:56
+#: backend/sms/ats_sms_operator.py:55
 msgid "type of SMS not specified"
 msgstr "type SMS zprávny není určen"
 
-#: backend/sms/ats_sms_operator.py:57
+#: backend/sms/ats_sms_operator.py:56
 msgid "SMS too long"
 msgstr "text SMS je moc dlouhý"
 
-#: backend/sms/ats_sms_operator.py:58
+#: backend/sms/ats_sms_operator.py:57
 msgid "too many SMS parts (max. is 10)"
 msgstr "příliš mnoho částí SMS (maximum je 10)"
 
-#: backend/sms/ats_sms_operator.py:59
+#: backend/sms/ats_sms_operator.py:58
 msgid "wrong number of sender/receiver"
 msgstr "špatné číslo odesílatele nebo příjemce"
 
-#: backend/sms/ats_sms_operator.py:60
+#: backend/sms/ats_sms_operator.py:59
 msgid "recipient is missing or in wrong format"
 msgstr "číslo příjemce chybí nebo je ve špatném formátu"
 
-#: backend/sms/ats_sms_operator.py:61
+#: backend/sms/ats_sms_operator.py:60
 msgid "using \"textid\" is not allowed"
 msgstr "použití hodnoty \"texstid\" není povoleno"
 
-#: backend/sms/ats_sms_operator.py:62
+#: backend/sms/ats_sms_operator.py:61
 msgid "\"textid\" is in wrong format"
 msgstr "hodnota \"textid\" má špatný formát"
 
-#: backend/sms/ats_sms_operator.py:63
+#: backend/sms/ats_sms_operator.py:62
 msgid "long SMS with \"textid\" not allowed"
 msgstr "dlouhá SMS s \"textid\" není povolena"
 
-#: backend/sms/ats_sms_operator.py:65
+#: backend/sms/ats_sms_operator.py:64
 msgid "XML body missing"
 msgstr "chybí tělo XML zprávy"
 
-#: backend/sms/ats_sms_operator.py:66
+#: backend/sms/ats_sms_operator.py:65
 msgid "XML is not readable"
 msgstr "XML zpráva není validní"
 
-#: backend/sms/ats_sms_operator.py:67
+#: backend/sms/ats_sms_operator.py:66
 msgid "unknown HTTP method or not HTTP POST"
 msgstr "neznámá HTTP metoda"
 
-#: backend/sms/ats_sms_operator.py:68
+#: backend/sms/ats_sms_operator.py:67
 msgid "XML invalid"
 msgstr "XML má špatný formát"
 
-#: backend/sms/sms_operator.py:30
+#: backend/sms/sms_operator.py:29
 msgid "number not exists"
 msgstr "číslo neexistuje"
 
-#: backend/sms/sms_operator.py:34
+#: backend/sms/sms_operator.py:33
 msgid "wrong number format"
 msgstr "špatný formát čísla"
 
-#: backend/sms/sms_operator.py:35
+#: backend/sms/sms_operator.py:34
 msgid "another error"
 msgstr "jiná chyba"
 
-#: backend/sms/sms_operator.py:36
+#: backend/sms/sms_operator.py:35
 msgid "event error"
 msgstr "chyba události"
 
-#: backend/sms/sms_operator.py:37
+#: backend/sms/sms_operator.py:36
 msgid "SMS text too long"
 msgstr "text SMS je moc dlouhý"
 
-#: backend/sms/sms_operator.py:40
+#: backend/sms/sms_operator.py:39
 msgid "partly delivered"
 msgstr "částečně doručeno"
 
-#: backend/sms/sms_operator.py:41 enums.py:52
+#: backend/sms/sms_operator.py:40 enums.py:52
 msgid "unknown"
 msgstr "stav neznámý"
 
-#: backend/sms/sms_operator.py:42
+#: backend/sms/sms_operator.py:41
 msgid "partly delivered, partly unknown"
 msgstr "částečně doručeno, částečně neznáme"
 
-#: backend/sms/sms_operator.py:43
+#: backend/sms/sms_operator.py:42
 msgid "partly not delivered, partly unknown"
 msgstr "částečně nedoručeno, částečně neznámé"
 
 #: enums.py:9 enums.py:32 enums.py:42 enums.py:51
 msgid "waiting"
 msgstr "čeká"
 
@@ -356,15 +356,15 @@
 
 #: models/common.py:185
 msgid "Error during template body rendering: \"{}\""
 msgstr "Chyba během vykreslování obsahu zprávy: \"{}\""
 
 #: models/dialer.py:27 models/dialer.py:96 models/emails.py:58
 #: models/emails.py:261 models/emails.py:276 models/push.py:22 models/sms.py:27
-#: models/sms.py:79
+#: models/sms.py:81
 msgid "template"
 msgstr "šablona"
 
 #: models/dialer.py:29 models/emails.py:60 models/push.py:24 models/sms.py:29
 msgid "state"
 msgstr "stav"
 
@@ -560,26 +560,30 @@
 msgid "related object of a SMS message"
 msgstr "vztažený objekt SMS zprávy"
 
 #: models/sms.py:57
 msgid "related objects of SMS messages"
 msgstr "vztažené objekty SMS zpráv"
 
-#: models/sms.py:68
+#: models/sms.py:62
+msgid "is secret"
+msgstr "je tajný"
+
+#: models/sms.py:70
 msgid "SMS template"
 msgstr "SMS šablona"
 
-#: models/sms.py:69
+#: models/sms.py:71
 msgid "SMS templates"
 msgstr "SMS šablony"
 
-#: models/sms.py:88
+#: models/sms.py:90
 msgid "disallowed object of an SMS template"
 msgstr "zakázaný objekt SMS zprávy"
 
-#: models/sms.py:89
+#: models/sms.py:91
 msgid "disallowed objects of SMS templates"
 msgstr "zakázané objekty SMS zpráv"
 
 #: utils/html.py:23
 msgid "HTML body contains one of banned tag: {}"
 msgstr "Tělo HTML obsahuje jeden ze zakázaných tagů: {}"
```

### Comparing `skip-django-pymess-0.7.6.1/pymess/management/commands/dump_emails.py` & `skip-django-pymess-0.7.6.2/pymess/management/commands/dump_emails.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/management/commands/pull_emails_info.py` & `skip-django-pymess-0.7.6.2/pymess/management/commands/pull_emails_info.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/management/commands/send_messages_batch.py` & `skip-django-pymess-0.7.6.2/pymess/management/commands/send_messages_batch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/management/commands/sync_emails.py` & `skip-django-pymess-0.7.6.2/pymess/management/commands/sync_emails.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0001_initial.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0003_dialer.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0003_dialer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0005_push_notifications.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0005_push_notifications.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0006_auto_20190322_1712.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0006_auto_20190322_1712.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0007_auto_20190401_1145.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0007_auto_20190401_1145.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0008_auto_20190726_1459.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0008_auto_20190726_1459.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0009_20191108_2007.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0009_20191108_2007.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0010_20191120_1002.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0010_20191120_1002.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0011_auto_20191210_1749.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0011_auto_20191210_1749.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0012_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0012_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0013_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0013_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0014_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0014_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0015_auto_20200110_0904.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0015_auto_20200110_0904.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0016_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0016_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0017_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0017_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0018_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0018_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0019_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0019_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0020_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0020_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0021_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0021_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0022_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0022_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0023_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0023_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0024_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0024_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0025_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0025_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0026_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0026_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/migrations/0027_migration.py` & `skip-django-pymess-0.7.6.2/pymess/migrations/0027_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/models/common.py` & `skip-django-pymess-0.7.6.2/pymess/models/common.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/models/dialer.py` & `skip-django-pymess-0.7.6.2/pymess/models/dialer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/models/emails.py` & `skip-django-pymess-0.7.6.2/pymess/models/emails.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/models/push.py` & `skip-django-pymess-0.7.6.2/pymess/models/push.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/models/sms.py` & `skip-django-pymess-0.7.6.2/pymess/models/sms.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     class Meta(BaseRelatedObject.Meta):
         verbose_name = _('related object of a SMS message')
         verbose_name_plural = _('related objects of SMS messages')
 
 
 class AbstractSMSTemplate(BaseAbstractTemplate):
 
+    is_secret = models.BooleanField(null=False, blank=False, verbose_name=_('is secret'))
+
     def get_controller(self):
         from pymess.backend.sms import SMSController
         return SMSController()
 
     class Meta(BaseAbstractTemplate.Meta):
         abstract = True
         verbose_name = _('SMS template')
```

### Comparing `skip-django-pymess-0.7.6.1/pymess/templatetags/pymess.py` & `skip-django-pymess-0.7.6.2/pymess/templatetags/pymess.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/utils/__init__.py` & `skip-django-pymess-0.7.6.2/pymess/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/utils/html.py` & `skip-django-pymess-0.7.6.2/pymess/utils/html.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/utils/logged_requests.py` & `skip-django-pymess-0.7.6.2/pymess/utils/logged_requests.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/utils/migrations.py` & `skip-django-pymess-0.7.6.2/pymess/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/pymess/webhooks/mandrill.py` & `skip-django-pymess-0.7.6.2/pymess/webhooks/mandrill.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/setup.py` & `skip-django-pymess-0.7.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/PKG-INFO` & `skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pymess
-Version: 0.7.6.1
+Version: 0.7.6.2
 Summary: Pymess is a Django framework for sending messages
 Home-page: https://github.com/skip-pay/django-pymess
 Author: Lubos Matl,Oskar Hollman
 Author-email: matllubos@gmail.com
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `skip-django-pymess-0.7.6.1/skip_django_pymess.egg-info/SOURCES.txt` & `skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 pymess/migrations/0021_migration.py
 pymess/migrations/0022_migration.py
 pymess/migrations/0023_migration.py
 pymess/migrations/0024_migration.py
 pymess/migrations/0025_migration.py
 pymess/migrations/0026_migration.py
 pymess/migrations/0027_migration.py
+pymess/migrations/0028_migration.py
 pymess/migrations/__init__.py
 pymess/models/__init__.py
 pymess/models/common.py
 pymess/models/dialer.py
 pymess/models/emails.py
 pymess/models/push.py
 pymess/models/sms.py
```

