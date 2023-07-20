# Comparing `tmp/zapf-0.4.6.tar.gz` & `tmp/zapf-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zapf-0.4.6.tar", last modified: Wed Jun 21 09:02:38 2023, max compression
+gzip compressed data, was "zapf-0.4.7.tar", last modified: Thu Jul 20 13:20:01 2023, max compression
```

## Comparing `zapf-0.4.6.tar` & `zapf-0.4.7.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.794714 zapf-0.4.6/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      107 2019-03-25 10:50:41.000000 zapf-0.4.6/.gitignore
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      177 2022-03-14 10:16:20.000000 zapf-0.4.6/.isort.cfg
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    18137 2019-03-25 10:50:41.000000 zapf-0.4.6/LICENSE
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1086 2021-04-22 08:48:58.000000 zapf-0.4.6/Makefile
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1697 2023-06-21 09:02:38.794714 zapf-0.4.6/PKG-INFO
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      907 2021-06-11 14:35:30.000000 zapf-0.4.6/README.rst
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.788714 zapf-0.4.6/debian/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     8596 2023-06-21 09:02:31.000000 zapf-0.4.6/debian/changelog
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        3 2021-04-23 11:05:09.000000 zapf-0.4.6/debian/compat
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      527 2022-05-19 16:40:52.000000 zapf-0.4.6/debian/control
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1178 2021-04-23 11:05:09.000000 zapf-0.4.6/debian/copyright
--rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)      502 2021-04-23 11:05:09.000000 zapf-0.4.6/debian/rules
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.789714 zapf-0.4.6/debian/source/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)       13 2021-04-23 11:05:09.000000 zapf-0.4.6/debian/source/format
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.789714 zapf-0.4.6/doc/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      634 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/Makefile
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.790714 zapf-0.4.6/doc/_static/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)   168539 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/_static/logo.png
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)   427468 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/_static/logo.xcf
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1273 2021-11-12 08:23:59.000000 zapf-0.4.6/doc/conf.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4388 2021-10-21 04:57:33.000000 zapf-0.4.6/doc/device.rst
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      203 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/errors.rst
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      263 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/index.rst
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      987 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/intro.rst
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      407 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/proto.rst
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      316 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/scanner.rst
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     7528 2021-04-23 11:05:09.000000 zapf-0.4.6/pylintrc
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      122 2022-05-12 11:50:21.000000 zapf-0.4.6/pyproject.toml
--rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)       15 2021-06-11 14:35:30.000000 zapf-0.4.6/requirements.txt
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      376 2022-03-14 10:16:16.000000 zapf-0.4.6/scan.py
--rwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)      872 2023-06-21 09:02:38.794714 zapf-0.4.6/setup.cfg
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       57 2022-05-12 11:50:21.000000 zapf-0.4.6/setup.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.791714 zapf-0.4.6/test/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        0 2021-04-22 08:48:58.000000 zapf-0.4.6/test/__init__.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6771 2021-11-08 08:47:11.000000 zapf-0.4.6/test/conftest.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    12169 2022-03-14 10:16:13.000000 zapf-0.4.6/test/test_devices.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3059 2021-11-08 08:47:11.000000 zapf-0.4.6/test/test_scan.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3464 2021-11-12 08:23:59.000000 zapf-0.4.6/test/test_spec.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    25286 2021-11-08 09:47:15.000000 zapf-0.4.6/test/testplc_2015_02.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    48576 2021-11-12 08:23:59.000000 zapf-0.4.6/test/testplc_2021_09.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.791714 zapf-0.4.6/tools/
--rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)     2524 2021-11-19 10:53:12.000000 zapf-0.4.6/tools/sim-standalone.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.792714 zapf-0.4.6/zapf/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        6 2022-05-11 17:22:16.000000 zapf-0.4.6/zapf/RELEASE-VERSION
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1809 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/__init__.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    39161 2023-05-18 05:30:50.000000 zapf-0.4.6/zapf/device.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10601 2022-10-26 05:57:09.000000 zapf-0.4.6/zapf/indexer.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    13837 2023-06-21 07:33:05.000000 zapf-0.4.6/zapf/io.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.793714 zapf-0.4.6/zapf/proto/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2560 2021-04-26 13:20:39.000000 zapf-0.4.6/zapf/proto/__init__.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    16488 2021-11-19 13:08:34.000000 zapf-0.4.6/zapf/proto/ads.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6081 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/proto/modbus.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4117 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/proto/sim.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     5178 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/proto/tango.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    14575 2023-05-18 05:30:50.000000 zapf-0.4.6/zapf/scan.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.793714 zapf-0.4.6/zapf/simulator/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        0 2021-04-26 13:20:39.000000 zapf-0.4.6/zapf/simulator/__init__.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1355 2021-10-11 05:32:57.000000 zapf-0.4.6/zapf/simulator/funcs.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    14573 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/simulator/runtime.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6742 2022-03-14 10:16:16.000000 zapf-0.4.6/zapf/simulator/server.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     5781 2021-11-08 08:44:16.000000 zapf-0.4.6/zapf/simulator/util.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.793714 zapf-0.4.6/zapf/spec/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4114 2021-11-08 08:47:11.000000 zapf-0.4.6/zapf/spec/__init__.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6062 2021-11-17 11:33:49.000000 zapf-0.4.6/zapf/spec/v_2015_02.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    33234 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/spec/v_2021_09.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9820 2022-03-14 10:16:16.000000 zapf-0.4.6/zapf/table.py
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3488 2021-11-08 09:47:15.000000 zapf-0.4.6/zapf/util.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.792714 zapf-0.4.6/zapf.egg-info/
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1697 2023-06-21 09:02:38.000000 zapf-0.4.6/zapf.egg-info/PKG-INFO
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1057 2023-06-21 09:02:38.000000 zapf-0.4.6/zapf.egg-info/SOURCES.txt
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        1 2023-06-21 09:02:38.000000 zapf-0.4.6/zapf.egg-info/dependency_links.txt
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        5 2023-06-21 09:02:38.000000 zapf-0.4.6/zapf.egg-info/top_level.txt
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.067543 zapf-0.4.7/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      107 2019-03-25 10:50:41.000000 zapf-0.4.7/.gitignore
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      177 2022-03-14 10:16:20.000000 zapf-0.4.7/.isort.cfg
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    18137 2019-03-25 10:50:41.000000 zapf-0.4.7/LICENSE
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1086 2021-04-22 08:48:58.000000 zapf-0.4.7/Makefile
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1697 2023-07-20 13:20:01.067543 zapf-0.4.7/PKG-INFO
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      907 2021-06-11 14:35:30.000000 zapf-0.4.7/README.rst
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.061543 zapf-0.4.7/debian/
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     8877 2023-07-20 13:19:53.000000 zapf-0.4.7/debian/changelog
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        3 2021-04-23 11:05:09.000000 zapf-0.4.7/debian/compat
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      527 2022-05-19 16:40:52.000000 zapf-0.4.7/debian/control
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1178 2021-04-23 11:05:09.000000 zapf-0.4.7/debian/copyright
+-rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)      502 2021-04-23 11:05:09.000000 zapf-0.4.7/debian/rules
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.062543 zapf-0.4.7/debian/source/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)       13 2021-04-23 11:05:09.000000 zapf-0.4.7/debian/source/format
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.062543 zapf-0.4.7/doc/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      634 2021-06-11 14:35:30.000000 zapf-0.4.7/doc/Makefile
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.063543 zapf-0.4.7/doc/_static/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)   168539 2021-06-11 14:35:30.000000 zapf-0.4.7/doc/_static/logo.png
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)   427468 2021-06-11 14:35:30.000000 zapf-0.4.7/doc/_static/logo.xcf
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1273 2021-11-12 08:23:59.000000 zapf-0.4.7/doc/conf.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4456 2023-07-03 16:13:31.000000 zapf-0.4.7/doc/device.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      203 2021-06-11 14:35:30.000000 zapf-0.4.7/doc/errors.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      263 2021-06-11 14:35:30.000000 zapf-0.4.7/doc/index.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      987 2021-06-11 14:35:30.000000 zapf-0.4.7/doc/intro.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      407 2021-06-11 14:35:30.000000 zapf-0.4.7/doc/proto.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      316 2021-06-11 14:35:30.000000 zapf-0.4.7/doc/scanner.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     7528 2021-04-23 11:05:09.000000 zapf-0.4.7/pylintrc
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      122 2022-05-12 11:50:21.000000 zapf-0.4.7/pyproject.toml
+-rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)       15 2021-06-11 14:35:30.000000 zapf-0.4.7/requirements.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      376 2022-03-14 10:16:16.000000 zapf-0.4.7/scan.py
+-rwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)      872 2023-07-20 13:20:01.068543 zapf-0.4.7/setup.cfg
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       57 2022-05-12 11:50:21.000000 zapf-0.4.7/setup.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.064543 zapf-0.4.7/test/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        0 2021-04-22 08:48:58.000000 zapf-0.4.7/test/__init__.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6771 2021-11-08 08:47:11.000000 zapf-0.4.7/test/conftest.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    12169 2022-03-14 10:16:13.000000 zapf-0.4.7/test/test_devices.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3059 2021-11-08 08:47:11.000000 zapf-0.4.7/test/test_scan.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3464 2021-11-12 08:23:59.000000 zapf-0.4.7/test/test_spec.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    25286 2021-11-08 09:47:15.000000 zapf-0.4.7/test/testplc_2015_02.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    48576 2021-11-12 08:23:59.000000 zapf-0.4.7/test/testplc_2021_09.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.064543 zapf-0.4.7/tools/
+-rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)     2524 2021-11-19 10:53:12.000000 zapf-0.4.7/tools/sim-standalone.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.065543 zapf-0.4.7/zapf/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        6 2022-05-11 17:22:16.000000 zapf-0.4.7/zapf/RELEASE-VERSION
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1809 2021-11-17 15:35:39.000000 zapf-0.4.7/zapf/__init__.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    39613 2023-07-03 16:13:31.000000 zapf-0.4.7/zapf/device.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10601 2022-10-26 05:57:09.000000 zapf-0.4.7/zapf/indexer.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    14032 2023-07-03 06:42:27.000000 zapf-0.4.7/zapf/io.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.066542 zapf-0.4.7/zapf/proto/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2575 2023-06-23 11:41:03.000000 zapf-0.4.7/zapf/proto/__init__.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    16488 2021-11-19 13:08:34.000000 zapf-0.4.7/zapf/proto/ads.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6081 2021-11-17 15:35:39.000000 zapf-0.4.7/zapf/proto/modbus.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4117 2021-11-17 15:35:39.000000 zapf-0.4.7/zapf/proto/sim.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     5178 2021-11-17 15:35:39.000000 zapf-0.4.7/zapf/proto/tango.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    14680 2023-07-03 16:13:31.000000 zapf-0.4.7/zapf/scan.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.067543 zapf-0.4.7/zapf/simulator/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        0 2021-04-26 13:20:39.000000 zapf-0.4.7/zapf/simulator/__init__.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1355 2021-10-11 05:32:57.000000 zapf-0.4.7/zapf/simulator/funcs.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    14573 2021-11-17 15:35:39.000000 zapf-0.4.7/zapf/simulator/runtime.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6742 2022-03-14 10:16:16.000000 zapf-0.4.7/zapf/simulator/server.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     5781 2021-11-08 08:44:16.000000 zapf-0.4.7/zapf/simulator/util.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.067543 zapf-0.4.7/zapf/spec/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4114 2021-11-08 08:47:11.000000 zapf-0.4.7/zapf/spec/__init__.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6062 2021-11-17 11:33:49.000000 zapf-0.4.7/zapf/spec/v_2015_02.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    33350 2023-07-03 16:13:34.000000 zapf-0.4.7/zapf/spec/v_2021_09.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9820 2022-03-14 10:16:16.000000 zapf-0.4.7/zapf/table.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3488 2021-11-08 09:47:15.000000 zapf-0.4.7/zapf/util.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-07-20 13:20:01.065543 zapf-0.4.7/zapf.egg-info/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1697 2023-07-20 13:20:00.000000 zapf-0.4.7/zapf.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1057 2023-07-20 13:20:01.000000 zapf-0.4.7/zapf.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        1 2023-07-20 13:20:00.000000 zapf-0.4.7/zapf.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        5 2023-07-20 13:20:00.000000 zapf-0.4.7/zapf.egg-info/top_level.txt
```

### Comparing `zapf-0.4.6/LICENSE` & `zapf-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/Makefile` & `zapf-0.4.7/Makefile`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/PKG-INFO` & `zapf-0.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zapf
-Version: 0.4.6
+Version: 0.4.7
 Summary: Client library for the PILS specification
 Home-page: https://forge.frm2.tum.de/review/plugins/gitiles/mlz/pils/zapf
 Author: Georg Brandl
 Author-email: g.brandl@fz-juelich.de
 License: GPL-2.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `zapf-0.4.6/README.rst` & `zapf-0.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/debian/changelog` & `zapf-0.4.7/debian/changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+python-zapf (0.4.7) focal; urgency=medium
+
+  [ Georg Brandl ]
+  * scan: add sim:// to valid addresses
+  * io: add disconnect() API
+
+  [ Enrico Faulhaber ]
+  * spec 2021: access is also ro if no target field
+
+ -- Georg Brandl <jenkins@frm2.tum.de>  Mon, 03 Jul 2023 18:13:44 +0200
+
 python-zapf (0.4.6) focal; urgency=medium
 
   * io: fix missing locked access to proto
 
  -- Georg Brandl <jenkins@frm2.tum.de>  Wed, 21 Jun 2023 09:34:30 +0200
 
 python-zapf (0.4.5) focal; urgency=medium
```

### Comparing `zapf-0.4.6/debian/control` & `zapf-0.4.7/debian/control`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/debian/copyright` & `zapf-0.4.7/debian/copyright`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/doc/Makefile` & `zapf-0.4.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/doc/_static/logo.png` & `zapf-0.4.7/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/doc/_static/logo.xcf` & `zapf-0.4.7/doc/_static/logo.xcf`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/doc/conf.py` & `zapf-0.4.7/doc/conf.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/doc/device.rst` & `zapf-0.4.7/doc/device.rst`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     Maps the PILS :ref:`type code <pils:type-codes>` to a namedtuple with the
     following items:
 
     * ``devcls``: The concrete `Device` subclass to use
     * ``value_fmt``: The basic Python `struct` format for the device values
     * ``num_values``: The number of main values of the device
     * ``has_target``: If the device has one or more "target" fields
+    * ``readonly``: If the device can only be read, not written to.
     * ``status_size``: The size, in bytes, of the device's status fields
     * ``num_params``: The number of parameter fields
     * ``has_pctrl``: Whether this device uses the :ref:`pils:param-ctrl` field
 
     Most of this information is used by the `Device` classes to determine their
     internal layout.
```

### Comparing `zapf-0.4.6/doc/intro.rst` & `zapf-0.4.7/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/pylintrc` & `zapf-0.4.7/pylintrc`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/setup.cfg` & `zapf-0.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/test/conftest.py` & `zapf-0.4.7/test/conftest.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/test/test_devices.py` & `zapf-0.4.7/test/test_devices.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/test/test_scan.py` & `zapf-0.4.7/test/test_scan.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/test/test_spec.py` & `zapf-0.4.7/test/test_spec.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/test/testplc_2015_02.py` & `zapf-0.4.7/test/testplc_2015_02.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/test/testplc_2021_09.py` & `zapf-0.4.7/test/testplc_2021_09.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/tools/sim-standalone.py` & `zapf-0.4.7/tools/sim-standalone.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/__init__.py` & `zapf-0.4.7/zapf/__init__.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/device.py` & `zapf-0.4.7/zapf/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -923,91 +923,93 @@
         if mailbox_state == 1:  # last part transferred
             return replies
         else:
             raise CommError(f'bad mailbox state! expected 1, got {mailbox_state}')
 
 
 # Note: has_target means that a target field is there, not that the device
-# is considered read-only.
+# is considered read-only. For this use readonly....
 Type = namedtuple(
     'Type',
-    'devcls value_fmt num_values has_target status_size num_params has_pctrl')
+    'devcls value_fmt num_values has_target readonly status_size num_params has_pctrl')
 
 
 TYPECODE_MAP = {
-    0x1201: Type(SimpleDiscreteIn,  'h', 1, False, 0, 0, False),
-    0x1202: Type(SimpleDiscreteIn,  'i', 1, False, 0, 0, False),
-    0x1204: Type(SimpleDiscreteIn,  'q', 1, False, 0, 0, False),
-    0x1302: Type(SimpleAnalogIn,    'f', 1, False, 0, 0, False),
-    0x1304: Type(SimpleAnalogIn,    'd', 1, False, 0, 0, False),
-    0x1401: Type(Keyword,           'H', 1, False, 0, 0, False),
-    0x1402: Type(Keyword,           'I', 1, False, 0, 0, False),
-    0x1404: Type(Keyword,           'Q', 1, False, 0, 0, False),
-    0x1502: Type(RealValue,         'f', 1, False, 0, 0, False),
-    0x1504: Type(RealValue,         'd', 1, False, 0, 0, False),
-    0x1602: Type(SimpleDiscreteOut, 'h', 1, True,  0, 0, False),
-    0x1604: Type(SimpleDiscreteOut, 'i', 1, True,  0, 0, False),
-    0x1608: Type(SimpleDiscreteOut, 'q', 1, True,  0, 0, False),
-    0x1704: Type(SimpleAnalogOut,   'f', 1, True,  0, 0, False),
-    0x1708: Type(SimpleAnalogOut,   'd', 1, True,  0, 0, False),
-    0x1801: Type(StatusWord,        'H', 1, False, 2, 0, False),
-    0x1802: Type(StatusWord,        'I', 1, False, 4, 0, False),
-    0x1a02: Type(DiscreteIn,        'h', 1, False, 2, 0, False),
-    0x1a04: Type(DiscreteIn,        'i', 1, False, 4, 0, False),
-    0x1a08: Type(DiscreteIn,        'q', 1, False, 6, 0, False),
-    0x1b03: Type(AnalogIn,          'f', 1, False, 2, 0, False),
-    0x1b04: Type(AnalogIn,          'f', 1, False, 4, 0, False),
-    0x1b08: Type(AnalogIn,          'd', 1, False, 6, 0, False),
-    0x1e03: Type(DiscreteOut,       'h', 1, True,  2, 0, False),
-    0x1e04: Type(DiscreteOut,       'h', 1, True,  4, 0, False),
-    0x1e06: Type(DiscreteOut,       'i', 1, True,  4, 0, False),
-    0x1e0c: Type(DiscreteOut,       'q', 1, True,  6, 0, False),
-    0x1f05: Type(AnalogOut,         'f', 1, True,  2, 0, False),
-    0x1f06: Type(AnalogOut,         'f', 1, True,  4, 0, False),
-    0x1f0c: Type(AnalogOut,         'd', 1, True,  6, 0, False),
-
-    0x4006: Type(ParamIn,           'f', 1, False, 2, 1, True),
-    0x4008: Type(ParamIn,           'f', 1, False, 6, 1, True),
-    0x400c: Type(ParamIn,           'd', 1, False, 6, 1, True),
-    0x5008: Type(ParamOut,          'f', 1, True,  2, 1, True),
-    0x500a: Type(ParamOut,          'f', 1, True,  6, 1, True),
-    0x5010: Type(ParamOut,          'd', 1, True,  6, 1, True),
+    0x1201: Type(SimpleDiscreteIn,  'h', 1, False, True,  0, 0, False),
+    0x1202: Type(SimpleDiscreteIn,  'i', 1, False, True,  0, 0, False),
+    0x1204: Type(SimpleDiscreteIn,  'q', 1, False, True,  0, 0, False),
+    0x1302: Type(SimpleAnalogIn,    'f', 1, False, True,  0, 0, False),
+    0x1304: Type(SimpleAnalogIn,    'd', 1, False, True,  0, 0, False),
+    0x1401: Type(Keyword,           'H', 1, False, False, 0, 0, False),
+    0x1402: Type(Keyword,           'I', 1, False, False, 0, 0, False),
+    0x1404: Type(Keyword,           'Q', 1, False, False, 0, 0, False),
+    0x1502: Type(RealValue,         'f', 1, False, False, 0, 0, False),
+    0x1504: Type(RealValue,         'd', 1, False, False, 0, 0, False),
+    0x1602: Type(SimpleDiscreteOut, 'h', 1, True,  False, 0, 0, False),
+    0x1604: Type(SimpleDiscreteOut, 'i', 1, True,  False, 0, 0, False),
+    0x1608: Type(SimpleDiscreteOut, 'q', 1, True,  False, 0, 0, False),
+    0x1704: Type(SimpleAnalogOut,   'f', 1, True,  False, 0, 0, False),
+    0x1708: Type(SimpleAnalogOut,   'd', 1, True,  False, 0, 0, False),
+    # changeable via start/Stop/reset/...
+    0x1801: Type(StatusWord,        'H', 1, False, True,  2, 0, False),
+    # changeable via start/Stop/reset/...
+    0x1802: Type(StatusWord,        'I', 1, False, True,  4, 0, False),
+    0x1a02: Type(DiscreteIn,        'h', 1, False, True,  2, 0, False),
+    0x1a04: Type(DiscreteIn,        'i', 1, False, True,  4, 0, False),
+    0x1a08: Type(DiscreteIn,        'q', 1, False, True,  6, 0, False),
+    0x1b03: Type(AnalogIn,          'f', 1, False, True,  2, 0, False),
+    0x1b04: Type(AnalogIn,          'f', 1, False, True,  4, 0, False),
+    0x1b08: Type(AnalogIn,          'd', 1, False, True,  6, 0, False),
+    0x1e03: Type(DiscreteOut,       'h', 1, True,  False, 2, 0, False),
+    0x1e04: Type(DiscreteOut,       'h', 1, True,  False, 4, 0, False),
+    0x1e06: Type(DiscreteOut,       'i', 1, True,  False, 4, 0, False),
+    0x1e0c: Type(DiscreteOut,       'q', 1, True,  False, 6, 0, False),
+    0x1f05: Type(AnalogOut,         'f', 1, True,  False, 2, 0, False),
+    0x1f06: Type(AnalogOut,         'f', 1, True,  False, 4, 0, False),
+    0x1f0c: Type(AnalogOut,         'd', 1, True,  False, 6, 0, False),
+
+    0x4006: Type(ParamIn,           'f', 1, False, True,  2, 1, True),
+    0x4008: Type(ParamIn,           'f', 1, False, True,  6, 1, True),
+    0x400c: Type(ParamIn,           'd', 1, False, True,  6, 1, True),
+    0x5008: Type(ParamOut,          'f', 1, True,  False, 2, 1, True),
+    0x500a: Type(ParamOut,          'f', 1, True,  False, 6, 1, True),
+    0x5010: Type(ParamOut,          'd', 1, True,  False, 6, 1, True),
 }
 
 for n in range(16):
     lfin32 =  0x2000 | (n << 8) | ( 6 + 2 * n)
     fin32 =   0x6000 | (n << 8) | ( 6 + 2 * n)
     fin64 =   0x2000 | (n << 8) | (12 + 4 * n)
     lfout32 = 0x3000 | (n << 8) | ( 8 + 2 * n)
     fout32 =  0x7000 | (n << 8) | ( 8 + 2 * n)
     fout64 =  0x3000 | (n << 8) | (16 + 4 * n)
-    TYPECODE_MAP[lfin32]  = Type(FlatIn, 'f', 1, False, 2, n + 1, False)
-    TYPECODE_MAP[fin32]   = Type(FlatIn, 'f', 1, False, 4, n + 1, False)
-    TYPECODE_MAP[fin64]   = Type(FlatIn, 'd', 1, False, 6, n + 1, False)
-    TYPECODE_MAP[lfout32] = Type(FlatOut, 'f', 1, True, 2, n + 1, False)
-    TYPECODE_MAP[fout32]  = Type(FlatOut, 'f', 1, True, 4, n + 1, False)
-    TYPECODE_MAP[fout64]  = Type(FlatOut, 'd', 1, True, 6, n + 1, False)
+    TYPECODE_MAP[lfin32]  = Type(FlatIn, 'f', 1, False, True, 2, n + 1, False)
+    TYPECODE_MAP[fin32]   = Type(FlatIn, 'f', 1, False, True, 4, n + 1, False)
+    TYPECODE_MAP[fin64]   = Type(FlatIn, 'd', 1, False, True, 6, n + 1, False)
+    TYPECODE_MAP[lfout32] = Type(FlatOut, 'f', 1, True, False, 2, n + 1, False)
+    TYPECODE_MAP[fout32]  = Type(FlatOut, 'f', 1, True, False, 4, n + 1, False)
+    TYPECODE_MAP[fout64]  = Type(FlatOut, 'd', 1, True, False, 6, n + 1, False)
 
     if n == 0:
         continue
 
     vin32 =  0x4000 | (n << 8) | ( 6 + 2 * n)
     vin64 =  0x4000 | (n << 8) | (12 + 4 * n)
     vout32 = 0x5000 | (n << 8) | ( 8 + 4 * n)
     vout64 = 0x5000 | (n << 8) | (16 + 8 * n)
-    TYPECODE_MAP[vin32]      = Type(VectorIn,  'f', n + 1, False, 2, 1, True)
-    TYPECODE_MAP[vin32 + 2]  = Type(VectorIn,  'f', n + 1, False, 6, 1, True)
-    TYPECODE_MAP[vin64]      = Type(VectorIn,  'd', n + 1, False, 6, 1, True)
-    TYPECODE_MAP[vout32]     = Type(VectorOut, 'f', n + 1, True,  2, 1, True)
-    TYPECODE_MAP[vout32 + 2] = Type(VectorOut, 'f', n + 1, True,  6, 1, True)
-    TYPECODE_MAP[vout64]     = Type(VectorOut, 'd', n + 1, True,  6, 1, True)
+    TYPECODE_MAP[vin32]      = Type(VectorIn,  'f', n + 1, False, True, 2, 1, True)
+    TYPECODE_MAP[vin32 + 2]  = Type(VectorIn,  'f', n + 1, False, True, 6, 1, True)
+    TYPECODE_MAP[vin64]      = Type(VectorIn,  'd', n + 1, False, True, 6, 1, True)
+    TYPECODE_MAP[vout32]     = Type(VectorOut, 'f', n + 1, True, False, 2, 1, True)
+    TYPECODE_MAP[vout32 + 2] = Type(VectorOut, 'f', n + 1, True, False, 6, 1, True)
+    TYPECODE_MAP[vout64]     = Type(VectorOut, 'd', n + 1, True, False, 6, 1, True)
 
 for n in range(4, 253, 2):
     msgio = 0x0500 | (n >> 1)
-    TYPECODE_MAP[msgio] = Type(MessageIO, f'{n-2}s', 1, False, 0, 0, False)
+    TYPECODE_MAP[msgio] = Type(MessageIO, f'{n-2}s', 1, False, True, 0, 0, False)
 
 
 def typecode_description(typecode):
     typeinfo = TYPECODE_MAP[typecode]
     name = typeinfo.devcls.__name__
     valuesize = calcsize(typeinfo.value_fmt)
     if typeinfo.num_params > 0 and not typeinfo.has_pctrl:
```

### Comparing `zapf-0.4.6/zapf/indexer.py` & `zapf-0.4.7/zapf/indexer.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/io.py` & `zapf-0.4.7/zapf/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,21 @@
 
     def start_cache(self):
         self.cache.start()
 
     def stop_cache(self):
         self.cache.stop()
 
+    def disconnect(self):
+        """Close the connection. This PlcIO object should not be used anymore
+        afterwards.
+        """
+        self.stop_cache()
+        self.proto.disconnect()
+
     # Cache related API.
 
     def register_cache_range(self, addr, length):
         """Register a cached area."""
         if length < 1:
             return
         self.cache.update_range(addr, length)
```

### Comparing `zapf-0.4.6/zapf/proto/__init__.py` & `zapf-0.4.7/zapf/proto/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 """Support for an abstract communication protocol."""
 
 from zapf import Error
 
 ADDRESSES = '''Valid addresses:
 ads://host[:port]/amsnetid:amsport
 modbus://host[:port]/slaveno
-tango://dbhost:dbport/tango/device/name'''
+tango://dbhost:dbport/tango/device/name
+sim://filepath'''
 
 
 class Protocol:
     OFFSETS = []
 
     def __init__(self, url, log):
         self.url = url
```

### Comparing `zapf-0.4.6/zapf/proto/ads.py` & `zapf-0.4.7/zapf/proto/ads.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/proto/modbus.py` & `zapf-0.4.7/zapf/proto/modbus.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/proto/sim.py` & `zapf-0.4.7/zapf/proto/sim.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/proto/tango.py` & `zapf-0.4.7/zapf/proto/tango.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/scan.py` & `zapf-0.4.7/zapf/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,19 @@
         turn connects to the PLC.
 
         The Tango device interface must conform to the `Profibus
         <https://forge.frm2.tum.de/entangle/defs/entangle-master/profibus/>`_
         Entangle interface specification.
 
         Example: ``tango://192.168.201.2:10000/box/plc/ads``
+
+    ``sim://filepath``
+        "Connection" to a software-simulated PLC.  Zapf starts it in the same
+        process when the address is requested.  See the `zapf.simulator`
+        package for details.
     """
 
     IGNORE_BAD_DEVICES = True
 
     def __init__(self, io_or_proto, log):
         self.log = log
         if isinstance(io_or_proto, PlcIO):
@@ -282,17 +287,15 @@
                         par = {'idx': i}  # parameter slot id
                         par.update(v_2015_02.PARAMETER_Specs[p])
                         if 'unit' in par:
                             par['unit'] = fix_unit(par.get('unit', ''), unit)
                         params[par.pop('name')] = par
 
             basetype, width = FMT_TO_BASETYPE.get(tce.value_fmt, (None, 0))
-            # Keyword/RealValue are special
-            access = 'rw' if (tce.has_target or typecode >> 8 in (0x14, 0x15)) \
-                else 'ro'
+            access = 'ro' if tce.readonly else 'rw'
 
             # fixup limits, if needed
             limits = FMT_LIMITS.get(tce.value_fmt)
             if limits:
                 absmin = max(absmin, limits[0])
                 absmax = min(absmax, limits[1])
```

### Comparing `zapf-0.4.6/zapf/simulator/funcs.py` & `zapf-0.4.7/zapf/simulator/funcs.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/simulator/runtime.py` & `zapf-0.4.7/zapf/simulator/runtime.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/simulator/server.py` & `zapf-0.4.7/zapf/simulator/server.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/simulator/util.py` & `zapf-0.4.7/zapf/simulator/util.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/spec/__init__.py` & `zapf-0.4.7/zapf/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/spec/v_2015_02.py` & `zapf-0.4.7/zapf/spec/v_2015_02.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/spec/v_2021_09.py` & `zapf-0.4.7/zapf/spec/v_2021_09.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,29 +270,31 @@
         main_param.pop('description', None)
 
         mp_basetype = main_param.pop('basetype', None)
         mp_width = main_param.pop('width', 0)
         # pylint: disable=import-outside-toplevel
         from zapf.device import TYPECODE_MAP
         try:
-            basetype, width = FMT_TO_BASETYPE[TYPECODE_MAP[self.typecode].value_fmt]
+            typecode_info = TYPECODE_MAP[self.typecode]
+            basetype, width = FMT_TO_BASETYPE[typecode_info.value_fmt]
+            readonly = typecode_info.readonly
             # correct basetype if param descriptor is enum
             if mp_basetype == 'enum' and basetype in ('int', 'uint'):
                 basetype = 'enum'
             # it is ok to have a mismatch int<->uint
             if mp_basetype and mp_basetype != basetype and \
                'float' in (mp_basetype, basetype):
                 raise DescError(self, f'type {mp_basetype} declared in main '
                                 'param descriptor does not match typecode')
             if mp_width and mp_width != width:
                 raise DescError(self, f'width {mp_width} declared in main '
                                 'param descriptor does not match typecode')
         except KeyError:
-            basetype, width = None, 0
-        access = 'ro' if 'readonly' in self.flags else 'rw'
+            basetype, width, readonly = None, 0, True
+        access = 'ro' if readonly or 'readonly' in self.flags else 'rw'
         absmin = main_param.pop('min_value', -FLOAT32_MAX)
         absmax = main_param.pop('max_value', FLOAT32_MAX)
         unit = main_param.pop('unit', '')
         enum_r = main_param.pop('enum_r', None)
         enum_w = main_param.pop('enum_w', None)
         params, funcs, tables = {}, {}, {}
         descr = self.accessibles
```

### Comparing `zapf-0.4.6/zapf/table.py` & `zapf-0.4.7/zapf/table.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf/util.py` & `zapf-0.4.7/zapf/util.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.6/zapf.egg-info/PKG-INFO` & `zapf-0.4.7/zapf.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zapf
-Version: 0.4.6
+Version: 0.4.7
 Summary: Client library for the PILS specification
 Home-page: https://forge.frm2.tum.de/review/plugins/gitiles/mlz/pils/zapf
 Author: Georg Brandl
 Author-email: g.brandl@fz-juelich.de
 License: GPL-2.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `zapf-0.4.6/zapf.egg-info/SOURCES.txt` & `zapf-0.4.7/zapf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

