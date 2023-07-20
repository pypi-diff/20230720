# Comparing `tmp/llfn-0.1.1.tar.gz` & `tmp/llfn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llfn-0.1.1.tar", max compression
+gzip compressed data, was "llfn-0.1.2.tar", max compression
```

## Comparing `llfn-0.1.1.tar` & `llfn-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1187 2023-07-20 10:51:32.176634 llfn-0.1.1/README.md
--rw-r--r--   0        0        0       43 2023-07-20 10:49:19.230094 llfn-0.1.1/llfn/__init__.py
--rw-r--r--   0        0        0     1334 2023-07-20 10:49:48.534775 llfn-0.1.1/llfn/llfn.py
--rw-r--r--   0        0        0      342 2023-07-20 10:51:52.819654 llfn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 llfn-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-07-20 11:12:16.267041 llfn-0.1.2/LICENSE
+-rw-r--r--   0        0        0    10940 2023-07-20 11:50:24.862974 llfn-0.1.2/README.md
+-rw-r--r--   0        0        0       43 2023-07-20 10:49:19.230094 llfn-0.1.2/llfn/__init__.py
+-rw-r--r--   0        0        0     1334 2023-07-20 11:14:39.091615 llfn-0.1.2/llfn/llfn.py
+-rw-r--r--   0        0        0      345 2023-07-20 11:50:29.436878 llfn-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11439 1970-01-01 00:00:00.000000 llfn-0.1.2/PKG-INFO
```

### Comparing `llfn-0.1.1/llfn/llfn.py` & `llfn-0.1.2/llfn/llfn.py`

 * *Files identical despite different names*

