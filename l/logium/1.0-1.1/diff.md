# Comparing `tmp/logium-1.0.tar.gz` & `tmp/logium-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logium-1.0.tar", last modified: Sat Jul 15 23:37:07 2023, max compression
+gzip compressed data, was "logium-1.1.tar", last modified: Thu Jul 20 12:57:23 2023, max compression
```

## Comparing `logium-1.0.tar` & `logium-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 23:37:07.688676 logium-1.0/
--rw-rw-rw-   0        0        0      157 2023-07-15 23:37:07.688676 logium-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 23:37:07.668450 logium-1.0/logium/
--rw-rw-rw-   0        0        0     6067 2023-07-15 23:35:48.000000 logium-1.0/logium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:37:07.688676 logium-1.0/logium.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-15 23:37:07.000000 logium-1.0/logium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-15 23:37:07.000000 logium-1.0/logium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 23:37:07.000000 logium-1.0/logium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 23:37:07.000000 logium-1.0/logium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 23:37:07.688676 logium-1.0/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-07-15 23:35:35.000000 logium-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:57:23.525413 logium-1.1/
+-rw-rw-rw-   0        0        0      157 2023-07-20 12:57:23.527415 logium-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 12:57:23.503408 logium-1.1/logium/
+-rw-rw-rw-   0        0        0     3653 2023-07-20 12:38:27.000000 logium-1.1/logium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:57:23.523407 logium-1.1/logium.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-20 12:57:23.000000 logium-1.1/logium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-20 12:57:23.000000 logium-1.1/logium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 12:57:23.000000 logium-1.1/logium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 12:57:23.000000 logium-1.1/logium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 12:57:23.531407 logium-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-07-20 12:55:28.000000 logium-1.1/setup.py
```

