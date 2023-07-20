# Comparing `tmp/hserv-0.0.4.tar.gz` & `tmp/hserv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hserv-0.0.4.tar", last modified: Thu Jul 20 06:59:32 2023, max compression
+gzip compressed data, was "hserv-0.0.5.tar", last modified: Thu Jul 20 15:12:23 2023, max compression
```

## Comparing `hserv-0.0.4.tar` & `hserv-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:59:32.550007 hserv-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-20 06:59:19.000000 hserv-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-20 06:59:19.000000 hserv-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 06:59:32.550007 hserv-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-20 06:59:19.000000 hserv-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:59:32.550007 hserv-0.0.4/hserv/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-20 06:59:19.000000 hserv-0.0.4/hserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-20 06:59:19.000000 hserv-0.0.4/hserv/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-07-20 06:59:19.000000 hserv-0.0.4/hserv/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    12193 2023-07-20 06:59:19.000000 hserv-0.0.4/hserv/supabase.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:59:32.550007 hserv-0.0.4/hserv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 06:59:32.000000 hserv-0.0.4/hserv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-20 06:59:32.000000 hserv-0.0.4/hserv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 06:59:32.000000 hserv-0.0.4/hserv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-20 06:59:32.000000 hserv-0.0.4/hserv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 06:59:32.000000 hserv-0.0.4/hserv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 06:59:19.000000 hserv-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 06:59:32.550007 hserv-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-20 06:59:19.000000 hserv-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:23.576403 hserv-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-20 15:12:12.000000 hserv-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-20 15:12:12.000000 hserv-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 15:12:23.576403 hserv-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-20 15:12:12.000000 hserv-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:23.572403 hserv-0.0.5/hserv/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4117 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:23.576403 hserv-0.0.5/hserv/supabase/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/supabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/supabase/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/supabase/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:23.576403 hserv-0.0.5/hserv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 15:12:12.000000 hserv-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 15:12:23.576403 hserv-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-20 15:12:12.000000 hserv-0.0.5/setup.py
```

### Comparing `hserv-0.0.4/LICENSE` & `hserv-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hserv-0.0.4/hserv/supabase.py` & `hserv-0.0.5/hserv/supabase/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import os
 import shutil
 import json
 from string import ascii_letters, digits
 from random import choice
 import re
 import yaml
-import socket
 
 import jwt
 
-from .server import HydrocodeServer
+from hserv.server import HydrocodeServer
 
 @dataclass
 class SupabaseController(object):
     project: str
     path: str = field(default=os.path.expanduser('~'))
     docker_path: str = field(init=False, repr=False)
     server: HydrocodeServer = field(default_factory=HydrocodeServer, repr=False)
```

### Comparing `hserv-0.0.4/setup.py` & `hserv-0.0.5/setup.py`

 * *Files identical despite different names*

