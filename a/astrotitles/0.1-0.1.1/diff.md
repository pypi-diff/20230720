# Comparing `tmp/astrotitles-0.1.tar.gz` & `tmp/astrotitles-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrotitles-0.1.tar", last modified: Thu Jul 20 15:01:15 2023, max compression
+gzip compressed data, was "astrotitles-0.1.1.tar", last modified: Thu Jul 20 15:05:42 2023, max compression
```

## Comparing `astrotitles-0.1.tar` & `astrotitles-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:01:15.032633 astrotitles-0.1/
--rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1/LICENCE.txt
--rw-r--r--   0 ben        (501) staff       (20)     4590 2023-07-20 15:01:15.032716 astrotitles-0.1/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     4215 2023-07-20 04:14:08.000000 astrotitles-0.1/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:01:15.031481 astrotitles-0.1/astrotitles/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1/astrotitles/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     1368 2023-07-20 13:56:37.000000 astrotitles-0.1/astrotitles/cli.py
--rw-r--r--   0 ben        (501) staff       (20)     2066 2023-07-20 14:05:31.000000 astrotitles-0.1/astrotitles/transcriber.py
--rw-r--r--   0 ben        (501) staff       (20)     1137 2023-07-20 13:42:14.000000 astrotitles-0.1/astrotitles/utils.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:01:15.032455 astrotitles-0.1/astrotitles.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     4590 2023-07-20 15:01:14.000000 astrotitles-0.1/astrotitles.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-20 15:01:15.000000 astrotitles-0.1/astrotitles.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-20 15:01:14.000000 astrotitles-0.1/astrotitles.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       53 2023-07-20 15:01:14.000000 astrotitles-0.1/astrotitles.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-20 15:01:14.000000 astrotitles-0.1/astrotitles.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-20 15:01:14.000000 astrotitles-0.1/astrotitles.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-20 15:01:15.033017 astrotitles-0.1/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      764 2023-07-20 15:01:10.000000 astrotitles-0.1/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:05:42.865552 astrotitles-0.1.1/
+-rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.1/LICENCE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     4592 2023-07-20 15:05:42.865624 astrotitles-0.1.1/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     4215 2023-07-20 15:02:58.000000 astrotitles-0.1.1/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:05:42.864316 astrotitles-0.1.1/astrotitles/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.1/astrotitles/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     1368 2023-07-20 13:56:37.000000 astrotitles-0.1.1/astrotitles/cli.py
+-rw-r--r--   0 ben        (501) staff       (20)     2066 2023-07-20 14:05:31.000000 astrotitles-0.1.1/astrotitles/transcriber.py
+-rw-r--r--   0 ben        (501) staff       (20)     1137 2023-07-20 13:42:14.000000 astrotitles-0.1.1/astrotitles/utils.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:05:42.865424 astrotitles-0.1.1/astrotitles.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     4592 2023-07-20 15:05:42.000000 astrotitles-0.1.1/astrotitles.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-20 15:05:42.000000 astrotitles-0.1.1/astrotitles.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-20 15:05:42.000000 astrotitles-0.1.1/astrotitles.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       53 2023-07-20 15:05:42.000000 astrotitles-0.1.1/astrotitles.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-20 15:05:42.000000 astrotitles-0.1.1/astrotitles.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-20 15:05:42.000000 astrotitles-0.1.1/astrotitles.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-20 15:05:42.865856 astrotitles-0.1.1/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)      766 2023-07-20 15:05:07.000000 astrotitles-0.1.1/setup.py
```

### Comparing `astrotitles-0.1/LICENCE.txt` & `astrotitles-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1/PKG-INFO` & `astrotitles-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1
+Version: 0.1.1
 Summary: Automatically generate subtitles using the Astrotitles command line interface.
 Home-page: https://github.com/Astrotitles/cli
 Download-URL: https://github.com/Astrotitles/cli.git
 Author: Ben Webster
 License: AGPL-3.0
 Keywords: AI,Whisper AI,Subtitles
 Description-Content-Type: markdown
@@ -46,15 +46,15 @@
 
 1. Install via pip
    ```sh
    pip install astrotitles
    ```
 2. Install via pip (github)
    ```sh
-   npm install https://github.com/Astrotitles/cli.git
+   pip install https://github.com/Astrotitles/cli.git
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.1 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
@@ -11,15 +11,15 @@
 
                  View_Web_App Â· Report_Bug Â· Request_Feature
 ## Getting Started Astrotitles CLI is a tool that allows you to generate a srt/
 vtt subtitle file from a audio/video file. Astrotitles has word-level
 timestamps, allowing you to control how many characters are in each subtitle
 segment. ### Prerequisites - Python: https://www.python.org/downloads/ ###
 Installation 1. Install via pip ```sh pip install astrotitles ``` 2. Install
-via pip (github) ```sh npm install https://github.com/Astrotitles/cli.git ```
+via pip (github) ```sh pip install https://github.com/Astrotitles/cli.git ```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
 format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
 audio/video file positional arguments: input Input audio/video file to be
```

### Comparing `astrotitles-0.1/README.md` & `astrotitles-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 1. Install via pip
    ```sh
    pip install astrotitles
    ```
 2. Install via pip (github)
    ```sh
-   npm install https://github.com/Astrotitles/cli.git
+   pip install https://github.com/Astrotitles/cli.git
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 
                  View_Web_App Â· Report_Bug Â· Request_Feature
 ## Getting Started Astrotitles CLI is a tool that allows you to generate a srt/
 vtt subtitle file from a audio/video file. Astrotitles has word-level
 timestamps, allowing you to control how many characters are in each subtitle
 segment. ### Prerequisites - Python: https://www.python.org/downloads/ ###
 Installation 1. Install via pip ```sh pip install astrotitles ``` 2. Install
-via pip (github) ```sh npm install https://github.com/Astrotitles/cli.git ```
+via pip (github) ```sh pip install https://github.com/Astrotitles/cli.git ```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
 format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
 audio/video file positional arguments: input Input audio/video file to be
```

### Comparing `astrotitles-0.1/astrotitles/cli.py` & `astrotitles-0.1.1/astrotitles/cli.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1/astrotitles/transcriber.py` & `astrotitles-0.1.1/astrotitles/transcriber.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1/astrotitles/utils.py` & `astrotitles-0.1.1/astrotitles/utils.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1/astrotitles.egg-info/PKG-INFO` & `astrotitles-0.1.1/astrotitles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1
+Version: 0.1.1
 Summary: Automatically generate subtitles using the Astrotitles command line interface.
 Home-page: https://github.com/Astrotitles/cli
 Download-URL: https://github.com/Astrotitles/cli.git
 Author: Ben Webster
 License: AGPL-3.0
 Keywords: AI,Whisper AI,Subtitles
 Description-Content-Type: markdown
@@ -46,15 +46,15 @@
 
 1. Install via pip
    ```sh
    pip install astrotitles
    ```
 2. Install via pip (github)
    ```sh
-   npm install https://github.com/Astrotitles/cli.git
+   pip install https://github.com/Astrotitles/cli.git
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.1 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
@@ -11,15 +11,15 @@
 
                  View_Web_App Â· Report_Bug Â· Request_Feature
 ## Getting Started Astrotitles CLI is a tool that allows you to generate a srt/
 vtt subtitle file from a audio/video file. Astrotitles has word-level
 timestamps, allowing you to control how many characters are in each subtitle
 segment. ### Prerequisites - Python: https://www.python.org/downloads/ ###
 Installation 1. Install via pip ```sh pip install astrotitles ``` 2. Install
-via pip (github) ```sh npm install https://github.com/Astrotitles/cli.git ```
+via pip (github) ```sh pip install https://github.com/Astrotitles/cli.git ```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
 format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
 audio/video file positional arguments: input Input audio/video file to be
```

### Comparing `astrotitles-0.1/setup.py` & `astrotitles-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    version="0.1",
+    version="0.1.1",
     name="astrotitles",
     packages=find_packages(),
     license="AGPL-3.0",
     author="Ben Webster",
     url="https://github.com/Astrotitles/cli",
     download_url="https://github.com/Astrotitles/cli.git",
     keywords=["AI", "Whisper AI", "Subtitles"],
```

