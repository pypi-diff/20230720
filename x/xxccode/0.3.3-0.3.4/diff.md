# Comparing `tmp/xxccode-0.3.3.tar.gz` & `tmp/xxccode-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxccode-0.3.3.tar", last modified: Thu Jul 20 14:56:09 2023, max compression
+gzip compressed data, was "xxccode-0.3.4.tar", last modified: Thu Jul 20 14:58:26 2023, max compression
```

## Comparing `xxccode-0.3.3.tar` & `xxccode-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 14:56:09.004927 xxccode-0.3.3/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       98 2023-07-20 14:56:09.000928 xxccode-0.3.3/PKG-INFO
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       38 2023-07-20 14:56:09.004927 xxccode-0.3.3/setup.cfg
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      247 2023-07-20 14:54:35.000000 xxccode-0.3.3/setup.py
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 14:56:08.956928 xxccode-0.3.3/xxccode/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       56 2023-07-20 14:51:38.000000 xxccode-0.3.3/xxccode/__init__.py
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      972 2023-07-20 14:51:38.000000 xxccode-0.3.3/xxccode/xreader.py
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      787 2023-07-20 14:51:38.000000 xxccode-0.3.3/xxccode/xwriter.py
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 14:56:09.000928 xxccode-0.3.3/xxccode.egg-info/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       98 2023-07-20 14:56:08.000000 xxccode-0.3.3/xxccode.egg-info/PKG-INFO
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      220 2023-07-20 14:56:08.000000 xxccode-0.3.3/xxccode.egg-info/SOURCES.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 14:56:08.000000 xxccode-0.3.3/xxccode.egg-info/dependency_links.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       13 2023-07-20 14:56:08.000000 xxccode-0.3.3/xxccode.egg-info/requires.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)        8 2023-07-20 14:56:08.000000 xxccode-0.3.3/xxccode.egg-info/top_level.txt
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 14:58:26.300501 xxccode-0.3.4/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       98 2023-07-20 14:58:26.300501 xxccode-0.3.4/PKG-INFO
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       38 2023-07-20 14:58:26.300501 xxccode-0.3.4/setup.cfg
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      247 2023-07-20 14:58:21.000000 xxccode-0.3.4/setup.py
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 14:58:26.284502 xxccode-0.3.4/xxccode/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       60 2023-07-20 14:57:47.000000 xxccode-0.3.4/xxccode/__init__.py
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      972 2023-07-20 14:51:38.000000 xxccode-0.3.4/xxccode/xreader.py
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      787 2023-07-20 14:51:38.000000 xxccode-0.3.4/xxccode/xwriter.py
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-20 14:58:26.296501 xxccode-0.3.4/xxccode.egg-info/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       98 2023-07-20 14:58:26.000000 xxccode-0.3.4/xxccode.egg-info/PKG-INFO
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      220 2023-07-20 14:58:26.000000 xxccode-0.3.4/xxccode.egg-info/SOURCES.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-20 14:58:26.000000 xxccode-0.3.4/xxccode.egg-info/dependency_links.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       13 2023-07-20 14:58:26.000000 xxccode-0.3.4/xxccode.egg-info/requires.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)        8 2023-07-20 14:58:26.000000 xxccode-0.3.4/xxccode.egg-info/top_level.txt
```

### Comparing `xxccode-0.3.3/xxccode/xreader.py` & `xxccode-0.3.4/xxccode/xreader.py`

 * *Files identical despite different names*

### Comparing `xxccode-0.3.3/xxccode/xwriter.py` & `xxccode-0.3.4/xxccode/xwriter.py`

 * *Files identical despite different names*

