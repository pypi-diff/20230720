# Comparing `tmp/xxccode-0.1.1.tar.gz` & `tmp/xxccode-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxccode-0.1.1.tar", last modified: Thu Jul 20 12:02:29 2023, max compression
+gzip compressed data, was "xxccode-0.2.tar", last modified: Thu Jul 20 12:03:34 2023, max compression
```

## Comparing `xxccode-0.1.1.tar` & `xxccode-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:02:29.508820 xxccode-0.1.1/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       98 2023-07-20 12:02:29.508820 xxccode-0.1.1/PKG-INFO
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       38 2023-07-20 12:02:29.508820 xxccode-0.1.1/setup.cfg
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      247 2023-07-20 12:02:22.000000 xxccode-0.1.1/setup.py
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:02:29.504820 xxccode-0.1.1/xxccode.egg-info/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       98 2023-07-20 12:02:29.000000 xxccode-0.1.1/xxccode.egg-info/PKG-INFO
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      162 2023-07-20 12:02:29.000000 xxccode-0.1.1/xxccode.egg-info/SOURCES.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 12:02:29.000000 xxccode-0.1.1/xxccode.egg-info/dependency_links.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       13 2023-07-20 12:02:29.000000 xxccode-0.1.1/xxccode.egg-info/requires.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 12:02:29.000000 xxccode-0.1.1/xxccode.egg-info/top_level.txt
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:03:34.224626 xxccode-0.2/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       96 2023-07-20 12:03:34.224626 xxccode-0.2/PKG-INFO
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       38 2023-07-20 12:03:34.224626 xxccode-0.2/setup.cfg
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      245 2023-07-20 12:03:09.000000 xxccode-0.2/setup.py
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:03:34.220626 xxccode-0.2/xxccode.egg-info/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       96 2023-07-20 12:03:34.000000 xxccode-0.2/xxccode.egg-info/PKG-INFO
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      162 2023-07-20 12:03:34.000000 xxccode-0.2/xxccode.egg-info/SOURCES.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 12:03:34.000000 xxccode-0.2/xxccode.egg-info/dependency_links.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       13 2023-07-20 12:03:34.000000 xxccode-0.2/xxccode.egg-info/requires.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 12:03:34.000000 xxccode-0.2/xxccode.egg-info/top_level.txt
```

