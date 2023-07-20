# Comparing `tmp/python-lemming-0.6.0.tar.gz` & `tmp/python-lemming-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lemming-0.6.0.tar", last modified: Tue Jul 11 13:00:24 2023, max compression
+gzip compressed data, was "python-lemming-0.6.1.tar", last modified: Thu Jul 20 10:39:31 2023, max compression
```

## Comparing `python-lemming-0.6.0.tar` & `python-lemming-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:00:24.747348 python-lemming-0.6.0/
--rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.6.0/LICENSE
--rw-rw-rw-   0        0        0    15930 2023-07-11 13:00:24.747348 python-lemming-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    14865 2023-07-11 12:59:00.000000 python-lemming-0.6.0/README.md
--rw-rw-rw-   0        0        0     1633 2023-07-11 12:59:00.000000 python-lemming-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0     1550 2023-07-11 13:00:24.758347 python-lemming-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:00:24.686347 python-lemming-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 13:00:24.704349 python-lemming-0.6.0/src/lemming/
--rw-rw-rw-   0        0        0      922 2023-07-11 12:59:29.000000 python-lemming-0.6.0/src/lemming/__init__.py
--rw-rw-rw-   0        0        0    17696 2023-07-11 12:59:00.000000 python-lemming-0.6.0/src/lemming/__main__.py
--rw-rw-rw-   0        0        0    13842 2023-07-11 12:59:00.000000 python-lemming-0.6.0/src/lemming/config.py
--rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.6.0/src/lemming/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-11 13:00:24.745348 python-lemming-0.6.0/src/python_lemming.egg-info/
--rw-rw-rw-   0        0        0    15930 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.6.0/src/python_lemming.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      106 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 10:39:31.964977 python-lemming-0.6.1/
+-rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0    15930 2023-07-20 10:39:31.965977 python-lemming-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14865 2023-07-11 12:59:00.000000 python-lemming-0.6.1/README.md
+-rw-rw-rw-   0        0        0     1615 2023-07-20 10:33:18.000000 python-lemming-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1557 2023-07-20 10:39:31.970978 python-lemming-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:39:31.901430 python-lemming-0.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 10:39:31.926978 python-lemming-0.6.1/src/lemming/
+-rw-rw-rw-   0        0        0      922 2023-07-20 10:37:18.000000 python-lemming-0.6.1/src/lemming/__init__.py
+-rw-rw-rw-   0        0        0    17716 2023-07-20 10:31:15.000000 python-lemming-0.6.1/src/lemming/__main__.py
+-rw-rw-rw-   0        0        0    13842 2023-07-11 12:59:00.000000 python-lemming-0.6.1/src/lemming/config.py
+-rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.6.1/src/lemming/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-20 10:39:31.963977 python-lemming-0.6.1/src/python_lemming.egg-info/
+-rw-rw-rw-   0        0        0    15930 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.6.1/src/python_lemming.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      113 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/top_level.txt
```

### Comparing `python-lemming-0.6.0/LICENSE` & `python-lemming-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lemming-0.6.0/PKG-INFO` & `python-lemming-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.6.0
+Version: 0.6.1
 Summary: Lemming is a tool for formatting and linting code.
 Home-page: https://github.com/koviubi56/lemming
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: lemming,format,formatter,lint,linting,linter
 Platform: unix
```

### Comparing `python-lemming-0.6.0/README.md` & `python-lemming-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `python-lemming-0.6.0/pyproject.toml` & `python-lemming-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ignore = [
     "ANN101",
     "ANN102",
     "ANN401",
     "COM",
     "D",
     "EM102",
+    "FA",
     "FBT",
     "T",
     "TRY003",
     "PLR0913",
 ]
 line-length = 79
 target-version = "py38"
@@ -75,8 +76,8 @@
 
 [[tool.lemming.linters]]
 packages = ["pyroma"]
 command = "{pyexe} -m pyroma {path}"
 
 [[tool.lemming.linters]]
 packages = ["vermin"]
-command = "vermin --target=3.7 --eval-annotations --backport typing --backport typing_extensions -vv src"
+command = "vermin --target=3.7 --eval-annotations --backport typing -vv src"
```

### Comparing `python-lemming-0.6.0/setup.cfg` & `python-lemming-0.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -63,35 +63,36 @@
 000003e0: 6e67 0d0a 696e 7374 616c 6c5f 7265 7175  ng..install_requ
 000003f0: 6972 6573 203d 200d 0a09 746f 6d6c 693b  ires = ...tomli;
 00000400: 2070 7974 686f 6e5f 7665 7273 696f 6e3c   python_version<
 00000410: 2733 2e31 3127 0d0a 0970 7974 686f 6e2d  '3.11'...python-
 00000420: 6d79 6c6f 673e 3d30 2e38 2e30 2d62 6574  mylog>=0.8.0-bet
 00000430: 612e 320d 0a09 7479 7069 6e67 2d65 7874  a.2...typing-ext
 00000440: 656e 7369 6f6e 733e 3d34 2e34 2e30 0d0a  ensions>=4.4.0..
-00000450: 0974 7970 6572 0d0a 0970 7964 616e 7469  .typer...pydanti
-00000460: 633e 3d31 2e35 0d0a 7079 7468 6f6e 5f72  c>=1.5..python_r
-00000470: 6571 7569 7265 7320 3d20 3e3d 332e 370d  equires = >=3.7.
-00000480: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000490: 0a09 3d73 7263 0d0a 7a69 705f 7361 6665  ..=src..zip_safe
-000004a0: 203d 206e 6f0d 0a0d 0a5b 6f70 7469 6f6e   = no....[option
-000004b0: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-000004c0: 0a6c 656d 6d69 6e67 203d 2070 792e 7479  .lemming = py.ty
-000004d0: 7065 640d 0a0d 0a5b 6f70 7469 6f6e 732e  ped....[options.
-000004e0: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
-000004f0: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
-00000500: 200d 0a09 6c65 6d6d 696e 6720 3d20 6c65   ...lemming = le
-00000510: 6d6d 696e 672e 5f5f 6d61 696e 5f5f 3a6d  mming.__main__:m
-00000520: 6169 6e0d 0a0d 0a5b 7079 636f 6465 7374  ain....[pycodest
-00000530: 796c 655d 0d0a 6967 6e6f 7265 203d 2045  yle]..ignore = E
-00000540: 3230 330d 0a0d 0a5b 7079 6c61 6d61 5d0d  203....[pylama].
-00000550: 0a69 676e 6f72 6520 3d20 5735 3033 0d0a  .ignore = W503..
-00000560: 0d0a 5b66 6c61 6b65 385d 0d0a 6578 7465  ..[flake8]..exte
-00000570: 6e64 2d69 676e 6f72 6520 3d20 5735 3033  nd-ignore = W503
-00000580: 0d0a 6578 7465 6e64 2d65 7863 6c75 6465  ..extend-exclude
-00000590: 203d 2076 656e 762c 2a63 6163 6865 2a0d   = venv,*cache*.
-000005a0: 0a70 6572 2d66 696c 652d 6967 6e6f 7265  .per-file-ignore
-000005b0: 7320 3d20 0d0a 0974 6573 7473 2f2a 3a20  s = ...tests/*: 
-000005c0: 5331 3031 0d0a 0d0a 5b69 736f 7274 5d0d  S101....[isort].
-000005d0: 0a70 726f 6669 6c65 203d 2062 6c61 636b  .profile = black
-000005e0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000005f0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000600: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000450: 0974 7970 6572 3e3d 302e 392e 300d 0a09  .typer>=0.9.0...
+00000460: 7079 6461 6e74 6963 3e3d 312e 350d 0a70  pydantic>=1.5..p
+00000470: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000480: 203e 3d33 2e37 0d0a 7061 636b 6167 655f   >=3.7..package_
+00000490: 6469 7220 3d20 0d0a 093d 7372 630d 0a7a  dir = ...=src..z
+000004a0: 6970 5f73 6166 6520 3d20 6e6f 0d0a 0d0a  ip_safe = no....
+000004b0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000004c0: 5f64 6174 615d 0d0a 6c65 6d6d 696e 6720  _data]..lemming 
+000004d0: 3d20 7079 2e74 7970 6564 0d0a 0d0a 5b6f  = py.typed....[o
+000004e0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
+000004f0: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
+00000500: 7269 7074 7320 3d20 0d0a 096c 656d 6d69  ripts = ...lemmi
+00000510: 6e67 203d 206c 656d 6d69 6e67 2e5f 5f6d  ng = lemming.__m
+00000520: 6169 6e5f 5f3a 6d61 696e 0d0a 0d0a 5b70  ain__:main....[p
+00000530: 7963 6f64 6573 7479 6c65 5d0d 0a69 676e  ycodestyle]..ign
+00000540: 6f72 6520 3d20 4532 3033 0d0a 0d0a 5b70  ore = E203....[p
+00000550: 796c 616d 615d 0d0a 6967 6e6f 7265 203d  ylama]..ignore =
+00000560: 2057 3530 330d 0a0d 0a5b 666c 616b 6538   W503....[flake8
+00000570: 5d0d 0a65 7874 656e 642d 6967 6e6f 7265  ]..extend-ignore
+00000580: 203d 2057 3530 330d 0a65 7874 656e 642d   = W503..extend-
+00000590: 6578 636c 7564 6520 3d20 7665 6e76 2c2a  exclude = venv,*
+000005a0: 6361 6368 652a 0d0a 7065 722d 6669 6c65  cache*..per-file
+000005b0: 2d69 676e 6f72 6573 203d 200d 0a09 7465  -ignores = ...te
+000005c0: 7374 732f 2a3a 2053 3130 310d 0a0d 0a5b  sts/*: S101....[
+000005d0: 6973 6f72 745d 0d0a 7072 6f66 696c 6520  isort]..profile 
+000005e0: 3d20 626c 6163 6b0d 0a0d 0a5b 6567 675f  = black....[egg_
+000005f0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000600: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000610: 300d 0a0d 0a                             0....
```

### Comparing `python-lemming-0.6.0/src/lemming/__init__.py` & `python-lemming-0.6.1/src/lemming/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # SPDX-License-Identifier: GPL-3.0-or-later
 __all__ = ["__version__", "logger"]
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 import mylog
 
 logger = mylog.root.get_child("lemming")
 logger.threshold = mylog.Level.info
```

### Comparing `python-lemming-0.6.0/src/lemming/__main__.py` & `python-lemming-0.6.1/src/lemming/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,18 +37,18 @@
     get_config_pyproject,
 )
 
 PRE_COMMIT_FILE = """#!/bin/sh
 #!/usr/bin/env bash
 # File generated by Lemming: https://github.com/koviubi56/lemming
 
-set -e
+set -euo pipefail
 PYTHON='{}'
 
-if [[ -n $LEMMING_VERBOSE ]]; then
+if [[ -n "${LEMMING_VERBOSE:-}" ]]; then
     exec $PYTHON -m lemming format --verbose $(pwd)
     ret_code=$?
 else
     exec $PYTHON -m lemming format --quiet-pip "$(pwd)"
     ret_code=$?
 fi
 exit $ret_code
@@ -70,15 +70,15 @@
     """
 
     what_to_quiet: WhatToQuiet
     config: Config
     only: Optional[List[str]]
 
     def should_run(self, name: str) -> bool:
-        if self.only is None:
+        if not self.only:
             return True
         return name in self.only
 
 
 class Timer:
     """A timer."""
 
@@ -532,15 +532,15 @@
     pre_commit = git_directory / "hooks" / "pre-commit"
     if pre_commit.exists():
         logger.warning(
             f"pre-commit file {pre_commit} already exists! Overwriting..."
         )
     logger.info(f"Creating pre-commit git hook (it will use {sys.executable})")
     try:
-        pre_commit.write_text(PRE_COMMIT_FILE.format(sys.executable))
+        pre_commit.write_text(PRE_COMMIT_FILE.replace("{}", sys.executable))
     except OSError as exception:
         logger.critical("Could not write pre-commit file!", True)
         raise typer.Exit(1) from exception
     logger.info("Successfully written pre-commit!")
 
 
 @app.command("pre-commit")
```

### Comparing `python-lemming-0.6.0/src/lemming/config.py` & `python-lemming-0.6.1/src/lemming/config.py`

 * *Files identical despite different names*

### Comparing `python-lemming-0.6.0/src/python_lemming.egg-info/PKG-INFO` & `python-lemming-0.6.1/src/python_lemming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.6.0
+Version: 0.6.1
 Summary: Lemming is a tool for formatting and linting code.
 Home-page: https://github.com/koviubi56/lemming
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: lemming,format,formatter,lint,linting,linter
 Platform: unix
```

