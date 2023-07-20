# Comparing `tmp/stlib-1.3.1.tar.gz` & `tmp/stlib-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlib-1.3.1.tar", last modified: Sat Apr  1 04:23:15 2023, max compression
+gzip compressed data, was "stlib-2.0.tar", last modified: Thu Jul 20 16:56:17 2023, max compression
```

## Comparing `stlib-1.3.1.tar` & `stlib-2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 04:23:15.025846 stlib-1.3.1/
--rwxr-xr-x   0 root         (0) root         (0)    34916 2023-04-01 04:21:39.000000 stlib-1.3.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-01 04:21:39.000000 stlib-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4423 2023-04-01 04:23:15.025846 stlib-1.3.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3206 2023-04-01 04:21:39.000000 stlib-1.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1377 2023-04-01 04:21:39.000000 stlib-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 04:23:15.025846 stlib-1.3.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2641 2023-04-01 04:21:39.000000 stlib-1.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 04:23:15.021846 stlib-1.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 04:23:15.021846 stlib-1.3.1/src/steamworks/
--rw-r--r--   0 root         (0) root         (0)      817 2023-04-01 04:21:39.000000 stlib-1.3.1/src/steamworks/common.cpp
--rw-r--r--   0 root         (0) root         (0)    13290 2023-04-01 04:21:39.000000 stlib-1.3.1/src/steamworks/steam_api.cpp
--rw-r--r--   0 root         (0) root         (0)    11647 2023-04-01 04:21:39.000000 stlib-1.3.1/src/steamworks/steam_gameserver.cpp
--rw-r--r--   0 root         (0) root         (0)     2390 2023-04-01 04:21:39.000000 stlib-1.3.1/src/steamworks/steamworks.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 04:23:15.025846 stlib-1.3.1/src/stlib/
--rwxr-xr-x   0 root         (0) root         (0)     4035 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4101 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/client.py
--rw-r--r--   0 root         (0) root         (0)    23805 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/community.py
--rw-r--r--   0 root         (0) root         (0)     7529 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/internals.py
--rw-r--r--   0 root         (0) root         (0)    10815 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/login.py
--rw-r--r--   0 root         (0) root         (0)     5366 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/plugins.py
--rwxr-xr-x   0 root         (0) root         (0)     5714 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/universe.py
--rw-r--r--   0 root         (0) root         (0)    15108 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/utils.py
--rw-r--r--   0 root         (0) root         (0)    10526 2023-04-01 04:21:39.000000 stlib-1.3.1/src/stlib/webapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 04:23:15.025846 stlib-1.3.1/src/stlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4423 2023-04-01 04:23:15.000000 stlib-1.3.1/src/stlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      562 2023-04-01 04:23:15.000000 stlib-1.3.1/src/stlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 04:23:15.000000 stlib-1.3.1/src/stlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 04:23:14.000000 stlib-1.3.1/src/stlib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-01 04:23:15.000000 stlib-1.3.1/src/stlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-01 04:23:15.000000 stlib-1.3.1/src/stlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.636408 stlib-2.0/
+-rwxr-xr-x   0 root         (0) root         (0)    34916 2023-07-20 16:54:45.000000 stlib-2.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-20 16:54:45.000000 stlib-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-07-20 16:56:17.636408 stlib-2.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3206 2023-07-20 16:54:45.000000 stlib-2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-20 16:54:45.000000 stlib-2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:56:17.636408 stlib-2.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2577 2023-07-20 16:54:45.000000 stlib-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.632408 stlib-2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.632408 stlib-2.0/src/steamworks/
+-rw-r--r--   0 root         (0) root         (0)      817 2023-07-20 16:54:45.000000 stlib-2.0/src/steamworks/common.cpp
+-rw-r--r--   0 root         (0) root         (0)    13290 2023-07-20 16:54:45.000000 stlib-2.0/src/steamworks/steam_api.cpp
+-rw-r--r--   0 root         (0) root         (0)    11647 2023-07-20 16:54:45.000000 stlib-2.0/src/steamworks/steam_gameserver.cpp
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-07-20 16:54:45.000000 stlib-2.0/src/steamworks/steamworks.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.632408 stlib-2.0/src/stlib/
+-rwxr-xr-x   0 root         (0) root         (0)     4017 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4101 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/client.py
+-rw-r--r--   0 root         (0) root         (0)    24601 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/community.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/internals.py
+-rw-r--r--   0 root         (0) root         (0)    11034 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/login.py
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/plugins.py
+-rwxr-xr-x   0 root         (0) root         (0)     5688 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/universe.py
+-rw-r--r--   0 root         (0) root         (0)    15087 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11695 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/webapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.636408 stlib-2.0/src/stlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      562 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/top_level.txt
```

### Comparing `stlib-1.3.1/LICENSE.md` & `stlib-2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stlib-1.3.1/PKG-INFO` & `stlib-2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: stlib
-Version: 1.3.1
+Version: 2.0
 Summary: Async library that provides features related to Steam client and compatible stuffs
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
-Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
+Project-URL: homepage, https://github.com/calendulish/stlib
 Project-URL: documentation, https://lara.monster/stlib
 Project-URL: repository, https://github.com
-Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
+Project-URL: changelog, https://github.com/calendulish/stlib/releases
 Keywords: steam,valve
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 stlib
 -----
@@ -35,15 +34,15 @@
 [![Coverage](https://codecov.io/gh/calendulish/stlib/branch/master/graph/badge.svg?token=DMKFKEUUZP)](https://codecov.io/gh/calendulish/stlib)
 [![Quality](https://api.codiga.io/project/33228/score/svg)](https://app.codiga.io/project/33228/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/stlib.svg?style=flat)](https://github.com/calendulish/stlib/releases)
 
 Async library that provides features related to Steam client and compatible stuff
 
-WARNING: stlib is not intended to be used in game development, there is no support to callbacks and I'll not work on that.
+WARNING: stlib is not intended to be used in game development, there is no support to callbacks, and I'll not work on that.
 stlib is intended to develop console or GUI applications that need interaction with SteamAPI or SteamWebAPI.
 
 stlib now supports plugins!
 ---------------------------
 See more at: [stlib-plugins](https://github.com/calendulish/stlib-plugins)
 
 Dependencies to build SteamWorks Python Extension (Optional)
@@ -79,15 +78,15 @@
 Made with stlib
 ---------------
 
 Steam Tools NG - https://github.com/calendulish/steam-tools-ng
 
 ___________________________________________________________________________________________
 
-This is an work in progress. You can request new features.
+This is a work in progress. You can request new features.
 
 The stlib is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 The stlib is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
```

### Comparing `stlib-1.3.1/README.md` & `stlib-2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Coverage](https://codecov.io/gh/calendulish/stlib/branch/master/graph/badge.svg?token=DMKFKEUUZP)](https://codecov.io/gh/calendulish/stlib)
 [![Quality](https://api.codiga.io/project/33228/score/svg)](https://app.codiga.io/project/33228/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/stlib.svg?style=flat)](https://github.com/calendulish/stlib/releases)
 
 Async library that provides features related to Steam client and compatible stuff
 
-WARNING: stlib is not intended to be used in game development, there is no support to callbacks and I'll not work on that.
+WARNING: stlib is not intended to be used in game development, there is no support to callbacks, and I'll not work on that.
 stlib is intended to develop console or GUI applications that need interaction with SteamAPI or SteamWebAPI.
 
 stlib now supports plugins!
 ---------------------------
 See more at: [stlib-plugins](https://github.com/calendulish/stlib-plugins)
 
 Dependencies to build SteamWorks Python Extension (Optional)
@@ -50,15 +50,15 @@
 Made with stlib
 ---------------
 
 Steam Tools NG - https://github.com/calendulish/steam-tools-ng
 
 ___________________________________________________________________________________________
 
-This is an work in progress. You can request new features.
+This is a work in progress. You can request new features.
 
 The stlib is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 The stlib is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
```

### Comparing `stlib-1.3.1/pyproject.toml` & `stlib-2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stlib"
-version = "1.3.1"
+version = "2.0"
 description = "Async library that provides features related to Steam client and compatible stuffs"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPLv3"}
 keywords = ["steam", "valve"]
 authors = [{email = "dev@lara.monster"}, {name = "Lara Maia"}]
 classifiers = [
-  "Development Status :: 5 - Production/Stable",
+  "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Topic :: Games/Entertainment",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Typing :: Typed"
 ]
 
 dependencies = [
   "aiohttp",
   "beautifulsoup4",
   "rsa"
 ]
 
 [project.urls]
-homepage = "https://github.com/calendulish/steam-tools-ng"
+homepage = "https://github.com/calendulish/stlib"
 documentation = "https://lara.monster/stlib"
 repository = "https://github.com"
-changelog = "https://github.com/calendulish/steam-tools-ng/releases"
+changelog = "https://github.com/calendulish/stlib/releases"
 
 [tool.setuptools]
 include-package-data = true
 zip-safe = false
 package-dir = {"" = "src"}
 packages = ["stlib"]
```

### Comparing `stlib-1.3.1/setup.py` & `stlib-2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,54 +24,48 @@
 from setuptools.command.build_ext import build_ext
 from pathlib import Path
 
 SOURCES_PATH = Path(os.getenv("SOURCES_PATH", Path('src', 'steamworks')))
 SDK_PATH = Path(os.getenv("SDK_PATH", Path(SOURCES_PATH, 'sdk')))
 HEADERS_PATH = Path(os.getenv("HEADERS_PATH", Path(SDK_PATH, 'public')))
 
-if sys.maxsize > 2 ** 32:
-    arch = '64'
-else:
-    arch = ''
-
+arch = '64' if sys.maxsize > 2 ** 32 else ''
 if os.name == 'nt':
-    REDIST_PATH = 'win' + arch
-    API_NAME = 'steam_api' + arch
-    EXTRA_NAME = API_NAME + '.dll'
+    REDIST_PATH = f'win{arch}'
+    API_NAME = f'steam_api{arch}'
+    EXTRA_NAME = f'{API_NAME}.dll'
 elif os.name == 'posix':
-    REDIST_PATH = 'linux' + arch if arch else '32'
+    REDIST_PATH = f'linux{arch}' if arch else '32'
     API_NAME = 'steam_api'
-    EXTRA_NAME = 'lib' + API_NAME + '.so'
+    EXTRA_NAME = f'lib{API_NAME}.so'
 else:
     print('Your system is currently not supported.')
     sys.exit(1)
 
 
 class OptionalBuild(build_ext):
     def run(self):
         bin_path = SDK_PATH / 'redistributable_bin'
         output_dir = Path(self.build_lib) / 'stlib'
         output_dir.mkdir(parents=True, exist_ok=True)
-        compatible = True if platform.machine() in ['x86_64', 'amd64', 'i386', 'x86'] else False
+        compatible = platform.machine().lower() in ['x86_64', 'amd64', 'i386', 'x86']
 
         if compatible and HEADERS_PATH.exists():
             shutil.copy(
                 bin_path / REDIST_PATH / EXTRA_NAME,
                 output_dir,
             )
             super().run()
         else:
             self.warn("build of steam_api C extension has been disabled")
 
 
-all_sources = []
-for file in SOURCES_PATH.iterdir():
-    if file.suffix == ".cpp":
-        all_sources.append(str(file))
-
+all_sources = [
+    str(file) for file in SOURCES_PATH.iterdir() if file.suffix == ".cpp"
+]
 steamworks = Extension(
     'stlib.steamworks',
     sources=all_sources,
     include_dirs=[SOURCES_PATH, HEADERS_PATH],
     library_dirs=[str(SDK_PATH / 'redistributable_bin' / REDIST_PATH)],
     libraries=[API_NAME],
     extra_compile_args=['-D_CRT_SECURE_NO_WARNINGS', '/std:c++17' if 'MSC' in sys.version else '-std=c++17'],
```

### Comparing `stlib-1.3.1/src/steamworks/common.cpp` & `stlib-2.0/src/steamworks/common.cpp`

 * *Files identical despite different names*

### Comparing `stlib-1.3.1/src/steamworks/steam_api.cpp` & `stlib-2.0/src/steamworks/steam_api.cpp`

 * *Files identical despite different names*

### Comparing `stlib-1.3.1/src/steamworks/steam_gameserver.cpp` & `stlib-2.0/src/steamworks/steam_gameserver.cpp`

 * *Files identical despite different names*

### Comparing `stlib-1.3.1/src/steamworks/steamworks.cpp` & `stlib-2.0/src/steamworks/steamworks.cpp`

 * *Files identical despite different names*

### Comparing `stlib-1.3.1/src/stlib/__init__.py` & `stlib-2.0/src/stlib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 stlib
 -----
 
 Async library that provides features related to Steam client and compatible stuff
 
 WARNING: stlib is not intended to be used in game development.
-There is no support to callbacks and I'll not work on that.
+There is no support for callbacks, and I'll not work on that.
 stlib is intended to develop console or GUI applications that need interaction with SteamAPI or SteamWebAPI.
 
 stlib now supports plugins!
 ---------------------------
 See more at: [stlib-plugins](https://github.com/calendulish/stlib-plugins)
 
 Dependencies to build SteamWorks Python Extension (Optional)
@@ -52,25 +52,25 @@
 Made with stlib
 ---------------
 
 Steam Tools NG - https://github.com/calendulish/steam-tools-ng
 
 ___________________________________________________________________________________________
 
-This is an work in progress. You can request new features.
+This is a work in progress. You can request new features.
 
 The stlib is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 The stlib is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program.
-If not, see http://www.gnu.org/licenses/.
+If not, see https://www.gnu.org/licenses/.
 
 Lara Maia <dev@lara.monster> 2015 ~ 2023
 
 """
 import os
 import site
 import sys
@@ -113,12 +113,11 @@
 
 
 async def set_default_http_params(session_index: int, *args: Any, **kwargs: Any) -> aiohttp.ClientSession:
     """
     Set default http params for stlib modules at given `session_index`
     :param session_index: Session number
     :param args: extra args when creating a new http session
-    :param kwargs: extra kargs when creating a new http session
-    :return: http session
+    :param kwargs: extra kwargs when creating a new http session
+    :return: `aiohttp.ClientSession`
     """
-    http_session = await _Base.new_http_session(session_index, *args, **kwargs)
-    return http_session
+    return await _Base.new_http_session(session_index, *args, **kwargs)
```

### Comparing `stlib-1.3.1/src/stlib/client.py` & `stlib-2.0/src/stlib/client.py`

 * *Files identical despite different names*

### Comparing `stlib-1.3.1/src/stlib/community.py` & `stlib-2.0/src/stlib/community.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,43 +60,60 @@
     """Expiration"""
     actions: List[Dict[str, str]]
     """List with custom actions for `Item`"""
 
 
 class Order(NamedTuple):
     name: str
+    """Item Name"""
     appid: int
+    """App ID"""
     hash_name: str
+    """Hash name"""
     type: str
+    """Item type"""
     price: str
+    """Item price"""
     amount: int
+    """Item amount"""
     orderid: int
+    """Order ID"""
     contextid: Optional[int]
+    """Context ID"""
     actions: List[Dict[str, str]]
+    """List of available actions"""
     icon_url: str
+    """Small icon url"""
     icon_url_large: str
+    """Large icon url"""
 
 
 class Confirmation(NamedTuple):
     mode_accept: str
     """Confirmation mode for accept action"""
     mode_cancel: str
     """Confirmation mode for cancel action"""
-    confid: int
-    """Configuration ID"""
+    id: int
+    """Confirmation ID"""
     creatorid: int
     """Creator ID"""
-    key: int
-    """Confirmation key"""
+    nonce: int
+    """Nonce key"""
+    time: int
+    """Creation time"""
+    icon: str
+    """Icon"""
     type: int
     """Confirmation type"""
+    summary: List[str]
+    """Trade summary"""
+    to: str
+    """Trade partner"""
     give: List[str]
     """List of items to give"""
-    to: str
-    """Trade destination"""
     receive: List[str]
     """List of items to receive"""
 
 
 class Badge(NamedTuple):
     name: str
     """Name"""
@@ -154,25 +171,23 @@
             steamid: universe.SteamId,
             identity_secret: str,
             tag: str,
     ) -> Dict[str, Any]:
         json_data = await self.request_json(f'{self.api_url}/ISteamWebAPIUtil/GetServerInfo/v1')
         server_time = json_data['servertime']
 
-        params = {
+        return {
             'p': deviceid,
             'a': steamid.id64,
             'k': universe.generate_time_hash(server_time, tag, identity_secret),
             't': server_time,
             'm': 'android',
             'tag': tag,
         }
 
-        return params
-
     async def get_steam_session_id(self) -> str:
         """Get steam session id"""
         response = await self.request(self.community_url)
 
         if 'sessionid' in response.cookies:
             return str(response.cookies['sessionid'].value)
 
@@ -200,31 +215,31 @@
         :param count: Max item count per page
         :return: List of `Item`
         """
         params = {'l': 'english', 'count': count}
         json_data = {}
 
         while True:
-            json_data.update(await self.request_json(
+            json_data |= await self.request_json(
                 f"{self.community_url}/inventory/{steamid.id64}/{appid}/{contextid}",
                 params=params,
-            ))
+                auto_recovery=False,
+            )
 
             if not json_data['success']:
                 raise AttributeError("Unable to get inventory details")
 
             if json_data['total_inventory_count'] == 0:
                 raise InventoryEmptyError(steamid, appid, contextid, "Inventory is empty")
 
-            if 'last_assetid' in json_data:
-                params['start_assetid'] = json_data['last_assetid']
-                await asyncio.sleep(10)
-            else:
+            if 'last_assetid' not in json_data:
                 break
 
+            params['start_assetid'] = json_data['last_assetid']
+            await asyncio.sleep(10)
         items = []
         for item in json_data['descriptions']:
             if 'market_name' in item:
                 name = item['market_name']
 
                 if item['type']:
                     name += f" - {item['type']}"
@@ -233,14 +248,15 @@
 
             for asset in json_data['assets']:
                 if asset['classid'] == item['classid']:
                     amount = asset['amount']
                     assetid = asset['assetid']
                     break
 
+            # noinspection PyUnboundLocalVariable
             kwargs = {
                 'name': name,
                 'type': item['type'],
                 'amount': amount,
                 'marketable': item['marketable'],
                 'tradable': item['tradable'],
                 'commodity': item['commodity'],
@@ -258,15 +274,15 @@
 
         return items
 
     async def get_badges(self, steamid: universe.SteamId, show_no_drops: bool = False) -> List[Badge]:
         """
         Get badges
         :param steamid: `SteamId`
-        :param show_no_drops: If true get badges with no drops too
+        :param show_no_drops: If true, get badges with no drops as well
         :return: List of `Badge`
         """
         badges = []
         params: Dict[str, Union[str, int]] = {'l': 'english'}
         html = await self.request_html(f"{steamid.profile_url}/badges/", params=params)
         badges_raw = html.find_all('div', class_='badge_title_row')
 
@@ -348,72 +364,63 @@
         Get confirmations for logged user
         :param identity_secret: User identity secret
         :param steamid: `SteamId`
         :param deviceid: Device ID
         :return: List of `Confirmation`
         """
         params = await self._new_mobileconf_query(deviceid, steamid, identity_secret, 'conf')
+        json_data = await self.request_json(f'{self.mobileconf_url}/getlist', params=params)
 
-        response = await self.request(
-            f'{self.mobileconf_url}/conf',
-            params=params,
-            allow_redirects=False,
-            raise_for_status=False,
-        )
-
-        if response.status == 302:
+        if not json_data['success']:
             raise login.LoginError('User is not logged in')
 
-        html = await self.get_html(response)
-
         confirmations = []
-        for confirmation in html.find_all('div', class_='mobileconf_list_entry'):
+        for confirmation in json_data['conf']:
             details_params = await self._new_mobileconf_query(
                 deviceid,
                 steamid,
                 identity_secret,
-                f"details{confirmation['data-confid']}",
+                f"details{confirmation['id']}",
             )
 
-            confid = confirmation['data-confid']
-            key = confirmation['data-key']
-            type_ = confirmation['data-type']
-
             log.debug(
                 "Getting human readable information from %s as type %s (%s)",
-                confid,
-                type_,
-                "Market" if type_ == '3' else 'Trade Item',
+                confirmation['id'],
+                confirmation['type'],
+                "Market" if confirmation['type'] == 3 else 'Trade Item',
             )
 
-            json_data = await self.request_json(f"{self.mobileconf_url}/details/{confid}", params=details_params)
+            json_data = await self.request_json(
+                f"{self.mobileconf_url}/details/{confirmation['id']}",
+                params=details_params,
+            )
 
             if not json_data['success']:
-                raise AttributeError(f"Unable to get details for confirmation {confid}")
+                raise AttributeError(f"Unable to get details for confirmation {confirmation['id']}")
 
             html = BeautifulSoup(json_data["html"], 'html.parser')
 
-            if type_ == "1" or type_ == "2":
-                to = html.find('span', class_="trade_partner_headline_sub").get_text()
+            if confirmation['type'] in (1, 2):
+                offer_friend = html.find('div', class_="mobileconf_offer_friend")
+                to = offer_friend.find_next('span').text.strip()
 
                 item_list = html.find_all('div', class_="tradeoffer_item_list")
 
                 give = []
                 for item in item_list[0].find_all('div', class_='trade_item'):
                     appid, classid = item['data-economy-item'].split('/')[1:3]
                     name = await self.get_item_name(appid, classid)
                     give.append(name)
 
                 receive = []
                 for item in item_list[1].find_all('div', class_='trade_item'):
                     appid, classid = item['data-economy-item'].split('/')[1:3]
                     name = await self.get_item_name(appid, classid)
                     receive.append(name)
-
-            elif type_ == "3":
+            elif confirmation['type'] == 3:
                 to = "Market"
 
                 listing_prices = html.find('div', class_="mobileconf_listing_prices")
                 final_price = listing_prices.find(text=lambda element: 'You receive' in element.text).next.next.strip()
                 sell_price = listing_prices.find(text=lambda element: 'Buyer pays' in element.text).next.next.strip()
                 receive = [f"{final_price} ({sell_price})"]
 
@@ -424,40 +431,43 @@
                     give = [json_data['market_name']]
 
                     if json_data['type']:
                         give[0] += f" - {json_data['type']}"
                 else:
                     give = [json_data['type']]
 
-                quantity = listing_prices.find(text=lambda element: 'Quantity' in element.text)
-
-                if quantity:
+                if quantity := listing_prices.find(
+                    text=lambda element: 'Quantity' in element.text
+                ):
                     give[0] = f'{quantity.next.next.strip()} {give[0]}'
-            elif type_ == '5':
+            elif confirmation['type'] == 5:
                 to = "Steam"
                 give = ["Change phone number"]
                 receive = ["Phone number has not been entered yet"]
-            elif type_ == '6':
+            elif confirmation['type'] == 6:
                 to = "Steam"
                 give = ["Make changes to your account"]
                 receive = [f"Number to match: {html.find_all('div')[3].text.strip()}"]
             else:
                 to = "NotImplemented"
-                give = [f"{confid}"]
-                receive = [f"{key}"]
+                give = [f"{confirmation['id']}"]
+                receive = [f"{confirmation['nonce']}"]
 
             confirmations.append(
                 Confirmation(
-                    confirmation['data-accept'],
-                    confirmation['data-cancel'],
-                    int(confid),
-                    int(confirmation['data-creator']),
-                    int(key),
-                    int(type_),
-                    give, to, receive,
+                    confirmation['accept'],
+                    confirmation['cancel'],
+                    confirmation['id'],
+                    confirmation['creator_id'],
+                    confirmation['nonce'],
+                    confirmation['creation_time'],
+                    confirmation['icon'],
+                    confirmation['type'],
+                    confirmation['summary'],
+                    to, give, receive,
                 )
             )
 
         return confirmations
 
     async def get_card_drops_remaining(self, steamid: universe.SteamId, appid: int) -> int:
         """
@@ -472,20 +482,19 @@
         stats = html.find('div', class_='badge_title_stats_drops')
 
         if stats is None:
             raise BadgeError(f"Unable to get card count for {appid}")
 
         progress = stats.find('span', class_='progress_info_bold')
 
-        if not progress or "No" in progress.text:
-            cards = 0
-        else:
-            cards = int(progress.text.split(' ', 3)[0])
-
-        return cards
+        return (
+            0
+            if not progress or "No" in progress.text
+            else int(progress.text.split(' ', 3)[0])
+        )
 
     async def get_last_played_game(self, steamid: universe.SteamId) -> Optional[int]:
         """
         Get last played game
         :param steamid: `SteamId`
         :return: gameid or None
         """
@@ -504,25 +513,26 @@
         Get list of orders for current logged user
         :return: sell orders (`Order`) and buy orders (`Order`)
         """
         params = {"start": 0, "count": 100, "norender": 1, "l": "english"}
         json_data = {}
 
         while True:
-            json_data.update(await self.request_json(f"{self.community_url}/market/mylistings", params=params))
+            json_data |= await self.request_json(
+                f"{self.community_url}/market/mylistings", params=params
+            )
 
             if not json_data['success']:
                 raise AttributeError("Unable to get order details")
 
-            if json_data['total_count'] > 100:
-                params['start'] += 100
-                await asyncio.sleep(5)
-            else:
+            if json_data['total_count'] <= 100:
                 break
 
+            params['start'] += 100
+            await asyncio.sleep(5)
         my_sell_orders = []
 
         for order in json_data['listings']:
             asset = order['asset']
             price_raw = int(order['price']) + int(order['fee'])
 
             my_sell_orders.append(
@@ -593,17 +603,17 @@
             'language': 'english',
             'currency': currency,
             'country': country,
             'item_nameid': item_nameid,
             'norender': 1,
         }
 
-        json_data = await self.request_json(f"{self.community_url}/market/itemordershistogram", params=params)
-
-        return json_data
+        return await self.request_json(
+            f"{self.community_url}/market/itemordershistogram", params=params
+        )
 
     async def send_trade_offer(
             self,
             steamid: universe.SteamId,
             token: str,
             contextid: int,
             me: List[Tuple[int, int, int]],
@@ -614,34 +624,32 @@
         :param steamid: `SteamId`
         :param token: Partner token
         :param contextid: Context ID
         :param me: List of my items to trade
         :param them: List of them items to trade
         :return: Json data
         """
-        me_assets = []
-
-        for item in me:
-            me_assets.append({
+        me_assets = [
+            {
                 'appid': item[0],
                 'contextid': str(contextid),
                 'amount': item[2],
                 'assetid': str(item[1]),
-            })
-
-        them_assets = []
-
-        for item in them:
-            them_assets.append({
+            }
+            for item in me
+        ]
+        them_assets = [
+            {
                 'appid': item[0],
                 'contextid': str(contextid),
                 'amount': item[2],
                 'assetid': str(item[1]),
-            })
-
+            }
+            for item in them
+        ]
         offer = {
             'newversion': True,
             'version': len(me_assets) + len(them_assets) + 1,
             'me': {
                 'assets': me_assets,
                 'currency': [],
                 'ready': False,
@@ -660,16 +668,17 @@
             'tradeoffermessage': '',
             'json_tradeoffer': json.dumps(offer),
             'captcha': None,  # TODO
             'trade_offer_create_params': json.dumps({'trade_offer_access_token': token}),
         }
 
         headers = {'referer': f'{self.community_url}/tradeoffer/new/?partner={steamid.id3}&token={token}'}
-        json_data = await self.request_json(f"{self.community_url}/tradeoffer/new/send", data=data, headers=headers)
-        return json_data
+        return await self.request_json(
+            f"{self.community_url}/tradeoffer/new/send", data=data, headers=headers
+        )
 
     async def send_confirmation(
             self,
             identity_secret: str,
             steamid: universe.SteamId,
             deviceid: str,
             trade_id: int,
@@ -684,32 +693,46 @@
         :param trade_id: trade ID
         :param trade_key: trade key
         :param action: Action to taken from [allow, cancel]
         :return: Json data
         """
         extra_params = {'cid': trade_id, 'ck': trade_key, 'op': action}
         params = await self._new_mobileconf_query(deviceid, steamid, identity_secret, 'conf')
-        json_data = await self.request_json(f'{self.mobileconf_url}/ajaxop', params={**params, **extra_params})
-        return json_data
+        return await self.request_json(
+            f'{self.mobileconf_url}/ajaxop', params={**params, **extra_params}
+        )
 
     async def revoke_api_key(self) -> None:
+        """
+        Revoke the developer API Key associated with the current logged account
+        :return: None
+        """
         data = {'sessionid': await self.get_steam_session_id()}
         await self.request(f'{self.community_url}/dev/revokekey', data=data)
 
     async def register_api_key(self, domain: str = 'stlib') -> None:
+        """
+        Register a new developer API Key for the current logged account
+        :param domain: app name
+        :return: None
+        """
         data = {
             'domain': domain,
             'agreeToTerms': 'agreed',
             'sessionid': await self.get_steam_session_id(),
             'Submit': 'Register',
         }
 
         await self.request(f'{self.community_url}/dev/registerkey', data=data)
 
     async def get_api_key(self) -> Tuple[str, str]:
+        """
+        Get developer API Key for the current logged account
+        :return: key, domain
+        """
         html = await self.request_html(f'{self.community_url}/dev/apikey')
         main = html.find('div', id='mainContents')
 
         if 'Access Denied' in main.find('h2').text:
             raise PermissionError("Your Steam account is limited")
 
         contents = html.find('div', id="bodyContents_ex")
```

### Comparing `stlib-1.3.1/src/stlib/internals.py` & `stlib-2.0/src/stlib/internals.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             game = await internals.get_game(480)
             ```
         """
         super().__init__(**kwargs)
         self.store_url = store_url
 
     # Despite this apparently accepts comma-separated parameters
-    # actualy isn't working without price_overview filter
+    # actually isn't working without price_overview filter
     async def get_game(self, appid: int) -> Game:
         """Get game details. See `Game`"""
         appid_string = str(appid)
         params = {'appids': appid_string}
         json_data = await self.request_json(f'{self.store_url}/api/appdetails', params=params)
 
         if not json_data[appid_string]['success']:
@@ -142,15 +142,15 @@
         return Game(**game_params)
 
     # Despite this apparently accepts comma-separated parameters, actually isn't working
     async def get_package(self, packageid: int) -> Package:
         """Get package details. See `Package`"""
         packageid_string = str(packageid)
         params = {'packageids': packageid_string}
-        json_data = await self.request_json(f'{self.store_url}/api/packagedetails', params=params)
+        json_data = await self.request_json(f'{self.store_url}/api/packagedetails', params=params, auto_recovery=False)
 
         if not json_data[packageid_string]['success']:
             raise ValueError(f"Failed to get details for package {packageid_string}")
 
         package_params = {
             'packageid': packageid_string,
             'name': json_data[packageid_string]['data']['name'],
```

### Comparing `stlib-1.3.1/src/stlib/login.py` & `stlib-2.0/src/stlib/login.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,73 +16,97 @@
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 """
 `login` interface is used to interact with undocumented steam login methods
 it supports both desktop and mobile login at steam services
 """
 
-import asyncio
-import http.cookies
-import json
 import logging
-import time
-from typing import Any, Dict, NamedTuple, Optional
+import random
+from enum import Enum
+from typing import Any, Dict, NamedTuple, Optional, List
 
 import rsa
 
 from . import universe, utils
 
 log = logging.getLogger(__name__)
 
 
+class TransferInfo(NamedTuple):
+    url: str
+    """url associated"""
+    nonce: str
+    """Nonce key"""
+    auth: str
+    """Auth token"""
+
+
 class LoginData(NamedTuple):
-    auth: Dict[str, Any]
-    """Auth data"""
-    oauth: Dict[str, Any]
-    """OAuth data"""
+    steamid: int
+    """Steam ID"""
+    client_id: str
+    """Client ID"""
+    sessionid: str
+    """Session ID"""
+    refresh_token: str
+    """Refresh token"""
+    access_token: str
+    """Access token"""
+    transfer_info: List[TransferInfo]
+    """List of `TransferInfo` associated"""
+
+
+class AuthCodeType(Enum):
+    email = 2
+    """email code"""
+    device = 3
+    """device code"""
+    machine = 6
+    """machine token"""
 
 
 class LoginError(ValueError):
     """Raised when login can`t be completed"""
-    pass
+
+    def __init__(self, message: str, captcha_requested: bool = False) -> None:
+        super().__init__(message)
+
+        self.captcha_requested = captcha_requested
 
 
 class LoginBlockedError(LoginError):
     """Raised when user is temporarily blocked from login session"""
     pass
 
 
 class CaptchaError(LoginError):
     """Raised when captcha is requested"""
 
-    def __init__(self, captcha_gid: int, captcha: bytes, message: str) -> None:
-        super().__init__(message)
-
-        self.captcha_gid = captcha_gid
-        self.captcha = captcha
+    def __init__(self, message: str) -> None:
+        super().__init__(message, captcha_requested=True)
 
 
 class MailCodeError(LoginError):
     """Raised when mail code is requested"""
     pass
 
 
 class TwoFactorCodeError(LoginError):
-    """Raised when two factor code is requested"""
+    """Raised when two-factor code is requested"""
     pass
 
 
 # Don't instantiate this class directly!
 # Use get_session to support multiple sessions!
 class Login(utils.Base):
     def __init__(
             self,
             *,
-            login_url: str = 'https://steamcommunity.com/login',
-            mobile_login_url: str = 'https://steamcommunity.com/mobilelogin',
+            login_url: str = 'https://login.steampowered.com',
             steamguard_url: str = 'https://steamcommunity.com/steamguard',
             api_url: str = 'https://api.steampowered.com',
             **kwargs: Any,
     ) -> None:
         """
         Main login class used to login a user on steam session
 
@@ -95,15 +119,14 @@
             await login_session.do_login()
             ```
         """
         super().__init__(**kwargs)
         self._username: Optional[str] = None
         self.__password: Optional[str] = None
         self.login_url = login_url
-        self.mobile_login_url = mobile_login_url
         self.steamguard_url = steamguard_url
         self.api_url = api_url
         self.login_trial = 3
 
     @property
     def username(self) -> str:
         """Steam username"""
@@ -121,63 +144,50 @@
         """Protected steam password"""
         raise PermissionError('Passwords are protected')
 
     @password.setter
     def password(self, __password: str) -> None:
         self.__password = __password
 
-    async def _new_login_data(
-            self,
-            authenticator_code: str = '',
-            emailauth: str = '',
-            captcha_gid: int = -1,
-            captcha_text: str = '',
-            mobile_login: bool = False,
-    ) -> Dict[str, Any]:
+    async def _new_login_data(self, mobile_login: bool = False) -> Dict[str, Any]:
         steam_key = await self.get_steam_key(self.username)
 
         if not self.__password:
             raise AttributeError('Password is required to login')
 
         encrypted_password = universe.encrypt_password(steam_key, self.__password)
 
-        data = {
-            'username': self.username,
-            "password": encrypted_password.decode(),
-            "emailauth": emailauth,
-            "twofactorcode": authenticator_code,
-            "captchagid": captcha_gid,
-            "captcha_text": captcha_text,
-            "loginfriendlyname": "stlib",
-            "rsatimestamp": steam_key.timestamp,
-            "remember_login": 'true',
-            "donotcache": ''.join([str(int(time.time())), '000']),
+        return {
+            "account_name": self.username,
+            "encrypted_password": encrypted_password.decode(),
+            "encryption_timestamp": steam_key.timestamp,
+            "device_friendly_name": "stlib",
+            "persistence": 1,
+            "platform_type": "3" if mobile_login else "2",
+            "website_id": "Mobile" if mobile_login else "Community",
         }
 
-        if mobile_login:
-            data['oauth_client_id'] = universe.STEAM_UNIVERSE['public']
-
-        return data
-
     async def get_steam_key(self, username: str) -> universe.SteamKey:
         """
         Get `SteamKey`
         :param username: Steam username as string
         :return: `SteamKey`
         """
-        params = {'username': username}
-        json_data = await self.request_json(f'{self.login_url}/getrsakey/', params=params)
+        params = {'account_name': username}
+        json_data = await self.request_json(
+            f'{self.api_url}/IAuthenticationService/GetPasswordRSAPublicKey/v1',
+            params=params,
+        )
 
-        if json_data['success']:
-            public_mod = int(json_data['publickey_mod'], 16)
-            public_exp = int(json_data['publickey_exp'], 16)
-            timestamp = int(json_data['timestamp'])
-        else:
+        if not json_data['response']:
             raise ValueError('Failed to get public key.')
 
+        public_mod = int(json_data['response']['publickey_mod'], 16)
+        public_exp = int(json_data['response']['publickey_exp'], 16)
+        timestamp = int(json_data['response']['timestamp'])
         return universe.SteamKey(rsa.PublicKey(public_mod, public_exp), timestamp)
 
     async def get_captcha(self, gid: int) -> bytes:
         """
         Get captcha image
         :param gid: Captcha GID
         :return: Image
@@ -209,108 +219,129 @@
         log.debug("User has phone? %s", json_data["has_phone"])
 
         return json_data["has_phone"]
 
     async def do_login(
             self,
             shared_secret: str = '',
-            emailauth: str = '',
-            captcha_gid: int = -1,
-            captcha_text: str = '',
+            auth_code: str = '',
+            auth_code_type: AuthCodeType = AuthCodeType.device,
             mobile_login: bool = False,
-            authenticator_code: str = '',
     ) -> LoginData:
         """
-        Login an user on Steam
+        Login a user on Steam
         :param shared_secret: User shared secret
-        :param emailauth: OTP received by email
-        :param captcha_gid: gid of received captcha
-        :param captcha_text: text of received captcha
+        :param auth_code: optional auth code to login
+        :param auth_code_type: auth code type
         :param mobile_login: True to request mobile session instead desktop one
-        :param authenticator_code: OTP from steam authenticator
         :return: Updated `LoginData`
         """
         _original_fargs = locals().copy()
         _original_fargs.pop('self')
 
+        data = await self._new_login_data(mobile_login)
+
+        json_data = await self.request_json(
+            f'{self.api_url}/IAuthenticationService/BeginAuthSessionViaCredentials/v1',
+            data=data,
+        )
+
+        if 'steamid' not in json_data['response']:
+            raise LoginError('Unable to log-in. Check your username and password.')
+
+        client_id = json_data['response']['client_id']
+        request_id = json_data['response']['request_id']
+        steamid = json_data['response']['steamid']
+
         if shared_secret:
-            json_data = await self.request_json(f'{self.api_url}/ISteamWebAPIUtil/GetServerInfo/v1')
-            server_time = json_data['servertime']
-            authenticator_code = universe.generate_steam_code(server_time, shared_secret)
-        else:
-            if authenticator_code:
-                log.warning("Using external authenticator code to log-in")
-            else:
-                log.warning("Logging without two-factor authentication.")
-
-        data = await self._new_login_data(authenticator_code, emailauth, captcha_gid, captcha_text, mobile_login)
-
-        if mobile_login:
-            login_url = self.mobile_login_url
-            cookies: http.cookies.SimpleCookie[str] = http.cookies.SimpleCookie()
-            cookies['mobileClientVersion'] = '0 (2.3.1)'
-            cookies['mobileClient'] = "android"
-            self.update_cookies(cookies)
+            server_data = await self.request_json(f'{self.api_url}/ISteamWebAPIUtil/GetServerInfo/v1')
+            server_time = server_data['servertime']
+            auth_code = universe.generate_steam_code(server_time, shared_secret)
+
+        if auth_code:
+            log.warning("Using external auth code to log-in")
+        elif not shared_secret:
+            log.warning("Logging without two-factor authentication.")
+
+        if auth_code:
+            data = {
+                "client_id": client_id,
+                "steamid": steamid,
+                "code": auth_code,
+                "code_type": auth_code_type.value,
+            }
+
+            auth_data = await self.request_json(
+                f'{self.api_url}/IAuthenticationService/UpdateAuthSessionWithSteamGuardCode/v1',
+                data=data,
+                raise_for_status=False,
+            )
+
+            if not auth_data['response']:
+                raise LoginError('SteamGuard code is wrong')
         else:
-            login_url = self.login_url
+            captcha_requested = len(json_data['response']['allowed_confirmations']) > 1
+            auth_code_type = json_data['response']['allowed_confirmations'][0]['confirmation_type']
 
-        json_data = await self.request_json(f'{login_url}/dologin', data=data)
+            if auth_code_type == 2:
+                raise MailCodeError("Mail code requested", captcha_requested)
 
-        if json_data['success']:
-            oauth_data = {}
+            if auth_code_type == 3:
+                raise TwoFactorCodeError("Authenticator code requested", captcha_requested)
 
-            if mobile_login:
-                oauth_data = json.loads(json_data.pop('oauth'))
+            if auth_code_type == 6:
+                raise CaptchaError("Captcha code requested")
 
-            return LoginData(json_data, oauth_data)
+        data = {
+            "client_id": client_id,
+            "request_id": request_id,
+        }
 
-        if 'message' in json_data and 'too many login failures' in json_data['message']:
-            raise LoginBlockedError("Your network is blocked. Please, try again later")
+        json_data = await self.request_json(
+            f'{self.api_url}/IAuthenticationService/PollAuthSessionStatus/v1',
+            data=data,
+        )
+
+        if 'refresh_token' not in json_data['response']:
+            raise LoginError('Tokens are not received. Try again.')
+
+        refresh_token = json_data['response']['refresh_token']
+        access_token = json_data['response']['access_token']
+        sessionid = ''.join(random.choices('0123456789abcdef', k=24))
 
-        if 'emailauth_needed' in json_data and json_data['emailauth_needed']:
-            raise MailCodeError("Mail code requested")
+        data = {
+            "nonce": refresh_token,
+            "sessionid": sessionid,
+        }
 
-        if 'requires_twofactor' in json_data and json_data['requires_twofactor']:
-            if self.login_trial > 0:
-                self.login_trial -= 1
-                await asyncio.sleep(5)
-                login_data = await self.do_login(**_original_fargs)
-                return login_data
+        json_data = await self.request_json(f'{self.login_url}/jwt/finalizelogin', data=data)
+        transfer_info = []
 
-            raise TwoFactorCodeError("Authenticator code requested")
+        for item in json_data['transfer_info']:
+            data = {
+                'nonce': item['params']['nonce'],
+                'auth': item['params']['auth'],
+                'steamID': steamid,
+            }
 
-        if 'captcha_needed' in json_data and json_data['captcha_needed']:
-            if captcha_text and captcha_gid:
-                if 'message' in json_data and 'verify your humanity' not in json_data['message']:
-                    raise LoginError(json_data['message'])
+            response = await self.request(item['url'], data=data)
 
-            captcha = await self.get_captcha(json_data['captcha_gid'])
-            raise CaptchaError(json_data['captcha_gid'], captcha, "Captcha code requested")
+            if 'steamLoginSecure' not in response.cookies:
+                raise LoginError('Error setting login cookies')
 
-        if mobile_login and 'oauth' not in json_data:
-            raise LoginError(f"Unable to log-in on mobile session: {json_data['message']}")
+            transfer_info.append(TransferInfo(item['url'], data['nonce'], data['auth']))
 
-        raise LoginError(f"Unable to log-in: {json_data['message']}")
+        return LoginData(steamid, client_id, sessionid, refresh_token, access_token, transfer_info)
 
-    async def is_logged_in(self, steamid: universe.SteamId) -> bool:
+    async def is_logged_in(self) -> bool:
+        """
+        Check if user is logged in
+        :return: bool
+        """
         try:
-            response = await self.request(f'{steamid.profile_url}/edit', allow_redirects=False, raise_for_status=False)
+            response = await self.request(
+                'https://store.steampowered.com/account', allow_redirects=False
+            )
         except LoginError:
             return False
 
-        if 'profile could not be found' in response.content:
-            log.error("steamid %s seems invalid", steamid.id64)
-            return False
-
         return response.status == 200
-
-    def restore_login(self, steamid: universe.SteamId, token: str, token_secure: str) -> None:
-        """
-        Restore a previous saved session
-        :param steamid: `SteamId`
-        :param token: Login token code
-        :param token_secure: Login token secure code
-        """
-        cookies: http.cookies.SimpleCookie[str] = http.cookies.SimpleCookie()
-        cookies['steamLogin'] = f'{steamid.id64}%7C%7C{token}'
-        cookies['steamLoginSecure'] = f'{steamid.id64}%7C%7C{token_secure}'
-        self.update_cookies(cookies)
```

### Comparing `stlib-1.3.1/src/stlib/plugins.py` & `stlib-2.0/src/stlib/plugins.py`

 * *Files identical despite different names*

### Comparing `stlib-1.3.1/src/stlib/universe.py` & `stlib-2.0/src/stlib/universe.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 def generate_steam_code(server_time: int, shared_secret: Union[str, bytes]) -> str:
     """
     Generate steam code
     :param server_time: Server Time
     :param shared_secret: User shared secret
     :return: Steam OTP
     """
-    msg = int(server_time / 30).to_bytes(8, 'big')
+    msg = (server_time // 30).to_bytes(8, 'big')
     key = base64.b64decode(shared_secret)
     auth_code_raw = generate_otp_code(msg, key)
 
     auth_code = []
     for _ in range(5):
         auth_code.append(__STEAM_ALPHABET[int(auth_code_raw % len(__STEAM_ALPHABET))])
         auth_code_raw //= len(__STEAM_ALPHABET)
@@ -174,17 +174,15 @@
     :param base: Base string
     :return: Device ID
     """
     digest = hashlib.sha256(base.encode()).hexdigest()
     device_id = ['android:']
 
     for start, end in ([0, 8], [8, 12], [12, 16], [16, 20], [20, 32]):
-        device_id.append(digest[start:end])
-        device_id.append('-')
-
+        device_id.extend((digest[start:end], '-'))
     device_id.pop(-1)
     return ''.join(device_id)
 
 
 def generate_time_hash(server_time: int, tag: str, secret: str) -> str:
     """Generate steam time hash"""
     key = base64.b64decode(secret)
```

### Comparing `stlib-1.3.1/src/stlib/utils.py` & `stlib-2.0/src/stlib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,40 +89,40 @@
             cls,
             session_index: int,
             raise_for_status: bool = True,
             *args: Any, **kwargs: Any,
     ) -> aiohttp.ClientSession:
         """
         Create a http session at given `session_index`.
-        If a previous instance exists in cache at same index, it will returns IndexError.
+        If a previous instance exists in cache at same index, it will raise IndexError.
 
         :param session_index: Session number
         :param raise_for_status: Raise if the response status is 400 or higher.
         :param args: extra args when creating a new http session
-        :param kwargs: extra kargs when creating a new http session
+        :param kwargs: extra kwargs when creating a new http session
         :return: Instance of module
         """
         if session_index in _session_cache['http_session']:
             raise IndexError(f"There's already a http_session session at index {session_index}")
 
-        if 'headers' in kwargs:
+        if 'headers' not in kwargs:
             kwargs['headers'] = {'User-Agent': 'Unknown/0.0.0'}
 
         log.info("Creating a new http session at index %s for custom http session", session_index)
         http_session = aiohttp.ClientSession(*args, raise_for_status=raise_for_status, **kwargs)
         _session_cache['http_session'][session_index] = http_session
 
         assert isinstance(http_session, aiohttp.ClientSession), "Wrong session type"
         return http_session
 
     @classmethod
     async def new_session(cls, session_index: int, *args: Any, **kwargs: Any) -> 'Base':
         """
         Create an instance of module at given `session_index`.
-        If a previous instance exists in cache at same index, it will returns IndexError.
+        If a previous instance exists in cache at same index, it will raise IndexError.
         The instance will be associated with a http session at same index.
         If a http session is not present in cache, it'll create a new one.
         If you need custom params for http session, use `new_http_session` before calling this method.
 
         :param session_index: Session number
         :param args: extra args when creating a new instance
         :param kwargs: extra kwargs when creating a new instance
@@ -164,23 +164,22 @@
 
         if cache_name in _session_cache and session_index in _session_cache[cache_name]:
             del _session_cache[cache_name][session_index]
             http_session = _session_cache['http_session'][session_index]
             assert isinstance(http_session, aiohttp.ClientSession), "Wrong http session type"
             await http_session.close()
             del _session_cache['http_session'][session_index]
-        else:
-            if not no_fail:
-                raise IndexError(f"There's no session at {session_index}")
+        elif not no_fail:
+            raise IndexError(f"There's no session at {session_index}")
 
     @classmethod
     def get_session(cls, session_index: int) -> 'Base':
         """
         Get an instance of module from cache at `session_index`.
-        If session isn't present in cache, it will returns IndexError
+        If session isn't present in cache, it will raise IndexError
         :param session_index: session number
         :return: instance of module
         """
         cache_name = f'{cls.__module__}.{cls.__name__}'
 
         if cache_name not in _session_cache or session_index not in _session_cache[cache_name]:
             raise IndexError(f"There's no session for {cache_name} at {session_index}")
```

### Comparing `stlib-1.3.1/src/stlib/webapi.py` & `stlib-2.0/src/stlib/webapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 #
 
 """
-`webapi` interface is used to interact with the oficial SteamWebAPI.
+`webapi` interface is used to interact with the official SteamWebAPI.
 """
 
 import logging
 import time
 from typing import Any, Dict, List, NamedTuple, Optional
 
 import aiohttp
 
-from . import universe, login, utils
+from . import universe, utils
 
 log = logging.getLogger(__name__)
 
 
 class Game(NamedTuple):
     name: str
     """Name"""
@@ -44,14 +44,35 @@
     """True if game has dlc"""
     has_market: bool
     """True if game has market items"""
     has_workshop: bool
     """True if game has workshop"""
 
 
+class AuthenticatorData(NamedTuple):
+    shared_secret: str
+    """shared secret"""
+    identity_secret: str
+    """identity secret"""
+    serial_number: int
+    """serial number"""
+    revocation_code: str
+    """revocation code"""
+    uri: str
+    """otpauth uri e.g.: otpauth://totp/Steam:<user>?secret=<secret>&issuer=Steam"""
+    token_gid: str
+    """token gid"""
+    account_name: str
+    """account name associated"""
+    server_time: int
+    """server time in unix format"""
+    phone_number_hint: int
+    """last 4 digits of phone number linked"""
+
+
 class PhoneNotRegistered(Exception):
     """Raised when no phone number is registered on account"""
     pass
 
 
 class AuthenticatorExists(Exception):
     """Raised when an authenticator is already active for the account"""
@@ -87,30 +108,26 @@
             ```
         """
         super().__init__(**kwargs)
         self.api_url = api_url
         self.api_key = api_key
 
     @staticmethod
-    async def _new_mobile_query(
+    async def _new_mobile_data(
             steamid: universe.SteamId,
-            oauth_token: str,
             token_type: str = 'mobileapp',
     ) -> Dict[str, Any]:
         current_time = int(time.time())
 
-        params = {
+        return {
             'steamid': steamid.id64,
-            'access_token': oauth_token,
             'authenticator_time': current_time,
             'authenticator_type': universe.TOKEN_TYPE[token_type],
         }
 
-        return params
-
     async def get_server_time(self) -> int:
         """Get server time"""
         json_data = await self.request_json(f'{self.api_url}/ISteamWebAPIUtil/GetServerInfo/v1')
         log.debug("server time found: %s", json_data['servertime'])
         return int(json_data['servertime'])
 
     async def get_custom_profile_url(self, steamid: universe.SteamId) -> str:
@@ -206,103 +223,136 @@
         log.debug("%s owned games found.", json_data['response']['game_count'])
 
         return games
 
     async def new_authenticator(
             self,
             steamid: universe.SteamId,
-            oauth_token: str,
+            access_token: str,
             phone_id: int = 1,
-    ) -> login.LoginData:
+    ) -> AuthenticatorData:
         """
         Initialize process to add a new authenticator to account
         :param steamid: `SteamId`
-        :param oauth_token: user oauth token
+        :param access_token: user access token
         :param phone_id: Index of phone number
         :return: Updated account login data
         """
-        data = await self._new_mobile_query(steamid, oauth_token)
-        data['device_identifier'] = universe.generate_device_id(oauth_token)
+        data = await self._new_mobile_data(steamid)
+        data['device_identifier'] = universe.generate_device_id(access_token)
         data['sms_phone_id'] = phone_id
 
-        json_data = await self.request_json(f'{self.api_url}/ITwoFactorService/AddAuthenticator/v1', data=data)
+        params = {'access_token': access_token}
+
+        json_data = await self.request_json(
+            f'{self.api_url}/ITwoFactorService/AddAuthenticator/v1',
+            data=data,
+            params=params,
+        )
+
         response: Dict[str, Any] = json_data['response']
 
         if response['status'] == 29:
             raise AuthenticatorExists('An Authenticator is already active for that account.')
 
-        if response['status'] == 84 or response['status'] == 2:
+        if response['status'] in [84, 2]:
             raise PhoneNotRegistered('Phone not registered on Steam Account.')
 
         if response['status'] != 1:
             raise NotImplementedError(f"add_authenticator is returning status {response['status']}")
 
-        return login.LoginData(auth=response, oauth={})
+        return AuthenticatorData(
+            response['shared_secret'],
+            response['identity_secret'],
+            int(response['serial_number']),
+            response['revocation_code'],
+            response['uri'],
+            response['token_gid'],
+            response['account_name'],
+            int(response['server_time']),
+            int(response['phone_number_hint']),
+        )
 
     async def add_authenticator(
             self,
             steamid: universe.SteamId,
-            oauth_token: str,
+            access_token: str,
             shared_secret: str,
             sms_code: str,
             email_type: int = 2,
     ) -> bool:
         """
         Finalize process to add a new authenticator to account
         :param steamid: User SteamID
-        :param oauth_token: User oauth token
+        :param access_token: User access token
         :param shared_secret: User shared secret
         :param sms_code: OTP received by SMS
         :param email_type: Email type
         :return: True if success
         """
-        data = await self._new_mobile_query(steamid, oauth_token)
+        data = await self._new_mobile_data(steamid)
         server_time = await self.get_server_time()
         data['authenticator_code'] = universe.generate_steam_code(server_time, shared_secret)
         data['activation_code'] = sms_code
-        json_data = await self.request_json(f'{self.api_url}/ITwoFactorService/FinalizeAddAuthenticator/v1', data=data)
+        data['validate_sms_code'] = 1
+
+        params = {'access_token': access_token}
+
+        json_data = await self.request_json(
+            f'{self.api_url}/ITwoFactorService/FinalizeAddAuthenticator/v1',
+            data=data,
+            params=params,
+        )
 
         if json_data['response']['status'] == 89:
             raise SMSCodeError("Invalid sms code")
 
         if json_data['response']['status'] == 2:
             data.pop('authenticator_code')
             data.pop('activation_code')
             data['email_type'] = email_type
 
             try:
-                await self.request_json(f'{self.api_url}/ITwoFactorService/SendEmail/v1', data=data)
+                await self.request_json(
+                    f'{self.api_url}/ITwoFactorService/SendEmail/v1',
+                    data=data,
+                    params=params,
+                )
             except aiohttp.ContentTypeError:
                 return False
             else:
                 return True
 
         return False
 
     async def remove_authenticator(
             self,
             steamid: universe.SteamId,
-            oauth_token: str,
+            access_token: str,
             revocation_code: str,
             scheme: int = 2,
     ) -> bool:
         """
         Remove authenticator from account
         :param steamid: User SteamID
-        :param oauth_token: User oauth token
+        :param access_token: User access token
         :param revocation_code: Steam auth revocation code
         :param scheme: Steam scheme
         :return: True if success
         """
-        data = await self._new_mobile_query(steamid, oauth_token)
+        data = await self._new_mobile_data(steamid)
         data['revocation_code'] = revocation_code
+        data['revocation_reason'] = 1
         data['steamguard_scheme'] = scheme
 
-        try:
-            json_data = await self.request_json(f'{self.api_url}/ITwoFactorService/RemoveAuthenticator/v1', data=data)
-        except aiohttp.ClientResponseError:
-            return False
+        params = {'access_token': access_token}
+
+        json_data = await self.request_json(
+            f'{self.api_url}/ITwoFactorService/RemoveAuthenticator/v1',
+            data=data,
+            params=params,
+        )
 
         if json_data['response']['revocation_attempts_remaining'] == 0:
             raise RevocationError('No more attempts')
 
         return 'success' in json_data['response'] and json_data['response']['success'] is True
```

### Comparing `stlib-1.3.1/src/stlib.egg-info/PKG-INFO` & `stlib-2.0/src/stlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: stlib
-Version: 1.3.1
+Version: 2.0
 Summary: Async library that provides features related to Steam client and compatible stuffs
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
-Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
+Project-URL: homepage, https://github.com/calendulish/stlib
 Project-URL: documentation, https://lara.monster/stlib
 Project-URL: repository, https://github.com
-Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
+Project-URL: changelog, https://github.com/calendulish/stlib/releases
 Keywords: steam,valve
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 stlib
 -----
@@ -35,15 +34,15 @@
 [![Coverage](https://codecov.io/gh/calendulish/stlib/branch/master/graph/badge.svg?token=DMKFKEUUZP)](https://codecov.io/gh/calendulish/stlib)
 [![Quality](https://api.codiga.io/project/33228/score/svg)](https://app.codiga.io/project/33228/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/stlib.svg?style=flat)](https://github.com/calendulish/stlib/releases)
 
 Async library that provides features related to Steam client and compatible stuff
 
-WARNING: stlib is not intended to be used in game development, there is no support to callbacks and I'll not work on that.
+WARNING: stlib is not intended to be used in game development, there is no support to callbacks, and I'll not work on that.
 stlib is intended to develop console or GUI applications that need interaction with SteamAPI or SteamWebAPI.
 
 stlib now supports plugins!
 ---------------------------
 See more at: [stlib-plugins](https://github.com/calendulish/stlib-plugins)
 
 Dependencies to build SteamWorks Python Extension (Optional)
@@ -79,15 +78,15 @@
 Made with stlib
 ---------------
 
 Steam Tools NG - https://github.com/calendulish/steam-tools-ng
 
 ___________________________________________________________________________________________
 
-This is an work in progress. You can request new features.
+This is a work in progress. You can request new features.
 
 The stlib is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 The stlib is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
```

### Comparing `stlib-1.3.1/src/stlib.egg-info/SOURCES.txt` & `stlib-2.0/src/stlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

