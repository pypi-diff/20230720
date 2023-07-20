# Comparing `tmp/up_nextflap-0.0.3.tar.gz` & `tmp/up_nextflap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_nextflap-0.0.3.tar", last modified: Thu Jul 20 16:08:22 2023, max compression
+gzip compressed data, was "up_nextflap-0.0.4.tar", last modified: Thu Jul 20 16:25:17 2023, max compression
```

## Comparing `up_nextflap-0.0.3.tar` & `up_nextflap-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 16:08:22.997218 up_nextflap-0.0.3/
--rw-rw-rw-   0        0        0    11357 2023-06-24 19:12:50.000000 up_nextflap-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      340 2023-07-20 16:08:22.997218 up_nextflap-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-07-20 15:53:16.000000 up_nextflap-0.0.3/README.md
--rw-rw-rw-   0        0        0 16222656 2023-05-06 22:33:43.000000 up_nextflap-0.0.3/libz3.dll
--rw-rw-rw-   0        0        0   781312 2023-07-20 15:06:45.000000 up_nextflap-0.0.3/nextflap.pyd
--rw-rw-rw-   0        0        0       42 2023-07-20 16:08:22.997218 up_nextflap-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-07-20 15:15:57.000000 up_nextflap-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:08:22.987216 up_nextflap-0.0.3/up_nextflap/
--rw-rw-rw-   0        0        0       38 2023-07-04 14:38:59.000000 up_nextflap-0.0.3/up_nextflap/__init__.py
--rw-rw-rw-   0        0        0    47569 2023-07-20 13:39:27.000000 up_nextflap-0.0.3/up_nextflap/up_nextflap.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:08:22.996215 up_nextflap-0.0.3/up_nextflap.egg-info/
--rw-rw-rw-   0        0        0      340 2023-07-20 16:08:22.000000 up_nextflap-0.0.3/up_nextflap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-07-20 16:08:22.000000 up_nextflap-0.0.3/up_nextflap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 16:08:22.000000 up_nextflap-0.0.3/up_nextflap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-20 16:08:22.000000 up_nextflap-0.0.3/up_nextflap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-20 16:08:22.000000 up_nextflap-0.0.3/up_nextflap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 16:25:17.251152 up_nextflap-0.0.4/
+-rw-rw-rw-   0        0        0    11357 2023-06-24 19:12:50.000000 up_nextflap-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      340 2023-07-20 16:25:17.251152 up_nextflap-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-07-20 15:53:16.000000 up_nextflap-0.0.4/README.md
+-rw-rw-rw-   0        0        0 16222656 2023-05-06 22:33:43.000000 up_nextflap-0.0.4/libz3.dll
+-rw-rw-rw-   0        0        0   781312 2023-07-20 15:06:45.000000 up_nextflap-0.0.4/nextflap.pyd
+-rw-rw-rw-   0        0        0       42 2023-07-20 16:25:17.251152 up_nextflap-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      652 2023-07-20 16:24:57.000000 up_nextflap-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:25:17.251152 up_nextflap-0.0.4/up_nextflap/
+-rw-rw-rw-   0        0        0       38 2023-07-04 14:38:59.000000 up_nextflap-0.0.4/up_nextflap/__init__.py
+-rw-rw-rw-   0        0        0    47569 2023-07-20 13:39:27.000000 up_nextflap-0.0.4/up_nextflap/up_nextflap.py
+drwxrwxrwx   0        0        0        0 2023-07-20 16:25:17.251152 up_nextflap-0.0.4/up_nextflap.egg-info/
+-rw-rw-rw-   0        0        0      340 2023-07-20 16:25:17.000000 up_nextflap-0.0.4/up_nextflap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-07-20 16:25:17.000000 up_nextflap-0.0.4/up_nextflap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 16:25:17.000000 up_nextflap-0.0.4/up_nextflap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-20 16:25:17.000000 up_nextflap-0.0.4/up_nextflap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-20 16:25:17.000000 up_nextflap-0.0.4/up_nextflap.egg-info/top_level.txt
```

### Comparing `up_nextflap-0.0.3/LICENSE` & `up_nextflap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `up_nextflap-0.0.3/README.md` & `up_nextflap-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `up_nextflap-0.0.3/libz3.dll` & `up_nextflap-0.0.4/libz3.dll`

 * *Files identical despite different names*

### Comparing `up_nextflap-0.0.3/up_nextflap/up_nextflap.py` & `up_nextflap-0.0.4/up_nextflap/up_nextflap.py`

 * *Files identical despite different names*

