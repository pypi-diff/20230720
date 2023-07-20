# Comparing `tmp/docblock-0.0.1a0.tar.gz` & `tmp/docblock-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docblock-0.0.1a0.tar", max compression
+gzip compressed data, was "docblock-0.0.1a1.tar", max compression
```

## Comparing `docblock-0.0.1a0.tar` & `docblock-0.0.1a1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-07-19 20:34:05.530959 docblock-0.0.1a0/LICENSE.md
--rw-r--r--   0        0        0      719 2023-07-19 20:34:05.530959 docblock-0.0.1a0/README.md
--rw-r--r--   0        0        0       37 2023-07-19 20:34:05.530959 docblock-0.0.1a0/docblock/__init__.py
--rw-r--r--   0        0        0      315 2023-07-19 20:34:05.530959 docblock-0.0.1a0/docblock/parse.py
--rw-r--r--   0        0        0        0 2023-07-19 20:34:05.530959 docblock-0.0.1a0/docblock/tests/__init__.py
--rw-r--r--   0        0        0      101 2023-07-19 20:34:05.530959 docblock-0.0.1a0/docblock/tests/test_parse.py
--rw-r--r--   0        0        0     1765 2023-07-19 20:34:05.530959 docblock-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 docblock-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 14:21:49.042286 docblock-0.0.1a1/LICENSE.md
+-rw-r--r--   0        0        0     2198 2023-07-20 14:21:49.042286 docblock-0.0.1a1/README.md
+-rw-r--r--   0        0        0       78 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/__init__.py
+-rw-r--r--   0        0        0      988 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/grammar.py
+-rw-r--r--   0        0        0     2110 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/parse.py
+-rw-r--r--   0        0        0      779 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/show_versions.py
+-rw-r--r--   0        0        0      792 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/utils.py
+-rw-r--r--   0        0        0     1827 2023-07-20 14:21:49.042286 docblock-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 docblock-0.0.1a1/PKG-INFO
```

### Comparing `docblock-0.0.1a0/LICENSE.md` & `docblock-0.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docblock-0.0.1a0/pyproject.toml` & `docblock-0.0.1a1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "docblock"
-version = "0.0.1a0"
-description = "Reads and parses documentation from C++ header files in pure Python."
+version = "0.0.1a1"
+description = "Reads and parses documentation from header files in pure Python."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/docblock"
 include = [
     "LICENSE.md",
 ]
@@ -55,14 +55,15 @@
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = "--cov=. --cov-report=xml"
 
 [tool.coverage.run]
 omit = [
+    "docblock/show_versions.py",  # only prints debug information
     "*/tests/*",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     # This excludes all abstract methods from code coverage checks,
     # as they are never instantiated directly anyway
```

