# Comparing `tmp/responsecurve-0.0.0.tar.gz` & `tmp/responsecurve-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsecurve-0.0.0.tar", last modified: Thu Jul 20 18:18:48 2023, max compression
+gzip compressed data, was "responsecurve-0.1.tar", last modified: Thu Jul 20 18:16:27 2023, max compression
```

## Comparing `responsecurve-0.0.0.tar` & `responsecurve-0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 18:18:48.623088 responsecurve-0.0.0/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      182 2023-07-20 18:18:48.622662 responsecurve-0.0.0/PKG-INFO
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 18:18:48.621807 responsecurve-0.0.0/responsecurve.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      182 2023-07-20 18:18:48.000000 responsecurve-0.0.0/responsecurve.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      192 2023-07-20 18:18:48.000000 responsecurve-0.0.0/responsecurve.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 18:18:48.000000 responsecurve-0.0.0/responsecurve.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       43 2023-07-20 18:18:48.000000 responsecurve-0.0.0/responsecurve.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 18:18:48.000000 responsecurve-0.0.0/responsecurve.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-20 18:18:48.623251 responsecurve-0.0.0/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      382 2023-07-20 18:18:30.000000 responsecurve-0.0.0/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 18:16:27.580157 responsecurve-0.1/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      180 2023-07-20 18:16:27.578986 responsecurve-0.1/PKG-INFO
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 18:16:27.577826 responsecurve-0.1/responsecurve.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      180 2023-07-20 18:16:27.000000 responsecurve-0.1/responsecurve.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      192 2023-07-20 18:16:27.000000 responsecurve-0.1/responsecurve.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 18:16:27.000000 responsecurve-0.1/responsecurve.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       43 2023-07-20 18:16:27.000000 responsecurve-0.1/responsecurve.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 18:16:27.000000 responsecurve-0.1/responsecurve.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-20 18:16:27.580477 responsecurve-0.1/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      401 2023-07-20 18:12:16.000000 responsecurve-0.1/setup.py
```

