# Comparing `tmp/prettynumbers-0.3.3.tar.gz` & `tmp/prettynumbers-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.3.3.tar", max compression
+gzip compressed data, was "prettynumbers-0.3.4.tar", max compression
```

## Comparing `prettynumbers-0.3.3.tar` & `prettynumbers-0.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    14849 2016-07-14 20:10:07.000000 prettynumbers-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0     1138 2023-05-09 14:21:39.562989 prettynumbers-0.3.3/README.md
--rw-r--r--   0        0        0      138 2023-05-11 11:51:36.017906 prettynumbers-0.3.3/pretty_numbers/__init__.py
--rwxr-xr-x   0        0        0     2580 2023-05-11 11:51:36.019065 prettynumbers-0.3.3/pretty_numbers/pretty_numbers.py
--rw-r--r--   0        0        0        0 2023-05-09 14:21:39.565816 prettynumbers-0.3.3/pretty_numbers/py.typed
--rw-r--r--   0        0        0      808 2023-06-06 09:48:20.872084 prettynumbers-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    14849 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/LICENSE.txt
+-rw-r--r--   0        0        0     1138 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/README.md
+-rw-r--r--   0        0        0      138 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/pretty_numbers/__init__.py
+-rwxr-xr-x   0        0        0     2580 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/pretty_numbers/pretty_numbers.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/pretty_numbers/py.typed
+-rw-r--r--   0        0        0      808 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.4/PKG-INFO
```

### Comparing `prettynumbers-0.3.3/LICENSE.txt` & `prettynumbers-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.3/README.md` & `prettynumbers-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.3/pretty_numbers/pretty_numbers.py` & `prettynumbers-0.3.4/pretty_numbers/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.3/pyproject.toml` & `prettynumbers-0.3.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prettynumbers"
-version = "0.3.3"
+version = "0.3.4"
 authors = ["gerardk <gerardk@gmail.com>"]
 description="Display a range of numbers in a human readable way"
 license="GNU GENERAL PUBLIC LICENSE"
 packages = [{include = "pretty_numbers"}]
 readme = "README.md"
 repository = "https://github.com/vfxGer/pretty-numbers"
```

### Comparing `prettynumbers-0.3.3/PKG-INFO` & `prettynumbers-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.3.3
+Version: 0.3.4
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 License: GNU GENERAL PUBLIC LICENSE
 Author: gerardk
 Author-email: gerardk@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```

