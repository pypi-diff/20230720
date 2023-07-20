# Comparing `tmp/inscodegpt-1.0.tar.gz` & `tmp/inscodegpt-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inscodegpt-1.0.tar", last modified: Thu Jul 20 14:39:53 2023, max compression
+gzip compressed data, was "inscodegpt-1.1.tar", last modified: Thu Jul 20 14:55:00 2023, max compression
```

## Comparing `inscodegpt-1.0.tar` & `inscodegpt-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 14:39:53.315408 inscodegpt-1.0/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 14:39:53.315408 inscodegpt-1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 14:39:53.314408 inscodegpt-1.0/inscodegpt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 14:32:20.000000 inscodegpt-1.0/inscodegpt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1186 2023-07-20 14:34:21.000000 inscodegpt-1.0/inscodegpt/inscode_gpt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 14:39:53.315408 inscodegpt-1.0/inscodegpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 14:39:53.000000 inscodegpt-1.0/inscodegpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-20 14:39:53.000000 inscodegpt-1.0/inscodegpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 14:39:53.000000 inscodegpt-1.0/inscodegpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-20 14:39:53.000000 inscodegpt-1.0/inscodegpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-20 14:39:53.000000 inscodegpt-1.0/inscodegpt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 14:39:53.315408 inscodegpt-1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-20 14:33:22.000000 inscodegpt-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 14:55:00.696547 inscodegpt-1.1/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 14:55:00.695547 inscodegpt-1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 14:55:00.695547 inscodegpt-1.1/inscodegpt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 14:32:20.000000 inscodegpt-1.1/inscodegpt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-07-20 14:34:21.000000 inscodegpt-1.1/inscodegpt/inscode_gpt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 14:55:00.695547 inscodegpt-1.1/inscodegpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 14:55:00.000000 inscodegpt-1.1/inscodegpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-20 14:55:00.000000 inscodegpt-1.1/inscodegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 14:55:00.000000 inscodegpt-1.1/inscodegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 14:55:00.000000 inscodegpt-1.1/inscodegpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-20 14:55:00.000000 inscodegpt-1.1/inscodegpt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 14:55:00.696547 inscodegpt-1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-20 14:54:48.000000 inscodegpt-1.1/setup.py
```

### Comparing `inscodegpt-1.0/inscodegpt/inscode_gpt.py` & `inscodegpt-1.1/inscodegpt/inscode_gpt.py`

 * *Files identical despite different names*

