# Comparing `tmp/gscp-1.0.8.tar.gz` & `tmp/gscp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscp-1.0.8.tar", max compression
+gzip compressed data, was "gscp-1.0.9.tar", max compression
```

## Comparing `gscp-1.0.8.tar` & `gscp-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/__init__.py
--rw-r--r--   0        0        0     2145 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/__main__.py
--rw-r--r--   0        0        0     1369 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/commit.py
--rw-r--r--   0        0        0       66 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/entry.py
--rw-r--r--   0        0        0      510 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/git.py
--rw-r--r--   0        0        0     2500 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/push_pull.py
--rw-r--r--   0        0        0      200 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/stage.py
--rw-r--r--   0        0        0     1363 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/version.py
--rw-r--r--   0        0        0     2929 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/wrappers.py
--rw-r--r--   0        0        0     1089 2023-06-16 17:59:37.508886 gscp-1.0.8/LICENSE
--rw-r--r--   0        0        0     1022 2023-06-16 17:59:37.508886 gscp-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1691 2023-06-16 17:59:37.508886 gscp-1.0.8/README.md
--rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 gscp-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/__init__.py
+-rw-r--r--   0        0        0     2690 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/__main__.py
+-rw-r--r--   0        0        0     2445 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/commit.py
+-rw-r--r--   0        0        0       66 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/entry.py
+-rw-r--r--   0        0        0      510 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/git.py
+-rw-r--r--   0        0        0     2500 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/push_pull.py
+-rw-r--r--   0        0        0      200 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/stage.py
+-rw-r--r--   0        0        0     1363 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/version.py
+-rw-r--r--   0        0        0     2929 2023-07-20 16:37:22.428593 gscp-1.0.9/gscp/wrappers.py
+-rw-r--r--   0        0        0     1089 2023-07-20 16:37:22.428593 gscp-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1022 2023-07-20 16:37:22.428593 gscp-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1691 2023-07-20 16:37:22.428593 gscp-1.0.9/README.md
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 gscp-1.0.9/PKG-INFO
```

### Comparing `gscp-1.0.8/gscp/__main__.py` & `gscp-1.0.9/gscp/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import argparse
 from typing import cast
 
 from rich.console import Console
 
-from gscp.commit import commit
+from gscp.commit import commit, pre_commit
 from gscp.git import git_is_in_repo
 from gscp.push_pull import push
 from gscp.stage import stage
 from gscp.version import ApplicationVersion
 
 
 def _create_argparser() -> argparse.ArgumentParser:
@@ -35,14 +35,21 @@
         default="",
         nargs="?",
         help="Commit message to use. If no message specified, "
         "it falls back to git's default behaviour with verbose mode",
     )
 
     parser.add_argument(
+        "-pre",
+        action="store_true",
+        help="Performs a pre-commit check before making the actual commit."
+        " Uses the git pre-commit hook.",
+    )
+
+    parser.add_argument(
         "-a",
         "--amend",
         action="store_true",
         help="If we using git amend mode (warning, this triggers a force push)",
     )
 
     parser.add_argument(
@@ -61,24 +68,35 @@
 
 def main() -> None:
     console = Console()
 
     parser = _create_argparser()
     args = parser.parse_args()
 
+    pre = cast(bool, args.pre)
     commit_push_only = cast(bool, args.commit_push)
     message = args.message if args.message else ""
     no_verify = cast(bool, args.no_verify)
     amend = cast(bool, args.amend)
     force = cast(bool, args.force)
 
     if not git_is_in_repo():
         console.print("You are not in a git repository", style="bold red")
         exit(1)
 
+    if pre:
+        pre_commit_result = pre_commit()
+
+        if isinstance(pre_commit_result, str):
+            print(pre_commit_result)
+            console.print(
+                "Pre-commit script failed. Fix errors then try again.", style="bold red"
+            )
+            exit(1)
+
     if not commit_push_only:
         stage(console)
 
     if commit(message, amend=amend, no_verify=no_verify, console=console):
         push(force=force or amend)
```

### Comparing `gscp-1.0.8/gscp/push_pull.py` & `gscp-1.0.9/gscp/push_pull.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.8/gscp/version.py` & `gscp-1.0.9/gscp/version.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.8/gscp/wrappers.py` & `gscp-1.0.9/gscp/wrappers.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.8/LICENSE` & `gscp-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gscp-1.0.8/pyproject.toml` & `gscp-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gscp"
-version = "1.0.8"
+version = "1.0.9"
 description = "A tool to quickly commit your work with git."
 authors = ["Samuel Yvon <samuelyvon9@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gscp" }]
 
 [tool.poetry.dependencies]
 rich = "^13.3.2"
```

### Comparing `gscp-1.0.8/README.md` & `gscp-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gscp-1.0.8/PKG-INFO` & `gscp-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscp
-Version: 1.0.8
+Version: 1.0.9
 Summary: A tool to quickly commit your work with git.
 Author: Samuel Yvon
 Author-email: samuelyvon9@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

