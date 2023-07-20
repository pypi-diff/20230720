# Comparing `tmp/nttblink-0.1.0.tar.gz` & `tmp/nttblink-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nttblink-0.1.0.tar", last modified: Thu Jul 20 18:31:53 2023, max compression
+gzip compressed data, was "nttblink-0.1.1.tar", last modified: Thu Jul 20 18:55:37 2023, max compression
```

## Comparing `nttblink-0.1.0.tar` & `nttblink-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0      501 dialout     (20)        0 2023-07-20 18:31:53.000000 nttblink-0.1.0/
--rw-r--r--   0      501 dialout     (20)     1080 2023-07-18 16:01:00.000000 nttblink-0.1.0/LICENSE
--rw-r--r--   0      501 dialout     (20)      445 2023-07-20 18:31:53.000000 nttblink-0.1.0/PKG-INFO
--rw-r--r--   0      501 dialout     (20)      135 2023-07-18 16:01:25.000000 nttblink-0.1.0/README.md
-drwxr-xr-x   0      501 dialout     (20)        0 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/
--rw-r--r--   0      501 dialout     (20)      445 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/PKG-INFO
--rw-r--r--   0      501 dialout     (20)      185 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/SOURCES.txt
--rw-r--r--   0      501 dialout     (20)        1 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/dependency_links.txt
--rw-r--r--   0      501 dialout     (20)       23 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/requires.txt
--rw-r--r--   0      501 dialout     (20)        1 2023-07-20 18:31:53.000000 nttblink-0.1.0/nttblink.egg-info/top_level.txt
--rw-r--r--   0      501 dialout     (20)       38 2023-07-20 18:31:53.000000 nttblink-0.1.0/setup.cfg
--rw-r--r--   0      501 dialout     (20)      490 2023-07-20 18:23:05.000000 nttblink-0.1.0/setup.py
+drwxr-xr-x   0      501 dialout     (20)        0 2023-07-20 18:55:38.000000 nttblink-0.1.1/
+-rw-r--r--   0      501 dialout     (20)     4468 2023-07-20 18:55:38.000000 nttblink-0.1.1/PKG-INFO
+-rw-r--r--   0      501 dialout     (20)     3959 2023-07-20 18:31:39.000000 nttblink-0.1.1/README.md
+drwxr-xr-x   0      501 dialout     (20)        0 2023-07-20 18:55:38.000000 nttblink-0.1.1/nttblink/
+-rw-r--r--   0      501 dialout     (20)       47 2023-07-20 18:12:09.000000 nttblink-0.1.1/nttblink/__init__.py
+-rw-r--r--   0      501 dialout     (20)     8596 2023-07-20 18:20:05.000000 nttblink-0.1.1/nttblink/nttblink.py
+-rw-r--r--   0      501 dialout     (20)      490 2023-07-20 18:52:22.000000 nttblink-0.1.1/nttblink/setup.py
+drwxr-xr-x   0      501 dialout     (20)        0 2023-07-20 18:55:38.000000 nttblink-0.1.1/nttblink.egg-info/
+-rw-r--r--   0      501 dialout     (20)     4468 2023-07-20 18:55:38.000000 nttblink-0.1.1/nttblink.egg-info/PKG-INFO
+-rw-r--r--   0      501 dialout     (20)      212 2023-07-20 18:55:38.000000 nttblink-0.1.1/nttblink.egg-info/SOURCES.txt
+-rw-r--r--   0      501 dialout     (20)        1 2023-07-20 18:55:38.000000 nttblink-0.1.1/nttblink.egg-info/dependency_links.txt
+-rw-r--r--   0      501 dialout     (20)        9 2023-07-20 18:55:38.000000 nttblink-0.1.1/nttblink.egg-info/top_level.txt
+-rw-r--r--   0      501 dialout     (20)      604 2023-07-20 18:55:32.000000 nttblink-0.1.1/pyproject.toml
+-rw-r--r--   0      501 dialout     (20)       38 2023-07-20 18:55:38.000000 nttblink-0.1.1/setup.cfg
```

