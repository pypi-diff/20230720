# Comparing `tmp/embykeeper-2.2.9.tar.gz` & `tmp/embykeeper-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.2.9.tar", last modified: Fri Jul  7 10:39:51 2023, max compression
+gzip compressed data, was "embykeeper-2.3.0.tar", last modified: Thu Jul 20 11:44:41 2023, max compression
```

## Comparing `embykeeper-2.2.9.tar` & `embykeeper-2.3.0.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.889610 embykeeper-2.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 10:39:41.000000 embykeeper-2.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 10:39:41.000000 embykeeper-2.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-07 10:39:51.889610 embykeeper-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-07-07 10:39:41.000000 embykeeper-2.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.881610 embykeeper-2.2.9/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.881610 embykeeper-2.2.9/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/bots/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 10:39:51.000000 embykeeper-2.2.9/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.877610 embykeeper-2.2.9/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.885610 embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.889610 embykeeper-2.2.9/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-07 10:39:41.000000 embykeeper-2.2.9/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-07 10:39:41.000000 embykeeper-2.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:39:51.889610 embykeeper-2.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:39:51.889610 embykeeper-2.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-07 10:39:41.000000 embykeeper-2.2.9/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.924343 embykeeper-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 11:44:27.000000 embykeeper-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 11:44:27.000000 embykeeper-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-07-20 11:44:41.924343 embykeeper-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-07-20 11:44:27.000000 embykeeper-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.908344 embykeeper-2.3.0/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.912344 embykeeper-2.3.0/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.912344 embykeeper-2.3.0/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.916344 embykeeper-2.3.0/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/bots/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.916344 embykeeper-2.3.0/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.908344 embykeeper-2.3.0/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 11:44:41.000000 embykeeper-2.3.0/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.904344 embykeeper-2.3.0/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.904344 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.904344 embykeeper-2.3.0/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.920343 embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.924343 embykeeper-2.3.0/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-20 11:44:27.000000 embykeeper-2.3.0/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-20 11:44:27.000000 embykeeper-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:44:41.924343 embykeeper-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:44:41.924343 embykeeper-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 11:44:27.000000 embykeeper-2.3.0/tests/test_cli.py
```

### Comparing `embykeeper-2.2.9/LICENSE` & `embykeeper-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/PKG-INFO` & `embykeeper-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.9
+Version: 2.3.0
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,40 +36,40 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/7Q7MzwYT) 获得社区帮助.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/QCVhBT5y) 获得社区帮助.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
 
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
-  - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
+  - Misty: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
+  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
-    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
-    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-    - ~~EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~ (停止签到)
+    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (关服)
+    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (关服)
+    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (关服)
 - Emby 保活
-
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
 
   - 默认禁用:
     - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
@@ -91,27 +90,27 @@
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
 
-#### 其他免费 Pass
+#### 其他免费 PaaS
 
 您也可以通过 [Patr.cloud](https://app.patr.cloud/) ([教程](https://blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) 等平台进行部署.
 
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考, 若您只需要进行机器人签到或 Emby 模拟观看, 您也可以只填写 `telegram` 部分或 `emby` 部分):
 
 ```toml
 [[telegram]]
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
@@ -124,14 +123,43 @@
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 ```
 
+<details>
+<summary>查看带代理的完整配置</summary>
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+
+[[telegram]]
+phone = "+8612109347899"
+
+[[emby]]
+url = "https://weiss-griffin.com/"
+username = "carrie19"
+password = "s*D7MMCpS$"
+```
+
+</details>
+
+若您需要启用某些默认禁用的站点, 或是关闭某些默认启用的站点, 请取消注释并修改:
+
+```toml
+[service]
+checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby", "singularity", "terminus"]
+monitor = ["bgk", "embyhub", "misty", "pornemby", "viper"]
+messager = []
+```
+
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -230,32 +258,29 @@
 pip install -U embykeeper
 ```
 
 然后重新运行应用.
 
 ### 从源码构建
 
-首先拉取并设置环境:
+拉取并设置环境:
 
 ```bash
 git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-python -m venv venv
-. ./venv/bin/activate
-pip install -e .
+make install && make run
 ```
 
-然后即可执行 Embykeeper:
+详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+
+若您需要通过 [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-tutorial-commands.html) 部署自启动服务, 您可以在成功运行一次后执行:
 
 ```bash
-embykeeper
+make systemd
 ```
 
-详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
-
 当版本更新时, 您需要执行:
 
 ```
 git pull
 ```
 
 然后重新运行应用.
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.9 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.3.0 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: <3.11,>=3.8
-Description-Content-Type: text/markdown License-File: LICENSE [![build status]
-(https://img.shields.io/github/actions/workflow/status/embykeeper/embykeeper/
-ci.yml?branch=main)](https://github.com/embykeeper/embykeeper/commits/main) [!
-[pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/
-project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE [![build status](https://img.shields.io/github/actions/workflow/status/
+embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/
+embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/
+embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://
+img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
@@ -39,46 +39,46 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
-æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/7Q7MzwYT) è·å¾ç¤¾åºå¸®å©.
+æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/QCVhBT5y) è·å¾ç¤¾åºå¸®å©.
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
 æºå¨äººç­¾å° - å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https:/
 /t.me/Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot) - ç»ç¹ç«: [é¢é]
 (https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
-t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
-(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
-(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
+t.me/EmbyPublicBot) - Singularity: [é¢é](https://t.me/
 Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
 [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
 peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
 t.me/peach_emby_bot) - Pornemby: [é¢é](https://t.me/pornembyservice)
 [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
 åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
 t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
-t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - Misty: [é¢é]
+(https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby) [æºå¨äºº]
+(https://t.me/EmbyMistyBot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»]
+(https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ - å¶ä»é Emby
 ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
 pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: - ~~BlueSea:
 [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~
-(æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
-(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~
-(æ ååº) - ~~EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
-emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ (åæ­¢ç­¾å°) - Emby ä¿æ´» -
-å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
-èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+(å³æ) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
+(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (å³æ)
+- Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/
+NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot) (å³æ) - Emby
+ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
 [é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
 åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
@@ -94,28 +94,38 @@
 å¨çº¿é¨ç½² #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
-å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ PaaS
 æ¨ä¹å¯ä»¥éè¿ [Patr.cloud](https://app.patr.cloud/) ([æç¨](https://
 blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) ç­å¹³å°è¿è¡é¨ç½². ###
 éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£
 docker](https://yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡:
 ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/
 embykeeper ``` å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml`
 æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
-(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
-"+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè,
+è¥æ¨åªéè¦è¿è¡æºå¨äººç­¾å°æ Emby æ¨¡æè§ç,
+æ¨ä¹å¯ä»¥åªå¡«å `telegram` é¨åæ `emby` é¨å): ```toml [[telegram]]
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
 `config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
-port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
-run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+port = 1080 scheme = "socks5" ```  æ¥çå¸¦ä»£ççå®æ´éç½® ```toml
+[proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] phone
+= "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ```
+è¥æ¨éè¦å¯ç¨æäºé»è®¤ç¦ç¨çç«ç¹,
+ææ¯å³é­æäºé»è®¤å¯ç¨çç«ç¹, è¯·åæ¶æ³¨éå¹¶ä¿®æ¹: ```toml
+[service] checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby",
+"singularity", "terminus"] monitor = ["bgk", "embyhub", "misty", "pornemby",
+"viper"] messager = [] ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -
+v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
@@ -147,26 +157,28 @@
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
-```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
-python -m venv venv . ./venv/bin/activate pip install -e . ```
-ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§
-[éè¿ Docker é¨ç½²](https://github.com/embykeeper/
-embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
-æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
-h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
-config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
-c å¯ç¨æ¯æ¥ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --
-emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash
+git clone https://github.com/embykeeper/embykeeper.git make install && make run
+``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/
+embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+è¥æ¨éè¦éè¿ [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-
+tutorial-commands.html) é¨ç½²èªå¯å¨æå¡,
+æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡: ```bash make systemd ```
+å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
+## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
+```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
 basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® --public å¯ç¨å¨çº¿é¨ç½²æ¨¡å¼ ```
 ä¾å¦: ```bash # å¯å¨ææåè½
```

### Comparing `embykeeper-2.2.9/README.md` & `embykeeper-2.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,40 +15,40 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/7Q7MzwYT) 获得社区帮助.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/QCVhBT5y) 获得社区帮助.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
 
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
-  - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
+  - Misty: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
+  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
-    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
-    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-    - ~~EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~ (停止签到)
+    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (关服)
+    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (关服)
+    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (关服)
 - Emby 保活
-
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
 
   - 默认禁用:
     - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
@@ -69,27 +69,27 @@
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
 
-#### 其他免费 Pass
+#### 其他免费 PaaS
 
 您也可以通过 [Patr.cloud](https://app.patr.cloud/) ([教程](https://blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) 等平台进行部署.
 
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考, 若您只需要进行机器人签到或 Emby 模拟观看, 您也可以只填写 `telegram` 部分或 `emby` 部分):
 
 ```toml
 [[telegram]]
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
@@ -102,14 +102,43 @@
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 ```
 
+<details>
+<summary>查看带代理的完整配置</summary>
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+
+[[telegram]]
+phone = "+8612109347899"
+
+[[emby]]
+url = "https://weiss-griffin.com/"
+username = "carrie19"
+password = "s*D7MMCpS$"
+```
+
+</details>
+
+若您需要启用某些默认禁用的站点, 或是关闭某些默认启用的站点, 请取消注释并修改:
+
+```toml
+[service]
+checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby", "singularity", "terminus"]
+monitor = ["bgk", "embyhub", "misty", "pornemby", "viper"]
+messager = []
+```
+
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -208,32 +237,29 @@
 pip install -U embykeeper
 ```
 
 然后重新运行应用.
 
 ### 从源码构建
 
-首先拉取并设置环境:
+拉取并设置环境:
 
 ```bash
 git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-python -m venv venv
-. ./venv/bin/activate
-pip install -e .
+make install && make run
 ```
 
-然后即可执行 Embykeeper:
+详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+
+若您需要通过 [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-tutorial-commands.html) 部署自启动服务, 您可以在成功运行一次后执行:
 
 ```bash
-embykeeper
+make systemd
 ```
 
-详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
-
 当版本更新时, 您需要执行:
 
 ```
 git pull
 ```
 
 然后重新运行应用.
```

#### html2text {}

```diff
@@ -27,46 +27,46 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
-æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/7Q7MzwYT) è·å¾ç¤¾åºå¸®å©.
+æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/QCVhBT5y) è·å¾ç¤¾åºå¸®å©.
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
 æºå¨äººç­¾å° - å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https:/
 /t.me/Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot) - ç»ç¹ç«: [é¢é]
 (https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
-t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
-(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
-(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
+t.me/EmbyPublicBot) - Singularity: [é¢é](https://t.me/
 Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
 [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
 peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
 t.me/peach_emby_bot) - Pornemby: [é¢é](https://t.me/pornembyservice)
 [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
 åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
 t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
-t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - Misty: [é¢é]
+(https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby) [æºå¨äºº]
+(https://t.me/EmbyMistyBot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»]
+(https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ - å¶ä»é Emby
 ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
 pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: - ~~BlueSea:
 [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~
-(æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
-(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~
-(æ ååº) - ~~EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
-emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ (åæ­¢ç­¾å°) - Emby ä¿æ´» -
-å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
-èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+(å³æ) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
+(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (å³æ)
+- Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/
+NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot) (å³æ) - Emby
+ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
 [é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
 åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
@@ -82,28 +82,38 @@
 å¨çº¿é¨ç½² #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
-å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ PaaS
 æ¨ä¹å¯ä»¥éè¿ [Patr.cloud](https://app.patr.cloud/) ([æç¨](https://
 blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) ç­å¹³å°è¿è¡é¨ç½². ###
 éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£
 docker](https://yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡:
 ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/
 embykeeper ``` å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml`
 æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
-(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
-"+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè,
+è¥æ¨åªéè¦è¿è¡æºå¨äººç­¾å°æ Emby æ¨¡æè§ç,
+æ¨ä¹å¯ä»¥åªå¡«å `telegram` é¨åæ `emby` é¨å): ```toml [[telegram]]
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
 `config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
-port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
-run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+port = 1080 scheme = "socks5" ```  æ¥çå¸¦ä»£ççå®æ´éç½® ```toml
+[proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] phone
+= "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ```
+è¥æ¨éè¦å¯ç¨æäºé»è®¤ç¦ç¨çç«ç¹,
+ææ¯å³é­æäºé»è®¤å¯ç¨çç«ç¹, è¯·åæ¶æ³¨éå¹¶ä¿®æ¹: ```toml
+[service] checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby",
+"singularity", "terminus"] monitor = ["bgk", "embyhub", "misty", "pornemby",
+"viper"] messager = [] ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -
+v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
@@ -135,26 +145,28 @@
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
-```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
-python -m venv venv . ./venv/bin/activate pip install -e . ```
-ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§
-[éè¿ Docker é¨ç½²](https://github.com/embykeeper/
-embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
-æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
-h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
-config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
-c å¯ç¨æ¯æ¥ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --
-emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash
+git clone https://github.com/embykeeper/embykeeper.git make install && make run
+``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/
+embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+è¥æ¨éè¦éè¿ [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-
+tutorial-commands.html) é¨ç½²èªå¯å¨æå¡,
+æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡: ```bash make systemd ```
+å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
+## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
+```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
 basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® --public å¯ç¨å¨çº¿é¨ç½²æ¨¡å¼ ```
 ä¾å¦: ```bash # å¯å¨ææåè½
```

### Comparing `embykeeper-2.2.9/embykeeper/cli.py` & `embykeeper-2.3.0/embykeeper/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,41 +51,44 @@
         "-e",
         rich_help_panel="模块开关",
         help="启用每隔天数Emby自动保活",
         show_default="不指定值时默认为每7天",
     ),
     monitor: bool = typer.Option(False, "--monitor", "-m", rich_help_panel="模块开关", help="启用群聊监视"),
     send: bool = typer.Option(False, "--send", "-s", rich_help_panel="模块开关", help="启用自动水群"),
+    version: bool = typer.Option(
+        None,
+        "--version",
+        "-v",
+        rich_help_panel="调试参数",
+        callback=version,
+        is_eager=True,
+        help=f"打印 {__name__.capitalize()} 版本",
+    ),
     instant: bool = typer.Option(
         True, "--instant/--no-instant", "-i/-I", rich_help_panel="调试参数", help="立刻执行一次任务"
     ),
     once: bool = typer.Option(False, "--once/--cron", "-o/-O", rich_help_panel="调试参数", help="仅执行一次任务而不计划执行"),
-    public: bool = typer.Option(False, rich_help_panel="调试参数", help="启用公共仓库部署模式"),
     debug: bool = typer.Option(
         False, "--debug", "-d", envvar="EK_DEBUG", show_envvar=False, rich_help_panel="调试参数", help="开启调试模式"
     ),
     debug_cron: bool = typer.Option(
         False, hidden=True, envvar="EK_DEBUG_CRON", show_envvar=False, help="开启任务调试模式, 在三秒后立刻开始执行计划任务"
     ),
-    version: bool = typer.Option(
-        None,
-        "--version",
-        "-v",
-        rich_help_panel="调试参数",
-        callback=version,
-        is_eager=True,
-        help=f"打印 {__name__.capitalize()} 版本",
-    ),
+    simple_log: bool = typer.Option(False, "--simple-log", "-L", help="简化日志输出格式"),
     follow: bool = typer.Option(False, "--follow", "-f", rich_help_panel="调试参数", help="仅启动消息调试"),
     analyze: bool = typer.Option(False, "--analyze", "-a", rich_help_panel="调试参数", help="仅启动历史信息分析"),
+    public: bool = typer.Option(False, rich_help_panel="调试参数", help="启用公共仓库部署模式"),
     basedir: Path = typer.Option(None, rich_help_panel="调试参数", help="设定输出文件位置"),
 ):
     from .log import logger, initialize
 
-    initialize(level="DEBUG" if debug else "INFO")
+    initialize(
+        level="DEBUG" if debug else "INFO", show_path=debug and (not simple_log), show_time=not simple_log
+    )
 
     config: dict = prepare_config(config, public=public)
 
     if debug:
         config["nofail"] = False
         logger.warning("您当前处于调试模式, 错误将会导致程序停止运行.")
     if debug_cron:
```

### Comparing `embykeeper-2.2.9/embykeeper/data.py` & `embykeeper-2.3.0/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/embywatcher/emby.py` & `embykeeper-2.3.0/embykeeper/embywatcher/emby.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from contextlib import asynccontextmanager
 import random
 
 import aiohttp
 from aiohttp_socks import ProxyConnector, ProxyType
 from embypy.emby import Emby as _Emby
 from embypy.objects import EmbyObject
 from embypy.utils.asyncio import async_func
@@ -57,14 +58,24 @@
                 if await self._process_resp(resp):
                     return resp
                 await asyncio.sleep(random.random() * i + 0.2)
             except (aiohttp.ClientConnectionError, OSError, asyncio.TimeoutError) as e:
                 pass
         raise aiohttp.ClientConnectionError("Emby server is probably down")
 
+    @async_func
+    async def get_stream_noreturn(self, path, **query):
+        try:
+            session = await self._get_session()
+            async with await self._req(session.get, path, **query) as resp:
+                async for _ in resp.content.iter_any():
+                    await asyncio.sleep(5)
+        finally:
+            await self._end_session()
+
 
 class Emby(_Emby):
     def __init__(self, url, **kargs):
         connector = Connector(url, **kargs)
         EmbyObject.__init__(self, {"ItemId": "", "Name": ""}, connector)
         self._partial_cache = {}
         self._cache_lock = asyncio.Condition()
```

### Comparing `embykeeper-2.2.9/embykeeper/embywatcher/main.py` & `embykeeper-2.3.0/embykeeper/embywatcher/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,27 +88,27 @@
         "PlayMethod": "DirectStream",
         "PlaySessionId": play_session_id,
         "MediaSourceId": media_source_id,
         "PositionTicks": 10000000 * progress,
         "CanSeek": True,
     }
     task = asyncio.create_task(send_playing(obj, playing_info))
-    timeout = c.timeout
     try:
-        c.timeout = time
-        await c.get(
-            f"/Videos/{obj.id}/stream",
-            static=True,
-            playSessionId=play_session_id,
-            MediaSourceId=media_source_id,
+        await asyncio.wait_for(
+            c.get_stream_noreturn(
+                f"/Videos/{obj.id}/stream",
+                static=True,
+                playSessionId=play_session_id,
+                MediaSourceId=media_source_id,
+            ),
+            timeout=time,
         )
     except asyncio.TimeoutError:
         pass
     finally:
-        c.timeout = timeout
         task.cancel()
     if not is_ok(await c.post("/Sessions/Playing/Stopped", **playing_info)):
         raise PlayError("无法正常结束播放")
     return True
 
 
 async def login(config):
@@ -151,43 +151,47 @@
                             last_played = get_last_played(obj)
                             if not last_played:
                                 raise PlayError("尝试播放后上次播放为空")
                             last_played = last_played.strftime("%Y-%m-%d %H:%M")
                             if not obj.percentage_played:
                                 raise PlayError("尝试播放后播放进度为空")
                             logger.bind(notify="成功保活.").info(
-                                f"[yellow]成功播放视频[/], 当前该视频播放{obj.play_count}次, 进度({obj.percentage_played}), 上次播放于 {last_played}."
+                                f"[yellow]成功播放视频[/], 进度 {int(obj.percentage_played * 100)} %."
                             )
+                            logger.debug(f"当前该视频播放 {obj.play_count} 次, 上次播放于 {last_played}.")
                             return True
-                    except (ClientError, OSError):
+                    except (ClientError, OSError) as e:
                         retry += 1
                         if retry > retries:
-                            logger.warning(f"超过最大重试次数, 保活失败.")
+                            logger.warning(f"超过最大重试次数, 保活失败: {e}.")
                             return False
                         else:
-                            logger.info(f"连接失败, 正在重试.")
+                            logger.info(f"连接失败, 正在重试: {e}.")
+                            await asyncio.sleep(1)
                     except PlayError as e:
                         logger.info(f"发生错误: {e}, 正在重试其他视频.")
+                        await asyncio.sleep(1)
                         break
                     finally:
                         try:
-                            if not await asyncio.shield(asyncio.wait_for(hide_from_resume(obj), 0.5)):
+                            if not await asyncio.shield(asyncio.wait_for(hide_from_resume(obj), 2)):
                                 logger.debug(f"未能成功从最近播放中隐藏视频.")
                         except asyncio.TimeoutError:
-                            logger.debug(f"未能成功从最近播放中隐藏视频.")
+                            logger.debug(f"从最近播放中隐藏视频超时.")
             else:
                 logger.warning(f"由于没有成功播放视频, 保活失败, 请重新检查配置.")
                 return False
-        except (ClientError, OSError):
+        except (ClientError, OSError) as e:
             retry += 1
             if retry > retries:
-                logger.warning(f"超过最大重试次数, 保活失败.")
+                logger.warning(f"超过最大重试次数, 保活失败: {e}.")
                 return False
             else:
-                logger.info(f"连接失败, 正在重试.")
+                logger.info(f"连接失败, 正在重试: {e}.")
+                await asyncio.sleep(1)
         except asyncio.CancelledError:
             raise
         except Exception as e:
             logger.opt(exception=e).warning("发生错误:")
             return False
```

### Comparing `embykeeper-2.2.9/embykeeper/log.py` & `embykeeper-2.3.0/embykeeper/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,17 +38,14 @@
         return f"[blue]{scheme_names[scheme]}[/]{ident}: {{message}}"
     elif scheme == "datamanager":
         return f"[blue]{scheme_names[scheme]}[/]: {{message}}"
     else:
         return "{message}"
 
 
-def initialize(level="INFO"):
+def initialize(level="INFO", **kw):
     logger.remove()
     handler = RichHandler(
-        console=Console(stderr=True),
-        markup=True,
-        rich_tracebacks=True,
-        tracebacks_suppress=[asyncio],
+        console=Console(stderr=True), markup=True, rich_tracebacks=True, tracebacks_suppress=[asyncio], **kw
     )
     handler.setFormatter(Formatter(None, "[%m/%d %H:%M]"))
     logger.add(handler, format=formatter, level=level, colorize=False)
```

### Comparing `embykeeper-2.2.9/embykeeper/settings.py` & `embykeeper-2.3.0/embykeeper/settings.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/bots/base.py` & `embykeeper-2.3.0/embykeeper/telechecker/bots/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,18 +179,21 @@
                         await self.send_checkin()
                     await asyncio.wait_for(self.finished.wait(), self.timeout)
                 except asyncio.CancelledError:
                     cancelled = True
                     raise
                 finally:
                     if not cancelled:
+                        if not await self.cleanup():
+                            self.log.debug(f"[gray50]执行清理失败: {ident}[/]")
                         if self._is_archived:
                             self.log.debug(f"[gray50]将会话重新归档: {ident}[/]")
                             try:
-                                await chat.archive()
+                                if await chat.archive():
+                                    self.log.debug(f"[gray50]重新归档成功: {ident}[/]")
                             except asyncio.TimeoutError:
                                 self.log.debug(f"[gray50]归档失败: {ident}[/]")
                         if not self.chat_name:
                             self.log.debug(f"[gray50]将会话设为已读: {ident}[/]")
                             try:
                                 if await self.client.read_chat_history(ident):
                                     self.log.debug(f"[gray50]设为已读成功: {ident}[/]")
@@ -203,14 +206,17 @@
             pass
         if not self.finished.is_set():
             self.log.warning("无法在时限内完成签到.")
             return False
         else:
             return self._retries <= self.retries
 
+    async def cleanup(self):
+        return True
+
     async def walk_history(self, limit=0):
         async for m in self.client.get_chat_history(
             self.chat_name or self.bot_id or self.bot_username, limit=limit
         ):
             if MessageType.CAPTCHA in self.message_type(m):
                 await self.on_photo(m)
                 return True
@@ -234,24 +240,26 @@
 
     async def _message_handler(self, client: Client, message: Message):
         try:
             await self.message_handler(client, message)
         except OSError as e:
             self.log.info(f'发生错误: "{e}", 正在重试.')
             await self.retry()
+            message.continue_propagation()
         except asyncio.CancelledError:
             raise
         except Exception as e:
-            if self.nofail:
-                self.log.opt(exception=e).warning(f"发生错误:")
+            if not self.nofail:
                 await self.fail()
+                raise
             else:
+                self.log.opt(exception=e).warning(f"发生错误:")
                 await self.fail()
-                raise
-        finally:
+                message.continue_propagation()
+        else:
             message.continue_propagation()
 
     async def message_handler(self, client: Client, message: Message, type=None):
         text = message.text or message.caption
         if text:
             for p, k in self._waiting.items():
                 if re.search(p, text):
@@ -303,53 +311,55 @@
 
     async def on_captcha(self, message: Message, captcha: str):
         await message.reply(captcha)
 
     async def on_text(self, message: Message, text: str):
         if any(s in text for s in to_iterable(self.bot_text_ignore)):
             pass
-        elif any(s in text for s in ("拉黑", "黑名单", "冻结", "未找到用户", "无资格", "退出群", "退群", "加群", "加入群聊", "请先关注")):
+        elif any(
+            s in text for s in ("拉黑", "黑名单", "冻结", "未找到用户", "无资格", "退出群", "退群", "加群", "加入群聊", "请先关注", "注册")
+        ):
             self.log.warning(f"签到失败: 账户错误.")
             await self.fail()
         elif any(s in text for s in ("已尝试", "过多")):
             self.log.warning(f"签到失败: 尝试次数过多.")
             await self.fail()
         elif any(s in text for s in ("失败", "错误", "超时")):
             self.log.info(f"签到失败: 验证码错误, 正在重试.")
             await self.retry()
         elif any(s in text for s in ("成功", "通过", "完成", "获得")):
             matches = re.search(self.bot_success_pat, text)
             if matches:
                 try:
                     self.log.info(f"[yellow]签到成功[/]: + {matches.group(1)} 分 -> {matches.group(2)} 分.")
                 except IndexError:
-                    self.log.info(f"[yellow]签到成功[/]: 当前/增加 {matches.group(0)} 分.")
+                    self.log.info(f"[yellow]签到成功[/]: 当前/增加 {matches.group(1)} 分.")
             else:
                 matches = re.search(r"\d+", text)
                 if matches:
                     self.log.info(f"[yellow]签到成功[/]: 当前/增加 {matches.group(0)} 分.")
                 else:
                     self.log.info(f"[yellow]签到成功[/].")
             self.finished.set()
-        elif any(s in text for s in ("只能", "已经", "下次", "过了", "签过", "明日再来")):
+        elif any(s in text for s in ("只能", "已经", "下次", "过了", "签过", "明日再来", "上次签到")):
             self.log.info(f"今日已经签到过了.")
             self.finished.set()
         else:
             self.log.warning(f"接收到异常返回信息: {text}")
 
     async def retry(self):
         self._retries += 1
         if self._retries <= self.retries:
             await asyncio.sleep(self.bot_retry_wait)
             await self.send_checkin(retry=True)
         else:
             self.log.warning("超过最大重试次数.")
             self.finished.set()
 
-    async def fail(self, message=None):
+    async def fail(self):
         self.finished.set()
         self._retries = float("inf")
 
     async def wait_until(self, pattern: str = ".", timeout: float = None):
         self._waiting[pattern] = e = asyncio.Event()
         try:
             await asyncio.wait_for(e.wait(), timeout)
```

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.3.0/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.3.0/embykeeper/telechecker/bots/jms.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,21 @@
                 with open(
                     await get_data(self.basedir, "idioms@v1.txt", proxy=self.proxy, caller=self.name)
                 ) as f:
                     self.__class__.idioms = [i for i in f.read().splitlines() if len(i) == 4]
         return await super().start()
 
     def to_idiom(self, captcha: str):
-        phrase, score = process.extractOne(captcha, self.idioms, scorer=fuzz.partial_token_sort_ratio)
+        phrase, score = process.extractOne(captcha, self.idioms)
         if score > 70 or len(captcha) < 4:
             result = phrase
-            self.log.debug(f'[gray50]已匹配识别验证码 "{captcha}" -> 成语 "{result}"[/]')
+            self.log.debug(f'[gray50]已匹配识别验证码 "{captcha}" -> 成语 "{result}".[/]')
         else:
             result = captcha
+            self.log.debug(f'[gray50]验证码 "{captcha}" 无法矫正, 使用原词.[/]')
         return result
 
     async def on_captcha(self, message: Message, captcha: str):
         captcha = self.to_idiom(captcha)
         async with self.operable:
             if not self.message:
                 await self.operable.wait()
```

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/bots/ljyy.py` & `embykeeper-2.3.0/embykeeper/telechecker/bots/ljyy.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.3.0/embykeeper/telechecker/bots/nebula.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from pyrogram.raw.functions.users import GetFullUser
 from fake_useragent import UserAgent
 
 from ...utils import remove_prefix
 from ..link import Link
 from .base import BaseBotCheckin
 
+__ignore__ = True
+
 
 class NebulaCheckin(BaseBotCheckin):
     name = "Nebula"
     bot_username = "Nebula_Account_bot"
 
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
@@ -54,15 +56,15 @@
         url_base = scheme._replace(path="/api/proxy/userCheckIn", query=f"data={data}", fragment="").geturl()
         scheme = urlparse(url_base)
         query = parse_qs(scheme.query, keep_blank_values=True)
         query = {k: v for k, v in query.items() if not k.startswith("tgWebApp")}
         token, proxy, useragent = await Link(self.client).captcha()
         if (not token) or (not proxy):
             self.log.warning("签到失败: 无法获得验证码.")
-            return self.fail()
+            return await self.fail()
         if not useragent:
             useragent = UserAgent(browsers=["edge"]).random
         query["token"] = token
         url_checkin = scheme._replace(query=urlencode(query, True)).geturl()
         connector = ProxyConnector.from_url(proxy)
         async with ClientSession(connector=connector) as session:
             async with session.get(url_checkin, headers={"User-Agent": useragent}) as resp:
```

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.3.0/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.3.0/embykeeper/telechecker/bots/pornemby.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,17 @@
         if not self.client.me.username:
             self.log.info(f"跳过签到: 需要设置用户名才可生效.")
             return None
         return await super().start()
 
     async def on_photo(self, message: Message):
         await asyncio.sleep(1)
-        try:
-            await message.click(0)
-        except TimeoutError:
-            pass
-        try:
-            msg = await self.client.wait_reply(self.bot_username, timeout=10)
-        except asyncio.TimeoutError:
-            self.log.warning(f"签到失败: 签到无回应, 您可能还没有注册{self.name}.")
-            await self.fail()
+        async with self.client.catch_reply(self.bot_username) as f:
+            try:
+                await message.click(0)
+            except TimeoutError:
+                pass
+            try:
+                await asyncio.wait_for(f, 10)
+            except asyncio.TimeoutError:
+                self.log.warning(f"签到失败: 签到无回应, 您可能还没有注册{self.name}.")
+                await self.fail()
```

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.3.0/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/link.py` & `embykeeper-2.3.0/embykeeper/telechecker/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     async def delete_messages(self, messages: List[Message]):
         async def delete(m: Message):
             try:
                 await m.delete(revoke=True)
                 text = m.text or m.caption or "图片或其他内容"
                 text = truncate_str(text.replace("\n", ""), 30)
-                self.log.debug(f"[gray50]删除了API消息记录: {text}[/]")
+                self.log.debug(f"[gray50]删除了 API 消息记录: {text}[/]")
             except asyncio.CancelledError:
                 pass
 
         return await asyncio.gather(*[delete(m) for m in messages])
 
     async def post(
         self, cmd, condition: Callable = None, timeout: int = 5, retries=3, name: str = None
```

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/log.py` & `embykeeper-2.3.0/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/main.py` & `embykeeper-2.3.0/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/messager/base.py` & `embykeeper-2.3.0/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/messager/common.py` & `embykeeper-2.3.0/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.3.0/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.3.0/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.3.0/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.3.0/embykeeper/telechecker/monitor/misty.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 
 from pyrogram.types import Message
 from PIL import Image
 from ddddocr import DdddOcr
 
 from ...utils import async_partial
 from ...data import get_datas
+from ..lock import misty_locks
 from .base import Monitor
 
+misty_monitor_pool = {}
+
 
 class MistyMonitor(Monitor):
     ocr = "digit5-teko@v1"
     lock = asyncio.Lock()
 
     name = "Misty"
     chat_name = "FreeEmbyGroup"
@@ -32,61 +35,75 @@
                         return False
                     else:
                         data.append(p)
                 self.__class__.ocr = DdddOcr(
                     show_ad=False, import_onnx_path=str(data[0]), charsets_path=str(data[1])
                 )
 
+        misty_monitor_pool[self.client.me.id] = self
         self.captcha = None
         self.log.info(f"正在初始化机器人状态.")
         wr = async_partial(self.client.wait_reply, self.bot_username)
-        for _ in range(20 if initial else 3):
-            try:
-                msg: Message = await wr("/cancel")
-                if msg.caption and "选择您要使用的功能" in msg.caption or msg.text:
-                    msg = await wr("🌏切换服务器")
-                    if "选择您要使用的服务器" in msg.text or msg.caption:
+        misty_locks.setdefault(self.client.me.id, asyncio.Lock())
+        lock = misty_locks.get(self.client.me.id, None)
+        async with lock:
+            for _ in range(20 if initial else 3):
+                try:
+                    msg: Message = await wr("/cancel")
+                    if "选择您要使用的功能" in (msg.caption or msg.text):
+                        await asyncio.sleep(1)
+                        msg = await wr("🌏切换服务器")
+                    if "选择您要使用的服务器" in (msg.text or msg.caption):
+                        await asyncio.sleep(1)
                         msg = await wr("✨Misty")
-                        if "选择您要使用的功能" in msg.caption or msg.text:
-                            msg = await wr("⚡️账号功能")
-                if msg.text and "请选择功能" in msg.text or msg.caption:
-                    msg = await wr("⚡️注册账号")
-                    if "请输入验证码" in msg.caption or msg.text:
-                        data = await self.client.download_media(msg, in_memory=True)
-                        image = Image.open(data)
-                        self.captcha = (
-                            self.ocr.classification(image)
-                            .translate(str.maketrans("", "", string.punctuation))
-                            .replace(" ", "")
-                        )
-                        self.log.debug(f"接收到验证码: {self.captcha}")
-            except (asyncio.TimeoutError, TypeError):
-                continue
-            else:
-                if self.captcha and len(self.captcha) == 5:
-                    self.log.info(f"机器人状态初始化完成, 当接收到邀请码时将输入验证码 {self.captcha} 以抢注, 请勿操作 @EmbyMistyBot.")
-                    return True
+                    if "选择您要使用的功能" in (msg.caption or msg.text):
+                        await asyncio.sleep(1)
+                        msg = await wr("⚡️账号功能")
+                    if "请选择功能" in (msg.text or msg.caption):
+                        await asyncio.sleep(1)
+                        msg = await wr("⚡️注册账号")
+                        if "请输入验证码" in (msg.caption or msg.text):
+                            data = await self.client.download_media(msg, in_memory=True)
+                            image = Image.open(data)
+                            self.captcha = (
+                                self.ocr.classification(image)
+                                .translate(str.maketrans("", "", string.punctuation))
+                                .replace(" ", "")
+                            )
+                            self.log.debug(f"接收到验证码: {self.captcha}")
+                except (asyncio.TimeoutError, TypeError):
+                    continue
                 else:
-                    self.log.info(f"机器人状态初始化失败, 正在重试.")
-        else:
-            self.log.bind(notify=True).warning(f"机器人状态初始化失败, 监控将停止.")
-            return False
+                    if self.captcha and len(self.captcha) == 5:
+                        self.log.info(f"机器人状态初始化完成, 当接收到邀请码时将输入验证码 {self.captcha} 以抢注, 请勿操作 @EmbyMistyBot.")
+                        return True
+                    else:
+                        self.log.info(f"机器人状态初始化失败, 正在重试.")
+            else:
+                self.log.bind(notify=True).warning(f"机器人状态初始化失败, 监控将停止.")
+                return False
 
     async def on_trigger(self, message: Message, keys, reply):
         wr = async_partial(self.client.wait_reply, self.bot_username)
-        for _ in range(3):
-            msg = await wr(self.captcha)
-            if "验证码错误" in msg.text:
-                self.log.info(f"验证码错误, 将重新初始化.")
-                if not await self.init():
-                    return
-            elif "暂时停止注册" in msg.text:
-                self.log.info(f"注册名额已满, 将进行重试.")
-                if not await self.init():
-                    return
-            elif "用户名" in msg.text:
-                msg = await wr(self.unique_name)
-                if "密码" in msg.text:
-                    await self.client.send_message(self.bot_username, "/cancel")
-                    self.log.bind(notify=True).info(f'已向Bot发送用户注册申请: "{self.unique_name}", 请检查结果.')
-        else:
-            self.log.info(f"未成功, 结束注册申请.")
+        misty_locks.setdefault(self.client.me.id, asyncio.Lock())
+        lock = misty_locks.get(self.client.me.id, None)
+        async with lock:
+            for _ in range(3):
+                try:
+                    msg = await wr(self.captcha)
+                    if "验证码错误" in msg.text:
+                        self.log.info(f"验证码错误, 将重新初始化.")
+                        if not await self.init():
+                            return
+                    elif "暂时停止注册" in msg.text:
+                        self.log.info(f"注册名额已满, 将进行重试.")
+                        if not await self.init():
+                            return
+                    elif "用户名" in msg.text:
+                        msg = await wr(self.unique_name)
+                        if "密码" in msg.text:
+                            await self.client.send_message(self.bot_username, "/cancel")
+                            self.log.bind(notify=True).info(f'已向Bot发送用户注册申请: "{self.unique_name}", 请检查结果.')
+                except asyncio.TimeoutError:
+                    pass
+            else:
+                self.log.info(f"未成功, 结束注册申请.")
```

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.3.0/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.3.0/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.3.0/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.3.0/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper/telechecker/tele.py` & `embykeeper-2.3.0/embykeeper/telechecker/tele.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from collections import OrderedDict
+from contextlib import asynccontextmanager
 
 from datetime import datetime
 import asyncio
 import inspect
 from typing import AsyncGenerator, Optional, Union
 
 from rich.prompt import Prompt
@@ -122,20 +123,20 @@
                                     self.client.executor, handler.callback, self.client, *args
                                 )
                         except pyrogram.StopPropagation:
                             raise
                         except pyrogram.ContinuePropagation:
                             continue
                         except Exception as e:
-                            logger.opt(exception=e).error(f"Update callback error: {e}")
+                            logger.opt(exception=e).error("更新回调函数内发生错误:")
                         break
             except pyrogram.StopPropagation:
                 pass
             except Exception as e:
-                logger.opt(exception=e).error(f"Update handling error: {e}")
+                logger.opt(exception=e).error("更新控制器错误:")
 
 
 class Client(pyrogram.Client):
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
         self.cache = Cache()
         self.dispatcher = Dispatcher(self)
@@ -275,34 +276,39 @@
                 yield dialog
 
                 current += 1
 
                 if current >= total:
                     return
 
-    async def wait_reply(
-        self, chat_id: Union[int, str], text: str = None, timeout: float = 3, outgoing=False
-    ):
+    @asynccontextmanager
+    async def catch_reply(self, chat_id: Union[int, str], outgoing=False):
         async def handler_func(client, message, future: asyncio.Future):
             future.set_result(message)
 
         future = asyncio.Future()
         filter = filters.chat(chat_id)
         if not outgoing:
             filter = filter & (~filters.outgoing)
         handler = MessageHandler(async_partial(handler_func, future=future), filter)
         await self.add_handler(handler, group=0)
         try:
-            if text:
-                await self.send_message(chat_id, text)
-            msg: types.Message = await asyncio.wait_for(future, timeout)
-            return msg
+            yield future
         finally:
             self.remove_handler(handler, group=0)
 
+    async def wait_reply(
+        self, chat_id: Union[int, str], send: str = None, timeout: float = 10, outgoing=False
+    ):
+        async with self.catch_reply(chat_id=chat_id, outgoing=outgoing) as f:
+            if send:
+                await self.send_message(chat_id, send)
+            msg: types.Message = await asyncio.wait_for(f, timeout)
+            return msg
+
     async def mute_chat(self, chat_id: Union[int, str], until: Union[int, datetime]):
         if isinstance(until, datetime):
             until = until.timestamp()
 
         return await self.invoke(
             raw.functions.account.UpdateNotifySettings(
                 peer=raw.types.InputNotifyPeer(peer=await self.resolve_peer(chat_id)),
```

### Comparing `embykeeper-2.2.9/embykeeper/utils.py` & `embykeeper-2.3.0/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.3.0/embykeeper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.9
+Version: 2.3.0
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,40 +36,40 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/7Q7MzwYT) 获得社区帮助.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Discord](https://discord.gg/QCVhBT5y) 获得社区帮助.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
 
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
-  - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
+  - Misty: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
+  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
-    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
-    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-    - ~~EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)~~ (停止签到)
+    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (关服)
+    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (关服)
+    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (关服)
 - Emby 保活
-
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
 
   - 默认禁用:
     - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
@@ -91,27 +90,27 @@
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 
 请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
 
-#### 其他免费 Pass
+#### 其他免费 PaaS
 
 您也可以通过 [Patr.cloud](https://app.patr.cloud/) ([教程](https://blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) 等平台进行部署.
 
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考, 若您只需要进行机器人签到或 Emby 模拟观看, 您也可以只填写 `telegram` 部分或 `emby` 部分):
 
 ```toml
 [[telegram]]
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
@@ -124,14 +123,43 @@
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 ```
 
+<details>
+<summary>查看带代理的完整配置</summary>
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+
+[[telegram]]
+phone = "+8612109347899"
+
+[[emby]]
+url = "https://weiss-griffin.com/"
+username = "carrie19"
+password = "s*D7MMCpS$"
+```
+
+</details>
+
+若您需要启用某些默认禁用的站点, 或是关闭某些默认启用的站点, 请取消注释并修改:
+
+```toml
+[service]
+checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby", "singularity", "terminus"]
+monitor = ["bgk", "embyhub", "misty", "pornemby", "viper"]
+messager = []
+```
+
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -230,32 +258,29 @@
 pip install -U embykeeper
 ```
 
 然后重新运行应用.
 
 ### 从源码构建
 
-首先拉取并设置环境:
+拉取并设置环境:
 
 ```bash
 git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-python -m venv venv
-. ./venv/bin/activate
-pip install -e .
+make install && make run
 ```
 
-然后即可执行 Embykeeper:
+详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+
+若您需要通过 [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-tutorial-commands.html) 部署自启动服务, 您可以在成功运行一次后执行:
 
 ```bash
-embykeeper
+make systemd
 ```
 
-详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
-
 当版本更新时, 您需要执行:
 
 ```
 git pull
 ```
 
 然后重新运行应用.
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.9 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.3.0 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: <3.11,>=3.8
-Description-Content-Type: text/markdown License-File: LICENSE [![build status]
-(https://img.shields.io/github/actions/workflow/status/embykeeper/embykeeper/
-ci.yml?branch=main)](https://github.com/embykeeper/embykeeper/commits/main) [!
-[pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/
-project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE [![build status](https://img.shields.io/github/actions/workflow/status/
+embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/
+embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/
+embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://
+img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
@@ -39,46 +39,46 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
-æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/7Q7MzwYT) è·å¾ç¤¾åºå¸®å©.
+æ¨ä¹å¯ä»¥éè¿ [Discord](https://discord.gg/QCVhBT5y) è·å¾ç¤¾åºå¸®å©.
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
 æºå¨äººç­¾å° - å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https:/
 /t.me/Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot) - ç»ç¹ç«: [é¢é]
 (https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
-t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
-(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
-(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
+t.me/EmbyPublicBot) - Singularity: [é¢é](https://t.me/
 Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
 [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
 peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
 t.me/peach_emby_bot) - Pornemby: [é¢é](https://t.me/pornembyservice)
 [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
 åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
 t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
-t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - Misty: [é¢é]
+(https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby) [æºå¨äºº]
+(https://t.me/EmbyMistyBot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»]
+(https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ - å¶ä»é Emby
 ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
 pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: - ~~BlueSea:
 [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~
-(æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
-(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~
-(æ ååº) - ~~EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
-emby_hub) [æºå¨äºº](https://t.me/EdHubot)~~ (åæ­¢ç­¾å°) - Emby ä¿æ´» -
-å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
-èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+(å³æ) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»]
+(https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (å³æ)
+- Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/
+NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot) (å³æ) - Emby
+ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
 [é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
 åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
@@ -94,28 +94,38 @@
 å¨çº¿é¨ç½² #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
 deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
 [Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
 tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
 è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
-å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ Pass
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». #### å¶ä»åè´¹ PaaS
 æ¨ä¹å¯ä»¥éè¿ [Patr.cloud](https://app.patr.cloud/) ([æç¨](https://
 blog.iair.top/2023/06/26/embykeeper-patr-tutorial/)) ç­å¹³å°è¿è¡é¨ç½². ###
 éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£
 docker](https://yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡:
 ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/
 embykeeper ``` å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml`
 æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
-(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
-"+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè,
+è¥æ¨åªéè¦è¿è¡æºå¨äººç­¾å°æ Emby æ¨¡æè§ç,
+æ¨ä¹å¯ä»¥åªå¡«å `telegram` é¨åæ `emby` é¨å): ```toml [[telegram]]
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
 "carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
 `config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
-port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
-run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+port = 1080 scheme = "socks5" ```  æ¥çå¸¦ä»£ççå®æ´éç½® ```toml
+[proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] phone
+= "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ```
+è¥æ¨éè¦å¯ç¨æäºé»è®¤ç¦ç¨çç«ç¹,
+ææ¯å³é­æäºé»è®¤å¯ç¨çç«ç¹, è¯·åæ¶æ³¨éå¹¶ä¿®æ¹: ```toml
+[service] checkiner = ["charon", "jms", "ljyy", "misty", "peach", "pornemby",
+"singularity", "terminus"] monitor = ["bgk", "embyhub", "misty", "pornemby",
+"viper"] messager = [] ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -
+v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
@@ -147,26 +157,28 @@
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
-```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
-python -m venv venv . ./venv/bin/activate pip install -e . ```
-ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§
-[éè¿ Docker é¨ç½²](https://github.com/embykeeper/
-embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
-æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
-h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
-config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
-c å¯ç¨æ¯æ¥ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --
-emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º æåå¹¶è®¾ç½®ç¯å¢: ```bash
+git clone https://github.com/embykeeper/embykeeper.git make install && make run
+``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [éè¿ Docker é¨ç½²](https://github.com/
+embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+è¥æ¨éè¦éè¿ [systemd](https://www.ruanyifeng.com/blog/2016/03/systemd-
+tutorial-commands.html) é¨ç½²èªå¯å¨æå¡,
+æ¨å¯ä»¥å¨æåè¿è¡ä¸æ¬¡åæ§è¡: ```bash make systemd ```
+å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
+## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
+```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
 basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® --public å¯ç¨å¨çº¿é¨ç½²æ¨¡å¼ ```
 ä¾å¦: ```bash # å¯å¨ææåè½
```

### Comparing `embykeeper-2.2.9/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.3.0/embykeeper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 embykeeper.egg-info/requires.txt
 embykeeper.egg-info/top_level.txt
 embykeeper/embywatcher/__init__.py
 embykeeper/embywatcher/emby.py
 embykeeper/embywatcher/main.py
 embykeeper/telechecker/__init__.py
 embykeeper/telechecker/link.py
+embykeeper/telechecker/lock.py
 embykeeper/telechecker/log.py
 embykeeper/telechecker/main.py
 embykeeper/telechecker/tele.py
 embykeeper/telechecker/bots/__init__.py
 embykeeper/telechecker/bots/base.py
 embykeeper/telechecker/bots/bluesea.py
 embykeeper/telechecker/bots/charon.py
 embykeeper/telechecker/bots/embyhub.py
 embykeeper/telechecker/bots/jms.py
 embykeeper/telechecker/bots/jms_iptv.py
 embykeeper/telechecker/bots/ljyy.py
+embykeeper/telechecker/bots/misty.py
 embykeeper/telechecker/bots/nebula.py
 embykeeper/telechecker/bots/peach.py
 embykeeper/telechecker/bots/pornemby.py
 embykeeper/telechecker/bots/singularity.py
 embykeeper/telechecker/bots/sssq.py
 embykeeper/telechecker/bots/terminus.py
 embykeeper/telechecker/bots/test.py
```

### Comparing `embykeeper-2.2.9/embykeeperweb/app.py` & `embykeeper-2.3.0/embykeeperweb/app.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/404.html` & `embykeeper-2.3.0/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.3.0/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.3.0/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-2.3.0/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.3.0/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.3.0/embykeeperweb/templates/assets/js/console.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.3.0/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/console.html` & `embykeeper-2.3.0/embykeeperweb/templates/console.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/embykeeperweb/templates/login.html` & `embykeeper-2.3.0/embykeeperweb/templates/login.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.9/pyproject.toml` & `embykeeper-2.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.2.9"
+version = "2.3.0"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
@@ -22,15 +22,14 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Environment :: Web Environment",
     "Intended Audience :: End Users/Desktop",
     "Natural Language :: Chinese (Simplified)",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.8,<3.11"
 dependencies = [
     "tomli",
@@ -44,15 +43,15 @@
     "aiohttp",
     "aiohttp_socks",
     "python-dateutil",
     "ddddocr",
     "embypy",
     "pyrogram",
     "tgcrypto",
-    "pillow",
+    "pillow<10.0.0",
     "thefuzz[speedup]",
     "schema",
     "aiocache",
     "fake_useragent",
     "pycryptodome",
     "flask",
     "flask_socketio",
```

### Comparing `embykeeper-2.2.9/tests/test_cli.py` & `embykeeper-2.3.0/tests/test_cli.py`

 * *Files identical despite different names*

