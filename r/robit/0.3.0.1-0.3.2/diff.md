# Comparing `tmp/robit-0.3.0.1.tar.gz` & `tmp/robit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robit-0.3.0.1.tar", last modified: Fri Apr 14 21:38:35 2023, max compression
+gzip compressed data, was "robit-0.3.2.tar", last modified: Thu Jul 20 17:30:56 2023, max compression
```

## Comparing `robit-0.3.0.1.tar` & `robit-0.3.2.tar`

### file list

```diff
@@ -1,59 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 21:38:26.000000 robit-0.3.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 21:38:26.000000 robit-0.3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-14 21:38:35.766015 robit-0.3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-14 21:38:26.000000 robit-0.3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 21:38:26.000000 robit-0.3.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.762015 robit-0.3.0.1/robit/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/health.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/web_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/alpine.js
--rw-r--r--   0 runner    (1001) docker     (123)   194855 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)    80448 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/core.js
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/index.css
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/worker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/job/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/job/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/job/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/monitor/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/monitor/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/test/test_cron.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/test/test_robit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/worker/web_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.762015 robit-0.3.0.1/robit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-14 21:38:35.000000 robit-0.3.0.1/robit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-14 21:38:35.000000 robit-0.3.0.1/robit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:38:35.000000 robit-0.3.0.1/robit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 21:38:35.000000 robit-0.3.0.1/robit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 21:38:35.766015 robit-0.3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 21:38:26.000000 robit-0.3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.539151 robit-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-20 17:30:45.000000 robit-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 17:30:45.000000 robit-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-20 17:30:56.539151 robit-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-20 17:30:45.000000 robit-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 17:30:45.000000 robit-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.531151 robit-0.3.2/robit/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 17:30:45.000000 robit-0.3.2/robit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 17:30:45.000000 robit-0.3.2/robit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.535151 robit-0.3.2/robit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 17:30:45.000000 robit-0.3.2/robit/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.535151 robit-0.3.2/robit/cron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/cron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-20 17:30:45.000000 robit-0.3.2/robit/cron/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 17:30:45.000000 robit-0.3.2/robit/cron/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-20 17:30:45.000000 robit-0.3.2/robit/cron/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-20 17:30:45.000000 robit-0.3.2/robit/cron/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.535151 robit-0.3.2/robit/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/alpine.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194855 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)    80448 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/core.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/worker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-20 17:30:45.000000 robit-0.3.2/robit/html/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.535151 robit-0.3.2/robit/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 17:30:45.000000 robit-0.3.2/robit/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 17:30:45.000000 robit-0.3.2/robit/job/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 17:30:45.000000 robit-0.3.2/robit/job/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-20 17:30:45.000000 robit-0.3.2/robit/job/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.535151 robit-0.3.2/robit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-20 17:30:45.000000 robit-0.3.2/robit/monitor/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-20 17:30:45.000000 robit-0.3.2/robit/monitor/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.535151 robit-0.3.2/robit/socket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/socket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-20 17:30:45.000000 robit-0.3.2/robit/socket/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.539151 robit-0.3.2/robit/status/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 17:30:45.000000 robit-0.3.2/robit/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 17:30:45.000000 robit-0.3.2/robit/status/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-20 17:30:45.000000 robit-0.3.2/robit/status/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.539151 robit-0.3.2/robit/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.539151 robit-0.3.2/robit/test/cron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/test/cron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/test/cron/test_cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-20 17:30:45.000000 robit-0.3.2/robit/test/cron/test_cron_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 17:30:45.000000 robit-0.3.2/robit/test/cron/test_cron_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-20 17:30:45.000000 robit-0.3.2/robit/test/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 17:30:45.000000 robit-0.3.2/robit/test/test_robit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.539151 robit-0.3.2/robit/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 17:30:45.000000 robit-0.3.2/robit/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 17:30:45.000000 robit-0.3.2/robit/timer/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-20 17:30:45.000000 robit-0.3.2/robit/timer/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.539151 robit-0.3.2/robit/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 17:30:45.000000 robit-0.3.2/robit/web_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 17:30:45.000000 robit-0.3.2/robit/web_server/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.539151 robit-0.3.2/robit/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:45.000000 robit-0.3.2/robit/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-20 17:30:45.000000 robit-0.3.2/robit/worker/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-20 17:30:45.000000 robit-0.3.2/robit/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:30:56.531151 robit-0.3.2/robit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-20 17:30:56.000000 robit-0.3.2/robit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-20 17:30:56.000000 robit-0.3.2/robit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:30:56.000000 robit-0.3.2/robit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 17:30:56.000000 robit-0.3.2/robit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-20 17:30:56.539151 robit-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 17:30:45.000000 robit-0.3.2/setup.py
```

### Comparing `robit-0.3.0.1/LICENSE.txt` & `robit-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/PKG-INFO` & `robit-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robit
-Version: 0.3.0.1
+Version: 0.3.2
 Summary: Service Worker Framework
 Home-page: https://github.com/stratusadv/robit
 Author: Nathan Johnson
 Author-email: nathanj@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robit-0.3.0.1/README.md` & `robit-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/core/alert.py` & `robit-0.3.2/robit/core/alert.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
-from datetime import datetime, timedelta
+from datetime import timedelta
 from typing import Callable
 
 from robit.core.health import Health
+from robit.core.utils import tz_now
 
 
 class Alert:
     def __init__(
             self,
             method: Callable,
             method_kwargs: dict = None,
@@ -20,22 +21,22 @@
             self.method_kwargs = method_kwargs
         else:
             self.method_kwargs = dict()
 
         self.health_threshold = health_threshold
         self.hours_between_messages = hours_between_messages
 
-        self.last_message_datetime = datetime.now() - timedelta(hours=self.hours_between_messages)
+        self.last_message_datetime = tz_now() - timedelta(hours=self.hours_between_messages)
 
     def check_health_threshold(self, name, health: Health):
-        if datetime.now() >= self.last_message_datetime + timedelta(hours=self.hours_between_messages):
+        if tz_now() >= self.last_message_datetime + timedelta(hours=self.hours_between_messages):
             if health.percentage_hundreds <= self.health_threshold:
                 alert_message = f'ALERT: {name} dropped below the {self.health_threshold} percentage health threshold.'
                 self.method_kwargs['alert_message'] = alert_message
 
                 try:
                     self.method(**self.method_kwargs)
-                    self.last_message_datetime = datetime.now()
+                    self.last_message_datetime = tz_now()
                     logging.warning(alert_message)
                 except Exception as e:
                     failed_message = f'ERROR: Alert method failed on exception "{e}"'
                     logging.warning(failed_message)
```

### Comparing `robit-0.3.0.1/robit/core/health.py` & `robit-0.3.2/robit/core/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,11 +64,11 @@
         if value > 100.0:
             self.percentage = 100.0
         elif value < 0.0:
             self.percentage = 0.0
         else:
             self.percentage = value
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         return {
             'percentage': self.percentage,
         }
```

### Comparing `robit-0.3.0.1/robit/core/log.py` & `robit-0.3.2/robit/core/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from robit.core.clock import Clock
 
 
 class Log:
+
     def __init__(
             self,
             max_messages: int = 5,
-            utc_offset: int = 0,
     ):
         self.max_messages = max_messages
         self.message_list = list()
 
-        self.clock = Clock(utc_offset=utc_offset)
+        self.clock = Clock()
 
     def add_message(self, message: str):
         self.message_list.insert(0, f'[{self.clock.now_tz_verbose}] {message}')
         self.trim()
 
     def trim(self):
         if len(self.message_list) > self.max_messages:
```

### Comparing `robit-0.3.0.1/robit/core/timer.py` & `robit-0.3.2/robit/timer/timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from robit.core.utils import tz_now
 
 
 class Timer:
     def __init__(
             self,
             duration_decimal_places: int = 2,
             duration_list_max: int = 20,
@@ -31,18 +31,18 @@
         total_duration = 0.0
         if len(self.duration_list) > 0:
             for duration in self.duration_list:
                 total_duration += duration
             self.average_duration = total_duration / len(self.duration_list)
 
     def start(self):
-        self.timer = datetime.utcnow()
+        self.timer = tz_now()
 
     def stop(self):
-        duration = (datetime.utcnow() - self.timer).total_seconds()
+        duration = (tz_now() - self.timer).total_seconds()
 
         self.last_duration = duration
         self.duration_list.insert(0, duration)
 
         if self.shortest_duration == 0 or duration < self.shortest_duration:
             self.shortest_duration = duration
```

### Comparing `robit-0.3.0.1/robit/core/web_server.py` & `robit-0.3.2/robit/web_server/web_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,46 @@
-import logging
+from typing import Optional
 from http.server import BaseHTTPRequestHandler
 from pathlib import Path
 import threading
 
-
-def get_text_from_file(name):
-    return Path(Path(__file__).parent.parent.resolve(), 'html', name).read_text()
-
-
-def html_encode_file(name, replace_dict: dict = None):
-    html = get_text_from_file(name)
-
-    if replace_dict:
-        html_str = str(html)
-
-        for key, val in replace_dict.items():
-            html_str = html_str.replace(f'||{key}||', val)
-
-        return html_str.encode("utf8")
-
-    else:
-        return html.encode("utf8")
+from robit.socket.socket import WebServerSocket
+from robit.web_server.utils import html_encode_file
 
 
 class WebRequestHandler(BaseHTTPRequestHandler):
     def not_found(self):
         self.wfile.write('Nothing to See Here'.encode("utf8"))
 
     @property
-    def path_list(self):
+    def path_list(self) -> list:
         temp_path_list = self.path.split('/')
         path_list = list()
 
         for path in temp_path_list:
             if len(path) > 0:
                 path_list.append(path)
 
         return path_list
 
-    def is_in_path_list(self, path_list: list):
+    def is_in_path_list(self, path_list: list) -> bool:
         if len(path_list) >= 1:
             if path_list[0] is None:
                 del path_list[0]
 
         if len(path_list) <= len(self.path_list):
             for i in range(len(path_list)):
                 if path_list[i] != self.path_list[i]:
                     return False
             else:
                 return True
         else:
             return False
 
-    def served_static(self):
+    def served_static(self) -> bool:
         if 1 < len(self.path.split('.')) < 3:
             extension = self.path[1:].split('.')[1]
             if extension in ('js', 'css', 'html', 'png'):
                 if len(self.path.split('/')) > 2:
                     file_name = self.path.split('/')[2]
                 else:
                     file_name = self.path[1:]
@@ -70,15 +54,15 @@
                     self._set_headers()
                     self.wfile.write(html_encode_file(file_name))
 
                 return True
 
         return False
 
-    def _set_headers(self, content_type='text/html'):
+    def _set_headers(self, content_type: str = 'text/html') -> None:
         self.send_response(200)
         self.send_header("Content-type", content_type)
         self.end_headers()
 
     def do_GET(self):
         pass
 
@@ -87,44 +71,53 @@
 
     def do_POST(self):
         self._set_headers()
         self.not_found()
 
 
 class WebServer:
-    def __init__(self, address='localhost', port=8000, key=None, html_replace_dict=None):
+    def __init__(
+            self,
+            address: str = 'localhost',
+            port: int = 8000,
+            key: Optional[str] = None,
+            html_replace_dict: Optional[dict] = None
+    ):
         self.api_dict = dict()
         self.post_dict = dict()
 
         self.address = address
-        self.port = int(port)
+        self.port = port
         self.key = key
 
         self.html_replace_dict = html_replace_dict
 
-        self.thread = threading.Thread(target=self.httpd_serve)
-        self.thread.daemon = True
-
     def httpd_serve(self):
         pass
 
     def restart(self):
         pass
 
+    def start_socket(self):
+        socket = WebServerSocket(web_server=self)
+        socket.start()
+        socket.process_requests()
+
     def start(self):
-        self.thread.start()
-        href_link = f'http://{self.address}:{self.port}'
+        threading.Thread(target=self.httpd_serve).start()
+        threading.Thread(target=self.start_socket).start()
 
+        href_link = f'http://{self.address}:{self.port}'
         if self.key:
             href_link += f'/{self.key}/'
 
         print(f'Starting httpd server at {href_link}')
 
         if self.key is None:
-            print(f'We do not reccomend running servers with out keys!')
+            print(f'We do not recommend running servers with out keys!')
 
     def stop(self):
         pass
 
     def update_api_dict(self, update_dict: dict):
         for key, val in update_dict.items():
             self.api_dict[key] = val
```

### Comparing `robit-0.3.0.1/robit/html/alpine.js` & `robit-0.3.2/robit/html/alpine.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/html/bootstrap.css` & `robit-0.3.2/robit/html/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/html/bootstrap.js` & `robit-0.3.2/robit/html/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/html/icon.png` & `robit-0.3.2/robit/html/icon.png`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/html/index.css` & `robit-0.3.2/robit/html/index.css`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/html/monitor.html` & `robit-0.3.2/robit/html/monitor.html`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/html/monitor.js` & `robit-0.3.2/robit/html/monitor.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/html/worker.html` & `robit-0.3.2/robit/html/worker.html`

 * *Files 2% similar despite different names*

```diff
@@ -77,23 +77,24 @@
                                                                         class="text-muted fw-normal"
                                                                         x-text="'next run at ' + job.next_run_datetime"></span></span>
                                                                 <br/>
                                                                 <span class="h6" x-text="job.name"></span>
                                                             </div>
                                                             <div class="col-6 col-sm-2 text-center pb-2 pb-sm-0">
                                                                 <span class="fs-7 text-worker-muted">Status</span><br/>
-                                                                <span x-show="job.status === 'Running'"
-                                                                      class="h6 text-status-running"
-                                                                      x-text="job.status"></span>
-                                                                <span x-show="job.status === 'Error'"
-                                                                      class="h6 text-status-error"
-                                                                      x-text="job.status"></span>
-                                                                <span x-show="job.status === 'Queued'"
-                                                                      class="h6 text-status-waiting"
-                                                                      x-text="job.status"></span>
+                                                                    <span
+                                                                        x-text="job.status"
+                                                                        class="h6"
+                                                                        :class="{
+                                                                            'text-status-running': job.status === 'Running',
+                                                                            'text-status-error': job.status === 'Error',
+                                                                            'text-status-waiting': job.status === 'Queued'
+                                                                        }"
+                                                                    ></span>
+
                                                             </div>
                                                             <div class="col-6 text-center pb-2 pb-sm-0 d-block d-sm-none">
                                                                 <span class="fs-7 text-worker-muted">Health</span><br/>
                                                                 <span class="h6" x-text="job.health + '%'"></span>
                                                             </div>
                                                             <div class="col-6 col-sm-2 text-center">
                                                                 <span class="fs-7 text-worker-muted">Success</span><br/>
```

#### html2text {}

```diff
@@ -10,15 +10,16 @@
 key="i" class="col-12">
 Group
 Health
 
 key="i" class="col-12 px-3 pb-2">
 Job
 Status
-
+class="{ 'text-status-running': job.status === 'Running', 'text-status-error':
+job.status === 'Error', 'text-status-waiting': job.status === 'Queued' }" >
 Health
 Success
 Failed
 Health
 id="'job-' + job.id" class="row" style="display: none;">
 ===============================================================================
 Method
```

### Comparing `robit-0.3.0.1/robit/html/worker.js` & `robit-0.3.2/robit/html/worker.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.0.1/robit/job/job.py` & `robit-0.3.2/robit/job/job.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,136 @@
 import logging
-from time import sleep
-from typing import Callable
+from typing import Callable, Optional
 
 from robit.core.alert import Alert
-from robit.core.clock import Clock
+from robit.core.clock import Clock, CREATED_DATE_FORMAT
 from robit.core.counter import Counter
-from robit.core.cron import Cron
+from robit.core.utils import tz_now
+from robit.cron.cron import Cron
 from robit.core.health import Health
 from robit.core.id import Id
 from robit.core.log import Log
 from robit.core.name import Name
-from robit.core.status import Status
-from robit.core.timer import Timer
+from robit.status import Status
+from robit.timer import Timer, timing_decorator
 
 
 class Job:
     def __init__(
             self,
             name: str,
-            method,
-            method_kwargs: dict = {},
-            utc_offset: int = 0,
-            cron: str = '* * * * * *',
+            method: Callable,
+            method_kwargs: Optional[dict] = None,
+            cron: str = '* * * * *',
+            execution_type: str = 'thread',
             alert_method: Callable = None,
             alert_method_kwargs: dict = None,
     ):
         self.id = Id()
         self.name = Name(name)
         self.method = method
-        self.method_kwargs = method_kwargs
+        self.execution_type = execution_type
 
-        self.cron = Cron(value=cron, utc_offset=utc_offset)
+        if method_kwargs is None:
+            self.method_kwargs = dict()
+        else:
+            self.method_kwargs = method_kwargs
+
+        self.cron = Cron(cron_syntax=cron)
+        self.next_run_datetime = self.cron.next_datetime()
 
         if 'alert_method' is not None:
             self.alert = Alert(
                 method=alert_method,
                 method_kwargs=alert_method_kwargs
             )
         else:
             self.alert = None
 
-        self.clock = Clock(utc_offset=utc_offset)
-
+        self.clock = Clock()
         self.timer = Timer()
-
         self.status = Status()
 
         self.success_count = Counter()
         self.failed_count = Counter()
-        self.failed_log = Log(max_messages=20, utc_offset=utc_offset)
+        self.failed_log = Log(max_messages=20)
 
         self.health = Health()
 
-        self.result_log = Log(max_messages=200, utc_offset=utc_offset)
+        self.result_log = Log(max_messages=200)
+
+    @timing_decorator
+    def execute_method(self):
+        if self.method_kwargs:
+            method_result = self.method(**self.method_kwargs)
+        else:
+            method_result = self.method()
+        return method_result
 
     @property
     def method_verbose(self):
         if self.method_kwargs:
             return f'{self.method.__name__}(kwargs={self.method_kwargs})'
         else:
             return f'{ self.method.__name__ }()'
 
-    def run(self):
-        if self.cron.is_past_next_run_datetime():
-            logging.warning(f'STARTING: Job "{self.name}"')
+    def next_run_datetime_verbose(self):
+        return self.next_run_datetime.strftime(CREATED_DATE_FORMAT)
 
-            self.status.set('run')
-            self.timer.start()
+    def set_next_run_datetime(self):
+        self.next_run_datetime = self.cron.next_datetime()
 
-            try:
-                if self.method_kwargs:
-                    method_result = self.method(**self.method_kwargs)
-                else:
-                    method_result = self.method()
-                self.timer.stop()
-                logging.warning(f'SUCCESS: Job "{self.name}" completed')
-                self.success_count.increase()
-                self.health.add_positive()
-                if method_result:
-                    self.result_log.add_message(str(method_result))
-            except Exception as e:
-                self.status.set('error')
-                failed_message = f'ERROR: Job "{self.name}" failed on exception "{e}"'
-                logging.warning(failed_message)
-                self.failed_log.add_message(failed_message)
-                self.failed_count.increase()
-                self.health.add_negative()
+    def should_run(self):
+        return tz_now() > self.next_run_datetime
 
-            if self.alert:
-                self.alert.check_health_threshold(f'Job "{self.name}"', self.health)
-        else:
-            if self.status.value != 'error':
-                self.status.set('queued')
+    def run(self):
+        self.status.running()
+
+        logging.warning(f'STARTING: Job "{self.name}"')
+
+        try:
+            method_result = self.execute_method()
+            logging.warning(f'SUCCESS: Job "{self.name}" completed')
+
+            self.success_count.increase()
+            self.health.add_positive()
+
+            if method_result:
+                self.result_log.add_message(str(method_result))
+
+            self.status.queued()
+        except Exception as e:
+            self.status.error()
+            failed_message = f'ERROR: Job "{self.name}" failed on exception "{e}"'
+            logging.warning(failed_message)
+            self.failed_log.add_message(failed_message)
+            self.failed_count.increase()
+            self.health.add_negative()
 
-            sleep(1)
+        if self.alert:
+            self.alert.check_health_threshold(f'Job "{self.name}"', self.health)
 
     def as_dict(self):
         return {
-            'id': self.id.__str__(),
-            'name': self.name.__str__(),
-            'status': self.status.__str__(),
-            'next_run_datetime': self.cron.next_run_datetime_verbose,
+            'id': str(self.id),
+            'name': str(self.name),
+            'status': str(self.status),
+            'next_run_datetime': self.next_run_datetime_verbose(),
             'success_count': self.success_count.total,
-            'health': self.health.__str__(),
+            'health': str(self.health),
             'failed_count': self.failed_count.total,
         }
 
     def as_dict_full(self):
         return {
-            'id': self.id.__str__(),
-            'name': self.name.__str__(),
+            'id': str(self.id),
+            'name': str(self.name),
             'method': self.method_verbose,
-            'status': self.status.__str__(),
+            'status': str(self.status),
             'result_log': self.result_log.message_list,
             'clock': self.clock.as_dict(),
             'timer': self.timer.as_dict(),
             'success_count': self.success_count.total,
-            'health': self.health.__str__(),
+            'health': str(self.health),
             'failed_count': self.failed_count.total,
             'failed_log': self.failed_log.message_list,
         }
```

### Comparing `robit-0.3.0.1/robit/monitor/monitor.py` & `robit-0.3.2/robit/monitor/monitor.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,42 +2,39 @@
 from typing import Callable
 
 from robit.core.alert import Alert
 from robit.core.clock import Clock
 from robit.core.health import Health
 from robit.core.id import Id
 from robit.core.name import Name
-from robit.core.status import Status
 from robit.monitor.web_server import MonitorWebServer
 
 
 class Monitor:
     def __init__(
             self,
             name: str,
             web_server: bool = True,
             web_server_address: str = '127.0.0.1',
             web_server_port: int = 8200,
             key: str = None,
-            utc_offset: int = 0,
             alert_method: Callable = None,
             alert_method_kwargs: dict = None,
     ):
         self.id = Id()
         self.name = Name(name)
-        self.clock = Clock(utc_offset=utc_offset)
+        self.clock = Clock()
         self.health = Health()
-        self.status = Status()
 
         if web_server:
             self.web_server = MonitorWebServer(
                 address=web_server_address,
                 port=web_server_port,
                 key=key,
-                html_replace_dict={'title': self.name.__str__()}
+                html_replace_dict={'title': str(self.name)}
             )
             self.web_server.post_dict['worker_dict'] = dict()
         else:
             self.web_server = None
 
         if 'alert_method' is not None:
             self.alert = Alert(
@@ -47,18 +44,17 @@
         else:
             self.alert = None
 
         self.worker_dict = self.web_server.post_dict['worker_dict']
 
     def as_dict(self):
         return {
-            'id': self.id.__str__(),
-            'name': self.name.__str__(),
-            'health': self.health.__str__(),
-            'status': self.status.__str__(),
+            'id': str(self.id),
+            'name': str(self.name),
+            'health': str(self.health),
             'clock': self.clock.as_dict(),
             'workers': self.calculate_workers_to_list(),
         }
 
     def calculate_health(self):
         self.health.reset()
 
@@ -87,10 +83,9 @@
                 self.alert.check_health_threshold(f'Monitor "{self.name}"', self.health)
 
             if self.web_server:
                 self.web_server.update_api_dict(self.as_dict())
 
             sleep(1)
 
-
     def stop(self):
-        pass
+        pass
```

### Comparing `robit-0.3.0.1/robit/monitor/web_server.py` & `robit-0.3.2/robit/monitor/web_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import json
 import urllib.parse
-from urllib import parse
 from http.server import HTTPServer
 
-from robit.core.web_server import WebServer, WebRequestHandler, html_encode_file
+from robit.web_server.web_server import WebServer, WebRequestHandler
+from robit.web_server.utils import html_encode_file
 
 
 class MonitorWebServer(WebServer):
     def httpd_serve(self):
         api_dict = self.api_dict
         post_dict = self.post_dict
         key = self.key
```

### Comparing `robit-0.3.0.1/robit/worker/web_server.py` & `robit-0.3.2/robit/worker/web_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from http.server import HTTPServer
 
-from robit.core.web_server import WebServer, WebRequestHandler, html_encode_file
+from robit.web_server.web_server import WebServer, WebRequestHandler
+from robit.web_server.utils import html_encode_file
 
 
 class WorkerWebServer(WebServer):
     def httpd_serve(self):
         api_dict = self.api_dict
         key = self.key
         html_replace_dict = self.html_replace_dict
@@ -16,15 +17,14 @@
                 if self.is_in_path_list([key, 'worker_api']):
                     self._set_headers()
                     worker_dict = {
                         'id': api_dict['id'],
                         'name': api_dict['name'],
                         'groups': api_dict['groups'],
                         'health': api_dict['health'],
-                        'status': api_dict['status'],
                         'clock': api_dict['clock'],
                     }
                     self.wfile.write(json.dumps(worker_dict, indent=4).encode("utf8"))
 
                 elif self.is_in_path_list([key, 'job_api']):
                     self._set_headers()
                     if len(self.path_list) == 3:
```

### Comparing `robit-0.3.0.1/robit.egg-info/PKG-INFO` & `robit-0.3.2/robit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robit
-Version: 0.3.0.1
+Version: 0.3.2
 Summary: Service Worker Framework
 Home-page: https://github.com/stratusadv/robit
 Author: Nathan Johnson
 Author-email: nathanj@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

