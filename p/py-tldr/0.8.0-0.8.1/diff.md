# Comparing `tmp/py-tldr-0.8.0.tar.gz` & `tmp/py-tldr-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-tldr-0.8.0.tar", last modified: Sun Jul 16 04:54:53 2023, max compression
+gzip compressed data, was "py-tldr-0.8.1.tar", last modified: Thu Jul 20 20:26:08 2023, max compression
```

## Comparing `py-tldr-0.8.0.tar` & `py-tldr-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.535751 py-tldr-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 04:54:42.000000 py-tldr-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-16 04:54:53.535751 py-tldr-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-16 04:54:42.000000 py-tldr-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-16 04:54:42.000000 py-tldr-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 04:54:53.535751 py-tldr-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.531751 py-tldr-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.535751 py-tldr-0.8.0/src/py_tldr/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-16 04:54:42.000000 py-tldr-0.8.0/src/py_tldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-16 04:54:42.000000 py-tldr-0.8.0/src/py_tldr/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-16 04:54:42.000000 py-tldr-0.8.0/src/py_tldr/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-16 04:54:42.000000 py-tldr-0.8.0/src/py_tldr/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.535751 py-tldr-0.8.0/src/py_tldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.535751 py-tldr-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-16 04:54:42.000000 py-tldr-0.8.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.287676 py-tldr-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 20:25:57.000000 py-tldr-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-20 20:26:08.287676 py-tldr-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-20 20:25:57.000000 py-tldr-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-20 20:25:57.000000 py-tldr-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:26:08.287676 py-tldr-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.283676 py-tldr-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.287676 py-tldr-0.8.1/src/py_tldr/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-20 20:25:57.000000 py-tldr-0.8.1/src/py_tldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-20 20:25:57.000000 py-tldr-0.8.1/src/py_tldr/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-20 20:25:57.000000 py-tldr-0.8.1/src/py_tldr/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-20 20:25:57.000000 py-tldr-0.8.1/src/py_tldr/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.287676 py-tldr-0.8.1/src/py_tldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:26:08.000000 py-tldr-0.8.1/src/py_tldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:26:08.287676 py-tldr-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-20 20:25:57.000000 py-tldr-0.8.1/tests/test_cli.py
```

### Comparing `py-tldr-0.8.0/PKG-INFO` & `py-tldr-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tldr
-Version: 0.8.0
+Version: 0.8.1
 Summary: New Python client for tldr pages
 Author-email: iamgodot <xugodot@gmail.com>
 License: MIT
 Project-URL: Issue Tracker, https://github.com/iamgodot/py-tldr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-tldr-0.8.0/README.md` & `py-tldr-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `py-tldr-0.8.0/pyproject.toml` & `py-tldr-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-tldr-0.8.0/src/py_tldr/__init__.py` & `py-tldr-0.8.1/src/py_tldr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from logging.config import dictConfig
 from os import environ
 
 from .core import cli
 from .page import PageCache, PageFinder, PageFormatter
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 
 logging_config = {
     "version": 1,
     "formatters": {
         "default": {
             "format": "[%(asctime)s] %(levelname)s in func `%(funcName)s` by logger `%(name)s`: %(message)s",  # NOQA
```

### Comparing `py-tldr-0.8.0/src/py_tldr/core.py` & `py-tldr-0.8.1/src/py_tldr/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import toml
 from click import Choice, argument, option, pass_context, secho
 from click import command as command_
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
-from .page import DownloadError, PageFinder, PageFormatter
-from .parse import parse_command, parse_language, parse_platform
+from py_tldr.page import DownloadError, PageFinder, PageFormatter
+from py_tldr.parse import parse_command, parse_language, parse_platform
 
 try:
     from importlib.metadata import version
 
     VERSION_CLI = version("py_tldr")
 except ModuleNotFoundError:
     try:
```

### Comparing `py-tldr-0.8.0/src/py_tldr/page.py` & `py-tldr-0.8.1/src/py_tldr/page.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from collections import defaultdict
 from datetime import datetime
 from http import HTTPStatus
 from logging import getLogger
 from pathlib import Path as LibPath
 from shutil import rmtree
 from typing import Dict, List, Tuple
 from zipfile import ZipFile
@@ -57,16 +58,16 @@
         if not self._validate_page_file(page_file):
             return ""
         with open(page_file, encoding="utf8") as f:
             res = f.read()
         return res
 
     def set(self, name: str, platform: str, content: str, language: str = "en"):
-        (self.location / platform).mkdir(parents=True, exist_ok=True)
         page_file = self._make_page_file(platform, name, language)
+        page_file.parent.mkdir(parents=True, exist_ok=True)
         with open(page_file, "w", encoding="utf8") as f:
             f.write(content)
 
     def update(self, language: str):
         """Download pages for specified language."""
         LOGGER.debug("Update cache for language: %s", language)
         data = download_data(self.download_url, proxies={"https": self.proxy_url})
@@ -97,18 +98,18 @@
     def update_index(self) -> None:
         """Download newest index.json and restructure it for better searching."""
         data = download_data(
             "https://tldr.sh/assets/index.json", proxies={"https": self.proxy_url}
         )
         index, index_compact = json.loads(data), {}
         for command in index["commands"]:
-            index_compact[command["name"]] = {
-                "platforms": command["platform"],
-                "languages": command["language"],
-            }
+            name = command["name"]
+            index_compact[name] = defaultdict(list)
+            for target in command["targets"]:
+                index_compact[name][target["os"]].append(target["language"])
         with open(self.index_file, "w") as f:
             json.dump(index_compact, f)
 
 
 class DownloadError(Exception):
     def __init__(self, *args, status_code: int = 0, **kwargs):
         self.status_code = status_code
@@ -194,30 +195,32 @@
         with open(self.cache.index_file) as f:
             return json.load(f)
 
     def search(
         self, name: str, platform: str = "", languages: List[str] = None
     ) -> Tuple[str, str, str]:
         """Search index for the best platform and language for the command."""
-        index = self.get_index()
-        info = index.get(name)
+        info = self.get_index().get(name)
         if not info:
             return "", "", ""
 
-        platforms = info["platforms"]
-        if platform not in platforms:
-            platform = "common" if "common" in platforms else platforms[0]
-
-        language = ""
-        languages_info = info["languages"]
-        for lang in languages:
-            if lang in languages_info:
-                language = lang
+        platforms = list(info.keys())
+        for pf in [platform, "common"]:
+            if pf in platforms:
+                platforms.remove(pf)
+        res_platform, res_language = "", ""
+        for pf in [platform, "common"] + platforms:
+            if pf in info:
+                for lang in languages:
+                    if lang in info[pf]:
+                        res_platform, res_language = pf, lang
+                        break
+            if res_platform and res_language:
                 break
-        return name, platform, language
+        return name, res_platform, res_language
 
     def sync(self, language: str) -> None:
         self.cache.update(language)
         self.cache.update_index()
 
 
 class Formatter:
```

### Comparing `py-tldr-0.8.0/src/py_tldr/parse.py` & `py-tldr-0.8.1/src/py_tldr/parse.py`

 * *Files identical despite different names*

### Comparing `py-tldr-0.8.0/src/py_tldr.egg-info/PKG-INFO` & `py-tldr-0.8.1/src/py_tldr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tldr
-Version: 0.8.0
+Version: 0.8.1
 Summary: New Python client for tldr pages
 Author-email: iamgodot <xugodot@gmail.com>
 License: MIT
 Project-URL: Issue Tracker, https://github.com/iamgodot/py-tldr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-tldr-0.8.0/tests/test_cli.py` & `py-tldr-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

