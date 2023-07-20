# Comparing `tmp/astrotitles-0.1.3.tar.gz` & `tmp/astrotitles-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrotitles-0.1.3.tar", last modified: Thu Jul 20 15:15:45 2023, max compression
+gzip compressed data, was "astrotitles-0.1.4.tar", last modified: Thu Jul 20 15:24:58 2023, max compression
```

## Comparing `astrotitles-0.1.3.tar` & `astrotitles-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:15:45.023398 astrotitles-0.1.3/
--rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.3/LICENCE.txt
--rw-r--r--   0 ben        (501) staff       (20)     4592 2023-07-20 15:15:45.023466 astrotitles-0.1.3/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     4215 2023-07-20 15:02:58.000000 astrotitles-0.1.3/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:15:45.022438 astrotitles-0.1.3/astrotitles/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.3/astrotitles/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     1393 2023-07-20 15:10:18.000000 astrotitles-0.1.3/astrotitles/cli.py
--rw-r--r--   0 ben        (501) staff       (20)     2114 2023-07-20 15:11:23.000000 astrotitles-0.1.3/astrotitles/transcriber.py
--rw-r--r--   0 ben        (501) staff       (20)     1137 2023-07-20 13:42:14.000000 astrotitles-0.1.3/astrotitles/utils.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:15:45.023267 astrotitles-0.1.3/astrotitles.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     4592 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-20 15:15:45.000000 astrotitles-0.1.3/astrotitles.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       53 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-20 15:15:44.000000 astrotitles-0.1.3/astrotitles.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-20 15:15:45.023705 astrotitles-0.1.3/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      766 2023-07-20 15:15:16.000000 astrotitles-0.1.3/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:24:58.589514 astrotitles-0.1.4/
+-rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.4/LICENCE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     4596 2023-07-20 15:24:58.589586 astrotitles-0.1.4/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     4219 2023-07-20 15:20:44.000000 astrotitles-0.1.4/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:24:58.588636 astrotitles-0.1.4/astrotitles/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.4/astrotitles/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     1406 2023-07-20 15:21:10.000000 astrotitles-0.1.4/astrotitles/cli.py
+-rw-r--r--   0 ben        (501) staff       (20)     2114 2023-07-20 15:11:23.000000 astrotitles-0.1.4/astrotitles/transcriber.py
+-rw-r--r--   0 ben        (501) staff       (20)     1137 2023-07-20 13:42:14.000000 astrotitles-0.1.4/astrotitles/utils.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:24:58.589398 astrotitles-0.1.4/astrotitles.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     4596 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       52 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-20 15:24:58.589829 astrotitles-0.1.4/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)      765 2023-07-20 15:24:12.000000 astrotitles-0.1.4/setup.py
```

### Comparing `astrotitles-0.1.3/LICENCE.txt` & `astrotitles-0.1.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.3/PKG-INFO` & `astrotitles-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1.3
+Version: 0.1.4
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
-   pip install https://github.com/Astrotitles/cli.git
+   pip install git+https://github.com/Astrotitles/cli.git
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1.3 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.4 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
@@ -11,15 +11,16 @@
 
                  View_Web_App Â· Report_Bug Â· Request_Feature
 ## Getting Started Astrotitles CLI is a tool that allows you to generate a srt/
 vtt subtitle file from a audio/video file. Astrotitles has word-level
 timestamps, allowing you to control how many characters are in each subtitle
 segment. ### Prerequisites - Python: https://www.python.org/downloads/ ###
 Installation 1. Install via pip ```sh pip install astrotitles ``` 2. Install
-via pip (github) ```sh pip install https://github.com/Astrotitles/cli.git ```
+via pip (github) ```sh pip install git+https://github.com/Astrotitles/cli.git
+```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
 format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
 audio/video file positional arguments: input Input audio/video file to be
```

### Comparing `astrotitles-0.1.3/README.md` & `astrotitles-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 1. Install via pip
    ```sh
    pip install astrotitles
    ```
 2. Install via pip (github)
    ```sh
-   pip install https://github.com/Astrotitles/cli.git
+   pip install git+https://github.com/Astrotitles/cli.git
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -6,15 +6,16 @@
 
                  View_Web_App Â· Report_Bug Â· Request_Feature
 ## Getting Started Astrotitles CLI is a tool that allows you to generate a srt/
 vtt subtitle file from a audio/video file. Astrotitles has word-level
 timestamps, allowing you to control how many characters are in each subtitle
 segment. ### Prerequisites - Python: https://www.python.org/downloads/ ###
 Installation 1. Install via pip ```sh pip install astrotitles ``` 2. Install
-via pip (github) ```sh pip install https://github.com/Astrotitles/cli.git ```
+via pip (github) ```sh pip install git+https://github.com/Astrotitles/cli.git
+```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
 format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
 audio/video file positional arguments: input Input audio/video file to be
```

### Comparing `astrotitles-0.1.3/astrotitles/cli.py` & `astrotitles-0.1.4/astrotitles/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
+
 from astrotitles.utils import checkPositive
+from astrotitles.transcriber import Transcriber
 
-from transcriber import Transcriber
 from whisper.utils import str2bool
 
 def cli():
     parser = argparse.ArgumentParser(
         prog="astrotitles",
         description="Generate a srt/vtt subtitle file from audio/video file",
         epilog="Thanks for using Astrotitles CLI!"
```

### Comparing `astrotitles-0.1.3/astrotitles/transcriber.py` & `astrotitles-0.1.4/astrotitles/transcriber.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.3/astrotitles/utils.py` & `astrotitles-0.1.4/astrotitles/utils.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.3/astrotitles.egg-info/PKG-INFO` & `astrotitles-0.1.4/astrotitles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1.3
+Version: 0.1.4
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
-   pip install https://github.com/Astrotitles/cli.git
+   pip install git+https://github.com/Astrotitles/cli.git
    ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1.3 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.4 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
@@ -11,15 +11,16 @@
 
                  View_Web_App Â· Report_Bug Â· Request_Feature
 ## Getting Started Astrotitles CLI is a tool that allows you to generate a srt/
 vtt subtitle file from a audio/video file. Astrotitles has word-level
 timestamps, allowing you to control how many characters are in each subtitle
 segment. ### Prerequisites - Python: https://www.python.org/downloads/ ###
 Installation 1. Install via pip ```sh pip install astrotitles ``` 2. Install
-via pip (github) ```sh pip install https://github.com/Astrotitles/cli.git ```
+via pip (github) ```sh pip install git+https://github.com/Astrotitles/cli.git
+```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
 format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
 audio/video file positional arguments: input Input audio/video file to be
```

### Comparing `astrotitles-0.1.3/setup.py` & `astrotitles-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    version="0.1.3",
+    version="0.1.4",
     name="astrotitles",
     packages=find_packages(),
     license="AGPL-3.0",
     author="Ben Webster",
     url="https://github.com/Astrotitles/cli",
     download_url="https://github.com/Astrotitles/cli.git",
     keywords=["AI", "Whisper AI", "Subtitles"],
     install_requires=[
         'whisper_timestamped',
     ],
     description="Automatically generate subtitles using the Astrotitles command line interface.",
     long_description=long_description,
     long_description_content_type="markdown",
     entry_points={
-        'console_scripts': ['astrotitles=astrotitles.cli:main'],
+        'console_scripts': ['astrotitles=astrotitles.cli:cli'],
     },
     include_package_data=True,
 )
```

