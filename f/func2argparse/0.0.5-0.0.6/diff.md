# Comparing `tmp/func2argparse-0.0.5.tar.gz` & `tmp/func2argparse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func2argparse-0.0.5.tar", last modified: Mon Jun 26 08:43:47 2023, max compression
+gzip compressed data, was "func2argparse-0.0.6.tar", last modified: Thu Jul 20 10:08:50 2023, max compression
```

## Comparing `func2argparse-0.0.5.tar` & `func2argparse-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:43:47.936403 func2argparse-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 08:43:31.000000 func2argparse-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-26 08:43:47.936403 func2argparse-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-26 08:43:31.000000 func2argparse-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:43:47.936403 func2argparse-0.0.5/func2argparse/
--rw-r--r--   0 runner    (1001) docker     (123)    19534 2023-06-26 08:43:31.000000 func2argparse-0.0.5/func2argparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 08:43:47.936403 func2argparse-0.0.5/func2argparse/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 08:43:31.000000 func2argparse-0.0.5/func2argparse/logging.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:43:47.936403 func2argparse-0.0.5/func2argparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-26 08:43:31.000000 func2argparse-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:43:47.936403 func2argparse-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 08:43:31.000000 func2argparse-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:43:47.936403 func2argparse-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-26 08:43:31.000000 func2argparse-0.0.5/tests/test_func_to_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:50.121959 func2argparse-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 10:08:28.000000 func2argparse-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-20 10:08:50.121959 func2argparse-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-20 10:08:28.000000 func2argparse-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:50.121959 func2argparse-0.0.6/func2argparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    20465 2023-07-20 10:08:28.000000 func2argparse-0.0.6/func2argparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 10:08:50.121959 func2argparse-0.0.6/func2argparse/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 10:08:28.000000 func2argparse-0.0.6/func2argparse/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:50.121959 func2argparse-0.0.6/func2argparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-20 10:08:50.000000 func2argparse-0.0.6/func2argparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 10:08:50.000000 func2argparse-0.0.6/func2argparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:08:50.000000 func2argparse-0.0.6/func2argparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:08:49.000000 func2argparse-0.0.6/func2argparse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 10:08:50.000000 func2argparse-0.0.6/func2argparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-20 10:08:28.000000 func2argparse-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:08:50.121959 func2argparse-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-20 10:08:28.000000 func2argparse-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:50.121959 func2argparse-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-20 10:08:28.000000 func2argparse-0.0.6/tests/test_func_to_argparse.py
```

### Comparing `func2argparse-0.0.5/PKG-INFO` & `func2argparse-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2argparse
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert python functions to argparse objects
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/func2argparse
 Project-URL: Bug Tracker, https://github.com/Acellera/func2argparse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
```

### Comparing `func2argparse-0.0.5/README.md` & `func2argparse-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `func2argparse-0.0.5/func2argparse/__init__.py` & `func2argparse-0.0.6/func2argparse/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+from collections import OrderedDict
 from func2argparse import _version
 
 __version__ = _version.get_versions()["version"]
 
 
 class LoadFromFile(argparse.Action):
     def __init__(self, unmatched_args="error", *args, **kwargs):
@@ -65,15 +66,15 @@
     for line in lines[1:]:
         if line.strip().startswith("Parameters"):
             break
         if len(line.strip()):
             description.append(line.strip())
     description = " ".join(description)
 
-    argdocs = {}
+    argdocs = OrderedDict()
     currvar = None
     paramsection = False
     for i in range(len(lines)):
         line = lines[i].strip()
         if paramsection:
             if reg1.match(line):
                 currvar = reg1.findall(line)[0]
@@ -117,15 +118,14 @@
             if abb not in abbrevs.values():
                 abbrevs[argname] = abb
                 break
     return abbrevs
 
 
 def func_to_manifest(func, file=None, pm_mode=True):
-    from collections import OrderedDict
     import json
     import yaml
     import os
     import inspect
     from typing import get_origin, get_args
 
     # Read existing manifest if it exists
@@ -151,25 +151,42 @@
 
     if "name" not in manifest:
         manifest["name"] = name
     if "version" not in manifest:
         manifest["version"] = "1"
     manifest["description"] = description
 
-    arguments = []
-    for argname in sig.parameters:
-        if argname[0] == "_" or argname in ("args", "kwargs"):
-            continue  # Don't add underscore arguments to argparser or args, kwargs
-        params = sig.parameters[argname]
+    # Don't add underscore arguments to argparser or args, kwargs
+    sigargs = []
+    for argn in sig.parameters:
+        if not (argn.startswith("_") or argn in ("args", "kwargs")):
+            sigargs.append(argn)
 
-        if argname not in argdocs:
+    for argn in sigargs:
+        if argn not in argdocs:
             raise RuntimeError(
-                f"Could not find help for argument {argname} in the docstring of the function. Please document it."
+                f"Could not find help for argument {argn} in the docstring of the function. Please document it."
+            )
+
+    for argn in argdocs:
+        if argn not in sigargs:
+            raise RuntimeError(
+                f"Found docs for argument {argn} in the docstring which is not in the function signature. Please remove it."
             )
 
+    for argn1, argn2 in zip(sigargs, argdocs):
+        if argn1 != argn2:
+            raise RuntimeError(
+                f"Argument order mismatch between function signature and documentation (need to have same order). {argn1} != {argn2}"
+            )
+
+    arguments = []
+    for argname in sigargs:
+        params = sig.parameters[argname]
+
         argtype = params.annotation
         nargs = None
         # This is needed for compound types like: list[str]
         if get_origin(params.annotation) is not None:
             origtype = get_origin(params.annotation)
             argtype = get_args(params.annotation)[0]
             if origtype in (list, tuple):
@@ -259,15 +276,22 @@
             type=open,
             action=lambda *x, **y: LoadFromFile(*x, **y, unmatched_args=unmatched_args),
         )
 
     # Calculate abbreviations
     abbrevs = _get_name_abbreviations([x["name"] for x in manifest["params"]])
 
-    type_map = {"Path": Path, "bool": bool, "int": int, "float": float, "str": str}
+    type_map = {
+        "Path": Path,
+        "bool": bool,
+        "int": int,
+        "float": float,
+        "str": str,
+        "dict": dict,
+    }
 
     for param in manifest["params"]:
         argname = param["name"]
         if param["type"] == "bool":
             if param["nargs"] is None:
                 parser.add_argument(
                     f"--{argname.replace('_', '-')}",
@@ -282,20 +306,28 @@
                     help=param["description"],
                     default=param["value"],
                     type=str_to_bool,
                     required=param["mandatory"],
                     nargs=param["nargs"],
                 )
         else:
+            if param["type"] in type_map:
+                param_type = type_map[param["type"]]
+            else:
+                print(
+                    f"Warning: Argument {argname} of type {param['type']} could not be mapped to a Python base type and thus will not be type-checked."
+                )
+                param_type = None
+
             parser.add_argument(
                 f"--{argname.replace('_', '-')}",
                 f"-{abbrevs[argname]}",
                 help=param["description"],
                 default=param["value"],
-                type=type_map[param["type"]],
+                type=param_type,
                 choices=param["choices"],
                 required=param["mandatory"],
                 nargs=param["nargs"],
             )
 
     return parser
 
@@ -417,15 +449,14 @@
         return False
     if value.lower() == "true":
         return True
     raise RuntimeError(f"Invalid boolean value {value}")
 
 
 def get_manifest(file, parser, pm_mode=True, cwl=False):
-    from collections import OrderedDict
     import json
     import os
 
     if cwl:
         return get_manifest_cwl(file, parser)
 
     manifest = OrderedDict()
```

### Comparing `func2argparse-0.0.5/func2argparse.egg-info/PKG-INFO` & `func2argparse-0.0.6/func2argparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2argparse
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert python functions to argparse objects
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/func2argparse
 Project-URL: Bug Tracker, https://github.com/Acellera/func2argparse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
```

### Comparing `func2argparse-0.0.5/pyproject.toml` & `func2argparse-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `func2argparse-0.0.5/tests/test_func_to_argparse.py` & `func2argparse-0.0.6/tests/test_func_to_argparse.py`

 * *Files identical despite different names*

