# Comparing `tmp/splineplot-0.1.0.tar.gz` & `tmp/splineplot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splineplot-0.1.0.tar", max compression
+gzip compressed data, was "splineplot-0.2.0.tar", max compression
```

## Comparing `splineplot-0.1.0.tar` & `splineplot-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-07-20 11:43:07.546254 splineplot-0.1.0/LICENSE
--rw-r--r--   0        0        0      256 2023-07-20 12:06:34.656029 splineplot-0.1.0/README.md
--rw-r--r--   0        0        0      433 2023-07-20 11:46:53.745700 splineplot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1224 2023-07-20 12:05:06.408220 splineplot-0.1.0/splineplot/__init__.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 splineplot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-20 11:43:07.546254 splineplot-0.2.0/LICENSE
+-rw-r--r--   0        0        0      256 2023-07-20 12:06:34.656029 splineplot-0.2.0/README.md
+-rw-r--r--   0        0        0      437 2023-07-20 12:28:09.374689 splineplot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1224 2023-07-20 12:05:06.408220 splineplot-0.2.0/splineplot/__init__.py
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 splineplot-0.2.0/PKG-INFO
```

### Comparing `splineplot-0.1.0/LICENSE` & `splineplot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splineplot-0.1.0/splineplot/__init__.py` & `splineplot-0.2.0/splineplot/__init__.py`

 * *Files identical despite different names*

