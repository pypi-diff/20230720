# Comparing `tmp/numbers_parser-4.1.1.tar.gz` & `tmp/numbers_parser-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-4.1.1.tar", max compression
+gzip compressed data, was "numbers_parser-4.1.2.tar", max compression
```

## Comparing `numbers_parser-4.1.1.tar` & `numbers_parser-4.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.1.1/LICENSE.rst
--rw-r--r--   0        0        0    20092 2023-07-16 14:26:24.846490 numbers_parser-4.1.1/README.md
--rw-r--r--   0        0        0     2096 2023-07-16 17:08:47.778752 numbers_parser-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     2045 2023-07-08 11:12:33.341467 numbers_parser-4.1.1/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     4350 2023-07-16 15:02:05.843221 numbers_parser-4.1.1/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5826 2023-07-16 15:04:36.595811 numbers_parser-4.1.1/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.1.1/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    17976 2023-07-16 17:03:54.394032 numbers_parser-4.1.1/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    29688 2023-07-16 17:05:59.012525 numbers_parser-4.1.1/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     1689 2023-07-16 11:18:31.505310 numbers_parser-4.1.1/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.1.1/src/numbers_parser/containers.py
--rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.1.1/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    17568 2023-07-16 14:14:17.514493 numbers_parser-4.1.1/src/numbers_parser/document.py
--rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.1.1/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.1.1/src/numbers_parser/experimental.py
--rw-r--r--   0        0        0     3865 2023-07-14 19:05:10.688785 numbers_parser-4.1.1/src/numbers_parser/file.py
--rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.1.1/src/numbers_parser/formula.py
--rw-r--r--   0        0        0    16007 2023-07-10 11:50:37.380120 numbers_parser-4.1.1/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2023-07-10 11:50:37.381233 numbers_parser-4.1.1/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2023-07-10 11:50:37.381940 numbers_parser-4.1.1/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2023-07-10 11:50:37.383021 numbers_parser-4.1.1/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    17361 2023-07-10 11:50:37.383432 numbers_parser-4.1.1/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2023-07-10 11:50:37.383703 numbers_parser-4.1.1/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2023-07-10 11:50:37.383945 numbers_parser-4.1.1/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64955 2023-07-10 11:50:37.384822 numbers_parser-4.1.1/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2023-07-10 11:50:37.385161 numbers_parser-4.1.1/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2023-07-10 11:50:37.385944 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    46323 2023-07-10 11:50:37.386335 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    22717 2023-07-10 11:50:37.386667 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    63730 2023-07-10 11:50:37.387194 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2023-07-10 11:50:37.387691 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2023-07-10 11:50:37.387967 numbers_parser-4.1.1/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    40151 2023-07-10 11:50:37.388832 numbers_parser-4.1.1/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2023-07-10 11:50:37.389137 numbers_parser-4.1.1/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2023-07-10 11:50:37.389550 numbers_parser-4.1.1/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53520 2023-07-10 11:50:37.390046 numbers_parser-4.1.1/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2023-07-10 11:50:37.390302 numbers_parser-4.1.1/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    18142 2023-07-10 11:50:37.390611 numbers_parser-4.1.1/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2023-07-10 11:50:37.390860 numbers_parser-4.1.1/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    12611 2023-07-10 11:50:37.391120 numbers_parser-4.1.1/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9717 2023-07-10 11:50:37.391599 numbers_parser-4.1.1/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2023-07-10 11:50:37.391866 numbers_parser-4.1.1/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88532 2023-07-10 11:50:37.392988 numbers_parser-4.1.1/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2023-07-10 11:50:37.393496 numbers_parser-4.1.1/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2023-07-10 11:50:37.394520 numbers_parser-4.1.1/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12644 2023-07-10 11:50:37.394909 numbers_parser-4.1.1/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    58663 2023-07-10 11:50:37.396073 numbers_parser-4.1.1/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    28840 2023-07-10 11:50:37.396468 numbers_parser-4.1.1/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2023-07-10 11:50:37.397211 numbers_parser-4.1.1/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2023-07-10 11:50:37.401529 numbers_parser-4.1.1/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    22604 2023-07-16 09:02:55.094582 numbers_parser-4.1.1/src/numbers_parser/generated/fontmap.py
--rw-r--r--   0        0        0     6082 2023-07-14 19:05:10.690473 numbers_parser-4.1.1/src/numbers_parser/generated/functionmap.py
--rw-r--r--   0        0        0    12032 2023-07-15 11:47:48.837033 numbers_parser-4.1.1/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    32100 2023-07-10 11:51:11.630380 numbers_parser-4.1.1/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0    75106 2023-07-16 16:55:17.689748 numbers_parser-4.1.1/src/numbers_parser/model.py
--rw-r--r--   0        0        0     2690 2023-07-08 11:12:33.356950 numbers_parser-4.1.1/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    21269 1970-01-01 00:00:00.000000 numbers_parser-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.1.2/LICENSE.rst
+-rw-r--r--   0        0        0    20092 2023-07-16 14:26:24.846490 numbers_parser-4.1.2/README.md
+-rw-r--r--   0        0        0     2112 2023-07-18 20:11:54.382694 numbers_parser-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2139 2023-07-18 20:05:00.796169 numbers_parser-4.1.2/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     4350 2023-07-16 15:02:05.843221 numbers_parser-4.1.2/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5826 2023-07-16 15:04:36.595811 numbers_parser-4.1.2/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.1.2/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    17992 2023-07-19 18:11:53.756245 numbers_parser-4.1.2/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    29688 2023-07-18 19:05:31.031251 numbers_parser-4.1.2/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     1689 2023-07-16 11:18:31.505310 numbers_parser-4.1.2/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.1.2/src/numbers_parser/containers.py
+-rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.1.2/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    17543 2023-07-20 18:34:33.748901 numbers_parser-4.1.2/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.1.2/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.1.2/src/numbers_parser/experimental.py
+-rw-r--r--   0        0        0     3865 2023-07-14 19:05:10.688785 numbers_parser-4.1.2/src/numbers_parser/file.py
+-rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.1.2/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0    16007 2023-07-10 11:50:37.380120 numbers_parser-4.1.2/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-07-10 11:50:37.381233 numbers_parser-4.1.2/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-07-10 11:50:37.381940 numbers_parser-4.1.2/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-07-10 11:50:37.383021 numbers_parser-4.1.2/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17361 2023-07-10 11:50:37.383432 numbers_parser-4.1.2/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-07-10 11:50:37.383703 numbers_parser-4.1.2/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-07-10 11:50:37.383945 numbers_parser-4.1.2/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64955 2023-07-10 11:50:37.384822 numbers_parser-4.1.2/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-07-10 11:50:37.385161 numbers_parser-4.1.2/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-07-10 11:50:37.385944 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    46323 2023-07-10 11:50:37.386335 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    22717 2023-07-10 11:50:37.386667 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    63730 2023-07-10 11:50:37.387194 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-07-10 11:50:37.387691 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-07-10 11:50:37.387967 numbers_parser-4.1.2/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    40151 2023-07-10 11:50:37.388832 numbers_parser-4.1.2/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-07-10 11:50:37.389137 numbers_parser-4.1.2/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-07-10 11:50:37.389550 numbers_parser-4.1.2/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53520 2023-07-10 11:50:37.390046 numbers_parser-4.1.2/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-07-10 11:50:37.390302 numbers_parser-4.1.2/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18142 2023-07-10 11:50:37.390611 numbers_parser-4.1.2/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-07-10 11:50:37.390860 numbers_parser-4.1.2/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    12611 2023-07-10 11:50:37.391120 numbers_parser-4.1.2/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9717 2023-07-10 11:50:37.391599 numbers_parser-4.1.2/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-07-10 11:50:37.391866 numbers_parser-4.1.2/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88532 2023-07-10 11:50:37.392988 numbers_parser-4.1.2/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-07-10 11:50:37.393496 numbers_parser-4.1.2/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-07-10 11:50:37.394520 numbers_parser-4.1.2/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12644 2023-07-10 11:50:37.394909 numbers_parser-4.1.2/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    58663 2023-07-10 11:50:37.396073 numbers_parser-4.1.2/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    28840 2023-07-10 11:50:37.396468 numbers_parser-4.1.2/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-07-10 11:50:37.397211 numbers_parser-4.1.2/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:50:37.401529 numbers_parser-4.1.2/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    22604 2023-07-16 09:02:55.094582 numbers_parser-4.1.2/src/numbers_parser/generated/fontmap.py
+-rw-r--r--   0        0        0     6082 2023-07-14 19:05:10.690473 numbers_parser-4.1.2/src/numbers_parser/generated/functionmap.py
+-rw-r--r--   0        0        0    12032 2023-07-15 11:47:48.837033 numbers_parser-4.1.2/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    32100 2023-07-10 11:51:11.630380 numbers_parser-4.1.2/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0    75677 2023-07-20 18:36:31.553525 numbers_parser-4.1.2/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     2690 2023-07-08 11:12:33.356950 numbers_parser-4.1.2/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    21269 1970-01-01 00:00:00.000000 numbers_parser-4.1.2/PKG-INFO
```

### Comparing `numbers_parser-4.1.1/LICENSE.rst` & `numbers_parser-4.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/README.md` & `numbers_parser-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/pyproject.toml` & `numbers_parser-4.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "4.1.1"
+version = "4.1.2"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
@@ -35,14 +35,15 @@
 pytest-console-scripts = "^1.3.1"
 pytest-cov = "^4.0.0"
 pytest-profiling = "^1.7.0"
 python-magic = "^0.4.27"
 termcolor = "^2.2.0"
 gprof2dot = "^2022.7.29"
 line-profiler = "^4.0.3"
+mock = "^5.1.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `numbers_parser-4.1.1/src/numbers_parser/__init__.py` & `numbers_parser-4.1.2/src/numbers_parser/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import importlib.metadata
 import os
 import plistlib
 import warnings
 
 from numbers_parser.document import Document  # NOQA
 from numbers_parser.cell import *  # NOQA
+from numbers_parser.exceptions import *  # NOQA
 
 __version__ = importlib.metadata.version("numbers-parser")
 
 _DEFAULT_NUMBERS_INSTALL_PATH = "/Applications/Numbers.app"
 _VERSION_PLIST_PATH = "Contents/version.plist"
 _SUPPORTED_NUMBERS_VERSIONS = [
     "10.3",
@@ -42,34 +43,36 @@
     "13.0",
     "13.1",
 ]
 
 # Don't print the source line
 old_warn_f = warnings.formatwarning
 warnings.formatwarning = (
-    lambda msg, catg, fname, lineno, line=None: old_warn_f(  # pragma: no cover
+    # pragma: no cover -- lambda not run by coverage
+    lambda msg, catg, fname, lineno, line=None: old_warn_f(
         msg, catg, fname, lineno, line=""
     )
 )
 
 
 def _get_version():
     return __version__
 
 
 def _check_installed_numbers_version():
     try:
         fp = open(
             os.path.join(_DEFAULT_NUMBERS_INSTALL_PATH, _VERSION_PLIST_PATH), "rb"
         )
-    except IOError:  # pragma: no cover
+    except IOError:
         return None
     version_dict = plistlib.load(fp)
     installed_version = version_dict["CFBundleShortVersionString"]
     if installed_version not in _SUPPORTED_NUMBERS_VERSIONS:
         warnings.warn(
             f"Numbers version {installed_version} not tested with this version"
         )
     fp.close()
+    return installed_version
 
 
-_check_installed_numbers_version()
+_ = _check_installed_numbers_version()
```

### Comparing `numbers_parser-4.1.1/src/numbers_parser/_cat_numbers.py` & `numbers_parser-4.1.2/src/numbers_parser/_cat_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-4.1.2/src/numbers_parser/_unpack_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/bullets.py` & `numbers_parser-4.1.2/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/cell.py` & `numbers_parser-4.1.2/src/numbers_parser/cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,16 @@
     font_size: float = DEFAULT_FONT_SIZE
     font_name: str = DEFAULT_FONT
     bold: bool = False
     italic: bool = False
     strikethrough: bool = False
     underline: bool = False
     name: str = None
-    _text_style_id: int = None
-    _cell_style_id: int = None
+    _text_style_obj_id: int = None
+    _cell_style_obj_id: int = None
     _update_cell_style: bool = False
     _update_text_style: bool = False
 
     @staticmethod
     def _text_attrs():
         return [
             "font_color",
@@ -140,16 +140,16 @@
             font_size=model.cell_font_size(cell_storage),
             font_name=model.cell_font_name(cell_storage),
             bold=model.cell_is_bold(cell_storage),
             italic=model.cell_is_italic(cell_storage),
             strikethrough=model.cell_is_strikethrough(cell_storage),
             underline=model.cell_is_underline(cell_storage),
             name=model.cell_style_name(cell_storage),
-            _text_style_id=model.text_style_object_id(cell_storage),
-            _cell_style_id=model.cell_style_object_id(cell_storage),
+            _text_style_obj_id=model.text_style_object_id(cell_storage),
+            _cell_style_obj_id=model.cell_style_object_id(cell_storage),
         )
         return style
 
     def __post_init__(self):
         if not isinstance(self.alignment, Alignment):
             raise TypeError("value must be an Alignment class")
```

### Comparing `numbers_parser-4.1.1/src/numbers_parser/cell_storage.py` & `numbers_parser-4.1.2/src/numbers_parser/cell_storage.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/constants.py` & `numbers_parser-4.1.2/src/numbers_parser/constants.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/containers.py` & `numbers_parser-4.1.2/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/data/empty.numbers` & `numbers_parser-4.1.2/src/numbers_parser/data/empty.numbers`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/document.py` & `numbers_parser-4.1.2/src/numbers_parser/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         """Add a new style to the current document. If no style name is
         provided, the next available numbered style will be generated"""
         if "name" in kwargs and kwargs["name"] is not None:
             if kwargs["name"] in self._model.styles.keys():
                 raise IndexError(f"style '{kwargs['name']}' already exists")
         style = Style(**kwargs)
         if style.name is None:
-            style.name = self._model.custom_style_name(self._model.styles.keys())
+            style.name = self._model.custom_style_name()
         style._update_styles = True
         self._model.styles[style.name] = style
         return style
 
 
 class Sheet:
     def __init__(self, model, sheet_id):
```

### Comparing `numbers_parser-4.1.1/src/numbers_parser/exceptions.py` & `numbers_parser-4.1.2/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/file.py` & `numbers_parser-4.1.2/src/numbers_parser/file.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/formula.py` & `numbers_parser-4.1.2/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/fontmap.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/fontmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/generated/functionmap.py` & `numbers_parser-4.1.2/src/numbers_parser/generated/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/iwafile.py` & `numbers_parser-4.1.2/src/numbers_parser/iwafile.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/mapping.py` & `numbers_parser-4.1.2/src/numbers_parser/mapping.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/src/numbers_parser/model.py` & `numbers_parser-4.1.2/src/numbers_parser/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,16 +363,14 @@
                     return base_owner_uid
 
     @lru_cache(maxsize=None)
     def formula_cell_ranges(self, table_id: int) -> list:
         """Exract all the formula cell ranges for the Table."""
         # https://github.com/masaccio/numbers-parser/blob/main/doc/Numbers.md#formula-ranges
         calc_engine = self.calc_engine()
-        if calc_engine is None:  # pragma: no cover
-            return []
 
         table_base_id = self.table_base_id(table_id)
         cell_records = []
         for finfo in calc_engine.dependency_tracker.formula_owner_info:
             if finfo.HasField("cell_dependencies"):  # pragma: no branch
                 formula_owner_id = NumbersUUID(finfo.formula_owner_id).hex
                 if formula_owner_id == table_base_id:
@@ -1166,25 +1164,30 @@
         presets_map = {
             self.objects[x.identifier].super.name: {
                 "id": x.identifier,
                 "obj": self.objects[x.identifier],
             }
             for x in presets
         }
+        # HorizontalJustification(cell_style.para_properties.alignment)
         return {
             k: Style(
+                alignment=Alignment(
+                    HorizontalJustification(v["obj"].para_properties.alignment),
+                    VerticalJustification(0),
+                ),
                 font_color=self.cell_font_color(v["obj"]),
                 font_size=self.cell_font_size(v["obj"]),
                 font_name=self.cell_font_name(v["obj"]),
                 bold=self.cell_is_bold(v["obj"]),
                 italic=self.cell_is_italic(v["obj"]),
                 underline=self.cell_is_underline(v["obj"]),
                 strikethrough=self.cell_is_strikethrough(v["obj"]),
                 name=self.cell_style_name(v["obj"]),
-                _text_style_id=v["id"],
+                _text_style_obj_id=v["id"],
             )
             for k, v in presets_map.items()
         }
 
     def add_paragraph_style(self, style: Style) -> int:
         if style.underline:
             underline = CharacterStyle.UnderlineType.kSingleUnderline
@@ -1263,15 +1266,15 @@
             underline = CharacterStyle.UnderlineType.kSingleUnderline
         else:
             underline = CharacterStyle.UnderlineType.kNoUnderline
         if style.strikethrough:
             strikethru = CharacterStyle.StrikethruType.kSingleStrikethru
         else:
             strikethru = CharacterStyle.StrikethruType.kNoStrikethru
-        style_obj = self.objects[style._text_style_id]
+        style_obj = self.objects[style._text_style_obj_id]
         style_obj.char_properties.font_color.r = style.font_color.r / 255
         style_obj.char_properties.font_color.g = style.font_color.g / 255
         style_obj.char_properties.font_color.b = style.font_color.b / 255
         style_obj.char_properties.bold = style.bold
         style_obj.char_properties.italic = style.italic
         style_obj.char_properties.underline = underline
         style_obj.char_properties.strikethru = strikethru
@@ -1281,22 +1284,22 @@
         style_obj.char_properties.tsd_fill.color.g = style.font_color.g / 255
         style_obj.char_properties.tsd_fill.color.b = style.font_color.b / 255
         style_obj.para_properties.alignment = style.alignment.horizontal
 
     def update_paragraph_styles(self):
         """Create new paragraph style archives for any new styles that
         have been created for this document"""
-        new_styles = [x for x in self.styles.values() if x._text_style_id is None]
+        new_styles = [x for x in self.styles.values() if x._text_style_obj_id is None]
         updated_styles = [
             x
             for x in self.styles.values()
-            if x._text_style_id is not None and x._update_text_style
+            if x._text_style_obj_id is not None and x._update_text_style
         ]
         for style in new_styles:
-            style._text_style_id = self.add_paragraph_style(style)
+            style._text_style_obj_id = self.add_paragraph_style(style)
             style._update_text_style = True
 
         for style in updated_styles:
             self.update_paragraph_style(style)
 
     def update_cell_styles(self, table_id: int, data: List):
         """Create new cell style archives for any cells whose styles
@@ -1312,15 +1315,15 @@
                             cell.style.alignment.vertical,
                             cell.style.bg_color.r,
                             cell.style.bg_color.g,
                             cell.style.bg_color.b,
                         )
                     if fingerprint not in cell_styles:
                         cell_styles[fingerprint] = self.add_cell_style(cell._style)
-                    cell._style._cell_style_id = cell_styles[fingerprint]
+                    cell._style._cell_style_obj_id = cell_styles[fingerprint]
 
     def add_cell_style(self, style: Style) -> int:
         if style.bg_color is not None:
             color_attrs = {
                 "cell_fill": {
                     "color": {
                         "model": "rgb",
@@ -1330,30 +1333,32 @@
                         "a": 1.0,
                         "rgbspace": "srgb",
                     }
                 }
             }
         else:
             color_attrs = {}
-        style_id_name = f"numbers-parser-custom-{style._cell_style_id}"
         cell_style_id, cell_style = self.objects.create_object_from_dict(
             "DocumentStylesheet",
             {
                 "super": {
                     "name": style.name,
-                    "style_identifier": style_id_name,
+                    "style_identifier": "",
                 },
                 "override_count": 1,
                 "cell_properties": {
                     **color_attrs,
                     "vertical_alignment": style.alignment.vertical,
                 },
             },
             TSTArchives.CellStyleArchive,
         )
+        style_id_name = f"numbers-parser-custom-{cell_style_id}"
+        cell_style.super.style_identifier = style_id_name
+
         stylesheet_id = self.objects[DOCUMENT_ID].stylesheet.identifier
         cell_style.super.stylesheet.MergeFrom(
             TSPMessages.Reference(identifier=stylesheet_id)
         )
         self.objects[stylesheet_id].styles.append(
             TSPMessages.Reference(identifier=cell_style_id)
         )
@@ -1377,18 +1382,19 @@
         if cell_storage.cell_style_id is None:
             return None
         entry = self._table_styles.lookup_value(
             cell_storage.table_id, cell_storage.cell_style_id
         )
         return entry.reference.identifier
 
-    def custom_style_name(self, current_styles: List[str]) -> Tuple[str, str]:
+    def custom_style_name(self) -> Tuple[str, str]:
         """Find custom styles in the current document and return the next
         highest numbered style"""
         stylesheet_id = self.objects[DOCUMENT_ID].stylesheet.identifier
+        current_styles = self.styles.keys()
         custom_styles = [
             x for x in current_styles if re.fullmatch(r"Custom Style \d+", x)
         ]
         for style_entry in self.objects[stylesheet_id].identifier_to_style_map:
             style_id = style_entry.style.identifier
             style_name = getattr(self.objects[style_id].super, "name", "")
             if re.fullmatch(r"Custom Style \d+", style_name):
@@ -1409,31 +1415,31 @@
         col_num: int,
         formula_id=None,
         num_format_id=None,
     ) -> bytearray:
         """Create a storage buffer for a cell using v5 (modern) layout"""
         cell = data[row_num][col_num]
         if cell._style is not None:
-            if cell.style._text_style_id is not None:
+            if cell._style._text_style_obj_id is not None:
                 cell._storage.text_style_id = self._table_styles.lookup_key(
                     cell._table_id,
-                    TSPMessages.Reference(identifier=cell.style._text_style_id),
+                    TSPMessages.Reference(identifier=cell._style._text_style_obj_id),
                 )
                 self.add_component_reference(
-                    cell.style._text_style_id,
+                    cell._style._text_style_obj_id,
                     parent_id=self._table_styles.id(cell._table_id),
                 )
 
-            if cell.style._cell_style_id is not None:
+            if cell._style._cell_style_obj_id is not None:
                 cell._storage.cell_style_id = self._table_styles.lookup_key(
                     cell._table_id,
-                    TSPMessages.Reference(identifier=cell.style._cell_style_id),
+                    TSPMessages.Reference(identifier=cell._style._cell_style_obj_id),
                 )
                 self.add_component_reference(
-                    cell.style._cell_style_id,
+                    cell._style._cell_style_obj_id,
                     parent_id=self._table_styles.id(cell._table_id),
                 )
 
         length = 12
         if isinstance(cell, NumberCell):
             flags = 1
             length += 16
@@ -1643,15 +1649,21 @@
                 start_row_num, table_model.number_of_header_rows
             ):
                 return self.objects[table_model.footer_row_text_style.identifier]
         return self.objects[table_model.body_text_style.identifier]
 
     def cell_alignment(self, cell_storage: object) -> Alignment:
         cell_style = self.cell_text_style(cell_storage)
-        horizontal = HorizontalJustification(cell_style.para_properties.alignment)
+        if cell_style.para_properties.HasField("alignment"):
+            horizontal = HorizontalJustification(cell_style.para_properties.alignment)
+        else:
+            parent_obj_id = cell_style.super.parent.identifier
+            horizontal = HorizontalJustification(
+                self.objects[parent_obj_id].para_properties.alignment
+            )
 
         if cell_storage.cell_style_id is None:
             vertical = VerticalJustification.TOP
         else:
             cell_style = self.table_style(
                 cell_storage.table_id, cell_storage.cell_style_id
             )
@@ -1683,15 +1695,15 @@
 
     def cell_is_bold(self, obj: object) -> bool:
         style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         return self.char_property(style, "bold")
 
     def cell_is_italic(self, obj: object) -> bool:
         style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
-        return self.char_property(style, "bold")
+        return self.char_property(style, "italic")
 
     def cell_is_underline(self, obj: object) -> bool:
         style = self.cell_text_style(obj) if isinstance(obj, CellStorage) else obj
         underline = self.char_property(style, "underline")
         return underline != CharacterStyle.UnderlineType.kNoUnderline
 
     def cell_is_strikethrough(self, obj: object) -> bool:
```

### Comparing `numbers_parser-4.1.1/src/numbers_parser/numbers_uuid.py` & `numbers_parser-4.1.2/src/numbers_parser/numbers_uuid.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.1.1/PKG-INFO` & `numbers_parser-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-parser
-Version: 4.1.1
+Version: 4.1.2
 Summary: Read and write Apple Numbers spreadsheets
 Home-page: https://github.com/masaccio/numbers-parser
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

