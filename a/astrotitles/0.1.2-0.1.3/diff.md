# Comparing `tmp/astrotitles-0.1.2.tar.gz` & `tmp/astrotitles-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrotitles-0.1.2.tar", last modified: Thu Jul 20 15:12:16 2023, max compression
+gzip compressed data, was "astrotitles-0.1.3.tar", last modified: Thu Jul 20 15:15:45 2023, max compression
```

## Comparing `astrotitles-0.1.2.tar` & `astrotitles-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:12:16.037705 astrotitles-0.1.2/
--rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.2/LICENCE.txt
--rw-r--r--   0 ben        (501) staff       (20)     4592 2023-07-20 15:12:16.037807 astrotitles-0.1.2/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     4215 2023-07-20 15:02:58.000000 astrotitles-0.1.2/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:12:16.036735 astrotitles-0.1.2/astrotitles/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.2/astrotitles/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     1393 2023-07-20 15:10:18.000000 astrotitles-0.1.2/astrotitles/cli.py
--rw-r--r--   0 ben        (501) staff       (20)     2114 2023-07-20 15:11:23.000000 astrotitles-0.1.2/astrotitles/transcriber.py
--rw-r--r--   0 ben        (501) staff       (20)     1137 2023-07-20 13:42:14.000000 astrotitles-0.1.2/astrotitles/utils.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:12:16.037582 astrotitles-0.1.2/astrotitles.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     4592 2023-07-20 15:12:15.000000 astrotitles-0.1.2/astrotitles.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-20 15:12:16.000000 astrotitles-0.1.2/astrotitles.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-20 15:12:15.000000 astrotitles-0.1.2/astrotitles.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       53 2023-07-20 15:12:15.000000 astrotitles-0.1.2/astrotitles.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-20 15:12:15.000000 astrotitles-0.1.2/astrotitles.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-20 15:12:15.000000 astrotitles-0.1.2/astrotitles.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-20 15:12:16.038231 astrotitles-0.1.2/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      766 2023-07-20 15:11:51.000000 astrotitles-0.1.2/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:15:45.023398 astrotitles-0.1.3/
+-rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.3/LICENCE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     4592 2023-07-20 15:15:45.023466 astrotitles-0.1.3/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     4215 2023-07-20 15:02:58.000000 astrotitles-0.1.3/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:15:45.022438 astrotitles-0.1.3/astrotitles/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.3/astrotitles/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     1393 2023-07-20 15:10:18.000000 astrotitles-0.1.3/astrotitles/cli.py
+-rw-r--r--   0 ben        (501) staff       (20)     2114 2023-07-20 15:11:23.000000 astrotitles-0.1.3/astrotitles/transcriber.py
+-rw-r--r--   0 ben        (501) staff       (20)     1137 2023-07-20 13:42:14.000000 astrotitles-0.1.3/astrotitles/utils.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:15:45.023267 astrotitles-0.1.3/astrotitles.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     4592 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-20 15:15:45.000000 astrotitles-0.1.3/astrotitles.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       53 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-20 15:15:45.023705 astrotitles-0.1.3/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)      766 2023-07-20 15:15:16.000000 astrotitles-0.1.3/setup.py
```

### Comparing `astrotitles-0.1.2/LICENCE.txt` & `astrotitles-0.1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.2/PKG-INFO` & `astrotitles-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatically generate subtitles using the Astrotitles command line interface.
 Home-page: https://github.com/Astrotitles/cli
 Download-URL: https://github.com/Astrotitles/cli.git
 Author: Ben Webster
 License: AGPL-3.0
 Keywords: AI,Whisper AI,Subtitles
 Description-Content-Type: markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1.2 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.3 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `astrotitles-0.1.2/README.md` & `astrotitles-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.2/astrotitles/cli.py` & `astrotitles-0.1.3/astrotitles/cli.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.2/astrotitles/transcriber.py` & `astrotitles-0.1.3/astrotitles/transcriber.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.2/astrotitles/utils.py` & `astrotitles-0.1.3/astrotitles/utils.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.2/astrotitles.egg-info/PKG-INFO` & `astrotitles-0.1.3/astrotitles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatically generate subtitles using the Astrotitles command line interface.
 Home-page: https://github.com/Astrotitles/cli
 Download-URL: https://github.com/Astrotitles/cli.git
 Author: Ben Webster
 License: AGPL-3.0
 Keywords: AI,Whisper AI,Subtitles
 Description-Content-Type: markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1.2 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.3 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `astrotitles-0.1.2/setup.py` & `astrotitles-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    version="0.1.2",
+    version="0.1.3",
     name="astrotitles",
     packages=find_packages(),
     license="AGPL-3.0",
     author="Ben Webster",
     url="https://github.com/Astrotitles/cli",
     download_url="https://github.com/Astrotitles/cli.git",
     keywords=["AI", "Whisper AI", "Subtitles"],
```

