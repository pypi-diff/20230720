# Comparing `tmp/xxccode-0.3.tar.gz` & `tmp/xxccode-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxccode-0.3.tar", last modified: Thu Jul 20 12:08:04 2023, max compression
+gzip compressed data, was "xxccode-0.3.2.tar", last modified: Thu Jul 20 12:12:02 2023, max compression
```

## Comparing `xxccode-0.3.tar` & `xxccode-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:08:04.307813 xxccode-0.3/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       96 2023-07-20 12:08:04.307813 xxccode-0.3/PKG-INFO
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       38 2023-07-20 12:08:04.307813 xxccode-0.3/setup.cfg
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      245 2023-07-20 12:07:57.000000 xxccode-0.3/setup.py
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:08:04.303813 xxccode-0.3/xxccode.egg-info/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       96 2023-07-20 12:08:04.000000 xxccode-0.3/xxccode.egg-info/PKG-INFO
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      162 2023-07-20 12:08:04.000000 xxccode-0.3/xxccode.egg-info/SOURCES.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 12:08:04.000000 xxccode-0.3/xxccode.egg-info/dependency_links.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       13 2023-07-20 12:08:04.000000 xxccode-0.3/xxccode.egg-info/requires.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 12:08:04.000000 xxccode-0.3/xxccode.egg-info/top_level.txt
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:12:02.243096 xxccode-0.3.2/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       98 2023-07-20 12:12:02.239096 xxccode-0.3.2/PKG-INFO
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       38 2023-07-20 12:12:02.243096 xxccode-0.3.2/setup.cfg
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      247 2023-07-20 12:11:58.000000 xxccode-0.3.2/setup.py
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:12:02.227096 xxccode-0.3.2/xfile/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       78 2023-07-20 12:11:48.000000 xxccode-0.3.2/xfile/__init__.py
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      972 2023-07-20 07:44:58.000000 xxccode-0.3.2/xfile/xreader.py
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      787 2023-07-20 07:45:03.000000 xxccode-0.3.2/xfile/xwriter.py
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 12:12:02.239096 xxccode-0.3.2/xxccode.egg-info/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       98 2023-07-20 12:12:02.000000 xxccode-0.3.2/xxccode.egg-info/PKG-INFO
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      214 2023-07-20 12:12:02.000000 xxccode-0.3.2/xxccode.egg-info/SOURCES.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 12:12:02.000000 xxccode-0.3.2/xxccode.egg-info/dependency_links.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       13 2023-07-20 12:12:02.000000 xxccode-0.3.2/xxccode.egg-info/requires.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)        6 2023-07-20 12:12:02.000000 xxccode-0.3.2/xxccode.egg-info/top_level.txt
```

