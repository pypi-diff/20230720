# Comparing `tmp/jkUnicode-2.0.6.tar.gz` & `tmp/jkUnicode-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jkUnicode-2.0.6.tar", last modified: Thu Jul  6 13:01:25 2023, max compression
+gzip compressed data, was "jkUnicode-2.0.7.tar", last modified: Thu Jul 20 08:15:42 2023, max compression
```

## Comparing `jkUnicode-2.0.6.tar` & `jkUnicode-2.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:25.868454 jkUnicode-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-06 13:01:25.868454 jkUnicode-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:25.860454 jkUnicode-2.0.6/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:25.864454 jkUnicode-2.0.6/lib/jkUnicode/
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/aglfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/aglfnData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:25.864454 jkUnicode-2.0.6/lib/jkUnicode/cmdline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/cmdline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/cmdline/ortho.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/cmdline/uniinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:25.868454 jkUnicode-2.0.6/lib/jkUnicode/json/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/json/ignored_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/json/ignored_languages.json
--rw-r--r--   0 runner    (1001) docker     (123)  1404126 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/json/language_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/json/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/json/scripts.json
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/json/territories.json
--rw-r--r--   0 runner    (1001) docker     (123)    31506 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/orthography.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:25.868454 jkUnicode-2.0.6/lib/jkUnicode/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/tools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/tools/jsonhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/tools/xmlhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)    58924 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniCase.py
--rw-r--r--   0 runner    (1001) docker     (123)   646770 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniCat.py
--rw-r--r--   0 runner    (1001) docker     (123)    54403 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniDecomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)  1478896 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniName.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniNiceName.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniRangesBits.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniScript.py
--rw-r--r--   0 runner    (1001) docker     (123)    74012 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/lib/jkUnicode/uniScriptData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:01:25.864454 jkUnicode-2.0.6/lib/jkUnicode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-06 13:01:25.000000 jkUnicode-2.0.6/lib/jkUnicode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-06 13:01:25.000000 jkUnicode-2.0.6/lib/jkUnicode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:01:25.000000 jkUnicode-2.0.6/lib/jkUnicode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 13:01:25.000000 jkUnicode-2.0.6/lib/jkUnicode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 13:01:25.000000 jkUnicode-2.0.6/lib/jkUnicode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 13:01:25.000000 jkUnicode-2.0.6/lib/jkUnicode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:01:25.000000 jkUnicode-2.0.6/lib/jkUnicode.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-06 13:01:25.868454 jkUnicode-2.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-07-06 13:01:14.000000 jkUnicode-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:42.532827 jkUnicode-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-20 08:15:42.532827 jkUnicode-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:42.524827 jkUnicode-2.0.7/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:42.528827 jkUnicode-2.0.7/lib/jkUnicode/
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/aglfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/aglfnData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:42.528827 jkUnicode-2.0.7/lib/jkUnicode/cmdline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/cmdline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/cmdline/ortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/cmdline/uniinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:42.532827 jkUnicode-2.0.7/lib/jkUnicode/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/json/ignored_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/json/ignored_languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1404126 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/json/language_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/json/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/json/scripts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/json/territories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31506 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/orthography.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:42.532827 jkUnicode-2.0.7/lib/jkUnicode/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/tools/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/tools/jsonhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/tools/xmlhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58924 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   646770 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniCat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54403 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniDecomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1478896 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniNiceName.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniRangesBits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74012 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/lib/jkUnicode/uniScriptData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:42.528827 jkUnicode-2.0.7/lib/jkUnicode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-20 08:15:42.000000 jkUnicode-2.0.7/lib/jkUnicode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-20 08:15:42.000000 jkUnicode-2.0.7/lib/jkUnicode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:15:42.000000 jkUnicode-2.0.7/lib/jkUnicode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 08:15:42.000000 jkUnicode-2.0.7/lib/jkUnicode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:15:42.000000 jkUnicode-2.0.7/lib/jkUnicode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 08:15:42.000000 jkUnicode-2.0.7/lib/jkUnicode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 08:15:42.000000 jkUnicode-2.0.7/lib/jkUnicode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-20 08:15:42.532827 jkUnicode-2.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-07-20 08:15:33.000000 jkUnicode-2.0.7/setup.py
```

### Comparing `jkUnicode-2.0.6/LICENSE` & `jkUnicode-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/PKG-INFO` & `jkUnicode-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: jkUnicode
-Version: 2.0.6
+Version: 2.0.7
 Summary: Unicode support libraries
 Home-page: https://pypi.org/project/jkUnicode/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Documentation, https://jkunicode.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/jenskutilek/jkUnicode
 Project-URL: Tracker, https://github.com/jenskutilek/jkUnicode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: woff
 License-File: LICENSE
 
 # jkUnicode
 
 A Python module for Unicode, glyph name, and orthography information.
 
 The orthography functions can be used via the command line script `ortho`. The Unicode info for one or more codepoints can be shown via the command `uniinfo`.
```

### Comparing `jkUnicode-2.0.6/README.md` & `jkUnicode-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/__init__.py` & `jkUnicode-2.0.7/lib/jkUnicode/__init__.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/aglfn.py` & `jkUnicode-2.0.7/lib/jkUnicode/aglfn.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/aglfnData.py` & `jkUnicode-2.0.7/lib/jkUnicode/aglfnData.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/cmdline/ortho.py` & `jkUnicode-2.0.7/lib/jkUnicode/cmdline/ortho.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/cmdline/uniinfo.py` & `jkUnicode-2.0.7/lib/jkUnicode/cmdline/uniinfo.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/json/ignored_languages.json` & `jkUnicode-2.0.7/lib/jkUnicode/json/ignored_languages.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/json/language_characters.json` & `jkUnicode-2.0.7/lib/jkUnicode/json/language_characters.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/json/languages.json` & `jkUnicode-2.0.7/lib/jkUnicode/json/languages.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/json/scripts.json` & `jkUnicode-2.0.7/lib/jkUnicode/json/scripts.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/json/territories.json` & `jkUnicode-2.0.7/lib/jkUnicode/json/territories.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/orthography.py` & `jkUnicode-2.0.7/lib/jkUnicode/orthography.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/tools/helpers.py` & `jkUnicode-2.0.7/lib/jkUnicode/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/tools/jsonhelpers.py` & `jkUnicode-2.0.7/lib/jkUnicode/tools/jsonhelpers.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/tools/xmlhelpers.py` & `jkUnicode-2.0.7/lib/jkUnicode/tools/xmlhelpers.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniBlock.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniBlock.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniBlockData.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniBlockData.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniCase.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniCase.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniCat.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniCat.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniDecomposition.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniDecomposition.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniName.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniName.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniNiceName.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniNiceName.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniRangesBits.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniRangesBits.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode/uniScriptData.py` & `jkUnicode-2.0.7/lib/jkUnicode/uniScriptData.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.6/lib/jkUnicode.egg-info/PKG-INFO` & `jkUnicode-2.0.7/lib/jkUnicode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: jkUnicode
-Version: 2.0.6
+Version: 2.0.7
 Summary: Unicode support libraries
 Home-page: https://pypi.org/project/jkUnicode/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Documentation, https://jkunicode.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/jenskutilek/jkUnicode
 Project-URL: Tracker, https://github.com/jenskutilek/jkUnicode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: woff
 License-File: LICENSE
 
 # jkUnicode
 
 A Python module for Unicode, glyph name, and orthography information.
 
 The orthography functions can be used via the command line script `ortho`. The Unicode info for one or more codepoints can be shown via the command `uniinfo`.
```

### Comparing `jkUnicode-2.0.6/lib/jkUnicode.egg-info/SOURCES.txt` & `jkUnicode-2.0.7/lib/jkUnicode.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 lib/jkUnicode/uniRangesBits.py
 lib/jkUnicode/uniScript.py
 lib/jkUnicode/uniScriptData.py
 lib/jkUnicode.egg-info/PKG-INFO
 lib/jkUnicode.egg-info/SOURCES.txt
 lib/jkUnicode.egg-info/dependency_links.txt
 lib/jkUnicode.egg-info/entry_points.txt
+lib/jkUnicode.egg-info/not-zip-safe
 lib/jkUnicode.egg-info/requires.txt
 lib/jkUnicode.egg-info/top_level.txt
-lib/jkUnicode.egg-info/zip-safe
 lib/jkUnicode/cmdline/__init__.py
 lib/jkUnicode/cmdline/ortho.py
 lib/jkUnicode/cmdline/uniinfo.py
 lib/jkUnicode/json/ignored_characters.json
 lib/jkUnicode/json/ignored_languages.json
 lib/jkUnicode/json/language_characters.json
 lib/jkUnicode/json/languages.json
```

### Comparing `jkUnicode-2.0.6/setup.cfg` & `jkUnicode-2.0.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jkUnicode
-version = 2.0.6
+version = 2.0.7
 description = Unicode support libraries
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://pypi.org/project/jkUnicode/
 author = Jens Kutilek
 license = MIT
 license_files = LICENSE
@@ -15,23 +15,26 @@
 	Environment :: Console
 project_urls = 
 	Documentation = https://jkunicode.readthedocs.io/en/latest/
 	Source = https://github.com/jenskutilek/jkUnicode
 	Tracker = https://github.com/jenskutilek/jkUnicode/issues
 
 [options]
-zip_safe = True
+zip_safe = False
 package_dir = 
 	=lib
 packages = find:
 platforms = any
 install_requires = 
-	fontTools[woff] >= 4.38.0
+	fontTools >= 4.38.0
 python_requires = >=3.8
 
+[options.extras_require]
+woff = fontTools[woff] >= 4.38.0
+
 [options.packages.find]
 where = lib
 
 [options.package_data]
 * = py.typed, json/ignored_characters.json, json/ignored_languages.json, json/language_characters.json, json/languages.json, json/scripts.json, json/territories.json
 
 [bdist_wheel]
```

