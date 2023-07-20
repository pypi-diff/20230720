# Comparing `tmp/nttblink-0.0.3.tar.gz` & `tmp/nttblink-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nttblink-0.0.3.tar", last modified: Wed Jul 19 00:23:27 2023, max compression
+gzip compressed data, was "nttblink-0.1.0.tar", last modified: Thu Jul 20 18:31:53 2023, max compression
```

## Comparing `nttblink-0.0.3.tar` & `nttblink-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0      501 dialout     (20)        0 2023-07-19 00:23:27.000000 nttblink-0.0.3/
--rw-r--r--   0      501 dialout     (20)     4303 2023-07-19 00:23:27.000000 nttblink-0.0.3/PKG-INFO
--rw-r--r--   0      501 dialout     (20)     3793 2023-07-18 16:23:55.000000 nttblink-0.0.3/README.md
-drwxr-xr-x   0      501 dialout     (20)        0 2023-07-19 00:23:27.000000 nttblink-0.0.3/nttblink/
--rw-r--r--   0      501 dialout     (20)       47 2023-07-18 16:01:00.000000 nttblink-0.0.3/nttblink/__init__.py
--rw-r--r--   0      501 dialout     (20)     6185 2023-07-19 00:19:50.000000 nttblink-0.0.3/nttblink/nttblink.py
--rw-r--r--   0      501 dialout     (20)      490 2023-07-18 19:33:44.000000 nttblink-0.0.3/nttblink/setup.py
-drwxr-xr-x   0      501 dialout     (20)        0 2023-07-19 00:23:27.000000 nttblink-0.0.3/nttblink.egg-info/
--rw-r--r--   0      501 dialout     (20)     4303 2023-07-19 00:23:27.000000 nttblink-0.0.3/nttblink.egg-info/PKG-INFO
--rw-r--r--   0      501 dialout     (20)      212 2023-07-19 00:23:27.000000 nttblink-0.0.3/nttblink.egg-info/SOURCES.txt
--rw-r--r--   0      501 dialout     (20)        1 2023-07-19 00:23:27.000000 nttblink-0.0.3/nttblink.egg-info/dependency_links.txt
--rw-r--r--   0      501 dialout     (20)        9 2023-07-19 00:23:27.000000 nttblink-0.0.3/nttblink.egg-info/top_level.txt
--rw-r--r--   0      501 dialout     (20)      604 2023-07-19 00:23:18.000000 nttblink-0.0.3/pyproject.toml
--rw-r--r--   0      501 dialout     (20)       38 2023-07-19 00:23:27.000000 nttblink-0.0.3/setup.cfg
+drwxr-xr-x   0      501 dialout     (20)        0 2023-07-20 18:31:53.000000 nttblink-0.1.0/
+-rw-r--r--   0      501 dialout     (20)     1080 2023-07-18 16:01:00.000000 nttblink-0.1.0/LICENSE
+-rw-r--r--   0      501 dialout     (20)      445 2023-07-20 18:31:53.000000 nttblink-0.1.0/PKG-INFO
+-rw-r--r--   0      501 dialout     (20)      135 2023-07-18 16:01:25.000000 nttblink-0.1.0/README.md
+drwxr-xr-x   0      501 dialout     (20)        0 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/
+-rw-r--r--   0      501 dialout     (20)      445 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/PKG-INFO
+-rw-r--r--   0      501 dialout     (20)      185 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/SOURCES.txt
+-rw-r--r--   0      501 dialout     (20)        1 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/dependency_links.txt
+-rw-r--r--   0      501 dialout     (20)       23 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/requires.txt
+-rw-r--r--   0      501 dialout     (20)        1 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/top_level.txt
+-rw-r--r--   0      501 dialout     (20)       38 2023-07-20 18:31:53.000000 nttblink-0.1.0/setup.cfg
+-rw-r--r--   0      501 dialout     (20)      490 2023-07-20 18:23:05.000000 nttblink-0.1.0/setup.py
```

