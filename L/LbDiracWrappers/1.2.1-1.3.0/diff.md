# Comparing `tmp/LbDiracWrappers-1.2.1.tar.gz` & `tmp/LbDiracWrappers-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbDiracWrappers-1.2.1.tar", last modified: Tue Mar  1 10:01:48 2022, max compression
+gzip compressed data, was "LbDiracWrappers-1.3.0.tar", last modified: Thu Jul 20 15:29:17 2023, max compression
```

## Comparing `LbDiracWrappers-1.2.1.tar` & `LbDiracWrappers-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:01:48.888000 LbDiracWrappers-1.2.1/
--rw-r--r--   0 root         (0) root         (0)       49 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1790 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1032 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    16282 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)    32472 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      780 2022-03-01 10:01:48.888000 LbDiracWrappers-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       72 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      287 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1302 2022-03-01 10:01:48.888000 LbDiracWrappers-1.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:01:48.884000 LbDiracWrappers-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:01:48.888000 LbDiracWrappers-1.2.1/src/LbDiracWrappers/
--rw-r--r--   0 root         (0) root         (0)     8992 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/src/LbDiracWrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:01:48.888000 LbDiracWrappers-1.2.1/src/LbDiracWrappers.egg-info/
--rw-r--r--   0 root         (0) root         (0)      780 2022-03-01 10:01:48.000000 LbDiracWrappers-1.2.1/src/LbDiracWrappers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2022-03-01 10:01:48.000000 LbDiracWrappers-1.2.1/src/LbDiracWrappers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-01 10:01:48.000000 LbDiracWrappers-1.2.1/src/LbDiracWrappers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2022-03-01 10:01:48.000000 LbDiracWrappers-1.2.1/src/LbDiracWrappers.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2022-03-01 10:01:48.000000 LbDiracWrappers-1.2.1/src/LbDiracWrappers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-03-01 10:01:48.000000 LbDiracWrappers-1.2.1/src/LbDiracWrappers.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 10:01:48.888000 LbDiracWrappers-1.2.1/tests/
--rw-r--r--   0 root         (0) root         (0)     8215 2022-03-01 10:01:27.000000 LbDiracWrappers-1.2.1/tests/test_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:29:17.824000 LbDiracWrappers-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      780 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    16300 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-20 15:29:17.824000 LbDiracWrappers-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 15:29:17.824000 LbDiracWrappers-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:29:17.820000 LbDiracWrappers-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:29:17.824000 LbDiracWrappers-1.3.0/src/LbDiracWrappers/
+-rw-r--r--   0 root         (0) root         (0)     9359 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/src/LbDiracWrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:29:17.824000 LbDiracWrappers-1.3.0/src/LbDiracWrappers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-20 15:29:17.000000 LbDiracWrappers-1.3.0/src/LbDiracWrappers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2023-07-20 15:29:17.000000 LbDiracWrappers-1.3.0/src/LbDiracWrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 15:29:17.000000 LbDiracWrappers-1.3.0/src/LbDiracWrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-20 15:29:17.000000 LbDiracWrappers-1.3.0/src/LbDiracWrappers.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-20 15:29:17.000000 LbDiracWrappers-1.3.0/src/LbDiracWrappers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 15:29:17.000000 LbDiracWrappers-1.3.0/src/LbDiracWrappers.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:29:17.824000 LbDiracWrappers-1.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     8215 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/tests/test_all.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-07-20 15:28:58.000000 LbDiracWrappers-1.3.0/tests/test_path.py
```

### Comparing `LbDiracWrappers-1.2.1/.gitlab-ci.yml` & `LbDiracWrappers-1.3.0/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
       - ${PRE_COMMIT_HOME}
 
 .test-setup:
   image: registry.cern.ch/docker.io/library/python:$PY_VER
   stage: test
   parallel:
     matrix:
-      - PY_VER: ["3.6", "3.7", "3.8", "3.9"]
+      - PY_VER: ["3.9", "3.10", "3.11"]
   before_script:
     - pip install .[testing]
 
 pylint:
   extends: .test-setup
   script:
     - pylint src/LbDiracWrappers
```

### Comparing `LbDiracWrappers-1.2.1/.pre-commit-config.yaml` & `LbDiracWrappers-1.3.0/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,33 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 exclude: ^(tests/data/)
 
 default_language_version:
-  python: python3.9
+  python: python3
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: no-commit-to-branch
         args: [--branch, master]
 
-  - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
-
   - repo: https://github.com/psf/black
-    rev: 22.1.0
+    rev: 23.7.0
     hooks:
       - id: black
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
-    hooks:
-      - id: flake8
-        # additional_dependencies: [flake8-bugbear]
-        files: src/
-
   - repo: "https://gitlab.cern.ch/lhcb-core/LbDevTools.git"
-    rev: 2.0.33
+    rev: 2.0.38
     hooks:
       - id: lb-add-copyright
 
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.278
     hooks:
-      - id: pyupgrade
-        args: ["--py38-plus"]
+      - id: ruff
+        args: ["--fix"]
```

### Comparing `LbDiracWrappers-1.2.1/.pylintrc` & `LbDiracWrappers-1.3.0/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -515,9 +515,9 @@
 min-public-methods=2
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "BaseException, Exception".
-overgeneral-exceptions=BaseException,
-                       Exception
+overgeneral-exceptions=builtins.BaseException,
+                       builtins.Exception
```

### Comparing `LbDiracWrappers-1.2.1/LICENSE` & `LbDiracWrappers-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LbDiracWrappers-1.2.1/src/LbDiracWrappers/__init__.py` & `LbDiracWrappers-1.3.0/src/LbDiracWrappers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 ###############################################################################
-# (c) Copyright 2018-2022 CERN                                                #
+# (c) Copyright 2018-2023 CERN                                                #
 #                                                                             #
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 import argparse
 import os
-import pipes
 import platform
 import re
+import shlex
+import subprocess
 import sys
 from pathlib import Path
 
 import packaging.version
 
 VERISON_PATTERN = re.compile(
     r"(prod(?:.py3)?|v\d+.\d+.\d+(a\d+)?\-x86_64|v\d+.\d+.\d+(a\d+)?)"
@@ -74,14 +75,22 @@
             v.pre[1] if v.is_prerelease else sys.maxsize,
             False,
         )
 
     return sorted(parsedVersions, key=parsedVersions.get, reverse=True)
 
 
+def get_default_path():
+    output = subprocess.check_output("echo PATH=$PATH", env={}, shell=True, text=True)
+    for line in output.split("\n"):
+        if line.startswith("PATH="):
+            return line.split("=", 1)[1]
+    return None
+
+
 class DIRACCVMFSInstall:
     def __init__(self, install_roots=None):
         if install_roots is None:
             try:
                 install_roots = [Path(os.environ["DIRAC_INSTALL_ROOT"])]
             except KeyError:
                 install_roots = [PROD_INSTALL_ROOT, DEV_INSTALL_ROOT]
@@ -133,14 +142,17 @@
 
         if dirac_path.is_file():
             with open(dirac_path, encoding="utf-8") as fp:
                 version = fp.read().strip()
             dirac_path, bashrc = self.versions[version]
 
         env = {k: v for k, v in os.environ.items() if ENV_VAR_WHITELIST.match(k)}
+        default_path = get_default_path()
+        if default_path:
+            env["PATH"] = default_path
         if "." in version or version == "prod":
             new_dirac_path = dirac_path / f"{platform.system()}-{platform.machine()}"
             if new_dirac_path.is_dir():
                 dirac_path = new_dirac_path
             else:
                 # Legacy style versions need the architecture adding
                 dirac_path = (
@@ -154,21 +166,21 @@
             env["X509_CERT_DIR"] = env.get("X509_CERT_DIR", LHCB_ETC / "certificates")
             env["X509_VOMS_DIR"] = env.get("X509_VOMS_DIR", LHCB_ETC / "vomsdir")
             env["X509_VOMSES"] = env.get("X509_VOMSES", LHCB_ETC / "vomses")
 
         if Path(command[0]).name == "bash":
             exec_command = "source $BASH_ENV; exec bash --norc --noprofile"
             for c in command[1:]:
-                exec_command += " " + pipes.quote(c)
+                exec_command += " " + shlex.quote(c)
         elif Path(command[0]).name in ["sh", "ksh", "csh", "tcsh", "zsh", "fish"]:
             raise NotImplementedError(
                 f"Unable to launch {command[0]} as only bash is supported by LHCbDIRAC"
             )
         else:
-            exec_command = " ".join(pipes.quote(x) for x in command)
+            exec_command = " ".join(shlex.quote(x) for x in command)
 
         sys.stdout.flush()
         sys.stderr.flush()
         os.execvpe("bash", ["bash", "--norc", "--noprofile", "-c", exec_command], env)
 
 
 def lb_dirac():
```

### Comparing `LbDiracWrappers-1.2.1/tests/test_all.py` & `LbDiracWrappers-1.3.0/tests/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     [
         ["--list"],
         ["--list", "bash"],
         ["--list", "exit", "100"],
     ],
 )
 def test_lb_dirac_list(cmd, require_cvmfs_lhcb):
-    stdout, stderr = check_output(["lb-dirac"] + cmd)
+    stdout, stderr = check_output(["lb-dirac", *cmd])
     assert "x86_64" not in stdout
     assert "aarch64" not in stdout
     assert "ppc64le" not in stdout
     lhcbdirac_versions = DIRACCVMFSInstall().versions
     for version in lhcbdirac_versions:
         if version.startswith("prod"):
             assert version not in stdout
```

