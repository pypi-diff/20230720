# Comparing `tmp/python-define-1.0.2.tar.gz` & `tmp/python-define-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-define-1.0.2.tar", last modified: Tue Jul 18 02:57:34 2023, max compression
+gzip compressed data, was "python-define-1.1.2.tar", last modified: Thu Jul 20 11:55:25 2023, max compression
```

## Comparing `python-define-1.0.2.tar` & `python-define-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-18 02:57:34.234836 python-define-1.0.2/
--rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.0.2/LICENSE
--rw-r--r--   0 grant     (1000) grant     (1000)    44847 2023-07-18 02:57:34.234836 python-define-1.0.2/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)     4368 2023-07-18 02:55:31.000000 python-define-1.0.2/README.md
--rwxr-xr-x   0 grant     (1000) grant     (1000)     5452 2023-07-18 01:50:22.000000 python-define-1.0.2/define.py
--rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-07-18 02:56:06.000000 python-define-1.0.2/pyproject.toml
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-18 02:57:34.234836 python-define-1.0.2/python_define.egg-info/
--rw-r--r--   0 grant     (1000) grant     (1000)    44847 2023-07-18 02:57:34.000000 python-define-1.0.2/python_define.egg-info/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-07-18 02:57:34.000000 python-define-1.0.2/python_define.egg-info/SOURCES.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-07-18 02:57:34.000000 python-define-1.0.2/python_define.egg-info/dependency_links.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-18 02:57:34.000000 python-define-1.0.2/python_define.egg-info/entry_points.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-07-18 02:57:34.000000 python-define-1.0.2/python_define.egg-info/requires.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-07-18 02:57:34.000000 python-define-1.0.2/python_define.egg-info/top_level.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-18 02:57:34.234836 python-define-1.0.2/setup.cfg
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-20 11:55:25.898506 python-define-1.1.2/
+-rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.1.2/LICENSE
+-rw-r--r--   0 grant     (1000) grant     (1000)    44847 2023-07-20 11:55:25.898506 python-define-1.1.2/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)     4368 2023-07-18 02:55:31.000000 python-define-1.1.2/README.md
+-rwxr-xr-x   0 grant     (1000) grant     (1000)     5620 2023-07-20 11:52:42.000000 python-define-1.1.2/define.py
+-rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-07-20 11:54:08.000000 python-define-1.1.2/pyproject.toml
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-20 11:55:25.898506 python-define-1.1.2/python_define.egg-info/
+-rw-r--r--   0 grant     (1000) grant     (1000)    44847 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/SOURCES.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/dependency_links.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/entry_points.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/requires.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/top_level.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-20 11:55:25.898506 python-define-1.1.2/setup.cfg
```

### Comparing `python-define-1.0.2/LICENSE` & `python-define-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-define-1.0.2/PKG-INFO` & `python-define-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.0.2
+Version: 1.1.2
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `python-define-1.0.2/README.md` & `python-define-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `python-define-1.0.2/define.py` & `python-define-1.1.2/define.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,19 +78,21 @@
 - **I will never complement you**, I need you to define the words.
 
 ## Constraints
 
 - Your answers will be for the **English Language**.
 - The users locale value is: **{{locale}}**.
 - Ensure you answer with the users **locale** values in mind.
+- **State the differences between English locale spellings**.
 - If it looks like I am commenting to you or complementing you, I am not, I am asking for an answer.
 
 ## Answer Format
 
-Spelling: <correct-spelling>
+Spelling <locale>: <correct-spelling>
+<list-of-alternate-spellings-if-they-exist-for-different-locales-omit-if-there-is-no-difference>
 Definition: <your-definition>
 
 Synonyms: <list-ten-synonyms-as-numbered-bullet-points>
 
 Antonyms: <list-ten-antonyms-as-numbered-bullet-points>
 
 """
```

### Comparing `python-define-1.0.2/pyproject.toml` & `python-define-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-define"
-version = "1.0.2"
+version = "1.1.2"
 description = "An OpenAI powered command-line linguistics assistant"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Grant Carthew", email = "grant@carthew.net"},
 ]
```

### Comparing `python-define-1.0.2/python_define.egg-info/PKG-INFO` & `python-define-1.1.2/python_define.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.0.2
+Version: 1.1.2
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

