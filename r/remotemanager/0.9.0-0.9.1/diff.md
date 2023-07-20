# Comparing `tmp/remotemanager-0.9.0.tar.gz` & `tmp/remotemanager-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.9.0.tar", last modified: Thu Jul 20 07:21:02 2023, max compression
+gzip compressed data, was "remotemanager-0.9.1.tar", last modified: Thu Jul 20 12:16:00 2023, max compression
```

## Comparing `remotemanager-0.9.0.tar` & `remotemanager-0.9.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.970439 remotemanager-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-20 07:21:02.970439 remotemanager-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-19 13:23:53.000000 remotemanager-0.9.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.962439 remotemanager-0.9.0/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-19 13:23:53.000000 remotemanager-0.9.0/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.962439 remotemanager-0.9.0/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.0/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.966439 remotemanager-0.9.0/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.0/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.0/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.0/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.0/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.0/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.0/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.966439 remotemanager-0.9.0/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    53193 2023-07-19 14:27:58.000000 remotemanager-0.9.0/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     9428 2023-07-19 13:19:17.000000 remotemanager-0.9.0/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.0/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    21248 2023-07-19 13:19:17.000000 remotemanager-0.9.0/remotemanager/dataset/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-18 13:45:10.000000 remotemanager-0.9.0/remotemanager/dataset/runnerstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.966439 remotemanager-0.9.0/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.0/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.0/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.966439 remotemanager-0.9.0/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.0/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.0/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.0/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.0/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.966439 remotemanager-0.9.0/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.0/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.0/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.0/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.970439 remotemanager-0.9.0/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.0/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.0/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.0/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.970439 remotemanager-0.9.0/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.0/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.0/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.0/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.970439 remotemanager-0.9.0/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.0/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.0/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 07:21:02.962439 remotemanager-0.9.0/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-20 07:21:02.000000 remotemanager-0.9.0/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-20 07:21:02.000000 remotemanager-0.9.0/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 07:21:02.000000 remotemanager-0.9.0/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-20 07:21:02.000000 remotemanager-0.9.0/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 07:21:02.000000 remotemanager-0.9.0/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 07:21:02.970439 remotemanager-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.797276 remotemanager-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-20 12:16:00.797276 remotemanager-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-20 11:20:29.000000 remotemanager-0.9.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.789276 remotemanager-0.9.1/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-20 11:20:29.000000 remotemanager-0.9.1/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.789276 remotemanager-0.9.1/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.1/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.789276 remotemanager-0.9.1/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.1/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.1/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.1/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.1/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.1/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.1/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.793276 remotemanager-0.9.1/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    53378 2023-07-20 10:54:58.000000 remotemanager-0.9.1/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     9606 2023-07-20 10:54:58.000000 remotemanager-0.9.1/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.1/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    21248 2023-07-19 13:19:17.000000 remotemanager-0.9.1/remotemanager/dataset/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-18 13:45:10.000000 remotemanager-0.9.1/remotemanager/dataset/runnerstates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.793276 remotemanager-0.9.1/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.1/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.1/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.793276 remotemanager-0.9.1/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.1/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.1/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.1/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.1/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.793276 remotemanager-0.9.1/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.1/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.1/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.1/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.793276 remotemanager-0.9.1/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.1/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.1/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.1/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.793276 remotemanager-0.9.1/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.1/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.1/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.1/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.797276 remotemanager-0.9.1/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.1/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.1/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:16:00.789276 remotemanager-0.9.1/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-20 12:16:00.000000 remotemanager-0.9.1/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-20 12:16:00.000000 remotemanager-0.9.1/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 12:16:00.000000 remotemanager-0.9.1/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-20 12:16:00.000000 remotemanager-0.9.1/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 12:16:00.000000 remotemanager-0.9.1/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 12:16:00.797276 remotemanager-0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.1/setup.py
```

### Comparing `remotemanager-0.9.0/LICENSE` & `remotemanager-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/PKG-INFO` & `remotemanager-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.0
+Version: 0.9.1
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.0/README.md` & `remotemanager-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/pyproject.toml` & `remotemanager-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.9.0"
+current_version = "0.9.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.9.0/remotemanager/connection/cmd.py` & `remotemanager-0.9.1/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/connection/computers/base.py` & `remotemanager-0.9.1/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/connection/computers/example.py` & `remotemanager-0.9.1/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/connection/computers/options.py` & `remotemanager-0.9.1/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/connection/computers/parsers.py` & `remotemanager-0.9.1/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/connection/testing_object.py` & `remotemanager-0.9.1/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/connection/url.py` & `remotemanager-0.9.1/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/dataset/dataset.py` & `remotemanager-0.9.1/remotemanager/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,15 +576,19 @@
         else:
             self._logger.important(f"runner {tmp.name} already exists")
 
         if not lazy:
             self.finish_append()
         Quiet.state = False
 
-    def finish_append(self):
+    def finish_append(self, dependency_call=False):
+        self._logger.info("finishing append")
+        if self.dependency is not None and not dependency_call:
+            return self.dependency.finish_append()
+
         self.database.update(self.pack())
 
     def lazy_append(self):
         return LazyAppend(self)
 
     def remove_run(self, id: any, dependency_call: bool = False) -> bool:
         """
```

### Comparing `remotemanager-0.9.0/remotemanager/dataset/dependency.py` & `remotemanager-0.9.1/remotemanager/dataset/dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         for ds in self.ds_list:
             ds.wipe_remote(files_only=files_only, dependency_call=True)
 
     def hard_reset(self, files_only: bool = False) -> None:
         for ds in self.ds_list:
             ds.hard_reset(files_only=files_only, dependency_call=True)
 
-    def append_run(self, caller, chain_run_args, run_args, *args, **kwargs):
+    def append_run(self, caller, chain_run_args, run_args, lazy, *args, **kwargs):
         """
         Appends runs with the same args to all datasets
 
         Args:
             caller:
                 (Dataset): The dataset which defers to the dependency
             chain_run_args (bool):
@@ -118,17 +118,17 @@
             self._logger.info("chain_args is True, propagating")
             kwargs.update(run_args)
 
         for ds in datasets:
             if ds == caller:
                 caller_args = {k: v for k, v in kwargs.items()}
                 caller_args.update(run_args)
-                ds.append_run(dependency_call=True, *args, **caller_args)
+                ds.append_run(dependency_call=True, lazy=lazy, *args, **caller_args)
             else:
-                ds.append_run(dependency_call=True, *args, **kwargs)
+                ds.append_run(dependency_call=True, lazy=lazy, *args, **kwargs)
 
         for ds in datasets:
             parents = self.get_parents(ds)
             if len(parents) > 1:
                 warnings.warn(
                     "Multiple parents detected. "
                     "Variable passing in this instance is unstable!"
@@ -154,15 +154,20 @@
                 tmp.append(
                     f"{child.url.submitter} {runner.jobscript.name} "
                     f"2>> {runner.errorfile.name}"
                 )
 
             ds.runners[-1]._dependency_info["child_submit"] = tmp
 
-            ds.database.update(ds.pack())
+            if not lazy:
+                ds.database.update(ds.pack())
+
+    def finish_append(self) -> None:
+        for ds in self.ds_list:
+            ds.finish_append(dependency_call=True)
 
     def run(
         self,
         dry_run: bool = False,
         **run_args,
     ):
         self._logger.info("dependency internal run call")
```

### Comparing `remotemanager-0.9.0/remotemanager/dataset/lazy_append.py` & `remotemanager-0.9.1/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/dataset/runner.py` & `remotemanager-0.9.1/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/dataset/runnerstates.py` & `remotemanager-0.9.1/remotemanager/dataset/runnerstates.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/jupyter/magic.py` & `remotemanager-0.9.1/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/logging/__init__.py` & `remotemanager-0.9.1/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/logging/log.py` & `remotemanager-0.9.1/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/logging/utils.py` & `remotemanager-0.9.1/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/logging/verbosity.py` & `remotemanager-0.9.1/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/serialisation/__init__.py` & `remotemanager-0.9.1/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/serialisation/serial.py` & `remotemanager-0.9.1/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.9.1/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.9.1/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/storage/database.py` & `remotemanager-0.9.1/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/storage/function.py` & `remotemanager-0.9.1/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/storage/remotefunction.py` & `remotemanager-0.9.1/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/storage/sendablemixin.py` & `remotemanager-0.9.1/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/storage/trackedfile.py` & `remotemanager-0.9.1/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/transport/cp.py` & `remotemanager-0.9.1/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/transport/rsync.py` & `remotemanager-0.9.1/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/transport/scp.py` & `remotemanager-0.9.1/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/transport/transport.py` & `remotemanager-0.9.1/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/utils/__init__.py` & `remotemanager-0.9.1/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/utils/flags.py` & `remotemanager-0.9.1/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager/utils/version.py` & `remotemanager-0.9.1/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.0/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.9.1/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.0
+Version: 0.9.1
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.0/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.9.1/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

