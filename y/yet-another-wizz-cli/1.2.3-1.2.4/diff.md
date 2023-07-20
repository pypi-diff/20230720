# Comparing `tmp/yet_another_wizz_cli-1.2.3.tar.gz` & `tmp/yet_another_wizz_cli-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz_cli-1.2.3.tar", last modified: Sat Jul 15 11:38:03 2023, max compression
+gzip compressed data, was "yet_another_wizz_cli-1.2.4.tar", last modified: Thu Jul 20 13:12:10 2023, max compression
```

## Comparing `yet_another_wizz_cli-1.2.3.tar` & `yet_another_wizz_cli-1.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.368470 yet_another_wizz_cli-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.368470 yet_another_wizz_cli-1.2.3/src/yaw_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.368470 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/default_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.764617 yet_another_wizz_cli-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.764617 yet_another_wizz_cli-1.2.4/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.764617 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17491 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/top_level.txt
```

### Comparing `yet_another_wizz_cli-1.2.3/LICENSE` & `yet_another_wizz_cli-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.3/PKG-INFO` & `yet_another_wizz_cli-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet_another_wizz_cli
-Version: 1.2.3
+Version: 1.2.4
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
-.. image:: https://github.com/jlvdb/yet_another_wizz/blob/main/docs/source/_static/logo-dark.png?raw=true
+.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz/main/docs/source/_static/logo-dark.png
     :width: 1000
     :alt: yet_another_wizz
 
 |
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
```

### Comparing `yet_another_wizz_cli-1.2.3/README.rst` & `yet_another_wizz_cli-1.2.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. image:: https://github.com/jlvdb/yet_another_wizz/blob/main/docs/source/_static/logo-dark.png?raw=true
+.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz/main/docs/source/_static/logo-dark.png
     :width: 1000
     :alt: yet_another_wizz
 
 |
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
```

### Comparing `yet_another_wizz_cli-1.2.3/pyproject.toml` & `yet_another_wizz_cli-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/main.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         )
         if binned:
             group.add_argument(
                 f"--{prefix}-idx",
                 type=int,
                 metavar="<int>",
                 nargs="+",
-                help=f"integer index to identify the input files (or bins) provided with [--{prefix}-path] (default: 0, 1, ...)",
+                help=f"integer index to identify the input files (or bins) provided with [--{prefix}-path] (default: 1, 2, ...)",
             )
         group.add_argument(
             f"--{prefix}-cache",
             action="store_true",
             help="cache the data in the project's cache directory",
         )
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/subcommands.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/subcommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import argparse
 import logging
 import sys
-from abc import ABC, abstractclassmethod
+from abc import ABC, abstractmethod
 
 from yaw import config as yaw_config
 from yaw.config import DEFAULT, OPTIONS, Configuration
 from yaw.core.docs import populate_parser
 
 from yaw_cli.commandline import utils
 from yaw_cli.commandline.main import Commandline
@@ -23,23 +23,26 @@
 
 
 class SubCommand(ABC):
     def __init_subclass__(cls, **kwargs) -> None:
         super().__init_subclass__(**kwargs)
         Commandline.register_subcommand(cls)
 
-    @abstractclassmethod
+    @classmethod
+    @abstractmethod
     def get_name(cls) -> str:
         return "command"
 
-    @abstractclassmethod
+    @classmethod
+    @abstractmethod
     def add_parser(cls) -> None:
         Commandline.register_subcommand(cls)
 
-    @abstractclassmethod
+    @classmethod
+    @abstractmethod
     def run(cls, args: argparse.Namespace) -> None:
         pass
 
 
 class CommandInit(SubCommand):
     @classmethod
     def get_name(cls) -> str:
@@ -474,10 +477,10 @@
             config = load_config_from_setup(args.config_from)
             setup["configuration"] = config.to_dict()  # replace original config
         if args.cache_path is not None:
             setup["data"]["cachepath"] = str(args.cache_path)
 
         # run the tasks in the job list
         with ProjectDirectory.from_dict(setup, path=args.wdir) as project:
-            logger.info(f"scheduling tasks: {project.tasks.view_history()}")
+            logger.info("scheduling tasks: %s", project.tasks.view_history())
             project.tasks.reschedule_history()
             project.tasks.process(progress=args.progress, threads=args.threads)
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/utils.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,17 @@
             nargs=0,
             const=const,
             required=required,
             help=help,
         )
 
     def __call__(self, parser, namespace, values, option_string):
-        from yaw_cli.pipeline.default_setup import setup_default
+        from yaw_cli.pipeline.default_setup import gen_default
 
-        print(setup_default)
+        print(gen_default())
         parser.exit()
 
 
 def Path_absolute(path: str) -> Path:
     return Path(path).expanduser().absolute()
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/__init__.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/data.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,24 +365,24 @@
             )
         elif catalog.patches is not None and not self.external_patches:
             raise InputConfigError(
                 "'n_patches' and catalog 'patches' are mutually exclusive"
             )
 
     def set_reference(self, data: Input, rand: Input | None = None) -> None:
-        logger.debug(f"registering reference data catalog '{data.filepath}'")
+        logger.debug("registering reference data catalog '%s'", data.filepath)
         self._check_patch_definition(data)
         self._reference["data"] = data
         if rand is not None:
             self._check_patch_definition(rand)
             self._reference["rand"] = rand
 
     def add_unknown(self, bin_idx: int, data: Input, rand: Input | None = None) -> None:
         logger.debug(
-            f"registering unknown bin {bin_idx} data catalog '{data.filepath}'"
+            "registering unknown bin %i data catalog '%s'", bin_idx, data.filepath
         )
         # make sure the bin indices will remain aligned
         if self._unknown["rand"] is not None and rand is None:
             raise ValueError(
                 "unknown randoms exist but no randoms for current bin provided"
             )
         elif (
@@ -484,18 +484,21 @@
             # store patch centers for consecutive loads
             if self._centers is None:
                 self._centers = catalog.centers
 
         return catalog
 
     def load_reference(self, kind: str, progress: bool = False) -> BaseCatalog:
-        logger.info(f"loading reference {'random' if kind == 'rand' else kind} catalog")
+        logger.info(
+            "loading reference %s catalog", "random" if kind == "rand" else kind
+        )
         return self._load_catalog("reference", kind, progress=progress)
 
     def load_unknown(
         self, kind: str, bin_idx: int, progress: bool = False
     ) -> BaseCatalog:
         logger.info(
-            f"loading unknown bin {bin_idx} "
-            f"{'random' if kind == 'rand' else kind} catalog"
+            "loading unknown bin %i %s catalog",
+            bin_idx,
+            "random" if kind == "rand" else kind,
         )
         return self._load_catalog("unknown", kind, bin_idx, progress=progress)
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/directories.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/directories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 import os
 import shutil
 import textwrap
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from pathlib import Path, _posix_flavour, _windows_flavour
 from typing import Any
 
 from yaw.core.utils import bytes_format
 
 logger = logging.getLogger(__name__)
@@ -65,37 +65,40 @@
         return set(
             _get_numeric_suffix(path)
             for path in self.iterdir()
             if path.name.startswith("unknown")
         )
 
     def drop(self, name: str) -> None:
-        logger.debug(f"dropping cache '{name}'")
+        logger.debug("dropping cache '%s'", name)
         path = self.joinpath(name)
         if path.is_dir():
             shutil.rmtree(str(path))
         else:
             path.unlink()
 
     def drop_all(self) -> None:
         logger.info("dropping cached data")
         for path in self.iterdir():
             self.drop(path.name)
 
 
 class DataDirectory(Directory, ABC):
-    @abstractproperty
+    @property
+    @abstractmethod
     def _auto_reference_prefix(self) -> str:
         pass
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def _cross_prefix(self) -> str:
         pass
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def _auto_prefix(self) -> str:
         pass
 
     @abstractmethod
     def get_auto_reference(self) -> Path:
         pass
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/logger.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/logger.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/merge.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     # merge and check scales
     common = set.intersection(*scale_sets)
     if len(common) == 0:
         MergeError("found no common scales")
     extra = set.union(*scale_sets) - common
     if len(extra) > 0:
-        logger.warning(f"ignoring unmatched scales: {', '.join(extra)}")
+        logger.warning("ignoring unmatched scales: %s", ", ".join(extra))
 
     # merge binning
     if merge_binning:
         bins = np.unique(np.concatenate(bins))
         bin_config = ManualBinningConfig(bins)
         if bin_config.zbin_num != n_bins:
             raise MergeError("cannot concatenate bins contiguously")
@@ -103,15 +103,15 @@
     for project in projects:
         bin_sets.append(project.get_bin_indices())
     common = set.intersection(*bin_sets)
     if len(common) == 0:
         MergeError("found no common bins")
     extra = set.union(*bin_sets) - common
     if len(extra) > 0:
-        logger.warning(f"ignoring uncommon bins: {', '.join(str(b) for b in extra)}")
+        logger.warning("ignoring uncommon bins: %s", ", ".join(str(b) for b in extra))
     return common
 
 
 def merge_state_attr(
     states: Iterable[ProjectState], attr: str, require: bool = False
 ) -> bool:
     attr_states = [getattr(state, attr) for state in states]
@@ -220,15 +220,15 @@
 
 
 class MergedDirectory(YawDirectory):
     @classmethod
     def from_projects(
         cls, path: TypePathStr, inputs: Sequence[TypePathStr], mode: str
     ) -> MergedDirectory:
-        logger.info(f"merging {len(inputs)} project directories")
+        logger.info("merging %i project directories", len(inputs))
         projects: list[YawDirectory] = []
         for project in inputs:
             projects.append(open_yaw_directory(project))
 
         # check and merge configurations
         if mode not in OPTIONS.merge:
             raise ValueError(f"invalid merge mode '{mode}'")
@@ -245,39 +245,48 @@
             sources=[str(path) for path in inputs],
             tasks=[],
         )
         merged = cls.from_dict(setup, path)
 
         # merge and write the pair counts files
         for scale, counts_dir in merged.iter_counts(create=True):
-            logmsg = f"merging {{:}} for scale '{scale}'"
             project_counts_dir = [project.get_counts_dir(scale) for project in projects]
             if merged_state.has_w_ss:
-                logger.info(logmsg.format("reference autocorrelation function"))
+                logger.info(
+                    "merging %s for scale '%s'",
+                    "reference autocorrelation function",
+                    scale,
+                )
                 cf = merge_cfs(
                     mode,
                     [
                         CorrFunc.from_file(cdir.get_auto_reference())
                         for cdir in project_counts_dir
                     ],
                 )
                 cf.to_file(counts_dir.get_auto_reference())
             if merged_state.has_w_sp:
-                logger.info(logmsg.format("unknown autocorrelation functions"))
+                logger.info(
+                    "merging %s for scale '%s'",
+                    "unknown autocorrelation functions",
+                    scale,
+                )
                 for bin_idx in bins:
                     cf = merge_cfs(
                         mode,
                         [
                             CorrFunc.from_file(cdir.get_cross(bin_idx))
                             for cdir in project_counts_dir
                         ],
                     )
                     cf.to_file(counts_dir.get_cross(bin_idx))
             if merged_state.has_w_pp:
-                logger.info(logmsg.format("crosscorrelation functions"))
+                logger.info(
+                    "merging %s for scale '%s'", "crosscorrelation functions", scale
+                )
                 for bin_idx in bins:
                     cf = merge_cfs(
                         mode,
                         [
                             CorrFunc.from_file(cdir.get_auto(bin_idx))
                             for cdir in project_counts_dir
                         ],
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/plot.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/plot.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/processing.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,18 +67,19 @@
 
     @property
     def state(self) -> ProjectState:
         return self.project.get_state()
 
     def _warn_patches(self):
         LIM = 512
-        msg = f"a large number of patches (>{LIM}) may degrade the performance"
         if not self._warned_patches:
             if self.project.inputs.get_n_patches() > LIM:
-                logger.warning(msg)
+                logger.warning(
+                    "a large number of patches (>%i) may degrade the performance", LIM
+                )
                 self._warned_patches = True
 
     def set_bin_idx(self, idx: int) -> None:
         if idx not in self.project.get_bin_indices():
             raise IndexError(f"bin with index {idx} not configured in setup")
         self._bin_idx = idx
         # reset internally referenced correlation functions
@@ -132,15 +133,15 @@
         estimator: str | None = None,
     ) -> _Tcd:
         cfs: _Tcf = getattr(self, f"_{cfs_kind}")
         data = getattr(self, f"_{cfs_kind}_data")
         if data is None:
             data = {}
         for scale, cf in cfs.items():
-            logger.debug(f"processing pair counts for {tag=} / {scale=}")
+            logger.debug("processing pair counts for tag=%s / scale=%s", tag, scale)
             data[(scale, tag)] = cf.sample(config, estimator=estimator, info=cfs_kind)
         setattr(self, f"_{cfs_kind}_data", data)
         return data
 
     def sample_auto_ref(
         self, *, tag: str, config: ResamplingConfig, estimator: str | None = None
     ) -> _Tcd:
@@ -207,24 +208,24 @@
     def plot(self):
         plot_dir = self.project.estimate_path
         try:
             import matplotlib.pyplot as plt
 
             from yaw_cli.pipeline.plot import Plotter
 
-            logger.info(f"creating check-plots in '{plot_dir}'")
+            logger.info("creating check-plots in '%s'", plot_dir)
         except ImportError:
             logger.error("could not import matplotlib, plotting disabled")
             return
 
         def plot_wrapper(method, title, name):
             fig = method(title)
             if fig is not None:
                 fig.tight_layout()
-                logger.info(f"plotting to '{name}'")
+                logger.info("plotting to '%s'", name)
                 fig.savefig(plot_dir.joinpath(name))
                 plt.close(fig)
                 return True
             return False
 
         plotter = Plotter(self.project)
         plotted = False
@@ -312,16 +313,15 @@
                 if cat is not None:
                     break
             else:
                 raise MissingCatalogError("no catalogs loaded")
             self._linkage = PatchLinkage.from_setup(self.config, cat)
             if self._linkage.density > 0.3 and not self._warned_linkage:
                 logger.warning(
-                    "linkage density > 0.3, either patches overlap "
-                    "significantly or are small compared to scales"
+                    "linkage density > 0.3, either patches overlap significantly or are small compared to scales"
                 )
                 self._warned_linkage = True
 
     def run_auto_ref(self, *, compute_rr: bool) -> _Tcf:
         if self._ref_rand is None:
             raise MissingCatalogError(
                 "reference autocorrelation requires reference randoms"
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/project.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 import os
 import shutil
-from abc import abstractmethod, abstractproperty
+from abc import abstractmethod
 from collections.abc import Iterator
 from dataclasses import dataclass
 from itertools import zip_longest
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import yaml
@@ -106,15 +106,15 @@
         try:
             return yaml.safe_load(f.read())
         except Exception as e:
             raise SetupError(f"parsing the setup file '{setup_file}' failed") from e
 
 
 def load_config_from_setup(setup_file: TypePathStr) -> Configuration:
-    logger.info(f"importing configuration from '{setup_file}'")
+    logger.info("importing configuration from '%s'", setup_file)
     setup_dict = load_setup_as_dict(setup_file)
     return parse_config_from_setup(setup_dict)
 
 
 def parse_config_from_setup(setup_dict: dict[str, Any]) -> Configuration:
     try:
         return Configuration.from_dict(setup_dict["configuration"])
@@ -145,17 +145,17 @@
             raise FileNotFoundError(f"project directory '{self.path}' does not exist")
         if not self.setup_file.exists():
             raise FileNotFoundError(
                 f"not a {self.__class__.__name__}, setup file "
                 f"'{self.setup_file}' does not exist"
             )
         if not self.log_file.exists():
-            logger.info(f"setting up log file '{self.log_file}'")
+            logger.info("setting up log file '%s'", self.log_file)
         else:
-            logger.info(f"resuming project at '{self._path}'")
+            logger.info("resuming project at '%s'", self._path)
         self._add_log_file_handle()
         with open(self.setup_file) as f:
             setup = yaml.safe_load(f.read())
         setup = substitute_env_var(setup)
         self.setup_reload(setup)
         # create any missing directories
         self.counts_path.mkdir(exist_ok=True)
@@ -177,15 +177,16 @@
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         # TODO: this is sometimes executed even if an exception was raised
         if exc_type is None:
             self.setup_write()
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def setup_file(self) -> Path:
         pass
 
     def setup_write(self) -> None:
         write_setup_file(self.setup_file, self.to_dict())
 
     @abstractmethod
@@ -339,30 +340,31 @@
     def tasks(self) -> TaskManager:
         return self._tasks
 
     @abstractmethod
     def get_bin_indices(self) -> set[int]:
         pass
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def n_bins(self) -> int:
         pass
 
 
 class ProjectDirectory(YawDirectory):
     @classmethod
     def create(
         cls,
         path: TypePathStr,
         config: Configuration,
         n_patches: int | None = None,
         cachepath: TypePathStr | None = None,
         backend: str = DEFAULT.backend,
     ) -> ProjectDirectory:
-        logger.info(f"creating new project at '{path}'")
+        logger.info("creating new project at '%s'", path)
         data = dict()
         if n_patches is not None:
             data["n_patches"] = n_patches
         if cachepath is not None:
             data["cachepath"] = cachepath
         if backend != DEFAULT.backend:
             data["backend"] = backend
@@ -392,15 +394,15 @@
             data = setup["data"]
         except KeyError as e:
             parse_section_error(e, "data", SetupError)
         # cache needs extra care: if None, set to default location
         if "cachepath" not in data or data["cachepath"] is None:
             data["cachepath"] = str(self.default_cache_path)
         else:
-            logger.info(f"using cache location '{data['cachepath']}'")
+            logger.info("using cache location '%s'", data["cachepath"])
         self._inputs = InputManager.from_dict(data)
         # try loading existsing patch centers
         if self.patch_file.exists():
             self._inputs.centers_from_file(self.patch_file)
 
     def to_dict(self) -> dict[str, Any]:
         # strip default values from config
@@ -431,22 +433,21 @@
         return self._path.joinpath("cache")
 
     def get_cache_dir(self) -> CacheDirectory:
         return self.inputs.get_cache()
 
     def set_reference(self, data: Input, rand: Input | None = None) -> None:
         if rand is not None:
-            logger.debug(f"registering reference random catalog '{rand.filepath}'")
+            logger.debug("registering reference random catalog '%s'", rand.filepath)
         self._inputs.set_reference(data, rand)
 
     def add_unknown(self, bin_idx: int, data: Input, rand: Input | None = None) -> None:
         if rand is not None:
             logger.debug(
-                f"registering unknown bin {bin_idx} random catalog "
-                f"'{rand.filepath}'"
+                "registering unknown bin %i random catalog '%s'", bin_idx, rand.filepath
             )
         self._inputs.add_unknown(bin_idx, data, rand)
 
     def get_bin_indices(self) -> set[int]:
         return self._inputs.get_bin_indices()
 
     @property
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/tasks.py` & `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import bisect
 import functools
 import logging
-from abc import abstractclassmethod, abstractmethod
+from abc import abstractmethod
 from collections import deque
 from collections.abc import Iterator, Sequence
 from dataclasses import MISSING, asdict, dataclass, field, fields
 from typing import TYPE_CHECKING, Any
 
 from yaw.config import OPTIONS, ResamplingConfig
 from yaw.config import default as DEFAULT
@@ -73,19 +73,23 @@
 
     def __post_init__(self) -> None:
         for par in fields(self):
             if par.default is MISSING:
                 name = f"{self.__class__.__name__}.{par.name}"
                 raise TaskError(f"no default value for '{name}' provided")
 
-    def __eq__(self, other: Task) -> bool:
-        return Task._order[self.get_name()] == Task._order[other.get_name()]
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, Task):
+            return Task._order[self.get_name()] == Task._order[other.get_name()]
+        return NotImplemented
 
     def __le__(self, other: Task) -> bool:
-        return Task._order[self.get_name()] < Task._order[other.get_name()]
+        if isinstance(other, Task):
+            return Task._order[self.get_name()] < Task._order[other.get_name()]
+        return NotImplemented
 
     @classmethod
     def from_argparse(cls, args: Namespace) -> Task:
         kwargs = {}
         for name in cls.get_parnames():
             kwargs[name] = getattr(args, name)
         return cls.from_dict(kwargs)
@@ -111,37 +115,43 @@
     def get_parnames(cls) -> list[str]:
         return [par.name for par in fields(cls)]
 
     @classmethod
     def get_defaults(cls) -> dict[str, Any]:
         return {par.name: par.default for par in fields(cls)}
 
-    @abstractclassmethod
+    @classmethod
+    @abstractmethod
     def get_name(cls) -> str:
         return "task"
 
-    @abstractclassmethod
+    @classmethod
+    @abstractmethod
     def get_help(cls) -> str:
         return "task"
 
 
 class MergedTask(Task):
     pass
 
 
 class RepeatableTask(Task):
     @abstractmethod
     def get_identifier(self) -> Any:
         pass
 
-    def __eq__(self, other: Task) -> bool:
-        if super().__eq__(other) and hasattr(other, "get_identifier"):
-            # additionally compare on the argument level
-            return self.get_identifier() == other.get_identifier()
-        return False
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, self.__class__):
+            return (
+                Task._order[self.get_name()] == Task._order[other.get_name()]
+                and self.get_identifier() == other.get_identifier()
+            )
+        elif isinstance(other, Task):
+            return False
+        return NotImplemented
 
 
 def get_task(name: str) -> Task:
     try:
         return Task._tasks[name]
     except KeyError as e:
         raise UndefinedTaskError(name) from e
@@ -149,15 +159,15 @@
 
 @dataclass(frozen=True)
 class TaskCrosscorr(Task):
     rr: bool = field(
         default=False,
         metadata=Parameter(
             type=bool,
-            help="compute random-random pair counts, even if both randoms are available",
+            help="compute random-random pair counts if both randoms are available",
         ),
     )
 
     @classmethod
     def get_name(cls) -> str:
         return "cross"
 
@@ -434,15 +444,15 @@
             pass
         bisect.insort(task_list, task)
 
     def schedule(self, task: Task) -> None:
         t_args = ", ".join(f"{k}={repr(v)}" for k, v in asdict(task).items())
         if len(t_args) == 0:
             t_args = "---"
-        logger.debug(f"'{task.get_name()}' arguments: {t_args}")
+        logger.debug("'%s' arguments: %s", task.get_name(), t_args)
         self._insert_task(task, self._queue)
 
     def reschedule_history(self) -> None:
         for task in self.get_history():
             self.schedule(task)
 
     def drop(self, task: Task) -> Task:
@@ -464,19 +474,19 @@
             task = self._queue.pop()
             self._insert_task(task, self._history)
 
     def run(
         self, task: Task, progress: bool = False, threads: int | None = None
     ) -> None:
         # log task
-        logger.info(f"running task '{task.get_name()}'")
+        logger.info("running task '%s'", task.get_name())
         args = ", ".join(f"{k}={repr(v)}" for k, v in asdict(task).items())
         if len(args) == 0:
             args = "---"
-        logger.debug(f"arguments: {args}")
+        logger.debug("arguments: %s", args)
         # use a temporary single item queue
         queue = self._queue
         try:
             self._queue = deque([])
             self._insert_task(task, self._queue)
             self.process(progress=progress, threads=threads)
         finally:
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/PKG-INFO` & `yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet-another-wizz-cli
-Version: 1.2.3
+Version: 1.2.4
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
-.. image:: https://github.com/jlvdb/yet_another_wizz/blob/main/docs/source/_static/logo-dark.png?raw=true
+.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz/main/docs/source/_static/logo-dark.png
     :width: 1000
     :alt: yet_another_wizz
 
 |
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
```

### Comparing `yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/SOURCES.txt` & `yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

