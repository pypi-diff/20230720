# Comparing `tmp/ipwb-0.2023.3.12.2026.tar.gz` & `tmp/ipwb-0.2023.7.20.2112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipwb-0.2023.3.12.2026.tar", last modified: Sun Mar 12 20:27:29 2023, max compression
+gzip compressed data, was "ipwb-0.2023.7.20.2112.tar", last modified: Thu Jul 20 21:13:54 2023, max compression
```

## Comparing `ipwb-0.2023.3.12.2026.tar` & `ipwb-0.2023.7.20.2112.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-12 20:27:29.649886 ipwb-0.2023.3.12.2026/
--rw-r--r--   0 runner    (1001) docker     (116)     1117 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    14994 2023-03-12 20:27:29.649886 ipwb-0.2023.3.12.2026/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    13810 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-12 20:27:29.641885 ipwb-0.2023.3.12.2026/ipwb/
--rw-r--r--   0 runner    (1001) docker     (116)       34 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6076 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-12 20:27:29.645885 ipwb-0.2023.3.12.2026/ipwb/assets/
--rw-r--r--   0 runner    (1001) docker     (116)      871 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/admin.css
--rw-r--r--   0 runner    (1001) docker     (116)      711 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/daemonController.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-12 20:27:29.645885 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/
--rw-r--r--   0 runner    (1001) docker     (116)     2561 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (116)     2347 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (116)      231 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (116)      418 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (116)      585 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (116)    15086 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      186 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/manifest.json
--rw-r--r--   0 runner    (1001) docker     (116)     1718 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (116)     7019 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/favicons/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (116)    19972 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (116)    15933 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/reconstructive-banner.js
--rw-r--r--   0 runner    (1001) docker     (116)     7965 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/reconstructive.js
--rw-r--r--   0 runner    (1001) docker     (116)     1695 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/serviceWorker.js
--rw-r--r--   0 runner    (1001) docker     (116)     2607 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/webui.css
--rw-r--r--   0 runner    (1001) docker     (116)     9489 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/assets/webui.js
--rw-r--r--   0 runner    (1001) docker     (116)     2716 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/backends.py
--rw-r--r--   0 runner    (1001) docker     (116)     1008 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)       97 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    13291 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/indexer.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    38742 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/replay.py
--rw-r--r--   0 runner    (1001) docker     (116)      760 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-12 20:27:29.645885 ipwb-0.2023.3.12.2026/ipwb/templates/
--rw-r--r--   0 runner    (1001) docker     (116)     2476 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/templates/admin.html
--rw-r--r--   0 runner    (1001) docker     (116)     3071 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (116)     9220 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/ipwb/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-12 20:27:29.645885 ipwb-0.2023.3.12.2026/ipwb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    14994 2023-03-12 20:27:29.000000 ipwb-0.2023.3.12.2026/ipwb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1277 2023-03-12 20:27:29.000000 ipwb-0.2023.3.12.2026/ipwb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-12 20:27:29.000000 ipwb-0.2023.3.12.2026/ipwb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2023-03-12 20:27:29.000000 ipwb-0.2023.3.12.2026/ipwb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-12 20:27:29.000000 ipwb-0.2023.3.12.2026/ipwb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      134 2023-03-12 20:27:29.000000 ipwb-0.2023.3.12.2026/ipwb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2023-03-12 20:27:29.000000 ipwb-0.2023.3.12.2026/ipwb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       95 2023-03-12 20:27:29.649886 ipwb-0.2023.3.12.2026/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-12 20:27:29.645885 ipwb-0.2023.3.12.2026/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     2239 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/testUtil.py
--rw-r--r--   0 runner    (1001) docker     (116)     1967 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (116)      340 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_compile_target_uri.py
--rw-r--r--   0 runner    (1001) docker     (116)      557 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)      965 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (116)     1559 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_ipfs_client.py
--rw-r--r--   0 runner    (1001) docker     (116)    12932 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_memento.py
--rw-r--r--   0 runner    (1001) docker     (116)      354 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_nodeToNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1684 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_randomized_add.py
--rw-r--r--   0 runner    (1001) docker     (116)     6793 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (116)     1221 2023-03-12 20:27:27.000000 ipwb-0.2023.3.12.2026/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 21:13:54.594590 ipwb-0.2023.7.20.2112/
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    14967 2023-07-20 21:13:54.594590 ipwb-0.2023.7.20.2112/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13810 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 21:13:54.586590 ipwb-0.2023.7.20.2112/ipwb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6738 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 21:13:54.590590 ipwb-0.2023.7.20.2112/ipwb/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/admin.css
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/daemonController.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 21:13:54.590590 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7019 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/favicons/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    19972 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)    15933 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/reconstructive-banner.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7965 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/reconstructive.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1695 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/serviceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/webui.css
+-rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/assets/webui.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13291 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/indexer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    38846 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/replay.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 21:13:54.594590 ipwb-0.2023.7.20.2112/ipwb/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2476 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/templates/admin.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3071 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     9385 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/ipwb/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 21:13:54.586590 ipwb-0.2023.7.20.2112/ipwb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14967 2023-07-20 21:13:54.000000 ipwb-0.2023.7.20.2112/ipwb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-07-20 21:13:54.000000 ipwb-0.2023.7.20.2112/ipwb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 21:13:54.000000 ipwb-0.2023.7.20.2112/ipwb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 21:13:54.000000 ipwb-0.2023.7.20.2112/ipwb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 21:13:54.000000 ipwb-0.2023.7.20.2112/ipwb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-20 21:13:54.000000 ipwb-0.2023.7.20.2112/ipwb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-20 21:13:54.000000 ipwb-0.2023.7.20.2112/ipwb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-20 21:13:54.594590 ipwb-0.2023.7.20.2112/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2158 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 21:13:54.594590 ipwb-0.2023.7.20.2112/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/testUtil.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_compile_target_uri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_ipfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12932 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_memento.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_nodeToNode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_randomized_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6793 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-07-20 21:13:51.000000 ipwb-0.2023.7.20.2112/tests/test_util.py
```

### Comparing `ipwb-0.2023.3.12.2026/LICENSE` & `ipwb-0.2023.7.20.2112/LICENSE`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/PKG-INFO` & `ipwb-0.2023.7.20.2112/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: ipwb
-Version: 0.2023.3.12.2026
+Version: 0.2023.7.20.2112
 Summary: InterPlanetary Wayback (ipwb): Web Archive integration with IPFS
 Home-page: https://github.com/oduwsdl/ipwb
 Download-URL: https://github.com/oduwsdl/ipwb
 Author: Mat Kelly
 Author-email: me@matkelly.com
 License: MIT
 Keywords: http web archives ipfs distributed odu wayback memento
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: Utilities
 Provides: ipwb
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![image](https://github.com/oduwsdl/ipwb/raw/master/docs/logo_stroked_400px.png)](https://pypi.python.org/pypi/ipwb)
 
 # InterPlanetary Wayback (ipwb)
 
@@ -49,15 +49,15 @@
 
 An important aspect of archival replay systems is rewriting various resource references for proper memento reconstruction so that they are dereferenced properly from the archive from around the same datetime as of the root memento and not from the live site (in which case the resource might have changed or gone missing). Many archival replay systems perform server-side rewriting, but it has its limitations when URIs are generated using JavaScript. To handle this we use [Service Worker](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API) for rerouting requests on the client-side when they are dereferenced to avoid any server-side rewiring. For this, we have implemented a separate library, [Reconstructive](https://oduwsdl.github.io/Reconstructive/), which is reusable and extendable by any archival replay system.
 
 Another important feature of archival replays is the inclusion of an archival banner in mementos. The purpose of an archival banner is to highlight that a replayed page is a memento and not a live page, to provide metadata about the memento and the archive, and to facilitate additional interactivity. Many archival banners used in different web archival replay systems are obtrusive in nature and have issues like style leakage. To eliminate both of these issues we have implemented a [Custom HTML Element](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_custom_elements), [<reconstructive-banner>](https://oduwsdl.github.io/Reconstructive/docs/class/Reconstructive/reconstructive-banner.js~ReconstructiveBanner.html) as part of the [Reconstructive](https://oduwsdl.github.io/Reconstructive/) library and used in the ipwb.
 
 ## Installing
 
-InterPlanetary Wayback (ipwb) requires Python 3.7+. ipwb can also be used with Docker ([see below](#user-content-using-docker)).
+InterPlanetary Wayback (ipwb) requires Python 3.8+. ipwb can also be used with Docker ([see below](#user-content-using-docker)).
 
 For conventional usage, the latest release of ipwb can be installed using pip:
 
 ```
 $ pip install ipwb
 ```
```

### Comparing `ipwb-0.2023.3.12.2026/README.md` & `ipwb-0.2023.7.20.2112/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 An important aspect of archival replay systems is rewriting various resource references for proper memento reconstruction so that they are dereferenced properly from the archive from around the same datetime as of the root memento and not from the live site (in which case the resource might have changed or gone missing). Many archival replay systems perform server-side rewriting, but it has its limitations when URIs are generated using JavaScript. To handle this we use [Service Worker](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API) for rerouting requests on the client-side when they are dereferenced to avoid any server-side rewiring. For this, we have implemented a separate library, [Reconstructive](https://oduwsdl.github.io/Reconstructive/), which is reusable and extendable by any archival replay system.
 
 Another important feature of archival replays is the inclusion of an archival banner in mementos. The purpose of an archival banner is to highlight that a replayed page is a memento and not a live page, to provide metadata about the memento and the archive, and to facilitate additional interactivity. Many archival banners used in different web archival replay systems are obtrusive in nature and have issues like style leakage. To eliminate both of these issues we have implemented a [Custom HTML Element](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_custom_elements), [<reconstructive-banner>](https://oduwsdl.github.io/Reconstructive/docs/class/Reconstructive/reconstructive-banner.js~ReconstructiveBanner.html) as part of the [Reconstructive](https://oduwsdl.github.io/Reconstructive/) library and used in the ipwb.
 
 ## Installing
 
-InterPlanetary Wayback (ipwb) requires Python 3.7+. ipwb can also be used with Docker ([see below](#user-content-using-docker)).
+InterPlanetary Wayback (ipwb) requires Python 3.8+. ipwb can also be used with Docker ([see below](#user-content-using-docker)).
 
 For conventional usage, the latest release of ipwb can be installed using pip:
 
 ```
 $ pip install ipwb
 ```
```

### Comparing `ipwb-0.2023.3.12.2026/ipwb/__main__.py` & `ipwb-0.2023.7.20.2112/ipwb/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import argparse
 import os
 import random  # For generating a temp file for stdin
 # import string  # For generating a temp file for stdin
 import sys
 import tempfile
 
+from multiaddr import Multiaddr
+from multiaddr import exceptions as multiaddr_exceptions
 # ipwb modules
 from ipwb import settings, replay, indexer, util
 from ipwb.error_handler import exception_logger
-from .__init__ import __version__ as ipwb_version
+from ipwb.__init__ import __version__ as ipwb_version
 
 
 @exception_logger(catch=not settings.DEBUG)
 def main():
     check_args(sys.argv)
 
 
-def check_args_index(args):
+def checkArgs_index(args):
+    # args.daemon_address is always set. Either default or by CLI
+    try:
+        # see if it parses
+        daemon = Multiaddr(args.daemon_address)
+    except multiaddr_exceptions.StringParseError as e:
+        print("Daemon address cannot be parsed")
+        raise e
+    settings.App.set("ipfsapi", str(daemon))
+
     util.check_daemon_is_alive()
 
     enc_key = None
     compression_level = None
     if args.e:
         enc_key = ''
     if args.c:
@@ -53,14 +64,21 @@
 
         supplied_index_parameter = True
 
     proxy = None
     if hasattr(args, 'proxy') and args.proxy is not None:
         print(f'Proxying to {args.proxy}')
         proxy = args.proxy
+    try:
+        # see if it parses
+        daemon = Multiaddr(args.daemon_address)
+    except multiaddr_exceptions.StringParseError as e:
+        print("Daemon address cannot be parsed")
+        raise e
+    settings.App.set("ipfsapi", str(daemon))
 
     port = replay.IPWBREPLAY_PORT
     if hasattr(args, 'port') and args.port is not None:
         print(f'Using custom port {args.port} for replay.')
         port = args.port
 
     # TODO: add any other sub-arguments for replay here
@@ -147,15 +165,15 @@
     replay_parser.set_defaults(func=check_args_replay,
                                onError=replay_parser.print_help)
 
     parser.add_argument(
         '-d', '--daemon',
         help=("Multi-address of IPFS daemon "
               "(default /dns/localhost/tcp/5001/http)"),
-        default=util.IPFSAPI_MUTLIADDRESS,
+        default=settings.App.config("ipfsapi"),
         dest='daemon_address')
     parser.add_argument(
         '-v', '--version', help='Report the version of ipwb', action='version',
         version=f'InterPlanetary Wayback {ipwb_version}')
     parser.add_argument(
         '-u', '--update-check',
         action='store_true',
```

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/admin.css` & `ipwb-0.2023.7.20.2112/ipwb/assets/admin.css`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/daemonController.js` & `ipwb-0.2023.7.20.2112/ipwb/assets/daemonController.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/favicons/android-chrome-192x192.png` & `ipwb-0.2023.7.20.2112/ipwb/assets/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/favicons/apple-touch-icon.png` & `ipwb-0.2023.7.20.2112/ipwb/assets/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/favicons/favicon-32x32.png` & `ipwb-0.2023.7.20.2112/ipwb/assets/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/favicons/favicon.ico` & `ipwb-0.2023.7.20.2112/ipwb/assets/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/favicons/mstile-150x150.png` & `ipwb-0.2023.7.20.2112/ipwb/assets/favicons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/favicons/safari-pinned-tab.svg` & `ipwb-0.2023.7.20.2112/ipwb/assets/favicons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/logo.png` & `ipwb-0.2023.7.20.2112/ipwb/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/reconstructive-banner.js` & `ipwb-0.2023.7.20.2112/ipwb/assets/reconstructive-banner.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/reconstructive.js` & `ipwb-0.2023.7.20.2112/ipwb/assets/reconstructive.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/serviceWorker.js` & `ipwb-0.2023.7.20.2112/ipwb/assets/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/webui.css` & `ipwb-0.2023.7.20.2112/ipwb/assets/webui.css`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/assets/webui.js` & `ipwb-0.2023.7.20.2112/ipwb/assets/webui.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/backends.py` & `ipwb-0.2023.7.20.2112/ipwb/backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 from typing import Optional
 from urllib.parse import urlparse
 
 import ipfshttpclient
 import requests
 
-from ipwb import util
+from ipwb import util, settings
 
 
 @dataclasses.dataclass(frozen=True)
 class BackendError(Exception):
     backend_name: str
 
     def __str__(self):
@@ -31,15 +31,15 @@
     """Fetch CDXJ file content from IPFS by hash."""
     ipfs_hash = format_ipfs_cid(path)
 
     if ipfs_hash is None:
         return None
 
     try:
-        with ipfshttpclient.connect(util.IPFSAPI_MUTLIADDRESS) as client:
+        with ipfshttpclient.connect(settings.App.config("ipfsapi")) as client:
             return client.cat(path).decode('utf-8')
 
     except ipfshttpclient.exceptions.StatusError as err:
         raise BackendError(backend_name='ipfs') from err
 
 
 def fetch_web_index(path: str) -> Optional[str]:
```

### Comparing `ipwb-0.2023.3.12.2026/ipwb/error_handler.py` & `ipwb-0.2023.7.20.2112/ipwb/error_handler.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/indexer.py` & `ipwb-0.2023.7.20.2112/ipwb/indexer.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/replay.py` & `ipwb-0.2023.7.20.2112/ipwb/replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 
 import base64
 
 from werkzeug.routing import BaseConverter
 from .__init__ import __version__ as ipwb_version
+from . import settings
 
 
 from flask import flash
 from werkzeug.utils import secure_filename
 from flask import send_from_directory
 from flask import make_response
 
@@ -132,28 +133,31 @@
 
 class UnsupportedIPFSVersions(Exception):
     pass
 
 
 @app.route('/ipfsdaemon/<cmd>')
 def command_daemon(cmd):
+    local_daemon = ipwb_utils.is_localhosty(settings.App.config("ipfsapi"))
+
     if cmd == 'status':
         return generate_daemon_status_button()
     elif cmd == 'version':
         return request_daemon_version_via_http()
-    elif cmd == 'start':
+    elif cmd == 'start' and local_daemon:
         subprocess.Popen(['ipfs', 'daemon'])
         return Response('IPFS daemon starting...')
 
-    elif cmd == 'stop':
+    elif cmd == 'stop' and local_daemon:
         try:
             ipfs_version = ipfs_client().version()['Version']
             if ipwb_utils.compare_versions(ipfs_version, '0.4.10') < 0:
                 raise UnsupportedIPFSVersions()
-            ipfs_client().stop()
+
+            ipfs_client().close()
         except (subprocess.CalledProcessError, UnsupportedIPFSVersions) as _:
             if os.name != 'nt':  # Big hammer
                 subprocess.call(['killall', 'ipfs'])
             else:
                 subprocess.call(['taskkill', '/im', 'ipfs.exe', '/F'])
 
         return Response('IPFS daemon stopping...')
@@ -653,15 +657,15 @@
 
     return 'Error', 500
 
 
 @app.route('/ipwbadmin', strict_slashes=False)
 def show_admin():
     status = {'ipwb_version': ipwb_version,
-              'ipfs_endpoint': ipwb_utils.IPFSAPI_MUTLIADDRESS}
+              'ipfs_endpoint': settings.App.config("ipfsapi")}
     index_file = ipwb_utils.get_ipwb_replay_index_path()
 
     memento_info = calculate_memento_info_in_index(index_file)
 
     m_count = memento_info['memento_count']
     unique_urirs = len(memento_info['surt_uris'].keys())
     html_count = memento_info['html_count']
@@ -702,15 +706,15 @@
                'html_count': html_count}
     uris = get_uris_and_datetimes_in_cdxj(index_file)
     return render_template('index.html', summary=summary, uris=uris)
 
 
 def show_uri(path, datetime=None):
     try:
-        ipwb_utils.check_daemon_is_alive(ipwb_utils.IPFSAPI_MUTLIADDRESS)
+        ipwb_utils.check_daemon_is_alive()
 
     except IPFSDaemonNotAvailable:
         err_str = ('IPFS daemon not running. '
                    'Start it using $ ipfs daemon on the command-line '
                    ' or from the <a href="/">'
                    'IPWB replay homepage</a>.')
```

### Comparing `ipwb-0.2023.3.12.2026/ipwb/templates/admin.html` & `ipwb-0.2023.7.20.2112/ipwb/templates/admin.html`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/templates/index.html` & `ipwb-0.2023.7.20.2112/ipwb/templates/index.html`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/ipwb/util.py` & `ipwb-0.2023.7.20.2112/ipwb/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from enum import Enum, auto
 
 from urllib.request import urlopen
 from urllib.error import URLError
 
 import json
 from .__init__ import __version__ as ipwb_version
+from . import settings
 
 from ipfshttpclient.exceptions import ConnectionError, AddressError
 from multiaddr.exceptions import StringParseError
 from pkg_resources import parse_version
 
 from .exceptions import IPFSDaemonNotAvailable
 
@@ -52,36 +53,38 @@
 log = logging.getLogger('werkzeug')
 log.setLevel(logging.ERROR)
 
 
 dt_pattern = re.compile(r"^(\d{4})(\d{2})?(\d{2})?(\d{2})?(\d{2})?(\d{2})?$")
 
 
-def create_ipfs_client(daemonMultiaddr=IPFSAPI_MUTLIADDRESS):
+def create_ipfs_client():
     """Create and return IPFS client."""
+    daemonMultiaddr = settings.App.config("ipfsapi")
     try:
         return ipfshttpclient.Client(daemonMultiaddr)
     except Exception as err:
         raise Exception('Cannot create an IPFS client.') from err
 
 
 @functools.lru_cache()
-def ipfs_client(daemonMultiaddr=IPFSAPI_MUTLIADDRESS):
+def ipfs_client():
     """
     Create and cache IPFS client instance.
 
     Caching is the single difference between this and
     `create_ipfs_client()` above.
     """
-    return create_ipfs_client(daemonMultiaddr)
+    return create_ipfs_client()
 
 
-def check_daemon_is_alive(daemonMultiaddr=IPFSAPI_MUTLIADDRESS):
+def check_daemon_is_alive():
     """Ensure that the IPFS daemon is running via HTTP before proceeding"""
     client = ipfs_client()
+    daemonMultiaddr = settings.App.config("ipfsapi")
 
     try:
         # ConnectionError/AttributeError if IPFS daemon not running
         client.id()
         return True
 
     except ConnectionError as err:
@@ -251,22 +254,24 @@
         ipfs_config_path = os.path.join(
             os.environ.get('IPFS_PATH'), 'config')
 
     with open(ipfs_config_path, 'w') as f:
         f.write(json.dumps(json_to_write, indent=4, sort_keys=True))
 
 
-def get_ipfsapi_host_and_port(ipfs_json=None):
-    if not ipfs_json:
-        ipfs_json = read_ipfs_config()
-
-    (scheme, host, protocol, port) = (
-        ipfs_json['Addresses']['API'][1:].split('/')
-    )
-    return host + ':' + port
+def get_ipfsapi_host_and_port():
+    daemon_address = settings.App.config("ipfsapi")
+    # format right now is "/dns/localhost/tcp/5001/http"
+
+    (scheme, host, protocol, port, protocol2) = daemon_address[1:].split('/')
+    if protocol2 == "https" and port == "443":
+        # if https is used, rely on a 301/302 redirect response
+        return host
+    else:
+        return host + ':' + port
 
 
 def get_ipwb_replay_config(ipfs_json=None):
     if not ipfs_json:
         ipfs_json = read_ipfs_config()
     port = None
     if ('Ipwb' in ipfs_json and 'Replay' in ipfs_json['Ipwb'] and
```

### Comparing `ipwb-0.2023.3.12.2026/ipwb.egg-info/PKG-INFO` & `ipwb-0.2023.7.20.2112/ipwb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: ipwb
-Version: 0.2023.3.12.2026
+Version: 0.2023.7.20.2112
 Summary: InterPlanetary Wayback (ipwb): Web Archive integration with IPFS
 Home-page: https://github.com/oduwsdl/ipwb
 Download-URL: https://github.com/oduwsdl/ipwb
 Author: Mat Kelly
 Author-email: me@matkelly.com
 License: MIT
 Keywords: http web archives ipfs distributed odu wayback memento
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: Utilities
 Provides: ipwb
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![image](https://github.com/oduwsdl/ipwb/raw/master/docs/logo_stroked_400px.png)](https://pypi.python.org/pypi/ipwb)
 
 # InterPlanetary Wayback (ipwb)
 
@@ -49,15 +49,15 @@
 
 An important aspect of archival replay systems is rewriting various resource references for proper memento reconstruction so that they are dereferenced properly from the archive from around the same datetime as of the root memento and not from the live site (in which case the resource might have changed or gone missing). Many archival replay systems perform server-side rewriting, but it has its limitations when URIs are generated using JavaScript. To handle this we use [Service Worker](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API) for rerouting requests on the client-side when they are dereferenced to avoid any server-side rewiring. For this, we have implemented a separate library, [Reconstructive](https://oduwsdl.github.io/Reconstructive/), which is reusable and extendable by any archival replay system.
 
 Another important feature of archival replays is the inclusion of an archival banner in mementos. The purpose of an archival banner is to highlight that a replayed page is a memento and not a live page, to provide metadata about the memento and the archive, and to facilitate additional interactivity. Many archival banners used in different web archival replay systems are obtrusive in nature and have issues like style leakage. To eliminate both of these issues we have implemented a [Custom HTML Element](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_custom_elements), [<reconstructive-banner>](https://oduwsdl.github.io/Reconstructive/docs/class/Reconstructive/reconstructive-banner.js~ReconstructiveBanner.html) as part of the [Reconstructive](https://oduwsdl.github.io/Reconstructive/) library and used in the ipwb.
 
 ## Installing
 
-InterPlanetary Wayback (ipwb) requires Python 3.7+. ipwb can also be used with Docker ([see below](#user-content-using-docker)).
+InterPlanetary Wayback (ipwb) requires Python 3.8+. ipwb can also be used with Docker ([see below](#user-content-using-docker)).
 
 For conventional usage, the latest release of ipwb can be installed using pip:
 
 ```
 $ pip install ipwb
 ```
```

### Comparing `ipwb-0.2023.3.12.2026/ipwb.egg-info/SOURCES.txt` & `ipwb-0.2023.7.20.2112/ipwb.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 ipwb/assets/favicons/mstile-150x150.png
 ipwb/assets/favicons/safari-pinned-tab.svg
 ipwb/templates/admin.html
 ipwb/templates/index.html
 tests/testUtil.py
 tests/test_backends.py
 tests/test_compile_target_uri.py
+tests/test_daemon.py
 tests/test_error_handler.py
 tests/test_indexing.py
 tests/test_ipfs_client.py
 tests/test_memento.py
 tests/test_nodeToNode.py
 tests/test_randomized_add.py
 tests/test_replay.py
```

### Comparing `ipwb-0.2023.3.12.2026/setup.py` & `ipwb-0.2023.7.20.2112/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,25 @@
     version=__version__,
     url='https://github.com/oduwsdl/ipwb',
     download_url="https://github.com/oduwsdl/ipwb",
     author='Mat Kelly',
     author_email='me@matkelly.com',
     description=desc,
     packages=['ipwb'],
+    python_requires='>=3.8',
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     provides=[
         'ipwb'
     ],
     install_requires=[
         'warcio>=1.5.3',
         'ipfshttpclient>=0.8.0a',
-        'Flask==2.0.3',
+        'Flask==2.3.2',
         'pycryptodome>=3.4.11',
         'requests>=2.19.1',
         'beautifulsoup4>=4.6.3',
         'six==1.11.0',
         'surt>=0.3.0'
     ],
     tests_require=[
@@ -52,15 +53,14 @@
     zip_safe=False,
     keywords='http web archives ipfs distributed odu wayback memento',
     classifiers=[
         'Development Status :: 4 - Beta',
 
         'Environment :: Web Environment',
 
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
 
         'License :: OSI Approved :: MIT License',
```

### Comparing `ipwb-0.2023.3.12.2026/tests/testUtil.py` & `ipwb-0.2023.7.20.2112/tests/testUtil.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/tests/test_backends.py` & `ipwb-0.2023.7.20.2112/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/tests/test_error_handler.py` & `ipwb-0.2023.7.20.2112/tests/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/tests/test_indexing.py` & `ipwb-0.2023.7.20.2112/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/tests/test_ipfs_client.py` & `ipwb-0.2023.7.20.2112/tests/test_ipfs_client.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/tests/test_memento.py` & `ipwb-0.2023.7.20.2112/tests/test_memento.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/tests/test_randomized_add.py` & `ipwb-0.2023.7.20.2112/tests/test_randomized_add.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/tests/test_replay.py` & `ipwb-0.2023.7.20.2112/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.3.12.2026/tests/test_util.py` & `ipwb-0.2023.7.20.2112/tests/test_util.py`

 * *Files identical despite different names*

