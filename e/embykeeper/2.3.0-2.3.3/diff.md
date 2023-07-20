# Comparing `tmp/embykeeper-2.3.0.tar.gz` & `tmp/embykeeper-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.3.0.tar", last modified: Thu Jul 20 11:44:41 2023, max compression
+gzip compressed data, was "embykeeper-2.3.3.tar", last modified: Thu Jul 20 17:21:15 2023, max compression
```

## Comparing `embykeeper-2.3.0.tar` & `embykeeper-2.3.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.924343 embykeeper-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 11:44:27.000000 embykeeper-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 11:44:27.000000 embykeeper-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-07-20 11:44:41.924343 embykeeper-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-07-20 11:44:27.000000 embykeeper-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.908344 embykeeper-2.3.0/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.912344 embykeeper-2.3.0/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.912344 embykeeper-2.3.0/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.916344 embykeeper-2.3.0/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.916344 embykeeper-2.3.0/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.908344 embykeeper-2.3.0/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.904344 embykeeper-2.3.0/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.904344 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.904344 embykeeper-2.3.0/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.924343 embykeeper-2.3.0/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-20 11:44:27.000000 embykeeper-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:44:41.924343 embykeeper-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.924343 embykeeper-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 11:44:27.000000 embykeeper-2.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.145521 embykeeper-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 17:21:05.000000 embykeeper-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 17:21:05.000000 embykeeper-2.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24347 2023-07-20 17:21:15.141521 embykeeper-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23448 2023-07-20 17:21:05.000000 embykeeper-2.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.137521 embykeeper-2.3.3/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.137521 embykeeper-2.3.3/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.137521 embykeeper-2.3.3/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24347 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:21:14.000000 embykeeper-2.3.3/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-20 17:21:05.000000 embykeeper-2.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:21:15.145521 embykeeper-2.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 17:21:05.000000 embykeeper-2.3.3/tests/test_cli.py
```

### Comparing `embykeeper-2.3.0/LICENSE` & `embykeeper-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/PKG-INFO` & `embykeeper-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.3.0
+Version: 2.3.3
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -162,14 +162,30 @@
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
 恭喜您！您已经成功部署了 Embykeeper.
 
+为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
+
+```bash
+tmux
+```
+
+这将启动一个 `tmux` 终端, 您可以在该终端中重新运行上述命令, 并按 Ctrl + B, 松开再按 D, 以脱离 `tmux` 终端.
+
+您随时可以通过运行:
+
+```bash
+tmux a
+```
+
+以重新连接到 `tmux` 终端.
+
 当您需要更新版本时, 您需要执行:
 
 ```bash
 docker pull embykeeper/embykeeper
 ```
 
 ### 通过 Docker Compose 部署
@@ -238,15 +254,15 @@
 
 恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
 
 ```bash
 tmux
 ```
 
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开再按 D, 以脱离 `tmux` 终端.
 
 您随时可以通过运行:
 
 ```bash
 tmux a
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.3.0 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.3.3 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -121,20 +121,25 @@
 [service] checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby",
 "singularity", "terminus"] monitor = ["bgk", "embyhub", "misty", "pornemby",
 "viper"] messager = [] ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -
 v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
-æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
-Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
-compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
-é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
-%E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­éæ°è¿è¡ä¸è¿°å½ä»¤, å¹¶æ Ctrl + B, æ¾å¼åæ
+D, ä»¥è±ç¦» `tmux` ç»ç«¯. æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ```
+ä»¥éæ°è¿æ¥å° `tmux` ç»ç«¯. å½æ¨éè¦æ´æ°çæ¬æ¶, æ¨éè¦æ§è¡:
+```bash docker pull embykeeper/embykeeper ``` ### éè¿ Docker Compose é¨ç½²
+æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) é¨ç½²
+Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker é¨ç½²](https://
+github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2)
+æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
@@ -154,27 +159,26 @@
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash
-git clone https://github.com/embykeeper/embykeeper.git make install && make run
-``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/
-embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
-è¥æ¨éè¦éè¿ [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-
-tutorial-commands.html) é¨ç½²èªå¯å¨æå¡,
-æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡: ```bash make systemd ```
-å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
-## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
-```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+Ctrl + B, æ¾å¼åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯. æ¨éæ¶å¯ä»¥éè¿è¿è¡:
+```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux` ç»ç«¯. å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` pip install -U embykeeper ``` ç¶åéæ°è¿è¡åºç¨.
+### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash git clone https://
+github.com/embykeeper/embykeeper.git make install && make run ```
+è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/embykeeper/
+embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). è¥æ¨éè¦éè¿
+[systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-tutorial-
+commands.html) é¨ç½²èªå¯å¨æå¡, æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡:
+```bash make systemd ``` å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ```
+ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper
+-h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
 æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
 (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
 (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
 e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
```

### Comparing `embykeeper-2.3.0/README.md` & `embykeeper-2.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,30 @@
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
 恭喜您！您已经成功部署了 Embykeeper.
 
+为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
+
+```bash
+tmux
+```
+
+这将启动一个 `tmux` 终端, 您可以在该终端中重新运行上述命令, 并按 Ctrl + B, 松开再按 D, 以脱离 `tmux` 终端.
+
+您随时可以通过运行:
+
+```bash
+tmux a
+```
+
+以重新连接到 `tmux` 终端.
+
 当您需要更新版本时, 您需要执行:
 
 ```bash
 docker pull embykeeper/embykeeper
 ```
 
 ### 通过 Docker Compose 部署
@@ -217,15 +233,15 @@
 
 恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
 
 ```bash
 tmux
 ```
 
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开再按 D, 以脱离 `tmux` 终端.
 
 您随时可以通过运行:
 
 ```bash
 tmux a
 ```
```

#### html2text {}

```diff
@@ -109,20 +109,25 @@
 [service] checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby",
 "singularity", "terminus"] monitor = ["bgk", "embyhub", "misty", "pornemby",
 "viper"] messager = [] ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -
 v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
-æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
-Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
-compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
-é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
-%E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­éæ°è¿è¡ä¸è¿°å½ä»¤, å¹¶æ Ctrl + B, æ¾å¼åæ
+D, ä»¥è±ç¦» `tmux` ç»ç«¯. æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ```
+ä»¥éæ°è¿æ¥å° `tmux` ç»ç«¯. å½æ¨éè¦æ´æ°çæ¬æ¶, æ¨éè¦æ§è¡:
+```bash docker pull embykeeper/embykeeper ``` ### éè¿ Docker Compose é¨ç½²
+æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) é¨ç½²
+Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker é¨ç½²](https://
+github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2)
+æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
@@ -142,27 +147,26 @@
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash
-git clone https://github.com/embykeeper/embykeeper.git make install && make run
-``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/
-embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
-è¥æ¨éè¦éè¿ [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-
-tutorial-commands.html) é¨ç½²èªå¯å¨æå¡,
-æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡: ```bash make systemd ```
-å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
-## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
-```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+Ctrl + B, æ¾å¼åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯. æ¨éæ¶å¯ä»¥éè¿è¿è¡:
+```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux` ç»ç«¯. å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` pip install -U embykeeper ``` ç¶åéæ°è¿è¡åºç¨.
+### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash git clone https://
+github.com/embykeeper/embykeeper.git make install && make run ```
+è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/embykeeper/
+embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). è¥æ¨éè¦éè¿
+[systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-tutorial-
+commands.html) é¨ç½²èªå¯å¨æå¡, æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡:
+```bash make systemd ``` å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ```
+ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper
+-h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
 æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
 (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
 (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
 e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
```

### Comparing `embykeeper-2.3.0/embykeeper/cli.py` & `embykeeper-2.3.3/embykeeper/cli.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/data.py` & `embykeeper-2.3.3/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/embywatcher/emby.py` & `embykeeper-2.3.3/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/embywatcher/main.py` & `embykeeper-2.3.3/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/log.py` & `embykeeper-2.3.3/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/settings.py` & `embykeeper-2.3.3/embykeeper/settings.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/base.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/ljyy.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/ljyy.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/misty.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.3.3/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/link.py` & `embykeeper-2.3.3/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/log.py` & `embykeeper-2.3.3/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/main.py` & `embykeeper-2.3.3/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/messager/base.py` & `embykeeper-2.3.3/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/messager/common.py` & `embykeeper-2.3.3/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.3.3/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.3.3/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.3.3/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.3.3/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.3.3/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.3.3/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.3.3/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.3.3/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/telechecker/tele.py` & `embykeeper-2.3.3/embykeeper/telechecker/tele.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper/utils.py` & `embykeeper-2.3.3/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.3.3/embykeeper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.3.0
+Version: 2.3.3
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -162,14 +162,30 @@
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
 恭喜您！您已经成功部署了 Embykeeper.
 
+为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
+
+```bash
+tmux
+```
+
+这将启动一个 `tmux` 终端, 您可以在该终端中重新运行上述命令, 并按 Ctrl + B, 松开再按 D, 以脱离 `tmux` 终端.
+
+您随时可以通过运行:
+
+```bash
+tmux a
+```
+
+以重新连接到 `tmux` 终端.
+
 当您需要更新版本时, 您需要执行:
 
 ```bash
 docker pull embykeeper/embykeeper
 ```
 
 ### 通过 Docker Compose 部署
@@ -238,15 +254,15 @@
 
 恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
 
 ```bash
 tmux
 ```
 
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开再按 D, 以脱离 `tmux` 终端.
 
 您随时可以通过运行:
 
 ```bash
 tmux a
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.3.0 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.3.3 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -121,20 +121,25 @@
 [service] checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby",
 "singularity", "terminus"] monitor = ["bgk", "embyhub", "misty", "pornemby",
 "viper"] messager = [] ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -
 v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
-æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
-Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
-compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
-é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
-%E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­éæ°è¿è¡ä¸è¿°å½ä»¤, å¹¶æ Ctrl + B, æ¾å¼åæ
+D, ä»¥è±ç¦» `tmux` ç»ç«¯. æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ```
+ä»¥éæ°è¿æ¥å° `tmux` ç»ç«¯. å½æ¨éè¦æ´æ°çæ¬æ¶, æ¨éè¦æ§è¡:
+```bash docker pull embykeeper/embykeeper ``` ### éè¿ Docker Compose é¨ç½²
+æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) é¨ç½²
+Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker é¨ç½²](https://
+github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2)
+æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
@@ -154,27 +159,26 @@
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash
-git clone https://github.com/embykeeper/embykeeper.git make install && make run
-``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/
-embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
-è¥æ¨éè¦éè¿ [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-
-tutorial-commands.html) é¨ç½²èªå¯å¨æå¡,
-æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡: ```bash make systemd ```
-å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
-## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
-```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+Ctrl + B, æ¾å¼åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯. æ¨éæ¶å¯ä»¥éè¿è¿è¡:
+```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux` ç»ç«¯. å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` pip install -U embykeeper ``` ç¶åéæ°è¿è¡åºç¨.
+### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash git clone https://
+github.com/embykeeper/embykeeper.git make install && make run ```
+è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/embykeeper/
+embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). è¥æ¨éè¦éè¿
+[systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-tutorial-
+commands.html) é¨ç½²èªå¯å¨æå¡, æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡:
+```bash make systemd ``` å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ```
+ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper
+-h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
 æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
 (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
 (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
 e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
```

### Comparing `embykeeper-2.3.0/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.3.3/embykeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/app.py` & `embykeeper-2.3.3/embykeeperweb/app.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/404.html` & `embykeeper-2.3.3/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.3.3/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-2.3.3/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.3.3/embykeeperweb/templates/assets/js/console.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.3.3/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/console.html` & `embykeeper-2.3.3/embykeeperweb/templates/console.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/embykeeperweb/templates/login.html` & `embykeeper-2.3.3/embykeeperweb/templates/login.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.0/pyproject.toml` & `embykeeper-2.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.3.0"
+version = "2.3.3"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
@@ -54,14 +54,15 @@
     "fake_useragent",
     "pycryptodome",
     "flask",
     "flask_socketio",
     "flask_login",
     "simple-websocket",
     "eventlet",
+    "cryptography",
 ]
 
 [project.urls]
 Homepage = "https://github.com/embykeeper/embykeeper"
 
 [project.readme]
 file = "README.md"
```

### Comparing `embykeeper-2.3.0/tests/test_cli.py` & `embykeeper-2.3.3/tests/test_cli.py`

 * *Files identical despite different names*

