# Comparing `tmp/bent-0.0.19.tar.gz` & `tmp/bent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bent-0.0.19.tar", last modified: Thu Jul 20 16:50:13 2023, max compression
+gzip compressed data, was "dist/bent-0.0.9.tar", last modified: Fri Feb  3 19:10:35 2023, max compression
```

## Comparing `bent-0.0.19.tar` & `bent-0.0.9.tar`

### file list

```diff
@@ -1,60 +1,57 @@
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    11340 2023-07-20 14:28:24.000000 bent-0.0.19/LICENSE.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)      202 2023-07-20 14:28:24.000000 bent-0.0.19/MANIFEST.in
--rw-rw-r--   0 pruas     (1000) pruas     (1000)    17894 2023-07-20 16:50:13.927462 bent-0.0.19/PKG-INFO
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     3733 2023-07-20 16:40:51.000000 bent-0.0.19/README.rst
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.923462 bent-0.0.19/bent/
--rw-rw-r--   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/__init__.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    13574 2023-07-20 14:28:24.000000 bent-0.0.19/bent/annotate.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1910 2023-07-20 14:28:24.000000 bent-0.0.19/bent/get_data.sh
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1885 2023-07-20 14:28:24.000000 bent-0.0.19/bent/get_kb_dicts.sh
--rw-rw-r--   0 pruas     (1000) pruas     (1000)      990 2023-07-20 14:28:24.000000 bent-0.0.19/bent/get_kbs.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)      203 2023-07-20 14:28:24.000000 bent-0.0.19/bent/requirements.txt
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2826 2023-07-20 14:28:24.000000 bent-0.0.19/bent/setup_package.sh
--rw-rw-r--   0 pruas     (1000) pruas     (1000)      185 2023-07-20 14:28:24.000000 bent-0.0.19/bent/setup_package_wrapper.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/bent/src/
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/bent/src/NILINKER/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/NILINKER/__init__.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    10851 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/NILINKER/nilinker.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1004 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/NILINKER/predict_nilinker.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    13207 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/NILINKER/utils.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/bent/src/REEL/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/__init__.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    14863 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/candidates.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2866 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/information_content.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2903 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/post_process.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20290 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/ppr_for_ned_all.class
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    39492 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/ppr_for_ned_all.java
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    15703 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/pre_process.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     3195 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/run.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1582 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/REEL/utils.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/__init__.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/bent/src/abbreviation_detector/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/abbreviation_detector/__init__.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)     2534 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/abbreviation_detector/run.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/bent/src/build/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/build/__init__.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/bent/src/build/annotations/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/build/annotations/__init__.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)    12272 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/build/annotations/dataset_entities.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/bent/src/build/kb/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/build/kb/__init__.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)     3724 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/build/kb/generate_dicts.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)    24029 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/build/kb/kb.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.927462 bent-0.0.19/bent/src/build/relation_extraction/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/build/relation_extraction/__init__.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)     8088 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/build/relation_extraction/dicts.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)      301 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/cfg.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     5803 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/classes.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2513 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/nel.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20008 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/ner.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20647 2023-07-20 14:28:24.000000 bent-0.0.19/bent/src/utils.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-07-20 16:50:13.923462 bent-0.0.19/bent.egg-info/
--rw-rw-r--   0 pruas     (1000) pruas     (1000)    17894 2023-07-20 16:50:13.000000 bent-0.0.19/bent.egg-info/PKG-INFO
--rw-rw-r--   0 pruas     (1000) pruas     (1000)     1247 2023-07-20 16:50:13.000000 bent-0.0.19/bent.egg-info/SOURCES.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)        1 2023-07-20 16:50:13.000000 bent-0.0.19/bent.egg-info/dependency_links.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)       63 2023-07-20 16:50:13.000000 bent-0.0.19/bent.egg-info/entry_points.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)      203 2023-07-20 16:50:13.000000 bent-0.0.19/bent.egg-info/requires.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)        5 2023-07-20 16:50:13.000000 bent-0.0.19/bent.egg-info/top_level.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)       38 2023-07-20 16:50:13.927462 bent-0.0.19/setup.cfg
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1973 2023-07-20 16:50:05.000000 bent-0.0.19/setup.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    11340 2023-02-03 16:59:19.000000 bent-0.0.9/LICENSE.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    17578 2023-02-03 19:10:35.000000 bent-0.0.9/PKG-INFO
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     3426 2023-02-03 16:59:19.000000 bent-0.0.9/README.rst
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/__init__.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    13167 2023-02-03 16:59:19.000000 bent-0.0.9/bent/annotate.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     1699 2023-02-03 16:59:19.000000 bent-0.0.9/bent/get_data.sh
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     1718 2023-02-03 16:59:19.000000 bent-0.0.9/bent/get_kb_dicts.sh
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)      203 2023-02-03 16:59:19.000000 bent-0.0.9/bent/requirements.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     2351 2023-02-03 16:59:19.000000 bent-0.0.9/bent/setup_package.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1909 2023-02-03 16:59:19.000000 bent-0.0.9/bent/setup_package.sh
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/NILINKER/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/NILINKER/__init__.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    10851 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/NILINKER/nilinker.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1003 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/NILINKER/predict_nilinker.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    13194 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/NILINKER/utils.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/REEL/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/__init__.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    14863 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/candidates.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2866 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/information_content.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2903 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/post_process.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20290 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/ppr_for_ned_all.class
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    39492 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/ppr_for_ned_all.java
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    15702 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/pre_process.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     3314 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/run.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     4303 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/utils.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/__init__.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/abbreviation_detector/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/abbreviation_detector/__init__.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     2541 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/abbreviation_detector/run.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)      284 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/cfg.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     5803 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/classes.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2453 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/nel.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    19947 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/ner.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/setup/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/__init__.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/setup/annotations/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/annotations/__init__.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    12270 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/annotations/dataset_entities.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/setup/kb/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/kb/__init__.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     3719 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/kb/generate_dicts.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    24028 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/kb/kb.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/setup/relation_extraction/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/relation_extraction/__init__.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     8085 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/relation_extraction/dicts.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20061 2023-02-03 19:05:11.000000 bent-0.0.9/bent/src/utils.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent.egg-info/
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    17578 2023-02-03 19:10:34.000000 bent-0.0.9/bent.egg-info/PKG-INFO
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     1180 2023-02-03 19:10:35.000000 bent-0.0.9/bent.egg-info/SOURCES.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)        1 2023-02-03 19:10:34.000000 bent-0.0.9/bent.egg-info/dependency_links.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)      203 2023-02-03 19:10:34.000000 bent-0.0.9/bent.egg-info/requires.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)        5 2023-02-03 19:10:34.000000 bent-0.0.9/bent.egg-info/top_level.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)       38 2023-02-03 19:10:35.000000 bent-0.0.9/setup.cfg
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     2172 2023-02-03 19:10:23.000000 bent-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `bent-0.0.19/LICENSE.txt` & `bent-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bent-0.0.19/PKG-INFO` & `bent-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bent
-Version: 0.0.19
+Version: 0.0.9
 Summary: BENT: Biomedical Entity Annotator
 Home-page: https://github.com/lasigeBioTM/bent
 Author: Pedro Ruas
 Author-email: pedrosimruas@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -219,143 +219,124 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Unix Shell
 Classifier: Programming Language :: Java
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7, <3.10
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 
 
 BENT: Biomedical Entity Annotator
 ---------------------------------
 
 Python Library for Named Entity Recognition (NER) and Linking (NEL) in the biomedical domain.
 
+NER models are based on `PubMedBERT <https://arxiv.org/pdf/2007.15779.pdf>`__ and a post-processing rule-based module.
+the NEL model is a graph-based approach based on the Personalized PageRank algorithm and Information content.
+
 BENT can be used for: 
 
 * Named Entity Recogniton (NER)
 * Named Entity Linking (NEL) 
 * Named Entity Recognition and Linking (NER+NEL)
 
-Access the full `documentation <https://bent.readthedocs.io/en/latest/>`__.
+Access the full documentation `here <https://bent.readthedocs.io/en/latest/>`__.
 
-Citation::
+Citation:
 
-  Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking. 
-  Journal of Biomedical Informatics, 132:104137, 2022. 
-  doi: https://doi.org/10.1016/j.jbi.2022.104137.
+* Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking <https://www.sciencedirect.com/science/article/pii/S1532046422001526>`__. Journal of Biomedical Informatics, 132:104137, 2022. doi: https://doi.org/10.1016/j.jbi.2022.104137.
 
 Installation
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~
 
 To use the current version of BENT it is required: 
 
-*  OS: Ubuntu/Debian 
+* OS based on Ubuntu/Debian 
+* `Conda <https://docs.conda.io/en/latest/>`__ environment 
+* Python>=3.7
+* Between 11 and 15 GB free space (5 GB Anaconda + 2.5 GB to install dependencies + 3.0 GB data or 7.5 GB if you use all available knowlegde bases for NEL)
 
-*  Python 3.7, 3.8 or 3.9
+.. note::
 
-*  Required space between 5.5 GB - 10 GB 
-   * Dependencies: 2.5 GB 
-   * Data: between 3.0 GB (base) or 7.5 GB (if you use all available knowlegde bases for Named Entity Linking)
+   Please ensure that you have the appropriate version of Conda installed.
 
 
-Install the BENT package using pip:
+Create a Conda environment (adapt for the name of your project):
 
 ::
 
-   pip install bent
+   conda create --name annotation_project python=3.7
 
 
-The following knowledge bases can be configured:
+Activate the environment:
 
-* 'medic' (`MEDIC <http://ctdbase.org/>`__)
+::
 
-* 'do' (`Disease ontology <https://disease-ontology.org/>`__)
+   conda activate annotation_project
 
-* 'chebi' (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
-* 'ctd_chem' (`CTD-Chemicals <http://ctdbase.org/>`__)
+Install the BENT package using pip:
 
-* 'ncbi_gene' (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
+::
 
-* 'ctd_gene' (`CTD-GENES <http://ctdbase.org/>`__)
+   pip install bent
 
-* 'ncbi_taxon' (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
-* 'go_bp' (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
+After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Specify the knowledge bases that will be used:
 
-* 'ctd_anat' (`CTD-Anatomy <http://ctdbase.org/>`__)
+::
 
-* 'fma' (`Foundation model of Anatomy <http://sig.biostr.washington.edu/projects/fm/AboutFM.html>`__)
+   python -c "from bent.setup_package import setup_package;setup_package([<kb1>, <kb2>, <kb3>])"
 
-* 'uberon' (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
+Available knowledge bases:
 
-* 'go_cc' (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
+* ‘medic’ (`MEDIC <http://ctdbase.org/>`__)
 
-* 'cell_ontology' (`Cell Ontology <https://cell-ontology.github.io/>`__)
+* ‘do’ (`Disease ontology <https://disease-ontology.org/>`__)
 
-* 'cellosaurus' (`Cellosaurus <https://www.cellosaurus.org/>`__)
+* 'chebi’ (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
+* ‘ctd_chem’ (`CTD-Chemicals <http://ctdbase.org/>`__)
 
-After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Run in the command line:
+* ‘ncbi_gene’ (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
 
-::
+* ‘ctd_gene’ (`CTD-GENES <http://ctdbase.org/>`__)
 
-   bent_setup
+* ‘ncbi_taxon’ (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
+* ‘go_bp’ (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
 
-Only the default knowledge bases 'medic' and 'chebi' will be available at this point.
+* ‘ctd_anat’ (`CTD-Anatomy <http://ctdbase.org/>`__)
 
-To disable annoyng messages in the terminal run:
+* ‘uberon’ (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
 
-::
+* ‘go_cc’ (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
 
-   export TF_CPP_MIN_LOG_LEVEL='3'
+* ‘cell_ontology’ (`Cell Ontology <https://cell-ontology.github.io/>`__)
 
+* cellosaurus’ (`Cellosaurus <https://www.cellosaurus.org/>`__)
 
-You can download more knowledge bases later by specifying the desired knowledge bases among the ones that are available:
+Example to download only the MEDIC vocabulary:
 
 ::
 
-   python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs([<kb1>, <kb2>])"
+   python -c "from bent.setup_package import setup_package;setup_package(['medic'])"
 
 
-Get started
-~~~~~~~~~~~
+If you want to download all knowledge bases, choose the option 'all':
 
-To apply the complete pipeline of entity extraction (NER+NEL) set the arguments:
+::
 
-* **recognize**: indicate that the NER module will be applied ('True')
-* **link**: indicate that the NEL module will be applied ('True')
-* **types**: entity types to recognize and the respective target knowledge bases.
-* **in_dir**: directory path containing the text files to be annotated (the directory must contain text files exclusively)
-* **out_dir**: the output directory that will contain the annotation files
+   python -c "from bent.setup_package import setup_package;setup_package(['all'])"
 
 
-Example:
+You can download more knowledge bases later by running the same command and specifying the desired knolwedge bases among the ones that are available and setting the argument ' only_kb_dicts' to True:
 
 ::
 
-   import bent.annotate as bt
-
-   bt.annotate(
-           recognize=True,
-           link=True,
-           types={
-            'disease': 'medic'
-            'chemical': 'chebi',
-            'gene': 'ncbi_gene',
-            'anatomical': 'uberon',
-            'cell_line': 'cellosaurus',
-            'bioprocess': 'go_bp'
-            },
-           in_dir='input/txt/',
-           out_dir='output/nel/'
-   )
-
+   python -c "from bent.setup_package import setup_package;setup_package([<kb>],  only_kb_dicts=True)"
 
-It is also possible to apply the pipeline (NER+NEL) to a string or a list or strings instantiated in the execution script.
 
-To see more usage examples, access the `documentation <https://bent.readthedocs.io/en/latest/usage.html>`__.
+Reinitiate the conda environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bent-0.0.19/README.rst` & `bent-0.0.9/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,114 @@
 
 
 BENT: Biomedical Entity Annotator
 ---------------------------------
 
 Python Library for Named Entity Recognition (NER) and Linking (NEL) in the biomedical domain.
 
+NER models are based on `PubMedBERT <https://arxiv.org/pdf/2007.15779.pdf>`__ and a post-processing rule-based module.
+the NEL model is a graph-based approach based on the Personalized PageRank algorithm and Information content.
+
 BENT can be used for: 
 
 * Named Entity Recogniton (NER)
 * Named Entity Linking (NEL) 
 * Named Entity Recognition and Linking (NER+NEL)
 
-Access the full `documentation <https://bent.readthedocs.io/en/latest/>`__.
+Access the full documentation `here <https://bent.readthedocs.io/en/latest/>`__.
 
-Citation::
+Citation:
 
-  Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking. 
-  Journal of Biomedical Informatics, 132:104137, 2022. 
-  doi: https://doi.org/10.1016/j.jbi.2022.104137.
+* Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking <https://www.sciencedirect.com/science/article/pii/S1532046422001526>`__. Journal of Biomedical Informatics, 132:104137, 2022. doi: https://doi.org/10.1016/j.jbi.2022.104137.
 
 Installation
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~
 
 To use the current version of BENT it is required: 
 
-*  OS: Ubuntu/Debian 
+* OS based on Ubuntu/Debian 
+* `Conda <https://docs.conda.io/en/latest/>`__ environment 
+* Python>=3.7
+* Between 11 and 15 GB free space (5 GB Anaconda + 2.5 GB to install dependencies + 3.0 GB data or 7.5 GB if you use all available knowlegde bases for NEL)
 
-*  Python 3.7, 3.8 or 3.9
+.. note::
 
-*  Required space between 5.5 GB - 10 GB 
-   * Dependencies: 2.5 GB 
-   * Data: between 3.0 GB (base) or 7.5 GB (if you use all available knowlegde bases for Named Entity Linking)
+   Please ensure that you have the appropriate version of Conda installed.
 
 
-Install the BENT package using pip:
+Create a Conda environment (adapt for the name of your project):
 
 ::
 
-   pip install bent
+   conda create --name annotation_project python=3.7
 
 
-The following knowledge bases can be configured:
+Activate the environment:
 
-* 'medic' (`MEDIC <http://ctdbase.org/>`__)
+::
 
-* 'do' (`Disease ontology <https://disease-ontology.org/>`__)
+   conda activate annotation_project
 
-* 'chebi' (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
-* 'ctd_chem' (`CTD-Chemicals <http://ctdbase.org/>`__)
+Install the BENT package using pip:
 
-* 'ncbi_gene' (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
+::
 
-* 'ctd_gene' (`CTD-GENES <http://ctdbase.org/>`__)
+   pip install bent
 
-* 'ncbi_taxon' (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
-* 'go_bp' (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
+After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Specify the knowledge bases that will be used:
 
-* 'ctd_anat' (`CTD-Anatomy <http://ctdbase.org/>`__)
+::
 
-* 'fma' (`Foundation model of Anatomy <http://sig.biostr.washington.edu/projects/fm/AboutFM.html>`__)
+   python -c "from bent.setup_package import setup_package;setup_package([<kb1>, <kb2>, <kb3>])"
 
-* 'uberon' (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
+Available knowledge bases:
 
-* 'go_cc' (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
+* ‘medic’ (`MEDIC <http://ctdbase.org/>`__)
 
-* 'cell_ontology' (`Cell Ontology <https://cell-ontology.github.io/>`__)
+* ‘do’ (`Disease ontology <https://disease-ontology.org/>`__)
 
-* 'cellosaurus' (`Cellosaurus <https://www.cellosaurus.org/>`__)
+* 'chebi’ (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
+* ‘ctd_chem’ (`CTD-Chemicals <http://ctdbase.org/>`__)
 
-After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Run in the command line:
+* ‘ncbi_gene’ (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
 
-::
+* ‘ctd_gene’ (`CTD-GENES <http://ctdbase.org/>`__)
 
-   bent_setup
+* ‘ncbi_taxon’ (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
+* ‘go_bp’ (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
 
-Only the default knowledge bases 'medic' and 'chebi' will be available at this point.
+* ‘ctd_anat’ (`CTD-Anatomy <http://ctdbase.org/>`__)
 
-To disable annoyng messages in the terminal run:
+* ‘uberon’ (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
 
-::
+* ‘go_cc’ (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
 
-   export TF_CPP_MIN_LOG_LEVEL='3'
+* ‘cell_ontology’ (`Cell Ontology <https://cell-ontology.github.io/>`__)
 
+* cellosaurus’ (`Cellosaurus <https://www.cellosaurus.org/>`__)
 
-You can download more knowledge bases later by specifying the desired knowledge bases among the ones that are available:
+Example to download only the MEDIC vocabulary:
 
 ::
 
-   python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs([<kb1>, <kb2>])"
+   python -c "from bent.setup_package import setup_package;setup_package(['medic'])"
 
 
-Get started
-~~~~~~~~~~~
+If you want to download all knowledge bases, choose the option 'all':
 
-To apply the complete pipeline of entity extraction (NER+NEL) set the arguments:
+::
 
-* **recognize**: indicate that the NER module will be applied ('True')
-* **link**: indicate that the NEL module will be applied ('True')
-* **types**: entity types to recognize and the respective target knowledge bases.
-* **in_dir**: directory path containing the text files to be annotated (the directory must contain text files exclusively)
-* **out_dir**: the output directory that will contain the annotation files
+   python -c "from bent.setup_package import setup_package;setup_package(['all'])"
 
 
-Example:
+You can download more knowledge bases later by running the same command and specifying the desired knolwedge bases among the ones that are available and setting the argument ' only_kb_dicts' to True:
 
 ::
 
-   import bent.annotate as bt
-
-   bt.annotate(
-           recognize=True,
-           link=True,
-           types={
-            'disease': 'medic'
-            'chemical': 'chebi',
-            'gene': 'ncbi_gene',
-            'anatomical': 'uberon',
-            'cell_line': 'cellosaurus',
-            'bioprocess': 'go_bp'
-            },
-           in_dir='input/txt/',
-           out_dir='output/nel/'
-   )
-
+   python -c "from bent.setup_package import setup_package;setup_package([<kb>],  only_kb_dicts=True)"
 
-It is also possible to apply the pipeline (NER+NEL) to a string or a list or strings instantiated in the execution script.
 
-To see more usage examples, access the `documentation <https://bent.readthedocs.io/en/latest/usage.html>`__.
+Reinitiate the conda environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bent-0.0.19/bent/annotate.py` & `bent-0.0.9/bent/annotate.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,38 +4,36 @@
 import string
 import spacy
 from tqdm import tqdm
 import bent.src.utils as utils
 from bent.src.ner import ner
 from bent.src.nel import nel
 from bent.src.classes import Dataset
-import bent.src.cfg as cfg
 
 
-def recognizer(
-        in_dir, entity_types, out_dir, ner_model, run_id, 
-        return_dataset=False, input_tmp=False):
+def recognizer(in_dir, input_text, entity_types, out_dir, ner_model, run_id):
     """Pipeline to perform Named Entity Recognition. For each input 
     document/text it outputs either an annotations file (BRAT format) or a 
     Dataset object including all documents and respective annotations.
 
     :param in_dir: path to directory containing text files to be annotated, 
         defaults to None
     :type in_dir: _type_, optional
+    :param input_text: text string or list of text strings (each element 
+        represinting a different document) to be annotated, defaults to None
+    :type input_text: str or list, optional
     :param types: the entity types that will be recognized 
         :type types: list
     :param out_dir: path to directory where the output of the pipeline will be
         located, optional. If 'out_dir' == None (deafult) a Dataset object 
         including all documents and respective annotations will be returned  
     :type out_dir: str, defaults to None
     :param ner_model: the Named Entity Recognition model that will be used, 
         defaults to 'pubmedbert'
     :type ner_model: str, optional
-    :param input_tmp: indicates if the input is composed of temporary text files. 
-    :type input_tmp: bool
     :return: dataset (an object including all the input texts along with the 
         annotations) if 'out_dir' is None; an annotation file for each inputed
         text if 'out_dir' is different that None
     :rtype: Dataset object, text file(s)
     """
     
     # Disable printing of annoying messages
@@ -44,57 +42,84 @@
     # Spacy language model to segment the inputed texts into sentences 
     lang_model = spacy.load('en_core_sci_lg')
     stopwords = lang_model.Defaults.stop_words
     
     # Load the NER models that will be used
     recognizer = ner(ner_model, entity_types, stopwords)
 
-    # Whether the input is a directory with text files or not
+    # Wether the input is a directory with text files or not
+    filename_mode = False 
+
     dataset = Dataset()
 
-    assert in_dir != None, 'Invalid "in_dir"!'
+    if out_dir == None:
+        # In this case a dataset object will be outputted and the 
+        # temporary annotation files will be stored in 'tmp/NER/' directory
+        tmp_out_dir = '.tmp/{}/'.format(run_id)
+        os.mkdir(tmp_out_dir)
 
     if recognizer.model_type == "bert":  
-        input_files = [
-            '{}{}'.format(in_dir, filename) for filename in os.listdir(in_dir)]    
+        input_files = None
+
+        if in_dir != None:
+            filename_mode = True
+            input_files = [
+                in_dir + filename for filename in os.listdir(in_dir)]
+            
+        elif input_text != None:
+            
+            if type(input_text) == str:
+                input_files = [input_text]
+            
+            elif type(input_text) == list:
+                input_files = input_text
 
         # Recognize entities in each document
         pbar = tqdm(total=len(input_files), colour= 'green', 
             desc='Recognizing entities (documents)')
         
-        for i, filename in enumerate(input_files, start=1):
+        for i, filename in enumerate(input_files):
             doc_id = ''
-
-            if input_tmp:
-                doc_id = 'doc_{}'.format(str(i))
-                
-            else:
-                doc_id = filename.strip(in_dir).strip('.txt')
-
             text = ''
-
-            with open(filename, 'r') as input_file:
-                text = input_file.read()
-                input_file.close()
+            
+            if filename_mode:
+                doc_id = filename.strip(in_dir).strip('.txt')
+               
+                with open(filename, 'r') as input_file:
+                    text = input_file.read()
+                    input_file.close()
+            
+            else:
+                text = filename
+                doc_id = str(i)
             
             # Sentence segmentation
             doc_sentences = utils.sentence_splitter(text, lang_model)
             
             # Objectify input
-            doc_obj = utils.objectify_ner_input(doc_id, text, doc_sentences)
+            doc_obj = utils.objectify_ner_input(
+                doc_id, text, doc_sentences)
             
             # Apply NER models to input text
             doc_entities = recognizer.apply(doc_obj)
 
             # Output recognized entities to a file
             # Prepare output string with annotations
             doc_annots = utils.prepare_output_from_objects(
                 doc_entities, only_ner=True)
-       
-            out_filename = '{}{}.ann'.format(out_dir, doc_id)
+
+            out_filename = ''
+
+            if out_dir == None:
+                out_filename = '{}{}.ann'.format(tmp_out_dir, doc_id)                
+                # Add Document object to Dataset object
+                dataset.add_doc(doc_entities)
+
+            else:
+                out_filename = out_dir + doc_id + '.ann'
 
             with open(out_filename, 'w') as out_file:
                 out_file.write(doc_annots[:-1])
                 out_file.close()
             
             del doc_annots
             del text
@@ -109,21 +134,21 @@
         pbar.close()
 
     del recognizer
     del lang_model
     del stopwords
     utils.garbage_collect()
 
-    if return_dataset:
+    if out_dir == None:
         return dataset
 
 
 def linker(
             recognize, types, nel_model, run_id, out_format=None, 
-            ner_dir=None, out_dir=None, dataset=None, return_dataset=False):
+            ner_dir=None, out_dir=None, dataset=None):
     """Pipeline to perform Named Entity Linking. For each input 
     annotation files with recognized entities it outputs an updated 
     annotations file (BRAT format) with knowledge base identifiers for each
     entity.
 
     :param recognize: specifies wether the pipeline performs Named Entity 
         Recognition, defaults to False
@@ -158,36 +183,42 @@
     :raises ValueError: if 'ner_dir'==None and recognize==False, which means
         that if the NER stage was not performed it is necessary nevertheless
         indicate the directory containing annotation files corresponding to 
         the NER output
     """
     
     # Link the recognized/inputted entities to the specified KBs
-    linker = nel(nel_model, run_id)
+    linker = nel(nel_model)
     target_kbs = {}
     
     for ent_type in types.keys():
         
         if types[ent_type] != '':
             target_kbs[ent_type] = types[ent_type]
     
     if recognize:
-        ner_dir = out_dir
+        
+        if out_dir == None:
+            ner_dir = '.tmp/{}/'.format(run_id)
+        
+        else:
+            # The output of the previous NER step is locacted in the out_dir
+            ner_dir = out_dir
     
     else:
 
         if ner_dir == None and run_id==None:
             raise ValueError('It is necessary to specify the directory \
                 containing the NER output ("ner_dir")')
     
     nel_run_ids = linker.apply(target_kbs, ner_dir=ner_dir)
     
     del linker
     
-    if return_dataset:
+    if out_dir == None:
         return utils.update_dataset_with_nel_output(dataset, nel_run_ids)
     
     else:
         utils.update_ner_file_with_nel_output(ner_dir, nel_run_ids, out_dir=out_dir)  
 
 
 def annotate(recognize=False, link=False, types={}, input_text=None,
@@ -248,102 +279,60 @@
     :return: dataset (an object including all the input texts along with the 
         annotations) if 'out_dir' is None; an annotation file for each inputed
         text if 'out_dir' is different that None
     :rtype: Dataset object, text file(s)
     """
     run_id = ''.join(random.choices(string.ascii_uppercase + string.digits, 
         k=15)) 
-    
-    os.mkdir(cfg.tmp_dir + run_id)
 
     # Check if input arguments are valid
     utils.check_input_args(recognize, link, types, input_format,
         input_text, in_dir, ner_dir, out_dir, ner_model, nel_model)
 
     if ner_dir != None:
-        # There are already files with NER annotations in the 'ner_dir'
         in_dir = ner_dir
     
     if out_dir != None:
         
         if not os.path.exists(out_dir):
             os.mkdir(out_dir)
     
-    
-
     #--------------------------------------------------------------------------
     #                   CONVERT INPUT TO THE BRAT FORMAT
     #-------------------------------------------------------------------------- 
-    input_tmp = False
-
     if input_text!= None:
-        # The input is either a string or a list of strings, so there is no 
-        # 'in_dir'.
-        # A temporary directory to store the text files will be created        
-        in_dir = '.tmp/'
-    
-        if not os.path.exists(in_dir):
-            os.mkdir(in_dir)
-
-        in_dir = '.tmp/{}/'.format(run_id)
-
-        if not os.path.exists(in_dir):
-            os.mkdir(in_dir)
-
-        in_dir = '{}txt/'.format(in_dir)
         
-        if not os.path.exists(in_dir):
-            os.mkdir(in_dir)
+        utils.convert_input_files(input_format, input_text=input_text, 
+            in_dir=in_dir, recognize=recognize)
         
-        utils.convert_input_files(
-            input_format, in_dir=in_dir, input_text=input_text, 
-            recognize=recognize)
-
-        input_tmp = True
+        in_dir += 'brat/'
         
     #--------------------------------------------------------------------------
     #                           NER
     #--------------------------------------------------------------------------
     if recognize:
         entity_types = types.keys()
 
         if out_dir != None:
             recognizer(
-                in_dir, entity_types, out_dir, ner_model, run_id, input_tmp=input_tmp)
+                in_dir, input_text, entity_types, out_dir, ner_model, run_id)
         
-        
-        elif out_dir == None:
-            # In this case a dataset object will be outputted and the 
-            # temporary annotation files will be stored in 'tmp/NER/' directory
-            tmp_out_dir = '{}ann/'.format(in_dir)
-            
-            if not os.path.exists(tmp_out_dir):
-                os.mkdir(tmp_out_dir)
-            
+        else:
             dataset = recognizer(
-                in_dir, entity_types, tmp_out_dir, ner_model, 
-                run_id, return_dataset=True, input_tmp=input_tmp)
-
-            if link:
-                # The input dir for the NEL module now is the directory 
-                # containing the annotation files outputted by the NER module
-                in_dir = tmp_out_dir
-    
+                in_dir, input_text, entity_types, out_dir, ner_model, run_id)
     #--------------------------------------------------------------------------
     #                           NEL
     #--------------------------------------------------------------------------
     if link:
 
         if out_dir != None:
-            # Annotation files with NER+NEL output will be created in 'out_dir'
             linker(
                 recognize, types, nel_model, run_id, out_format=out_format,
-                    ner_dir=in_dir, out_dir=out_dir)
+                    ner_dir=in_dir, 
+                out_dir=out_dir)
 
         else:
-            # A Dataset object will be returned containing NER+NEL output
             dataset = linker(
                 recognize, types, nel_model, run_id, out_format=out_format, 
-                ner_dir=in_dir, dataset=dataset, out_dir=tmp_out_dir,
-                return_dataset=True)
+                ner_dir=in_dir, dataset=dataset, out_dir=out_dir)
             
             return dataset
```

### Comparing `bent-0.0.19/bent/get_kb_dicts.sh` & `bent-0.0.9/bent/get_kb_dicts.sh`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 #!/bin/bash
 
-root_path=$(python - <<END
-import pkg_resources
-package = pkg_resources.get_distribution('bent')
-print(package.location)
-END
-)
-
-package_path="${root_path}/bent"
-
-cd ${package_path}/data/kbs/dicts/
+cd ../data/kb_dicts/dicts/
 
 target_kb=$1
 
 if [ $target_kb = 'medic' ]
 then
     download_url='https://drive.google.com/uc?id=1Q0SYp0NBOEg5hUUS-Gu1tdBfQvJx5Wax'
 
 elif [ $target_kb = 'cellosaurus' ]
 then
-    download_url='https://drive.google.com/uc?id=1M2KSW0w8l0KXcmdntgdslxOwV8kturvh'
+    download_url='https://drive.google.com/uc?id=1hb_MVEApaivEyU3eaziX1jj9uAqyoLqt'
 
 elif [ $target_kb = 'chebi' ]
 then
     download_url='https://drive.google.com/uc?id=1Var1gzVrKghH07NWdPFC2re-AgSZaIFD'
 
 elif [ $target_kb = 'cl' ]
 then
@@ -68,8 +59,8 @@
 fi
 
 gdown $download_url
 tar -xvf $target_kb.tar.gz
 rm $target_kb.tar.gz
 
 
-cd ../../
+cd ../../../
```

### Comparing `bent-0.0.19/bent/src/NILINKER/nilinker.py` & `bent-0.0.9/bent/src/NILINKER/nilinker.py`

 * *Files identical despite different names*

### Comparing `bent-0.0.19/bent/src/NILINKER/predict_nilinker.py` & `bent-0.0.9/bent/src/NILINKER/predict_nilinker.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     :rtype: tf.keras.Model() object 
     """
 
     word_embeds, candidate_embeds, wc, embeds_word2id = get_wc_embeds(partition)
     params = [200, wc.candidate_num, top_k]
     id_to_name = get_kb_data(partition)
     
-    model_dir = "{}/data/NILINKER/nilinker_files/{}/train/".format(cfg.root_path, partition)
+    model_dir = "{}data/NILINKER/nilinker_files/{}/train/".format(cfg.root_path, partition)
     
     model = Nilinker(
         word_embeds, candidate_embeds, params, wc, id_to_name, embeds_word2id)
     model.compile(run_eagerly = True)
     model.built = True
     model.load_weights(model_dir + "best.h5")
```

### Comparing `bent-0.0.19/bent/src/NILINKER/utils.py` & `bent-0.0.9/bent/src/NILINKER/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     
     __slots__ = ['partition', 'filepath', 'word2candidates', 'word2id',
         'id2word', 'candidate_num', 'candidate2id', 'id2candidate', 
         'root_concept_int' ]
     def __init__(self, partition):
     
         self.partition = partition
-        self.filepath = "{}/data/NILINKER/word_concept/wc_{}.json".format(cfg.root_path, partition)
+        self.filepath = "{}data/NILINKER/word_concept/wc_{}.json".format(cfg.root_path, partition)
         self.word2candidates = None
         self.word2id = None
         self.id2word = None
         self.candidate_num = None
         self.candidate2id = None
         self.id2candidate = None
         self.root_concept_int = None
@@ -31,15 +31,15 @@
         """Fill a WordConcept object with info about words belonging to 
         the considered Word-Concept (WC) dict, and candidates and respectives 
         int ids. (*note: Candidate int ids are distinct from WC words ids). 
         """
 
         # Load node_id_to_int
         with open(
-                "{}/data/NILINKER/embeddings/{}/node_id_to_int_{}.json"\
+                "{}data/NILINKER/embeddings/{}/node_id_to_int_{}.json"\
                 .format(cfg.root_path, self.partition, self.partition)) as in_file:
             node_id_to_int = json.loads(in_file.read())
 
         # Create candidate2id and id2candidate
         id2candidate, candidate2id = {}, {}
         
         for concept in node_id_to_int.keys():
@@ -248,15 +248,15 @@
     :param partition: has value 'medic', 'ctd_chem', 'hp', 'chebi', 'go_bp', 
         'ctd_anat'
     :type partition: str
     :return: word_embeds, candidate_embeds, wc
     :rtype: Numpy array, Numpy array, WordConcept object
     """
 
-    embeds_dir = "{}/data/NILINKER/embeddings/{}/".format(cfg.root_path, partition)
+    embeds_dir = "{}data/NILINKER/embeddings/{}/".format(cfg.root_path, partition)
     word_embeds_filepath = embeds_dir 
     candidates_embeds_filepath = embeds_dir + partition + ".emb"
 
     wc = WordConcept(partition)
     wc.build()
 
     word_embeds, embeds_word2id = load_word_embeds(word_embeds_filepath)
@@ -374,18 +374,18 @@
     :param partition: has value 'medic', 'ctd_chem', 'hp', 'chebi', 
         'go_bp' or 'ctd_anat'
     :type partition: str
     :return: kb_data representing the given KB
     :rtype: KnowledgeBase object
     """
 
-    source_filename = '{}/data/kbs/dicts/{}/id_to_name.json'.format(cfg.root_path, partition)
+    source_filename = '{}data/dicts/{}/id_to_name.json'.format(cfg.root_path, partition)
 
     if partition == 'chebi':
-        source_filename = '{}/data/kbs/dicts/chebi/id_to_name_nilinker.json'.format(cfg.root_path)
+        source_filename = '{}data/dicts/chebi/id_to_name_nilinker.json'.format(cfg.root_path)
 
     with open(source_filename, 'r') as in_file:
         id_to_name = json.loads(in_file.read()) 
         in_file.close()
 
     # Format the KB identifiers (MESH:D019967 passa a MESH_D019967)
     id_to_name_up = {}
```

### Comparing `bent-0.0.19/bent/src/REEL/candidates.py` & `bent-0.0.9/bent/src/REEL/candidates.py`

 * *Files identical despite different names*

### Comparing `bent-0.0.19/bent/src/REEL/information_content.py` & `bent-0.0.9/bent/src/REEL/information_content.py`

 * *Files identical despite different names*

### Comparing `bent-0.0.19/bent/src/REEL/post_process.py` & `bent-0.0.9/bent/src/REEL/post_process.py`

 * *Files identical despite different names*

### Comparing `bent-0.0.19/bent/src/REEL/ppr_for_ned_all.class` & `bent-0.0.9/bent/src/REEL/ppr_for_ned_all.class`

 * *Files identical despite different names*

### Comparing `bent-0.0.19/bent/src/REEL/ppr_for_ned_all.java` & `bent-0.0.9/bent/src/REEL/ppr_for_ned_all.java`

 * *Files identical despite different names*

### Comparing `bent-0.0.19/bent/src/REEL/pre_process.py` & `bent-0.0.9/bent/src/REEL/pre_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,17 @@
     """
     
     doc_count = 0
     changed_cache_final = False
     kb_cache_up = None
     names = set(name_to_id.keys())
     synonyms = set(synonym_to_id.keys())
-    ner_out_docs = os.listdir(ner_dir)
 
+    ner_out_docs = os.listdir(ner_dir)
+    
     for doc in ner_out_docs:
         ner_annots = None
         doc_id = doc.strip('.ann')
 
         with open(ner_dir + doc, 'r') as ner_doc:
             ner_annots = ner_doc.readlines()
             ner_doc.close()
@@ -255,15 +256,15 @@
     #-------------------------------------------------------------------------
     #                            Import KB info
     #-------------------------------------------------------------------------
 
     # Load preprocessed dicts
     name_to_id = {}
     synonym_to_id = {}
-    kb_dicts_dir = '{}/data/kbs/dicts/{}/'.format(cfg.root_path, kb) 
+    kb_dicts_dir = '{}data/dicts/{}/'.format(cfg.root_path, kb) 
     
     with open(kb_dicts_dir + 'name_to_id.json', 'r') as dict_file:
         name_to_id = json.loads(dict_file.read())
         dict_file.close()
 
     synonyms_filepath = kb_dicts_dir + 'synonym_to_id_full.json'
 
@@ -311,15 +312,15 @@
     
     #-------------------------------------------------------------------------
     #            Import relations to add to the disambiguation graphs
     #-------------------------------------------------------------------------
     extracted_relations = {}
     
     if link_mode == 'corpus' or link_mode == 'kb_corpus': 
-        relations_dir = '{}/data/relations/'.format(cfg.root_path)
+        relations_dir = '{}data/relations/'.format(cfg.root_path)
         rel_filenames = os.listdir(relations_dir)    
         rel_filename = '{}_{}_relations.json'.format(entity_type, kb)
 
         if rel_filename in rel_filenames:
 
             with open(relations_dir + rel_filename, 'r') as rel_file:
                 extracted_relations = json.loads(rel_file.read())
```

### Comparing `bent-0.0.19/bent/src/REEL/run.py` & `bent-0.0.9/bent/src/REEL/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 
 import bent.src.cfg as cfg
 import os
+import random
+import string
 from bent.src.REEL.pre_process import pre_process
 from bent.src.REEL.post_process import process_results
 
 
-def run(run_id, ner_dir, kb, entity_type, abbreviations):
+def run(ner_dir, kb, entity_type, abbreviations):
     """Apply the REEL model (preprocess, candidate scoring with PPR, 
     postprocess) to the entities present in files in ner_dir.
 
     :param ner_dir: path to directory where the recognized entities are
         stored in the annotations files
     :type ner_dir: str
     :param kb: target knowledge base
@@ -22,15 +24,17 @@
     :type abbreviations: dict
     :return: nel_run_id representing the identifier of the current run of REEL.
         The results of the run will be located in the directory 
         'tmp/REEL/results/<run_id/>'.
     :rtype: str
     """
 
-    nel_run_name = '{}/{}'.format(run_id, entity_type)
+    nel_run_id = ''.join(random.choices(string.ascii_uppercase + string.digits, 
+        k=15))
+    nel_run_name = nel_run_id + '_' + entity_type
 
     # Use relations extracted from external corpora and relations described in 
     # the targer knowledge base
     link_mode='kb_corpus' 
 
     # Use NILINKER model if available
     nil_mode = 'none'
@@ -53,17 +57,17 @@
     #         Builds a disambiguation graph from each candidates file:            
     #         the nodes are the candidates and relations are added                
     #         according to candidate link_mode. After the disambiguation          
     #         graph is built, it runs the PPR algorithm over the graph            
     #         and ranks each candidate.                                           
     #------------------------------------------------------------------------#
     if kb != 'ncbi_gene':
-        ppr_dir = '{}/src/REEL/'.format(cfg.root_path)
+        ppr_filepath = '{}scripts/'.format(cfg.root_path)
         comm = 'java -classpath :{} ppr_for_ned_all {} ppr_ic'.\
-            format(ppr_dir, nel_run_name)
+            format(ppr_filepath, nel_run_name)
         os.system(comm)
 
     #------------------------------------------------------------------------#
     #                         REEL: Post-processing                                                                      
     #------------------------------------------------------------------------# 
     process_results(nel_run_name, entity_type, kb)
```

### Comparing `bent-0.0.19/bent/src/abbreviation_detector/run.py` & `bent-0.0.9/bent/src/abbreviation_detector/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     :rtype: dict
     """
 
     filepaths = [file for file in os.listdir(input_dir)]
 
     # change to Ab3P directory
     cwd = os.getcwd()
-    os.chdir(cfg.root_path + '/abbreviation_detector/Ab3P/')
+    os.chdir(cfg.root_path + 'scripts/abbreviation_detector/Ab3P/')
 
     if not os.path.exists('tmp/'):
         os.mkdir('tmp/')
 
     # Run Ab3P for each text file
     for filepath in filepaths:
         doc_id = ''
```

### Comparing `bent-0.0.19/bent/src/build/annotations/dataset_entities.py` & `bent-0.0.9/bent/src/setup/annotations/dataset_entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,16 +344,16 @@
 
     with open(out_filename, 'w') as out_file:
         out_file.write(output)
         out_file.close()
 
 
 def generate_annotation_dicts():
-    corpora_dir = cfg.root_path + '/data/datasets/'
-    dicts_dir = cfg.root_path + '/data/kbs/dicts/'
+    corpora_dir = cfg.root_path + 'data/datasets/'
+    dicts_dir = cfg.root_path + 'data/kbs/dicts/'
 
     kbs = ['ncbi_taxon', 'medic', 'ctd_chem', 'chebi', 'go_bp', 'ncbi_gene',
         'go_cc', 'cl', 'uberon']
     #kbs = ['medic']
 
     for kb in kbs:
         build_annotations_dict(corpora_dir, dicts_dir, kb)
```

### Comparing `bent-0.0.19/bent/src/build/kb/generate_dicts.py` & `bent-0.0.9/bent/src/setup/kb/generate_dicts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import bent.src.cfg as cfg
 import orjson as json
 import os
-from bent.src.build.kb.kb import KnowledgeBase
+from bent.src.setup.kb.kb import KnowledgeBase
 
-dict_dir = cfg.root_path + '/data/kbs/dicts/'
+dict_dir = cfg.root_path + 'data/dicts/'
 
 
 def generate_dicts_4_kb(kb=None, mode='reel', terms_filename=None, 
         edges_filename=None, kb_filename=None, input_format=None):
     
     out_dir = dict_dir + kb
```

### Comparing `bent-0.0.19/bent/src/build/kb/kb.py` & `bent-0.0.9/bent/src/setup/kb/kb.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 objects (dictionaries and Networkx graph)."""
 
 import csv
 import networkx as nx
 import obonet
 import bent.src.cfg as cfg
 
-data_dir = cfg.root_path + '/data/kbs/original_files/'
+data_dir = cfg.root_path + 'data/kbs/original_files/'
 
 
 class KnowledgeBase:
     """Represents a knowledge base that is loaded from a given local file."""
 
     def __init__(self, kb, mode, terms_filename=None, edges_filename=None, 
             kb_filename=None, input_format=None):
```

### Comparing `bent-0.0.19/bent/src/build/relation_extraction/dicts.py` & `bent-0.0.9/bent/src/setup/relation_extraction/dicts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 
 # Build dictionaries of extracted relations to further inclusion in the NEL module
 import bent.src.cfg as cfg
 import json
-#import pandas as pd
+import pandas as pd
 
-datasets_dir = cfg.root_path + '/data/datasets/'
-relations_dir = cfg.root_path + '/data/relations/'
+datasets_dir = cfg.root_path + 'data/datasets/'
+relations_dir = cfg.root_path + 'data/relations/'
 
 
 def update_dict(id1, id2, relations):
 
     if id1 not in relations:
         relations[id1] = [id2]
```

### Comparing `bent-0.0.19/bent/src/classes.py` & `bent-0.0.9/bent/src/classes.py`

 * *Files identical despite different names*

### Comparing `bent-0.0.19/bent/src/nel.py` & `bent-0.0.9/bent/src/nel.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from bent.src.abbreviation_detector.run import run_Ab3P
 from bent.src.REEL.run import run
 from tqdm import tqdm
 
 
 class nel():
     """Represent a Named Entity Linking (NEL) pipeline"""
-    __slots__ = ['model', 'run_id']
-    def __init__(self, model, run_id):
+    __slots__ = ['model']
+    def __init__(self, model):
         self.model = model
-        self.run_id = run_id
     
     def apply(self, target_kbs, ner_dir=None):
         """Link or normalise input entities to target knwoledge bases using 
         the previously specified model.
 
         :param in_dir: path to the directory including the texts of the 
             documents where the entities were recognized
@@ -45,15 +44,15 @@
             # ----------------------------------------------------------------
             #Sequentially link entities to the respective target knowledge base
             # ----------------------------------------------------------------
             for ent_type in target_kbs.keys():
                 kb = target_kbs[ent_type]
                 
                 # Run REEL
-                nel_run_name = run(self.run_id, ner_dir, kb, ent_type, abbreviations)
+                nel_run_name = run(ner_dir, kb, ent_type, abbreviations)
                 nel_runs.append(nel_run_name)
                 
                 pbar.update(1)
             
             pbar.close()
         
         else:
```

### Comparing `bent-0.0.19/bent/src/ner.py` & `bent-0.0.9/bent/src/ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,87 +41,77 @@
         if self.name == 'pubmedbert':
             self.model_type = 'bert'
             
             if 'disease' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Disease"
                 self.models['disease'] = ner.load_transformer_model(model_name)
                 dict_filename = '{}data/overlapping_entities/disease.json'.format(module_root_path)
-                
                 if len(types) > 1:
                     self.disease_prob = ner.load_probabilities_file(dict_filename)
                 
             if 'chemical' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Chemical"
                 self.models['chemical'] = ner.load_transformer_model(model_name)
                 dict_filename = '{}data/overlapping_entities/chemical.json'.format(module_root_path)
-                
                 if len(types) > 1:
                     self.chemical_prob = ner.load_probabilities_file(dict_filename)
            
             if 'gene' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Gene"
                 self.models['gene'] = ner.load_transformer_model(model_name)
                 dict_filename = '{}/data/overlapping_entities/gene.json'.format(module_root_path)
-                
                 if len(types) > 1:
                     self.gene_prob = ner.load_probabilities_file(dict_filename)
 
             if 'organism' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Organism"
                 self.models['organism'] = ner.load_transformer_model(model_name)
                 dict_filename = '{}data/overlapping_entities/organism.json'.format(module_root_path)
-                
                 if len(types) > 1:    
                     self.organism_prob = ner.load_probabilities_file(dict_filename)
 
             if 'bioprocess' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Bioprocess"
                 self.models['bioprocess'] = ner.load_transformer_model(model_name)   
                 dict_filename = '{}data/overlapping_entities/bioprocess.json'.format(module_root_path)
-                
                 if len(types) > 1:    
                     self.bioprocess_prob = ner.load_probabilities_file(dict_filename)
 
             if 'anatomical' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Anatomical"
                 self.models['anatomical'] = ner.load_transformer_model(model_name)   
                 dict_filename = '{}data/overlapping_entities/anatomical.json'.format(module_root_path)
-                
                 if len(types) > 1:    
                     self.anatomical_prob = ner.load_probabilities_file(dict_filename)
             
             if 'cell_component' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Cell-Component"
                 self.models['cell_component'] = ner.load_transformer_model(model_name)   
                 dict_filename = '{}data/overlapping_entities/cell_component.json'.format(module_root_path)
-                
                 if len(types) > 1:    
                     self.cell_component_prob = ner.load_probabilities_file(dict_filename)
             
             if 'cell_line' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Cell-Line"
                 self.models['cell_line'] = ner.load_transformer_model(model_name)   
                 dict_filename = '{}data/overlapping_entities/cell_line.json'.format(module_root_path)
-                
                 if len(types) > 1:    
                     self.cell_line_prob = ner.load_probabilities_file(dict_filename)
             
             if 'cell_type' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Cell-Type"
                 self.models['cell_type'] = ner.load_transformer_model(model_name)   
                 dict_filename = '{}data/overlapping_entities/cell_type.json'.format(module_root_path)
-                
                 if len(types) > 1:    
                     self.cell_type_prob = ner.load_probabilities_file(dict_filename)
 
             if 'variant' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Variant"
                 self.models['variant'] = ner.load_transformer_model(model_name)   
                 dict_filename = '{}data/overlapping_entities/variant.json'.format(module_root_path)
-                
                 if len(types) > 1:    
                     self.variant_prob = ner.load_probabilities_file(dict_filename)  
         
         else:
             raise ValueError('Model not implemented!')
 
     @staticmethod
@@ -139,15 +129,17 @@
         
         model = AutoModelForTokenClassification.from_pretrained(model_filepath)
         tokenizer_1 = AutoTokenizer.from_pretrained(
             model_filepath, model_max_length=512)
         loaded_model = TokenClassificationPipeline(task='ner', 
                         model=model, 
                         tokenizer=tokenizer_1,
-                        aggregation_strategy='simple')
+                        aggregation_strategy='simple')#, 
+                        #grouped_entities=True)#,
+                        #aggregation_strategy='simple')
         
         return loaded_model
     
     @staticmethod
     def load_probabilities_file(dict_filename):
         
         type_dict = {}
```

### Comparing `bent-0.0.19/bent/src/utils.py` & `bent-0.0.9/bent/src/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,78 +30,69 @@
             'anatomical', 'cell_component', 'cell_line', 'cell_type', 
             'variant']
        
         for ent_type in types:
             
             if ent_type != '':
                 assert ent_type in available_types, \
-                    '{} is an invalid entity type to recognize! Options:\
+                    '{} is an invalid entity type! Options:\
                     "disease", "chemical", "gene", "organism", "bioprocess", \
                     "bioprocess", "anatomical", "cell_component", "cell_line",\
                     "cell_type", "variant"'.format(ent_type)
                         
 
 def check_input_args(recognize, link, types, input_format, input_text, 
         in_dir, ner_dir, out_dir, ner_model, nel_model):
-    """Verify if the input arguments are valid."""
+    """Verify if the input arguments are valid"""
 
     available_formats = ['brat', 'bioc_xml', 'bioc_json', 'pubtator'] 
 
     # Verify selected task(s)
     assert recognize == True or link == True, \
         'It is available Named Entity Recognition (NER) and/or Named Entity \
         ensure that either recognize == True and/or link == True'
 
     # Verify the inputed entity types and respective target KBs
     check_input_types(types)
 
-    # Verify input format and directory arguments
+    # Verify input format and dir
     if recognize:
 
         if input_text == None and in_dir == None:
-            raise ValueError('It is necessary to input either a text or a \
-                list of texts (by setting the argument "input_text") \
-                OR a directory containing file(s) with texts to annotate \
-                (by setting the argument "text_dir").') 
+            raise ValueError('It is necessary to input either a text \
+                ("input_text") OR a directory containing file(s) with text \
+                to annotate ("text_dir").') 
         
         if input_format == 'bioc_json' or input_format == 'bioc_xml' \
                 or input_format == 'pubtator':
 
                 assert in_dir != None or ner_dir != None, \
-                    'For input formats "bioc_json", "bioc_xml"and "pubtator" \
-                    it is necessary to specify the input directory by setting \
-                    the argument "in_dir"'
+                    'For input formats "bioc_json"\
+                    , "bioc_xml"and "pubtator" it is necessary to specify\
+                    the input directory "in_dir"'
 
     if link:
 
         if not recognize:
 
-            assert ner_dir != None, 'No NER will be performed, only NEL: \
-                it is necessary to specfiy the directory containing \
-                NER annotations (by setting the argument "ner_dir").' 
-
-    # Check directory paths
+            assert ner_dir != None, 'It is necessary to specfiy the directory \
+                containing the ouput from the NER stage ("ner_dir").' 
 
+    #Check directories paths
     if in_dir != None:
-        assert in_dir[-1:] == '/', 'Invalid argument "in_dir": the last \
-            character in the directory path must be "/"\n. Examples: \
-            "dataset/txt" -> INVALID directory path \
-            "dataset/txt/" -> VALID directory path'
+        assert in_dir[-1:] == '/', 'Invalid "in_dir". Last character in \
+            directory name must be "/"'
 
     if ner_dir != None:
-        assert ner_dir[-1:] == '/', 'Invalid argument "ner_dir": the last \
-            character in the directory path must be "/"\n. Examples: \
-            "dataset/ann" -> INVALID directory path \
-            "dataset/ann/" -> VALID directory path'
+        assert ner_dir[-1:] == '/', 'Invalid "ner_dir". Last character in \
+            directory name must be "/"'
 
     if out_dir != None:
-        assert out_dir[-1:] == '/', 'Invalid argument "out_dir": the last \
-            character in the directory path must be "/"\n. Examples: \
-            "dataset/ann" -> INVALID directory path \
-            "dataset/ann/" -> VALID directory path'
+        assert out_dir[-1:] == '/', 'Invalid "out_dir". Last character in \
+            directory name must be "/"'
         
 
 #------------------------------------------------------------------------------
 #                       INPUT FILE FORMAT CONVERSION
 #------------------------------------------------------------------------------
 
 def parse_bioc_json_file(filename, include_text=True):
@@ -125,14 +116,15 @@
                 title = passage['text']
 
             if passage['infons']['type'] == 'abstract':
                 abstract = passage['text']
 
                 for annot in passage['annotations']:
                     ent_type = annot['infons']['type']
+                    #kb_id = annot['infons']['identifier']
                     text = annot['text']
 
                     begin = annot['locations'][0]['offset']
                     end = str(int(begin) + int(annot['locations'][0]['length']))
 
                     annotation = (ent_type, begin, end, text)
                     annotations.append(annotation)
@@ -164,52 +156,53 @@
         with open(out_dir + 'txt/' + doc_id + '.txt', 'w') as txt_file:
             txt_file.write(doc_text)
             txt_file.close()
        
         if not recognize:
             # In this case only the NEL step will be performed
             # Make annotations file
+        
             annotations = parsed_data[doc_id][1]
             annot_str = ''
 
             for i, annot in enumerate(annotations):
                 annot_str += 'T{}\t{} {} {}\t{}\n'.format(
                     str(i+1), annot[0], annot[1], annot[2], annot[3]) 
         
             with open(out_dir + 'ann/' + doc_id + '.ann', 'w') as ann_file:
                 ann_file.write(annot_str)
                 ann_file.close()
         
 
-def convert_input_files(format, in_dir=None, input_text=None, recognize=False):
-    """Convert input file(s) into brat/standoff format"""
+def convert_input_files(format, input_text=None, in_dir=None, recognize=False):
+    """Convert input file(s) into brat/standoof format"""
     
     if input_text != None:
 
         if type(input_text) == str:
             input_files = [input_text]
             
         elif type(input_text) == list:
             input_files = input_text
 
         # Create a txt file for later use in the NEL module.
-        for i, text in enumerate(input_files, start=1):
-            doc_id = 'doc_{}'.format(str(i))
+        for i, text in enumerate(input_files):
+            doc_id = str(i)
             
-            with open('{}{}.txt'.format(in_dir, doc_id), 'w') as txt_file:
+            with open(out_dir + doc_id + '.txt', 'w') as txt_file:
                 txt_file.write(text)
                 txt_file.close()
     
-    """
     else:
 
         assert format == 'bioc_xml' or format == 'bioc_json' \
             or format == 'pubtator',  'Invalid format. Options: "brat", \
             "bioc_xml", "bioc_json", "pubtator"'
         
+        
         filenames = [in_dir + filename for filename in os.listdir(in_dir)]
         out_dir = in_dir + 'brat/'
             
         for filename in filenames:
             output = False
             
             if format == 'bioc_xml' and filename[-3:] == 'xml':
@@ -226,15 +219,15 @@
 
             if output:
 
                 if not os.path.exists(out_dir):
                     os.mkdir(out_dir)
                 
                 output_parsed_docs(parsed_data, out_dir, recognize=recognize)
-    """
+        
 
 #------------------------------------------------------------------------------
 #                       TEXT PARSING AND OBJECTIFICATION 
 #------------------------------------------------------------------------------
 
 def sentence_splitter(doc_text, lang_model):
     """Split given text into sentences using SpaCy and the ScispaCy model 
@@ -432,20 +425,20 @@
         Named Entity Linking step from files
     :type nel_run_ids: list
     :return: linked_entities with format: {'entity_text': 'kb_id'}
     :rtype: dict
     """
     
     linked_entities = {}
-    
+
     for run_id in nel_run_ids:
         results_dir = '{}{}/REEL/results/'.format(cfg.tmp_dir, run_id)
         results_files = os.listdir(results_dir)
         linked_entities_type = {}       
-        ent_type = run_id.split('/')[1] 
+        ent_type = run_id.split('_')[1] 
         target_filename = doc_id + '.json'
 
         if target_filename in results_files:
             filepath = results_dir + target_filename
             
             with open(filepath, 'r') as infile:
                 linked_entities_type = json.loads(infile.read())
@@ -580,8 +573,8 @@
 
     :param threshold: amount of memory usage that triggers the garbage 
         collection, defaults to 50.0
     :type threshold: float, optional
     """
 
     if psutil.virtual_memory().percent >= threshold:
-        gc.collect()
+        gc.collect()
```

### Comparing `bent-0.0.19/bent.egg-info/PKG-INFO` & `bent-0.0.9/bent.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bent
-Version: 0.0.19
+Version: 0.0.9
 Summary: BENT: Biomedical Entity Annotator
 Home-page: https://github.com/lasigeBioTM/bent
 Author: Pedro Ruas
 Author-email: pedrosimruas@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -219,143 +219,124 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Unix Shell
 Classifier: Programming Language :: Java
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7, <3.10
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 
 
 BENT: Biomedical Entity Annotator
 ---------------------------------
 
 Python Library for Named Entity Recognition (NER) and Linking (NEL) in the biomedical domain.
 
+NER models are based on `PubMedBERT <https://arxiv.org/pdf/2007.15779.pdf>`__ and a post-processing rule-based module.
+the NEL model is a graph-based approach based on the Personalized PageRank algorithm and Information content.
+
 BENT can be used for: 
 
 * Named Entity Recogniton (NER)
 * Named Entity Linking (NEL) 
 * Named Entity Recognition and Linking (NER+NEL)
 
-Access the full `documentation <https://bent.readthedocs.io/en/latest/>`__.
+Access the full documentation `here <https://bent.readthedocs.io/en/latest/>`__.
 
-Citation::
+Citation:
 
-  Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking. 
-  Journal of Biomedical Informatics, 132:104137, 2022. 
-  doi: https://doi.org/10.1016/j.jbi.2022.104137.
+* Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking <https://www.sciencedirect.com/science/article/pii/S1532046422001526>`__. Journal of Biomedical Informatics, 132:104137, 2022. doi: https://doi.org/10.1016/j.jbi.2022.104137.
 
 Installation
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~
 
 To use the current version of BENT it is required: 
 
-*  OS: Ubuntu/Debian 
+* OS based on Ubuntu/Debian 
+* `Conda <https://docs.conda.io/en/latest/>`__ environment 
+* Python>=3.7
+* Between 11 and 15 GB free space (5 GB Anaconda + 2.5 GB to install dependencies + 3.0 GB data or 7.5 GB if you use all available knowlegde bases for NEL)
 
-*  Python 3.7, 3.8 or 3.9
+.. note::
 
-*  Required space between 5.5 GB - 10 GB 
-   * Dependencies: 2.5 GB 
-   * Data: between 3.0 GB (base) or 7.5 GB (if you use all available knowlegde bases for Named Entity Linking)
+   Please ensure that you have the appropriate version of Conda installed.
 
 
-Install the BENT package using pip:
+Create a Conda environment (adapt for the name of your project):
 
 ::
 
-   pip install bent
+   conda create --name annotation_project python=3.7
 
 
-The following knowledge bases can be configured:
+Activate the environment:
 
-* 'medic' (`MEDIC <http://ctdbase.org/>`__)
+::
 
-* 'do' (`Disease ontology <https://disease-ontology.org/>`__)
+   conda activate annotation_project
 
-* 'chebi' (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
-* 'ctd_chem' (`CTD-Chemicals <http://ctdbase.org/>`__)
+Install the BENT package using pip:
 
-* 'ncbi_gene' (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
+::
 
-* 'ctd_gene' (`CTD-GENES <http://ctdbase.org/>`__)
+   pip install bent
 
-* 'ncbi_taxon' (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
-* 'go_bp' (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
+After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Specify the knowledge bases that will be used:
 
-* 'ctd_anat' (`CTD-Anatomy <http://ctdbase.org/>`__)
+::
 
-* 'fma' (`Foundation model of Anatomy <http://sig.biostr.washington.edu/projects/fm/AboutFM.html>`__)
+   python -c "from bent.setup_package import setup_package;setup_package([<kb1>, <kb2>, <kb3>])"
 
-* 'uberon' (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
+Available knowledge bases:
 
-* 'go_cc' (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
+* ‘medic’ (`MEDIC <http://ctdbase.org/>`__)
 
-* 'cell_ontology' (`Cell Ontology <https://cell-ontology.github.io/>`__)
+* ‘do’ (`Disease ontology <https://disease-ontology.org/>`__)
 
-* 'cellosaurus' (`Cellosaurus <https://www.cellosaurus.org/>`__)
+* 'chebi’ (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
+* ‘ctd_chem’ (`CTD-Chemicals <http://ctdbase.org/>`__)
 
-After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Run in the command line:
+* ‘ncbi_gene’ (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
 
-::
+* ‘ctd_gene’ (`CTD-GENES <http://ctdbase.org/>`__)
 
-   bent_setup
+* ‘ncbi_taxon’ (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
+* ‘go_bp’ (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
 
-Only the default knowledge bases 'medic' and 'chebi' will be available at this point.
+* ‘ctd_anat’ (`CTD-Anatomy <http://ctdbase.org/>`__)
 
-To disable annoyng messages in the terminal run:
+* ‘uberon’ (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
 
-::
+* ‘go_cc’ (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
 
-   export TF_CPP_MIN_LOG_LEVEL='3'
+* ‘cell_ontology’ (`Cell Ontology <https://cell-ontology.github.io/>`__)
 
+* cellosaurus’ (`Cellosaurus <https://www.cellosaurus.org/>`__)
 
-You can download more knowledge bases later by specifying the desired knowledge bases among the ones that are available:
+Example to download only the MEDIC vocabulary:
 
 ::
 
-   python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs([<kb1>, <kb2>])"
+   python -c "from bent.setup_package import setup_package;setup_package(['medic'])"
 
 
-Get started
-~~~~~~~~~~~
+If you want to download all knowledge bases, choose the option 'all':
 
-To apply the complete pipeline of entity extraction (NER+NEL) set the arguments:
+::
 
-* **recognize**: indicate that the NER module will be applied ('True')
-* **link**: indicate that the NEL module will be applied ('True')
-* **types**: entity types to recognize and the respective target knowledge bases.
-* **in_dir**: directory path containing the text files to be annotated (the directory must contain text files exclusively)
-* **out_dir**: the output directory that will contain the annotation files
+   python -c "from bent.setup_package import setup_package;setup_package(['all'])"
 
 
-Example:
+You can download more knowledge bases later by running the same command and specifying the desired knolwedge bases among the ones that are available and setting the argument ' only_kb_dicts' to True:
 
 ::
 
-   import bent.annotate as bt
-
-   bt.annotate(
-           recognize=True,
-           link=True,
-           types={
-            'disease': 'medic'
-            'chemical': 'chebi',
-            'gene': 'ncbi_gene',
-            'anatomical': 'uberon',
-            'cell_line': 'cellosaurus',
-            'bioprocess': 'go_bp'
-            },
-           in_dir='input/txt/',
-           out_dir='output/nel/'
-   )
-
+   python -c "from bent.setup_package import setup_package;setup_package([<kb>],  only_kb_dicts=True)"
 
-It is also possible to apply the pipeline (NER+NEL) to a string or a list or strings instantiated in the execution script.
 
-To see more usage examples, access the `documentation <https://bent.readthedocs.io/en/latest/usage.html>`__.
+Reinitiate the conda environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bent-0.0.19/bent.egg-info/SOURCES.txt` & `bent-0.0.9/bent.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 LICENSE.txt
-MANIFEST.in
 README.rst
 setup.py
 bent/__init__.py
 bent/annotate.py
 bent/get_data.sh
 bent/get_kb_dicts.sh
-bent/get_kbs.py
 bent/requirements.txt
+bent/setup_package.py
 bent/setup_package.sh
-bent/setup_package_wrapper.py
 bent.egg-info/PKG-INFO
 bent.egg-info/SOURCES.txt
 bent.egg-info/dependency_links.txt
-bent.egg-info/entry_points.txt
 bent.egg-info/requires.txt
 bent.egg-info/top_level.txt
 bent/src/__init__.py
 bent/src/cfg.py
 bent/src/classes.py
 bent/src/nel.py
 bent/src/ner.py
@@ -33,15 +30,15 @@
 bent/src/REEL/ppr_for_ned_all.class
 bent/src/REEL/ppr_for_ned_all.java
 bent/src/REEL/pre_process.py
 bent/src/REEL/run.py
 bent/src/REEL/utils.py
 bent/src/abbreviation_detector/__init__.py
 bent/src/abbreviation_detector/run.py
-bent/src/build/__init__.py
-bent/src/build/annotations/__init__.py
-bent/src/build/annotations/dataset_entities.py
-bent/src/build/kb/__init__.py
-bent/src/build/kb/generate_dicts.py
-bent/src/build/kb/kb.py
-bent/src/build/relation_extraction/__init__.py
-bent/src/build/relation_extraction/dicts.py
+bent/src/setup/__init__.py
+bent/src/setup/annotations/__init__.py
+bent/src/setup/annotations/dataset_entities.py
+bent/src/setup/kb/__init__.py
+bent/src/setup/kb/generate_dicts.py
+bent/src/setup/kb/kb.py
+bent/src/setup/relation_extraction/__init__.py
+bent/src/setup/relation_extraction/dicts.py
```

