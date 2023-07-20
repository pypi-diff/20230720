# Comparing `tmp/thanos-gen-1.0.0.tar.gz` & `tmp/thanos-gen-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thanos-gen-1.0.0.tar", last modified: Thu Jul 20 02:54:39 2023, max compression
+gzip compressed data, was "thanos-gen-2.1.1.tar", last modified: Thu Jul 20 10:36:26 2023, max compression
```

## Comparing `thanos-gen-1.0.0.tar` & `thanos-gen-2.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 02:54:39.215556 thanos-gen-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      126 2023-07-20 02:54:39.211556 thanos-gen-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 02:54:39.215556 thanos-gen-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-20 02:53:38.000000 thanos-gen-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 02:54:39.211556 thanos-gen-1.0.0/thanos_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)      126 2023-07-20 02:54:37.000000 thanos-gen-1.0.0/thanos_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-20 02:54:38.000000 thanos-gen-1.0.0/thanos_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 02:54:37.000000 thanos-gen-1.0.0/thanos_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 02:54:37.000000 thanos-gen-1.0.0/thanos_gen.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 02:54:37.000000 thanos-gen-1.0.0/thanos_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:36:26.527017 thanos-gen-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-20 10:36:26.527017 thanos-gen-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 10:36:26.527017 thanos-gen-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-20 10:33:21.000000 thanos-gen-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:36:26.523017 thanos-gen-2.1.1/thanos_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-20 10:36:25.000000 thanos-gen-2.1.1/thanos_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-20 10:36:26.000000 thanos-gen-2.1.1/thanos_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 10:36:25.000000 thanos-gen-2.1.1/thanos_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 02:54:37.000000 thanos-gen-2.1.1/thanos_gen.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 10:36:26.000000 thanos-gen-2.1.1/thanos_gen.egg-info/top_level.txt
```

