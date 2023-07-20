# Comparing `tmp/pyjedai-0.0.8.tar.gz` & `tmp/pyjedai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjedai-0.0.8.tar", last modified: Wed Jul  5 18:56:49 2023, max compression
+gzip compressed data, was "pyjedai-0.0.9.tar", last modified: Thu Jul 20 14:10:52 2023, max compression
```

## Comparing `pyjedai-0.0.8.tar` & `pyjedai-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.533818 pyjedai-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-07-05 18:56:34.000000 pyjedai-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-05 18:56:49.533818 pyjedai-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-05 18:56:34.000000 pyjedai-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-05 18:56:34.000000 pyjedai-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:56:49.533818 pyjedai-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.529818 pyjedai-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.533818 pyjedai-0.0.8/src/pyjedai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18191 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/block_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/block_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    52141 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/comparison_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/joins.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25997 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)    50691 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/prioritization.py
--rw-r--r--   0 runner    (1001) docker     (123)    23995 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23817 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/vector_based_blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.533818 pyjedai-0.0.8/src/pyjedai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.533818 pyjedai-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_block_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_block_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_comparison_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_joins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:52.131459 pyjedai-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-07-20 14:10:30.000000 pyjedai-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-07-20 14:10:52.131459 pyjedai-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-07-20 14:10:30.000000 pyjedai-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-20 14:10:30.000000 pyjedai-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:10:52.131459 pyjedai-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:52.127458 pyjedai-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:52.131459 pyjedai-0.0.9/src/pyjedai/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19930 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/block_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/block_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53241 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/comparison_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/joins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50691 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/prioritization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23995 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/vector_based_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30594 2023-07-20 14:10:30.000000 pyjedai-0.0.9/src/pyjedai/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:52.131459 pyjedai-0.0.9/src/pyjedai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-07-20 14:10:52.000000 pyjedai-0.0.9/src/pyjedai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-20 14:10:52.000000 pyjedai-0.0.9/src/pyjedai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:10:52.000000 pyjedai-0.0.9/src/pyjedai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-20 14:10:52.000000 pyjedai-0.0.9/src/pyjedai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 14:10:52.000000 pyjedai-0.0.9/src/pyjedai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:52.131459 pyjedai-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-20 14:10:31.000000 pyjedai-0.0.9/tests/test_block_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-20 14:10:31.000000 pyjedai-0.0.9/tests/test_block_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-20 14:10:31.000000 pyjedai-0.0.9/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-20 14:10:31.000000 pyjedai-0.0.9/tests/test_comparison_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:31.000000 pyjedai-0.0.9/tests/test_joins.py
```

### Comparing `pyjedai-0.0.8/LICENSE` & `pyjedai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/PKG-INFO` & `pyjedai-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyjedai
-Version: 0.0.8
+Version: 0.0.9
 Summary: An open-source library that builds powerful end-to-end Entity Resolution workflows.
 Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>, Jakub Maciejewski <jacobb.maciejewski@gmail.com>
 License: Apache Software License 2.0
 Project-URL: Homepage, http://pyjedai.rtfd.io
 Project-URL: Documentation, http://pyjedai.rtfd.io
 Project-URL: Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues
 Project-URL: Source code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai
 Keywords: deduplication,entity-resolution,link-discovery
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
@@ -29,24 +30,26 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
     <br>
-    <img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
+    <img align="center" src="https://github.com/AI-team-UoA/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
 </div>
 <br>
 <br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
+
 ---
 
+
 # Overview
 
 pyJedAI is a python framework, aiming to offer experts and novice users, robust and fast solutions for multiple types of Entity Resolution problems. It is builded using state-of-the-art python frameworks. pyJedAI constitutes the sole open-source Link Discovery tool that is capable of exploiting the latest breakthroughs in Deep Learning and NLP techniques, which are publicly available through the Python data science ecosystem. This applies to both blocking and matching, thus ensuring high time efficiency, high scalability as well as high effectiveness, without requiring any labelled instances from the user.
 
 ### Key-Features
 
 - Input data-type independent. Both structured and semi-structured data can be processed.
@@ -54,18 +57,18 @@
 - Easy-to-use.
 - Utilizes some of the famous and cutting-edge machine learning packages.
 - Offers supervised and un-supervised ML techniques.
 
 __Open demos are available in:__
 
 <div align="center">
-    <a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+    <a href="https://nbviewer.org/github/AI-team-UoA/pyJedAI/blob/main/docs/tutorials/Demo.ipynb">
         <img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
     </a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-    <a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+    <a href="https://github.com/AI-team-UoA/pyJedAI/blob/main/docs/tutorials/Demo.ipynb">
         <img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
     </a>
 </div>
 
 __Google Colab Hands-on demo:__ 
 
 <div align="center">
@@ -110,25 +113,33 @@
     <img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
 </div>
 <br>
 
-See the full list of dependencies and all versions used, in this [file](https://github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt).
+See the full list of dependencies and all versions used, in this [file](https://github.com/AI-team-UoA/pyJedAI/blob/main/pyproject.toml).
 
-__Status__ 
+__Status__
 
-[![Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml)
+[![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml)
+[![PyPi](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/pypi-publish.yml)
 [![made-with-python](https://readthedocs.org/projects/pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/AI-team-UoA/pyjedai/branch/master/graph/badge.svg?token=4QR0X315CL)](https://codecov.io/gh/AI-team-UoA/pyjedai)
+
+
+__Statistics & Info__
+
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyjedai)
+[![PyPI version](https://img.shields.io/pypi/v/pyjedai.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pyjedai/)
 
 
 # Bugs, Discussions & News
 
-[GitHub Discussions](https://github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues).
+[GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Java - Wed Application 
 
 <img align="left" src="https://github.com/scify/JedAIToolkit/blob/master/documentation/JedAI_logo.png?raw=true" alt="pyJedAI" width="130"/>
 
 For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows. <br><br> JedAI constitutes an open source, high scalability toolkit that offers out-of-the-box solutions for any data integration task, e.g., Record Linkage, Entity Resolution and Link Discovery. At its core lies a set of domain-independent, state-of-the-art techniques that apply to both RDF and relational data.
 
@@ -143,15 +154,15 @@
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
 
 # License
 
-Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE).
+Released under the Apache-2.0 license (see [LICENSE.txt](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)).
 
 Copyright © 2023 AI-Team, University of Athens
 
 <div align="center">
     <hr>
     <br>
     <a href="https://stelar-project.eu">
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: pyjedai Version: 0.0.8 Summary: An open-source
+Metadata-Version: 2.1 Name: pyjedai Version: 0.0.9 Summary: An open-source
 library that builds powerful end-to-end Entity Resolution workflows. Author-
 email: Konstantinos Nikoletos
 kon@gmail.com>, George Papadakis
 gmail.com>, Jakub Maciejewski
 maciejewski@gmail.com> License: Apache Software License 2.0 Project-URL:
 Homepage, http://pyjedai.rtfd.io Project-URL: Documentation, http://
 pyjedai.rtfd.io Project-URL: Bug Tracker, https://github.com/AI-team-UoA/
 pyJedAI/issues Project-URL: Source code, https://github.com/AI-team-UoA/
 pyJedAI/tree/main/pyjedai Keywords: deduplication,entity-resolution,link-
 discovery Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: Implementation
-Classifier: Intended Audience :: Information Technology Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English Classifier: Operating System ::
-Microsoft :: Windows Classifier: Operating System :: Unix Classifier: Operating
-System :: iOS Classifier: Topic :: Database Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: Implementation Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers Classifier: Natural Language ::
+English Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: Unix Classifier: Operating System :: iOS Classifier: Topic
+:: Database Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev License-File: LICENSE
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
@@ -66,39 +67,46 @@
 
  [https://www.kornosk.me/resources/language-model/featured.png]     [https://
    repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-
 745fdcbeffe8]     [https://networkx.org/_static/networkx_logo.svg]     [https:/
           /raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png]
 
 See the full list of dependencies and all versions used, in this [file](https:/
-/github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt). __Status__ [!
-[Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/
-badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
-workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
-pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
-?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
-github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general
-questions and discussions and our recommended starting point. Please report any
-bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues). #
-Java - Wed Application [pyJedAI] For Java users checkout the initial [JedAI]
-(https://github.com/scify/JedAIToolkit). There you can find Java based code and
-a Web Application for interactive creation of ER workflows.
+/github.com/AI-team-UoA/pyJedAI/blob/main/pyproject.toml). __Status__ [![Tests]
+(https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/
+badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/
+workflows/tests.yml) [![PyPi](https://github.com/AI-team-UoA/pyJedAI/actions/
+workflows/pypi-publish.yml/badge.svg)](https://github.com/AI-team-UoA/pyJedAI/
+actions/workflows/pypi-publish.yml) [![made-with-python](https://
+readthedocs.org/projects/pyjedai/badge/?version=latest)](https://
+pyjedai.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
+gh/AI-team-UoA/pyjedai/branch/master/graph/badge.svg?token=4QR0X315CL)](https:/
+/codecov.io/gh/AI-team-UoA/pyjedai) __Statistics & Info__ ![PyPI - Downloads]
+(https://img.shields.io/pypi/dm/pyjedai) [![PyPI version](https://
+img.shields.io/pypi/v/pyjedai.svg?logo=pypi&logoColor=FFE873)](https://
+pypi.org/project/pyjedai/) # Bugs, Discussions & News [GitHub Discussions]
+(https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum
+for general questions and discussions and our recommended starting point.
+Please report any bugs that you find [here](https://github.com/AI-team-UoA/
+pyJedAI/issues). # Java - Wed Application [pyJedAI] For Java users checkout the
+initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java
+based code and a Web Application for interactive creation of ER workflows.
 
 JedAI constitutes an open source, high scalability toolkit that offers out-of-
 the-box solutions for any data integration task, e.g., Record Linkage, Entity
 Resolution and Link Discovery. At its core lies a set of domain-independent,
 state-of-the-art techniques that apply to both RDF and relational data.
 # Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
 k.github.io) - Jakub Maciejewski - [George Papadakis](https://
 gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
 ) Research and development is made under the supervision of Pr. Manolis
 Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
 of the Department of Informatics and Telecommunications at the University of
-Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
-(https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE). Copyright Â© 2023
+Athens. # License Released under the Apache-2.0 license (see [LICENSE.txt]
+(https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)). Copyright Â© 2023
 AI-Team, University of Athens
 ===============================================================================
 
   [https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png]
               [https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/
               Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png]
```

### Comparing `pyjedai-0.0.8/README.md` & `pyjedai-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 <div align="center">
     <br>
-    <img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
+    <img align="center" src="https://github.com/AI-team-UoA/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
 </div>
 <br>
 <br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
+
 ---
 
+
 # Overview
 
 pyJedAI is a python framework, aiming to offer experts and novice users, robust and fast solutions for multiple types of Entity Resolution problems. It is builded using state-of-the-art python frameworks. pyJedAI constitutes the sole open-source Link Discovery tool that is capable of exploiting the latest breakthroughs in Deep Learning and NLP techniques, which are publicly available through the Python data science ecosystem. This applies to both blocking and matching, thus ensuring high time efficiency, high scalability as well as high effectiveness, without requiring any labelled instances from the user.
 
 ### Key-Features
 
 - Input data-type independent. Both structured and semi-structured data can be processed.
@@ -21,18 +23,18 @@
 - Easy-to-use.
 - Utilizes some of the famous and cutting-edge machine learning packages.
 - Offers supervised and un-supervised ML techniques.
 
 __Open demos are available in:__
 
 <div align="center">
-    <a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+    <a href="https://nbviewer.org/github/AI-team-UoA/pyJedAI/blob/main/docs/tutorials/Demo.ipynb">
         <img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
     </a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-    <a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+    <a href="https://github.com/AI-team-UoA/pyJedAI/blob/main/docs/tutorials/Demo.ipynb">
         <img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
     </a>
 </div>
 
 __Google Colab Hands-on demo:__ 
 
 <div align="center">
@@ -77,25 +79,33 @@
     <img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
 </div>
 <br>
 
-See the full list of dependencies and all versions used, in this [file](https://github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt).
+See the full list of dependencies and all versions used, in this [file](https://github.com/AI-team-UoA/pyJedAI/blob/main/pyproject.toml).
 
-__Status__ 
+__Status__
 
-[![Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml)
+[![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml)
+[![PyPi](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/pypi-publish.yml)
 [![made-with-python](https://readthedocs.org/projects/pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/AI-team-UoA/pyjedai/branch/master/graph/badge.svg?token=4QR0X315CL)](https://codecov.io/gh/AI-team-UoA/pyjedai)
+
+
+__Statistics & Info__
+
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyjedai)
+[![PyPI version](https://img.shields.io/pypi/v/pyjedai.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pyjedai/)
 
 
 # Bugs, Discussions & News
 
-[GitHub Discussions](https://github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues).
+[GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Java - Wed Application 
 
 <img align="left" src="https://github.com/scify/JedAIToolkit/blob/master/documentation/JedAI_logo.png?raw=true" alt="pyJedAI" width="130"/>
 
 For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows. <br><br> JedAI constitutes an open source, high scalability toolkit that offers out-of-the-box solutions for any data integration task, e.g., Record Linkage, Entity Resolution and Link Discovery. At its core lies a set of domain-independent, state-of-the-art techniques that apply to both RDF and relational data.
 
@@ -110,15 +120,15 @@
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
 
 # License
 
-Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE).
+Released under the Apache-2.0 license (see [LICENSE.txt](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)).
 
 Copyright © 2023 AI-Team, University of Athens
 
 <div align="center">
     <hr>
     <br>
     <a href="https://stelar-project.eu">
```

#### html2text {}

```diff
@@ -43,39 +43,46 @@
 
  [https://www.kornosk.me/resources/language-model/featured.png]     [https://
    repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-
 745fdcbeffe8]     [https://networkx.org/_static/networkx_logo.svg]     [https:/
           /raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png]
 
 See the full list of dependencies and all versions used, in this [file](https:/
-/github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt). __Status__ [!
-[Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/
-badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
-workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
-pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
-?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
-github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general
-questions and discussions and our recommended starting point. Please report any
-bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues). #
-Java - Wed Application [pyJedAI] For Java users checkout the initial [JedAI]
-(https://github.com/scify/JedAIToolkit). There you can find Java based code and
-a Web Application for interactive creation of ER workflows.
+/github.com/AI-team-UoA/pyJedAI/blob/main/pyproject.toml). __Status__ [![Tests]
+(https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/
+badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/
+workflows/tests.yml) [![PyPi](https://github.com/AI-team-UoA/pyJedAI/actions/
+workflows/pypi-publish.yml/badge.svg)](https://github.com/AI-team-UoA/pyJedAI/
+actions/workflows/pypi-publish.yml) [![made-with-python](https://
+readthedocs.org/projects/pyjedai/badge/?version=latest)](https://
+pyjedai.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
+gh/AI-team-UoA/pyjedai/branch/master/graph/badge.svg?token=4QR0X315CL)](https:/
+/codecov.io/gh/AI-team-UoA/pyjedai) __Statistics & Info__ ![PyPI - Downloads]
+(https://img.shields.io/pypi/dm/pyjedai) [![PyPI version](https://
+img.shields.io/pypi/v/pyjedai.svg?logo=pypi&logoColor=FFE873)](https://
+pypi.org/project/pyjedai/) # Bugs, Discussions & News [GitHub Discussions]
+(https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum
+for general questions and discussions and our recommended starting point.
+Please report any bugs that you find [here](https://github.com/AI-team-UoA/
+pyJedAI/issues). # Java - Wed Application [pyJedAI] For Java users checkout the
+initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java
+based code and a Web Application for interactive creation of ER workflows.
 
 JedAI constitutes an open source, high scalability toolkit that offers out-of-
 the-box solutions for any data integration task, e.g., Record Linkage, Entity
 Resolution and Link Discovery. At its core lies a set of domain-independent,
 state-of-the-art techniques that apply to both RDF and relational data.
 # Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
 k.github.io) - Jakub Maciejewski - [George Papadakis](https://
 gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
 ) Research and development is made under the supervision of Pr. Manolis
 Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
 of the Department of Informatics and Telecommunications at the University of
-Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
-(https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE). Copyright Â© 2023
+Athens. # License Released under the Apache-2.0 license (see [LICENSE.txt]
+(https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)). Copyright Â© 2023
 AI-Team, University of Athens
 ===============================================================================
 
   [https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png]
               [https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/
               Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png]
```

### Comparing `pyjedai-0.0.8/pyproject.toml` & `pyjedai-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyjedai"
-version = "0.0.8"
+version = "0.0.9"
 description = "An open-source library that builds powerful end-to-end Entity Resolution workflows."
 readme = "README.md"
 authors = [
     { name = "Konstantinos Nikoletos", email = "nikoletos.kon@gmail.com" },
     { name = "George Papadakis", email = "gpapadis84@gmail.com" },
     { name = "Jakub Maciejewski", email = "jacobb.maciejewski@gmail.com"}
 ]
@@ -18,14 +18,15 @@
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: Unix",
@@ -57,15 +58,14 @@
     "tqdm >= 4.64",
     "transformers >= 4.21",
     "sentence-transformers >= 2.2",
     "faiss-cpu >= 1.7",
     "optuna >= 3.0",
     'tomli; python_version < "3.11"',
     "py-stringmatching >= 0.4",
-    "whoosh >= 2.7",
     "valentine>=0.1.5",
     "ordered-set >= 4.0",
 ]
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest"]
```

### Comparing `pyjedai-0.0.8/src/pyjedai/block_building.py` & `pyjedai-0.0.9/src/pyjedai/block_building.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
 import logging as log
 import math
 import re
 import time
+import pandas as pd
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import Tuple
 
 import nltk
 import numpy as np
 from tqdm.auto import tqdm
@@ -122,14 +123,49 @@
             "\n\tNumber of comparisons: " + str(self.total_num_of_comparisons) +
             "\n\tMax comparisons per block: " + str(self.max_block_comparisons) +
             "\n\tMin comparisons per block: " + str(self.min_block_comparisons) +
             "\n\tEntities in blocks: " + str(len(self.entities_in_blocks))
         )
         print(u'\u2500' * 123)
 
+    def export_to_df(
+        self,
+        blocks: dict
+    ) -> pd.DataFrame:
+        """creates a dataframe for the evaluation report
+
+        Args:
+            blocks (any): Predicted blocks
+            data (Data): initial dataset
+
+        Returns:
+            pd.DataFrame: Dataframe predicted pairs (can be exported to csv)
+        """
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. \
+                Data object mush have initialized with the ground-truth file")
+        pairs_df = pd.DataFrame(columns=['id1', 'id2'])
+        for _, block in blocks.items():
+            if self.data.is_dirty_er:
+                lblock = list(block.entities_D1)
+                for i1 in range(0, len(lblock)):
+                    for i2 in range(i1+1, len(lblock)):
+                        id1 = self.data._gt_to_ids_reversed_1[lblock[i1]]
+                        id2 = self.data._gt_to_ids_reversed_1[lblock[i2]] if self.data.is_dirty_er \
+                            else self.data._gt_to_ids_reversed_2[lblock[i2]]
+                        pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
+            else:
+                for i1 in block.entities_D1:
+                    for i2 in block.entities_D2:
+                        id1 = self.data._gt_to_ids_reversed_1[i1]
+                        id2 = self.data._gt_to_ids_reversed_1[i2] if self.data.is_dirty_er \
+                            else self.data._gt_to_ids_reversed_2[i2]
+                        pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
+        return pairs_df
+
 class AbstractBlockBuilding(AbstractBlockProcessing):
     """Abstract class for the block building method
     """
 
     _method_name: str
     _method_info: str
     _method_short_name: str
```

### Comparing `pyjedai-0.0.8/src/pyjedai/block_cleaning.py` & `pyjedai-0.0.9/src/pyjedai/block_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/src/pyjedai/clustering.py` & `pyjedai-0.0.9/src/pyjedai/clustering.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from queue import PriorityQueue
 from time import time
 
+import pandas as pd
 from networkx import Graph, connected_components
 from tqdm.autonotebook import tqdm
 
 from .datamodel import Data, PYJEDAIFeature
 from .evaluation import Evaluation
 from .utils import are_matching
 
@@ -54,14 +55,46 @@
                                 export_to_dict,
                                 with_classification_report,
                                 verbose)
     
     def stats(self) -> None:
         pass
 
+    def export_to_df(self, prediction: list) -> pd.DataFrame:
+        """creates a dataframe for the evaluation report
+
+        Args:
+            prediction (any): Predicted clusters
+
+        Returns:
+            pd.DataFrame: Dataframe containg evaluation scores and stats
+        """
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. \
+                Data object mush have initialized with the ground-truth file")
+        pairs_df = pd.DataFrame(columns=['id1', 'id2'])
+        for cluster in prediction:
+            lcluster = list(cluster)
+            for i1 in range(0, len(lcluster)):
+                for i2 in range(i1+1, len(lcluster)):
+                    if lcluster[i1] < self.data.dataset_limit:
+                        id1 = self.data._gt_to_ids_reversed_1[lcluster[i1]]
+                        id2 = self.data._gt_to_ids_reversed_1[lcluster[i2]] if self.data.is_dirty_er else self.data._gt_to_ids_reversed_2[lcluster[i2]]
+                    else:
+                        id2 = self.data._gt_to_ids_reversed_2[lcluster[i1]]
+                        id1 = self.data._gt_to_ids_reversed_1[lcluster[i2]]
+                    pairs_df = pd.concat(
+                        [pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], 
+                        ignore_index=True
+                    )
+        return pairs_df
+    
+    
+    
+
 class ConnectedComponentsClustering(AbstractClustering):
     """Creates the connected components of the graph. \
         Applied to graph created from entity matching. \
         Input graph consists of the entity ids (nodes) and the similarity scores (edges).
     """
 
     _method_name: str = "Connected Components Clustering"
```

### Comparing `pyjedai-0.0.8/src/pyjedai/comparison_cleaning.py` & `pyjedai-0.0.9/src/pyjedai/comparison_cleaning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import warnings
+import pandas as pd
 from itertools import chain
 from collections import defaultdict
 from logging import warning
 from math import log10, sqrt
 from queue import PriorityQueue
 from time import time
 
@@ -92,15 +93,14 @@
 
     @abstractmethod
     def _configuration(self) -> dict:
         pass
     
     def stats(self) -> None:
         pass
-
     
     def get_precalculated_weight(self, entity_id: int, neighbor_id: int) -> float:
         """Returns the precalculated weight for given pair
 
         Args:
             entity_id (int): Entity ID
             neighbor_id (int): Neighbor ID
@@ -144,14 +144,38 @@
                                   total_matching_pairs=total_matching_pairs)
         return eval_obj.report(self.method_configuration(),
                                 export_to_df,
                                 export_to_dict,
                                 with_classification_report,
                                 verbose)
 
+    def export_to_df(self, prediction) -> pd.DataFrame:
+        """creates a dataframe with the predicted pairs
+
+        Args:
+            prediction (any): Predicted candidate pairs
+
+        Returns:
+            pd.DataFrame: Dataframe with the predicted pairs
+        """
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. \
+                Data object mush have initialized with the ground-truth file")
+        pairs_df = pd.DataFrame(columns=['id1', 'id2'])
+        
+        for entity_id, candidates in prediction.items():
+            id1 = self.data._gt_to_ids_reversed_1[entity_id]                                            
+            for candiadate_id in candidates:
+                id2 = self.data._gt_to_ids_reversed_1[candiadate_id] if self.data.is_dirty_er \
+                        else self.data._gt_to_ids_reversed_2[candiadate_id]
+                pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
+
+        return pairs_df
+
+
 class AbstractMetablocking(AbstractComparisonCleaning, ABC):
     """Restructure a redundancy-positive block collection into a new
         one that contains substantially lower number of redundant
         and superfluous comparisons, while maintaining the original number of matching ones
     """
 
     def __init__(self) -> None:
```

### Comparing `pyjedai-0.0.8/src/pyjedai/datamodel.py` & `pyjedai-0.0.9/src/pyjedai/datamodel.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/src/pyjedai/evaluation.py` & `pyjedai-0.0.9/src/pyjedai/evaluation.py`

 * *Files 14% similar despite different names*

```diff
@@ -378,71 +378,7 @@
             self._matchers_auc_roc_data.append((matcher_name, normalized_auc, cumulative_recall))
             matcher_prediction_data.set_total_emissions(self._total_emissions)
             matcher_prediction_data.set_normalized_auc(normalized_auc)
             matcher_prediction_data.set_cumulative_recall(cumulative_recall[-1])
             progressive_matcher.set_prediction_data(matcher_prediction_data)
 
         self.visualize_roc(methods_data = self._matchers_auc_roc_data, proportional = proportional)
-
-def write(
-        prediction: any,
-        data: Data
-    ) -> pd.DataFrame:
-    """creates a dataframe for the evaluation report
-
-    Args:
-        prediction (any): Predicted pairs, blocks, candidate pairs or graph
-        data (Data): initial dataset
-
-    Returns:
-        pd.DataFrame: Dataframe containg evaluation scores and stats
-    """
-    if data.ground_truth is None:
-        raise AttributeError("Can not proceed to evaluation without a ground-truth file. \
-            Data object mush have initialized with the ground-truth file")
-    pairs_df = pd.DataFrame(columns=['id1', 'id2'])
-    if isinstance(prediction, list): # clusters evaluation
-        for cluster in prediction:
-            lcluster = list(cluster)
-            for i1 in range(0, len(lcluster)):
-                for i2 in range(i1+1, len(lcluster)):
-                    id1 = data._gt_to_ids_reversed_1[lcluster[i1]]
-                    id2 = data._gt_to_ids_reversed_1[lcluster[i2]] if data.is_dirty_er \
-                            else data._gt_to_ids_reversed_2[lcluster[i2]]
-                    pairs_df = pd.concat(
-                        [pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], 
-                        ignore_index=True
-                    )
-    elif 'Block' in str(type(list(prediction.values())[0])): # blocks evaluation
-        for _, block in prediction.items():
-            if data.is_dirty_er:
-                lblock = list(block.entities_D1)
-                for i1 in range(0, len(lblock)):
-                    for i2 in range(i1+1, len(lblock)):
-                        id1 = data._gt_to_ids_reversed_1[lblock[i1]]
-                        id2 = data._gt_to_ids_reversed_1[lblock[i2]] if data.is_dirty_er \
-                            else data._gt_to_ids_reversed_2[lblock[i2]]
-                        pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
-            else:
-                for i1 in block.entities_D1:
-                    for i2 in block.entities_D2:
-                        id1 = data._gt_to_ids_reversed_1[i1]
-                        id2 = data._gt_to_ids_reversed_1[i2] if data.is_dirty_er \
-                            else data._gt_to_ids_reversed_2[i2]
-                        pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
-    elif isinstance(prediction, dict) and isinstance(list(prediction.values())[0], set):# candidate pairs
-        for entity_id, candidates in prediction:
-            id1 = data._gt_to_ids_reversed_1[entity_id]                                            
-            for candiadate_id in candidates:
-                id2 = data._gt_to_ids_reversed_1[candiadate_id] if data.is_dirty_er \
-                        else data._gt_to_ids_reversed_2[candiadate_id]
-                pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
-    elif isinstance(prediction, nx.Graph): # graph
-        for edge in prediction.edges:
-            id1 = data._gt_to_ids_reversed_1[edge[0]]
-            id2 = data._gt_to_ids_reversed_1[edge[1]] if data.is_dirty_er \
-                        else data._gt_to_ids_reversed_2[edge[1]]
-            pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
-    else:
-        raise TypeError("Not supported type")
-
-    return pairs_df
```

### Comparing `pyjedai-0.0.8/src/pyjedai/joins.py` & `pyjedai-0.0.9/src/pyjedai/joins.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,25 +264,46 @@
                         export_to_dict,
                         with_classification_report,
                         verbose)
         
     def stats(self) -> None:
         pass
 
-    def stats(self) -> None:
-        pass
-
     def _configuration(self) -> dict:
         return {
             "similarity_threshold" : self.similarity_threshold,
             "metric" : self.metric,
             "tokenization" : self.tokenization,
             "qgrams": self.qgrams
         }    
 
+    def export_to_df(self, prediction) -> pd.DataFrame:
+        """creates a dataframe with the predicted pairs
+
+        Args:
+            prediction (any): Predicted candidate pairs
+
+        Returns:
+            pd.DataFrame: Dataframe with the predicted pairs
+        """
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. \
+                Data object mush have initialized with the ground-truth file")
+        pairs_df = pd.DataFrame(columns=['id1', 'id2'])
+        for edge in prediction.edges:
+            id1 = self.data._gt_to_ids_reversed_1[edge[0]]
+            id2 = self.data._gt_to_ids_reversed_1[edge[1]] if self.data.is_dirty_er \
+                        else self.data._gt_to_ids_reversed_2[edge[1]]
+            pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
+
+        return pairs_df
+
+    
+    
+    
 class EJoin(AbstractJoin):
     """
      E Join algorithm
     """
     _method_name = "EJoin"
     _method_info = " EJoin algorithm"
     _method_short_name = "EJ"
```

### Comparing `pyjedai-0.0.8/src/pyjedai/logs.py` & `pyjedai-0.0.9/src/pyjedai/logs.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/src/pyjedai/matching.py` & `pyjedai-0.0.9/src/pyjedai/matching.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Entity Matching Module
 """
 import statistics
+import pandas as pd
 from time import time
 
 import matplotlib.pyplot as plt
 import numpy as np
 from networkx import Graph
 from py_stringmatching.similarity_measure.cosine import Cosine
 from py_stringmatching.similarity_measure.dice import Dice
@@ -14,53 +15,46 @@
 from py_stringmatching.similarity_measure.jaro import Jaro
 from py_stringmatching.similarity_measure.levenshtein import Levenshtein
 from py_stringmatching.similarity_measure.overlap_coefficient import \
     OverlapCoefficient
 from py_stringmatching.tokenizer.qgram_tokenizer import QgramTokenizer
 from py_stringmatching.tokenizer.whitespace_tokenizer import \
     WhitespaceTokenizer
-from scipy.spatial.distance import dice, jaccard
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 from sklearn.metrics.pairwise import pairwise_distances
 from tqdm.autonotebook import tqdm
-from whoosh.scoring import BM25F, PL2, TF_IDF, Frequency
 
 from .datamodel import Data, PYJEDAIFeature
 from .evaluation import Evaluation
 from .utils import WordQgramTokenizer, cosine, get_qgram_from_tokenizer_name
 
-# Package import from https://anhaidgroup.github.io/py_stringmatching/v0.4.2/index.html
 
 metrics_mapping = {
     'edit_distance': Levenshtein(),
     'cosine' : Cosine(),
     'jaro' : Jaro(),
     'jaccard' : Jaccard(),
     'generalized_jaccard' : GeneralizedJaccard(),
     'dice': Dice(),
     'overlap_coefficient' : OverlapCoefficient(),
-    'TF-IDF' : TF_IDF(),
-    'Frequency' : Frequency(),
-    'PL2' : PL2(),
-    'BM25F' : BM25F()
 }
 
 vector_metrics_mapping = {
     'cosine': cosine
 }
 
 string_metrics = [
     'jaro', 'edit_distance'
 ]
 
 set_metrics = [
     'cosine', 'dice', 'generalized_jaccard', 'jaccard', 'overlap_coefficient'
 ]
 
-vector_metrics = [
+vector_metrics = [ 
     'cosine', 'dice', 'jaccard'
 ]
 
 whoosh_index_metrics = [
     'TF-IDF', 'Frequency', 'PL2', 'BM25F'
 ] 
 
@@ -291,29 +285,51 @@
                                 export_to_dict,
                                 with_classification_report,
                                 verbose)
         
     def stats(self) -> None:
         pass
     
-    def export_pairs(self, filename: str, with_similarity: bool = True) -> None:
+    def export_pairs_to_csv(self, filename: str, with_similarity: bool = True) -> None:
         if self.pairs is None:
             raise AttributeError("Pairs have not been initialized yet. " +
                                  "Please run the method `run` first.")
 
         with open(filename, 'w') as f:
             for e1, e2, similarity in self.pairs.edges(data='weight'):
                 e1 = self.data._ids_mapping_1[e1] if e1 < self.data.dataset_limit else self.data._ids_mapping_2[e1]
                 e2 = self.data._ids_mapping_1[e2] if e2 < self.data.dataset_limit else self.data._ids_mapping_2[e2]
                 if with_similarity:
                     f.write(f"{e1}, {e2}, {similarity}\n")
                 else:
                     f.write(f"{e1}, {e2}\n")
             f.close()
 
+    def export_to_df(self, prediction: Graph) -> pd.DataFrame:
+        """creates a dataframe with the predicted pairs
+
+        Args:
+            prediction (any): Predicted graph
+
+        Returns:
+            pd.DataFrame: Dataframe with the predicted pairs
+        """
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. \
+                Data object mush have initialized with the ground-truth file")
+        pairs_df = pd.DataFrame(columns=['id1', 'id2'])
+        for edge in prediction.edges:
+            id1 = self.data._gt_to_ids_reversed_1[edge[0]]
+            id2 = self.data._gt_to_ids_reversed_1[edge[1]] if self.data.is_dirty_er \
+                        else self.data._gt_to_ids_reversed_2[edge[1]]
+            pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
+
+        return pairs_df
+
+
 class EntityMatching(AbstractEntityMatching):
     """Calculates similarity from 0.0 to 1.0 for all blocks
     """
 
     _method_name: str = "Entity Matching"
     _method_info: str = "Calculates similarity from 0. to 1. for all blocks"
```

### Comparing `pyjedai-0.0.8/src/pyjedai/prioritization.py` & `pyjedai-0.0.9/src/pyjedai/prioritization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/src/pyjedai/utils.py` & `pyjedai-0.0.9/src/pyjedai/utils.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/src/pyjedai/vector_based_blocking.py` & `pyjedai-0.0.9/src/pyjedai/vector_based_blocking.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 and then performing NNs methods for cluster formation.
 '''
 import os
 import pickle
 import re
 import sys
 import warnings
+import pandas as pd
 from time import time
 from typing import List, Tuple
 
 import faiss
 import gensim.downloader as api
 import networkx as nx
 import numpy as np
@@ -388,15 +389,18 @@
 
         if self.simiarity_distance == 'cosine':
             faiss.normalize_L2(self.vectors_1)
             faiss.normalize_L2(self.vectors_2)
         
         self.distances, self.neighbors = index.search(self.vectors_1 if self.data.is_dirty_er else self.vectors_2,
                                     self.top_k)
-        
+
+        if self.simiarity_distance == 'euclidean':
+            self.distances = 1/(1 + self.distances)
+
         self.blocks = dict()
         
         for _entity in range(0, self.neighbors.shape[0]):
             
             _entity_id = self._si.d1_retained_ids[_entity] if self.data.is_dirty_er else self._si.d2_retained_ids[_entity]
             
             if _entity_id not in self.blocks:
@@ -415,42 +419,18 @@
                 self.blocks[_neighbor_id].add(_entity_id)
                 self.blocks[_entity_id].add(_neighbor_id)
                 
                 if self.with_entity_matching:
                     self.graph.add_edge(_entity_id, _neighbor_id, weight=self.distances[_entity][_neighbor_index])
 
     def _similarity_search_with_FALCONN(self):
-        pass
+        raise NotImplementedError("FALCONN is not implemented yet.")
 
     def _similarity_search_with_SCANN(self):
-        if not LINUX_ENV:
-            raise ImportError("Can't use SCANN in windows environment. Use FAISS instead.")
-
-        searcher = scann.scann_ops_pybind.builder(self.vectors_1,
-                                                    num_neighbors=self.top_k, 
-                                                    distance_measure="dot_product") \
-                                        .tree(num_leaves=2000, num_leaves_to_search=100, training_sample_size=250000) \
-                                        .score_ah(2, anisotropic_quantization_threshold=0.2) \
-                                        .reorder(100) \
-                                        .build()
-
-        self.neighbors, self.distances = searcher.search_batched(
-            self.vectors_1 if self.data.is_dirty_er else self.vectors_2,
-            final_num_neighbors=self.top_k
-        )
-        if self.data.is_dirty_er:
-            self.blocks = {
-                self._si.d1_retained_ids[i] : set(x for x in self.neighbors[i] if x not in [-1, i]) \
-                        for i in range(0, self.neighbors.shape[0])
-            }
-        else:
-            self.blocks = {
-                self._si.d2_retained_ids[i] : set(x for x in self.neighbors[i] if x != -1) \
-                        for i in range(0, self.neighbors.shape[0])
-            }
+        raise NotImplementedError("SCANN is not implemented yet.")
 
     def _create_vector(self, tokens: List[str], vocabulary) -> np.array:
         num_of_tokens = 0
         vector = np.zeros(self.vector_size)
         for token in tokens.split():
             if token in vocabulary:
                 vector += vocabulary[token]
@@ -520,8 +500,31 @@
                 "\n\tIndices shape returned after search: " + str(self.neighbors.shape)
             )
         elif self.similarity_search == 'falconn':           
             pass
         elif self.similarity_search == 'scann'  and LINUX_ENV:
             pass
         
-        print(u'\u2500' * 123)
+        print(u'\u2500' * 123)
+        
+    
+    def export_to_df(self, prediction) -> pd.DataFrame:
+        """creates a dataframe with the predicted pairs
+
+        Args:
+            prediction (any): Predicted candidate pairs
+
+        Returns:
+            pd.DataFrame: Dataframe with the predicted pairs
+        """
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. \
+                Data object mush have initialized with the ground-truth file")
+        pairs_df = pd.DataFrame(columns=['id1', 'id2'])
+        for entity_id, candidates in prediction:
+            id1 = self.data._gt_to_ids_reversed_1[entity_id]                                            
+            for candiadate_id in candidates:
+                id2 = self.data._gt_to_ids_reversed_1[candiadate_id] if self.data.is_dirty_er \
+                        else self.data._gt_to_ids_reversed_2[candiadate_id]
+                pairs_df = pd.concat([pairs_df, pd.DataFrame([{'id1':id1, 'id2':id2}], index=[0])], ignore_index=True)
+
+        return pairs_df
```

### Comparing `pyjedai-0.0.8/src/pyjedai/visualization.py` & `pyjedai-0.0.9/src/pyjedai/visualization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/src/pyjedai/workflow.py` & `pyjedai-0.0.9/src/pyjedai/workflow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,181 +1,59 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 from itertools import count
 from time import time
 from typing import Callable, List, Tuple
 
 import matplotlib.pyplot as plt
 import optuna
 import pandas as pd
 from networkx import Graph
-# import plotly.express as px
 from tqdm.autonotebook import tqdm
 
 from .datamodel import Data
-from .evaluation import Evaluation, write
+from .evaluation import Evaluation
 from .block_building import StandardBlocking
 from .block_cleaning import BlockFiltering, BlockPurging
-from .comparison_cleaning import CardinalityNodePruning
+from .comparison_cleaning import *
 from .matching import EntityMatching
 from .clustering import ConnectedComponentsClustering, UniqueMappingClustering
+from .vector_based_blocking import EmbeddingsNNBlockBuilding
+from .joins import EJoin, TopKJoin
 
 plt.style.use('seaborn-whitegrid')
 
-class WorkFlow(ABC):
+class PYJEDAIWorkFlow(ABC):
     """Main module of the pyjedAI and the simplest way to create an end-to-end ER workflow.
     """
 
     _id = count()
 
     def __init__(
             self,
-            block_building: dict = None,
-            entity_matching: dict = None,
-            block_cleaning: dict = None,
-            comparison_cleaning: dict = None,
-            clustering: dict = None,
-            joins: dict = None,
             name: str = None
     ) -> None:
-        self.block_cleaning, self.block_building, self.comparison_cleaning, \
-            self.clustering, self.joins, self.entity_matching = \
-            block_cleaning, block_building, comparison_cleaning, clustering, joins, entity_matching
         self.f1: list = []
         self.recall: list = []
         self.precision: list = []
         self.runtime: list = []
         self.configurations: list = []
         self.workflow_exec_time: float
         self._id: int = next(self._id)
         self.name: str = name if name else "Workflow-" + str(self._id)
         self._workflow_bar: tqdm
         self.final_pairs = None
 
+    @abstractmethod
     def run(self,
             data: Data,
             verbose: bool = False,
             with_classification_report: bool = False,
             workflow_step_tqdm_disable: bool = True,
-            workflow_tqdm_enable: bool = False
-        ) -> None:
-        """Main function for creating an Entity resolution workflow.
-
-        Args:
-            data (Data): Dataset module.
-            verbose (bool, optional): Print detailed report for each step. Defaults to False.
-            with_classification_report (bool, optional): Print pairs counts. Defaults to False.
-            workflow_step_tqdm_disable (bool, optional):  Tqdm progress bar in each step. Defaults to True.
-            workflow_tqdm_enable (bool, optional): Overall progress bar. Defaults to False.
-        """
-        steps = [self.block_building, self.entity_matching, self.clustering, self.joins, self.block_cleaning, self.comparison_cleaning]
-        num_of_steps = sum(x is not None for x in steps)
-        self._workflow_bar = tqdm(total=num_of_steps,
-                                  desc=self.name,
-                                  disable=not workflow_tqdm_enable)
-        self.data = data
-        self._init_experiment()
-        start_time = time()
-        #
-        # Block building step: Only one algorithm can be performed
-        #
-        block_building_method = self.block_building['method'](**self.block_building["params"]) \
-                                                    if "params" in self.block_building \
-                                                    else self.block_building['method']()
-
-        block_building_blocks = \
-            block_building_method.build_blocks(data,
-                                               attributes_1=self.block_building["attributes_1"] \
-                                                                if "attributes_1" in self.block_building else None,
-                                                attributes_2=self.block_building["attributes_2"] \
-                                                                if "attributes_2" in self.block_building else None,
-                                                tqdm_disable=workflow_step_tqdm_disable)
-        self.final_pairs = block_building_blocks
-        res = block_building_method.evaluate(block_building_blocks,
-                                            export_to_dict=True,
-                                            with_classification_report=with_classification_report,
-                                            verbose=verbose)
-        self._save_step(res, block_building_method.method_configuration())
-        self._workflow_bar.update(1)
-        #
-        # Block cleaning step [optional]: Multiple algorithms
-        #
-        block_cleaning_blocks = None
-        if self.block_cleaning:
-            if isinstance(self.block_cleaning, dict):
-                self.block_cleaning = list(self.block_cleaning)
-            bblocks = block_building_blocks
-            for block_cleaning in self.block_cleaning:
-                block_cleaning_method = block_cleaning['method'](**block_cleaning["params"]) \
-                                                    if "params" in block_cleaning \
-                                                    else block_cleaning['method']()
-                block_cleaning_blocks = block_cleaning_method.process(bblocks,
-                                                                      data,
-                                                                      tqdm_disable=workflow_step_tqdm_disable)
-                
-                self.final_pairs = bblocks = block_cleaning_blocks
-                res = block_cleaning_method.evaluate(bblocks,
-                                                    export_to_dict=True,
-                                                    with_classification_report=with_classification_report,
-                                                    verbose=verbose)
-                self._save_step(res, block_cleaning_method.method_configuration())
-                self._workflow_bar.update(1)
-        #
-        # Comparison cleaning step [optional]
-        #
-        comparison_cleaning_blocks = None
-        if self.comparison_cleaning:
-            comparison_cleaning_method = self.comparison_cleaning['method'](**self.comparison_cleaning["params"]) \
-                                            if "params" in self.comparison_cleaning \
-                                            else self.comparison_cleaning['method']()
-            self.final_pairs = \
-            comparison_cleaning_blocks = \
-            comparison_cleaning_method.process(block_cleaning_blocks if block_cleaning_blocks is not None \
-                                                    else block_building_blocks,
-                                                data,
-                                                tqdm_disable=workflow_step_tqdm_disable)
-            res = comparison_cleaning_method.evaluate(comparison_cleaning_blocks,
-                                                      export_to_dict=True,
-                                                      with_classification_report=with_classification_report,
-                                                      verbose=verbose)
-            self._save_step(res, comparison_cleaning_method.method_configuration())
-            self._workflow_bar.update(1)
-        #
-        # Entity Matching step
-        #
-        entity_matching_method = self.entity_matching['method'](**self.entity_matching["params"]) \
-                                        if "params" in self.entity_matching \
-                                        else self.entity_matching['method']()
-        self.final_pairs = em_graph = entity_matching_method.predict(
-            comparison_cleaning_blocks if comparison_cleaning_blocks is not None \
-                else block_building_blocks,
-            data,
-            tqdm_disable=workflow_step_tqdm_disable
-        )
-        res = entity_matching_method.evaluate(em_graph,
-                                                export_to_dict=True,
-                                                with_classification_report=with_classification_report,
-                                                verbose=verbose)
-        self._save_step(res, entity_matching_method.method_configuration())
-        self._workflow_bar.update(1)
-        #
-        # Clustering step [optional]
-        #
-        if self.clustering:
-            clustering_method = self.clustering['method'](**self.clustering["params"]) \
-                                            if "params" in self.clustering \
-                                            else self.clustering['method']()
-            self.final_pairs = components = clustering_method.process(em_graph, data)
-            res = clustering_method.evaluate(components,
-                                            export_to_dict=True,
-                                            with_classification_report=False,
-                                            verbose=verbose)
-            self._save_step(res, clustering_method.method_configuration())
-            self.workflow_exec_time = time() - start_time
-            self._workflow_bar.update(1)
-        # self.runtime.append(self.workflow_exec_time)
+            workflow_tqdm_enable: bool = False) -> None:
+        pass
 
     def _init_experiment(self) -> None:
         self.f1: list = []
         self.recall: list = []
         self.precision: list = []
         self.runtime: list = []
         self.configurations: list = []
@@ -323,19 +201,19 @@
         """Final scores in the last step of the workflow.
 
         Returns:
             Tuple[float, float, float]: F-Measure, Precision, Recall.
         """
         return self.f1[-1], self.precision[-1], self.recall[-1]
 
-def compare_workflows(workflows: List[WorkFlow], with_visualization=True) -> pd.DataFrame:
+def compare_workflows(workflows: List[PYJEDAIWorkFlow], with_visualization=True) -> pd.DataFrame:
     """Compares workflows by creating multiple plots and tables with results.
 
     Args:
-        workflows (List[WorkFlow]): Different workflows
+        workflows (List[PYJEDAIWorkFlow]): Different workflows
         with_visualization (bool, optional): Diagram generation. Defaults to True.
 
     Returns:
         pd.DataFrame: Results
     """
     workflow_df = pd.DataFrame(columns=['Name', 'F1', 'Recall', 'Precision', 'Runtime (sec)'])
     if with_visualization:
@@ -370,129 +248,14 @@
         axs[1, 0].bar(workflow_df['Name'], workflow_df['F1'], color='orange')
         axs[1, 1].bar(workflow_df['Name'], workflow_df['Runtime (sec)'], color='r')
     fig.autofmt_xdate()
     plt.show()
 
     return workflow_df
 
-
-############################################
-#  Pre-defined workflows same as JedAI     #
-############################################
-
-def get_best_blocking_workflow_ccer() -> WorkFlow:
-    """Best CC-ER workflow.
-
-    Returns:
-        WorkFlow: Best workflow
-    """
-    return WorkFlow(
-        block_building = dict(
-            method=StandardBlocking
-        ),
-        block_cleaning = [
-            dict(
-                method=BlockPurging,
-                params=dict(smoothing_factor=1.0)
-            ),
-            dict(
-                method=BlockFiltering
-            )
-
-        ],
-        comparison_cleaning = dict(method=CardinalityNodePruning),
-        entity_matching = dict(
-            method=EntityMatching,
-            metric='cosine',
-            similarity_threshold=0.55
-        ),
-        clustering = dict(
-            method=ConnectedComponentsClustering
-        ),
-        name="best-ccer-workflow"
-    )
-
-def get_best_blocking_workflow_der():
-    """Best D-ER workflow.
-
-    Returns:
-        WorkFlow: Best workflow
-    """
-    return WorkFlow(
-        block_building = dict(
-            method=StandardBlocking
-        ),
-        block_cleaning = [
-            dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
-            dict(method=BlockFiltering)
-        ],
-        comparison_cleaning = dict(method=CardinalityNodePruning,
-                                   params=dict(weighting_scheme='JS')),
-        entity_matching = dict(method=EntityMatching, 
-                               params=dict(metric='cosine',
-                                           similarity_threshold=0.55)),
-        clustering = dict(method=ConnectedComponentsClustering),
-        name="best-der-workflow"
-    )
-
-def get_default_blocking_workflow_ccer():
-    """Default CC-ER workflow.
-
-    Returns:
-        WorkFlow: Default workflow
-    """
-    return WorkFlow(
-        block_building = dict(
-            method=StandardBlocking
-        ),
-        block_cleaning = [
-            dict(
-                method=BlockPurging,
-                params=dict(smoothing_factor=1.0)
-            ),
-            dict(
-                method=BlockFiltering
-            )
-
-        ],
-        comparison_cleaning = dict(method=CardinalityNodePruning),
-        entity_matching = dict(
-            method=EntityMatching,
-            metric='cosine',
-            similarity_threshold=0.55
-        ),
-        clustering = dict(
-            method=UniqueMappingClustering
-        ),
-        name="default-ccer-workflow"
-    )
-
-def get_default_blocking_workflow_der():
-    """Default D-ER workflow.
-
-    Returns:
-        WorkFlow: Best workflow
-    """
-    return WorkFlow(
-        block_building = dict(
-            method=StandardBlocking
-        ),
-        block_cleaning = [
-            dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
-            dict(method=BlockFiltering)
-        ],
-        comparison_cleaning = dict(method=CardinalityNodePruning, 
-                                   params=dict(weighting_scheme='JS')),
-        entity_matching = dict(method=EntityMatching,
-                               params=dict(metric='cosine',
-                                           similarity_threshold=0.55)),
-        name="default-der-workflow"
-    )
-
-
 class OptimizeWorkflow:
     """Optuna Framework for GridSearch/RandomSearch/Prunning in a given pyjedai workflow.
     """
 
     _id = count()
 
     def __init__(
@@ -584,7 +347,334 @@
         pass
     
     def get_best_trial(self):
         pass
     
     def to_df():
         pass
+
+class BlockingBasedWorkFlow(PYJEDAIWorkFlow):
+    """Blocking-based workflow.
+    """
+
+    def __init__(
+            self,
+            block_building: dict = None,
+            entity_matching: dict = None,
+            block_cleaning: dict = None,
+            comparison_cleaning: dict = None,
+            clustering: dict = None,
+            joins: dict = None,
+            name: str = None
+    ) -> None:
+        super().__init__()
+        self.block_cleaning, self.block_building, self.comparison_cleaning, \
+            self.clustering, self.joins, self.entity_matching = \
+            block_cleaning, block_building, comparison_cleaning, clustering, joins, entity_matching
+        self.name: str = name if name else "BlockingBasedWorkFlow-" + str(self._id)
+
+    def run(self,
+            data: Data,
+            verbose: bool = False,
+            with_classification_report: bool = False,
+            workflow_step_tqdm_disable: bool = True,
+            workflow_tqdm_enable: bool = False
+        ) -> None:
+        """Main function for creating an Entity resolution workflow.
+
+        Args:
+            data (Data): Dataset module.
+            verbose (bool, optional): Print detailed report for each step. Defaults to False.
+            with_classification_report (bool, optional): Print pairs counts. Defaults to False.
+            workflow_step_tqdm_disable (bool, optional):  Tqdm progress bar in each step. Defaults to True.
+            workflow_tqdm_enable (bool, optional): Overall progress bar. Defaults to False.
+        """
+        steps = [self.block_building, self.entity_matching, self.clustering, self.joins, self.block_cleaning, self.comparison_cleaning]
+        num_of_steps = sum(x is not None for x in steps)
+        self._workflow_bar = tqdm(total=num_of_steps,
+                                  desc=self.name,
+                                  disable=not workflow_tqdm_enable)
+        self.data = data
+        self._init_experiment()
+        start_time = time()
+        #
+        # Block building step: Only one algorithm can be performed
+        #
+        block_building_method = self.block_building['method'](**self.block_building["params"]) \
+                                                    if "params" in self.block_building \
+                                                    else self.block_building['method']()
+
+        block_building_blocks = \
+            block_building_method.build_blocks(data,
+                                               attributes_1=self.block_building["attributes_1"] \
+                                                                if "attributes_1" in self.block_building else None,
+                                                attributes_2=self.block_building["attributes_2"] \
+                                                                if "attributes_2" in self.block_building else None,
+                                                tqdm_disable=workflow_step_tqdm_disable)
+        self.final_pairs = block_building_blocks
+        res = block_building_method.evaluate(block_building_blocks,
+                                            export_to_dict=True,
+                                            with_classification_report=with_classification_report,
+                                            verbose=verbose)
+        self._save_step(res, block_building_method.method_configuration())
+        self._workflow_bar.update(1)
+        #
+        # Block cleaning step [optional]: Multiple algorithms
+        #
+        block_cleaning_blocks = None
+        if self.block_cleaning:
+            if isinstance(self.block_cleaning, dict):
+                self.block_cleaning = list(self.block_cleaning)
+            bblocks = block_building_blocks
+            for block_cleaning in self.block_cleaning:
+                block_cleaning_method = block_cleaning['method'](**block_cleaning["params"]) \
+                                                    if "params" in block_cleaning \
+                                                    else block_cleaning['method']()
+                block_cleaning_blocks = block_cleaning_method.process(bblocks,
+                                                                      data,
+                                                                      tqdm_disable=workflow_step_tqdm_disable)
+                
+                self.final_pairs = bblocks = block_cleaning_blocks
+                res = block_cleaning_method.evaluate(bblocks,
+                                                    export_to_dict=True,
+                                                    with_classification_report=with_classification_report,
+                                                    verbose=verbose)
+                self._save_step(res, block_cleaning_method.method_configuration())
+                self._workflow_bar.update(1)
+        #
+        # Comparison cleaning step [optional]
+        #
+        comparison_cleaning_blocks = None
+        if self.comparison_cleaning:
+            comparison_cleaning_method = self.comparison_cleaning['method'](**self.comparison_cleaning["params"]) \
+                                            if "params" in self.comparison_cleaning \
+                                            else self.comparison_cleaning['method']()
+            self.final_pairs = \
+            comparison_cleaning_blocks = \
+            comparison_cleaning_method.process(block_cleaning_blocks if block_cleaning_blocks is not None \
+                                                    else block_building_blocks,
+                                                data,
+                                                tqdm_disable=workflow_step_tqdm_disable)
+            res = comparison_cleaning_method.evaluate(comparison_cleaning_blocks,
+                                                      export_to_dict=True,
+                                                      with_classification_report=with_classification_report,
+                                                      verbose=verbose)
+            self._save_step(res, comparison_cleaning_method.method_configuration())
+            self._workflow_bar.update(1)
+        #
+        # Entity Matching step
+        #
+        entity_matching_method = self.entity_matching['method'](**self.entity_matching["params"]) \
+                                        if "params" in self.entity_matching \
+                                        else self.entity_matching['method']()
+                                        
+        if "exec_params" not in self.entity_matching:
+            self.final_pairs = em_graph = entity_matching_method.predict(
+                comparison_cleaning_blocks if comparison_cleaning_blocks is not None \
+                    else block_building_blocks,
+                data,
+                tqdm_disable=workflow_step_tqdm_disable)
+        else:
+            self.final_pairs = em_graph = entity_matching_method.predict(
+                comparison_cleaning_blocks if comparison_cleaning_blocks is not None \
+                    else block_building_blocks,
+                data,
+                tqdm_disable=workflow_step_tqdm_disable,
+                **self.entity_matching["exec_params"])
+
+        res = entity_matching_method.evaluate(em_graph,
+                                                export_to_dict=True,
+                                                with_classification_report=with_classification_report,
+                                                verbose=verbose)
+        self._save_step(res, entity_matching_method.method_configuration())
+        self._workflow_bar.update(1)
+        #
+        # Clustering step [optional]
+        #
+        if self.clustering:
+            clustering_method = self.clustering['method'](**self.clustering["params"]) \
+                                            if "params" in self.clustering \
+                                            else self.clustering['method']()
+            if "exec_params" not in self.clustering:
+                self.final_pairs = components = clustering_method.process(em_graph, data)
+            else:
+                self.final_pairs = components = clustering_method.process(em_graph, data, **self.clustering["exec_params"])
+            
+            res = clustering_method.evaluate(components,
+                                            export_to_dict=True,
+                                            with_classification_report=False,
+                                            verbose=verbose)
+            self._save_step(res, clustering_method.method_configuration())
+            self.workflow_exec_time = time() - start_time
+            self._workflow_bar.update(1)
+        # self.runtime.append(self.workflow_exec_time)
+
+    ############################################
+    #  Pre-defined workflows same as JedAI     #
+    ############################################
+
+    def best_blocking_workflow_ccer(self) -> None:
+        """Best CC-ER workflow.
+
+        Returns:
+            PYJEDAIWorkFlow: Best workflow
+        """
+        self.block_building = dict(method=StandardBlocking)
+        self.block_cleaning = [dict(
+            method=BlockFiltering,
+            params=dict(ratio=0.9)
+        )]
+        self.comparison_cleaning = dict(method=WeightedEdgePruning, params=dict(weighting_scheme='EJS'))
+        self.entity_matching = dict(method=EntityMatching,
+                                    params=dict(metric='cosine',
+                                                     tokenizer='tfidf_char_3gram', 
+                                                     similarity_threshold=0.0))
+        self.clustering = dict(method=UniqueMappingClustering, 
+                               exec_params=dict(similarity_threshold=0.17))
+        self.name="best-ccer-workflow"
+
+    def best_blocking_workflow_der(self) -> None:
+        """Best D-ER workflow.
+
+        Returns:
+            PYJEDAIWorkFlow: Best workflow
+        """
+        self.block_building = dict(method=StandardBlocking)
+        self.block_cleaning = [
+            dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
+            dict(method=BlockFiltering)
+        ]
+        self.comparison_cleaning = dict(method=CardinalityNodePruning,
+                                    params=dict(weighting_scheme='JS'))
+        self.entity_matching = dict(method=EntityMatching, 
+                                    params=dict(metric='cosine',
+                                                similarity_threshold=0.55))
+        self.clustering = dict(method=ConnectedComponentsClustering),
+        self.name="best-der-workflow"
+
+    def default_blocking_workflow_ccer(self) -> None:
+        """Default CC-ER workflow.
+        """
+        self.block_building = dict(method=StandardBlocking)
+        self.block_cleaning = [
+                dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
+                dict(method=BlockFiltering)
+            ]
+        self.comparison_cleaning = dict(method=CardinalityNodePruning)
+        self.entity_matching = dict(method=EntityMatching,
+                                    metric='cosine',
+                                    similarity_threshold=0.55)
+        self.clustering = dict(method=UniqueMappingClustering)
+        self.name="default-ccer-workflow"
+
+    def default_blocking_workflow_der(self) -> None:
+        """Default D-ER workflow.
+
+        Returns:
+            PYJEDAIWorkFlow: Best workflow
+        """
+        self.block_building = dict(method=StandardBlocking)
+        self.block_cleaning = [
+                dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
+                dict(method=BlockFiltering)
+        ]
+        self.comparison_cleaning = dict(method=CardinalityNodePruning, 
+                                        params=dict(weighting_scheme='JS'))
+        self.entity_matching = dict(method=EntityMatching,
+                                    params=dict(metric='cosine', 
+                                                similarity_threshold=0.55))
+        self.name="default-der-workflow"
+ 
+class EmbeddingsNNWorkFlow(PYJEDAIWorkFlow):
+    """Blocking-based workflow.
+    """
+
+    def __init__(
+            self,
+            block_building: dict,
+            clustering: dict = None,
+            name: str = None
+    ) -> None:
+        super().__init__()
+        self.block_building, self.clustering = block_building, clustering
+        self.name: str = name if name else "Workflow-" + str(self._id)
+
+    def run(self,
+            data: Data,
+            verbose: bool = False,
+            with_classification_report: bool = False,
+            workflow_step_tqdm_disable: bool = False,
+            workflow_tqdm_enable: bool = False
+        ) -> None:
+        """Main function for creating an Entity resolution workflow.
+
+        Args:
+            data (Data): Dataset module.
+            verbose (bool, optional): Print detailed report for each step. Defaults to False.
+            with_classification_report (bool, optional): Print pairs counts. Defaults to False.
+            workflow_step_tqdm_disable (bool, optional):  Tqdm progress bar in each step. Defaults to True.
+            workflow_tqdm_enable (bool, optional): Overall progress bar. Defaults to False.
+        """
+        steps = [self.block_building, self.clustering]
+        num_of_steps = sum(x is not None for x in steps)
+        self._workflow_bar = tqdm(total=num_of_steps,
+                                  desc=self.name,
+                                  disable=not workflow_tqdm_enable)
+        self.data = data
+        self._init_experiment()
+        start_time = time()
+        #
+        # Block building step: Only one algorithm can be performed
+        #
+        block_building_method = self.block_building['method'](**self.block_building["params"]) \
+                                                    if "params" in self.block_building \
+                                                    else self.block_building['method']()
+
+        
+        if "exec_params" not in self.block_building:
+            block_building_blocks, em_graph = \
+                block_building_method.build_blocks(data,
+                                            attributes_1=self.block_building["attributes_1"] \
+                                                                if "attributes_1" in self.block_building else None,
+                                                attributes_2=self.block_building["attributes_2"] \
+                                                                if "attributes_2" in self.block_building else None,
+                                                tqdm_disable=workflow_step_tqdm_disable)
+        else:
+            block_building_blocks, em_graph = \
+                block_building_method.build_blocks(data, 
+                                                   attributes_1=self.block_building["attributes_1"] \
+                                                                if "attributes_1" in self.block_building else None,
+                                                    attributes_2=self.block_building["attributes_2"] \
+                                                                if "attributes_2" in self.block_building else None,
+                                                tqdm_disable=workflow_step_tqdm_disable,
+                                                with_entity_matching=True,
+                                                **self.block_building["exec_params"])                
+
+        self.final_pairs = block_building_blocks
+        res = block_building_method.evaluate(block_building_blocks,
+                                            export_to_dict=True,
+                                            with_classification_report=with_classification_report,
+                                            verbose=verbose)
+        self._save_step(res, block_building_method.method_configuration())
+        self._workflow_bar.update(1)
+        #
+        # Clustering step [optional]
+        #
+        if self.clustering:
+            clustering_method = self.clustering['method'](**self.clustering["params"]) \
+                                            if "params" in self.clustering \
+                                            else self.clustering['method']()
+            self.final_pairs = components = clustering_method.process(em_graph, data)
+            res = clustering_method.evaluate(components,
+                                            export_to_dict=True,
+                                            with_classification_report=False,
+                                            verbose=verbose)
+            self._save_step(res, clustering_method.method_configuration())
+            self.workflow_exec_time = time() - start_time
+            self._workflow_bar.update(1)
+        # self.runtime.append(self.workflow_exec_time)
+
+# class SimilarityJoinsWorkFlow(PYJEDAIWorkFlow):
+#     raise NotImplementedError("Joins workflow is not implemented yet.")
+
+# class ProgressiveWorkFlow(PYJEDAIWorkFlow):
+#     raise NotImplementedError("Progressive workflow is not implemented yet.")
```

### Comparing `pyjedai-0.0.8/src/pyjedai.egg-info/PKG-INFO` & `pyjedai-0.0.9/src/pyjedai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyjedai
-Version: 0.0.8
+Version: 0.0.9
 Summary: An open-source library that builds powerful end-to-end Entity Resolution workflows.
 Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>, Jakub Maciejewski <jacobb.maciejewski@gmail.com>
 License: Apache Software License 2.0
 Project-URL: Homepage, http://pyjedai.rtfd.io
 Project-URL: Documentation, http://pyjedai.rtfd.io
 Project-URL: Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues
 Project-URL: Source code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai
 Keywords: deduplication,entity-resolution,link-discovery
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
@@ -29,24 +30,26 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
     <br>
-    <img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
+    <img align="center" src="https://github.com/AI-team-UoA/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
 </div>
 <br>
 <br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
+
 ---
 
+
 # Overview
 
 pyJedAI is a python framework, aiming to offer experts and novice users, robust and fast solutions for multiple types of Entity Resolution problems. It is builded using state-of-the-art python frameworks. pyJedAI constitutes the sole open-source Link Discovery tool that is capable of exploiting the latest breakthroughs in Deep Learning and NLP techniques, which are publicly available through the Python data science ecosystem. This applies to both blocking and matching, thus ensuring high time efficiency, high scalability as well as high effectiveness, without requiring any labelled instances from the user.
 
 ### Key-Features
 
 - Input data-type independent. Both structured and semi-structured data can be processed.
@@ -54,18 +57,18 @@
 - Easy-to-use.
 - Utilizes some of the famous and cutting-edge machine learning packages.
 - Offers supervised and un-supervised ML techniques.
 
 __Open demos are available in:__
 
 <div align="center">
-    <a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+    <a href="https://nbviewer.org/github/AI-team-UoA/pyJedAI/blob/main/docs/tutorials/Demo.ipynb">
         <img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
     </a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-    <a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+    <a href="https://github.com/AI-team-UoA/pyJedAI/blob/main/docs/tutorials/Demo.ipynb">
         <img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
     </a>
 </div>
 
 __Google Colab Hands-on demo:__ 
 
 <div align="center">
@@ -110,25 +113,33 @@
     <img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
     <img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
 </div>
 <br>
 
-See the full list of dependencies and all versions used, in this [file](https://github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt).
+See the full list of dependencies and all versions used, in this [file](https://github.com/AI-team-UoA/pyJedAI/blob/main/pyproject.toml).
 
-__Status__ 
+__Status__
 
-[![Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml)
+[![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml)
+[![PyPi](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/pypi-publish.yml)
 [![made-with-python](https://readthedocs.org/projects/pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/AI-team-UoA/pyjedai/branch/master/graph/badge.svg?token=4QR0X315CL)](https://codecov.io/gh/AI-team-UoA/pyjedai)
+
+
+__Statistics & Info__
+
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyjedai)
+[![PyPI version](https://img.shields.io/pypi/v/pyjedai.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pyjedai/)
 
 
 # Bugs, Discussions & News
 
-[GitHub Discussions](https://github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues).
+[GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Java - Wed Application 
 
 <img align="left" src="https://github.com/scify/JedAIToolkit/blob/master/documentation/JedAI_logo.png?raw=true" alt="pyJedAI" width="130"/>
 
 For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows. <br><br> JedAI constitutes an open source, high scalability toolkit that offers out-of-the-box solutions for any data integration task, e.g., Record Linkage, Entity Resolution and Link Discovery. At its core lies a set of domain-independent, state-of-the-art techniques that apply to both RDF and relational data.
 
@@ -143,15 +154,15 @@
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
 
 # License
 
-Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE).
+Released under the Apache-2.0 license (see [LICENSE.txt](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)).
 
 Copyright © 2023 AI-Team, University of Athens
 
 <div align="center">
     <hr>
     <br>
     <a href="https://stelar-project.eu">
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: pyjedai Version: 0.0.8 Summary: An open-source
+Metadata-Version: 2.1 Name: pyjedai Version: 0.0.9 Summary: An open-source
 library that builds powerful end-to-end Entity Resolution workflows. Author-
 email: Konstantinos Nikoletos
 kon@gmail.com>, George Papadakis
 gmail.com>, Jakub Maciejewski
 maciejewski@gmail.com> License: Apache Software License 2.0 Project-URL:
 Homepage, http://pyjedai.rtfd.io Project-URL: Documentation, http://
 pyjedai.rtfd.io Project-URL: Bug Tracker, https://github.com/AI-team-UoA/
 pyJedAI/issues Project-URL: Source code, https://github.com/AI-team-UoA/
 pyJedAI/tree/main/pyjedai Keywords: deduplication,entity-resolution,link-
 discovery Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: Implementation
-Classifier: Intended Audience :: Information Technology Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English Classifier: Operating System ::
-Microsoft :: Windows Classifier: Operating System :: Unix Classifier: Operating
-System :: iOS Classifier: Topic :: Database Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: Implementation Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers Classifier: Natural Language ::
+English Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: Unix Classifier: Operating System :: iOS Classifier: Topic
+:: Database Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev License-File: LICENSE
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
@@ -66,39 +67,46 @@
 
  [https://www.kornosk.me/resources/language-model/featured.png]     [https://
    repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-
 745fdcbeffe8]     [https://networkx.org/_static/networkx_logo.svg]     [https:/
           /raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png]
 
 See the full list of dependencies and all versions used, in this [file](https:/
-/github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt). __Status__ [!
-[Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/
-badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
-workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
-pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
-?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
-github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general
-questions and discussions and our recommended starting point. Please report any
-bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues). #
-Java - Wed Application [pyJedAI] For Java users checkout the initial [JedAI]
-(https://github.com/scify/JedAIToolkit). There you can find Java based code and
-a Web Application for interactive creation of ER workflows.
+/github.com/AI-team-UoA/pyJedAI/blob/main/pyproject.toml). __Status__ [![Tests]
+(https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/
+badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/
+workflows/tests.yml) [![PyPi](https://github.com/AI-team-UoA/pyJedAI/actions/
+workflows/pypi-publish.yml/badge.svg)](https://github.com/AI-team-UoA/pyJedAI/
+actions/workflows/pypi-publish.yml) [![made-with-python](https://
+readthedocs.org/projects/pyjedai/badge/?version=latest)](https://
+pyjedai.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
+gh/AI-team-UoA/pyjedai/branch/master/graph/badge.svg?token=4QR0X315CL)](https:/
+/codecov.io/gh/AI-team-UoA/pyjedai) __Statistics & Info__ ![PyPI - Downloads]
+(https://img.shields.io/pypi/dm/pyjedai) [![PyPI version](https://
+img.shields.io/pypi/v/pyjedai.svg?logo=pypi&logoColor=FFE873)](https://
+pypi.org/project/pyjedai/) # Bugs, Discussions & News [GitHub Discussions]
+(https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum
+for general questions and discussions and our recommended starting point.
+Please report any bugs that you find [here](https://github.com/AI-team-UoA/
+pyJedAI/issues). # Java - Wed Application [pyJedAI] For Java users checkout the
+initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java
+based code and a Web Application for interactive creation of ER workflows.
 
 JedAI constitutes an open source, high scalability toolkit that offers out-of-
 the-box solutions for any data integration task, e.g., Record Linkage, Entity
 Resolution and Link Discovery. At its core lies a set of domain-independent,
 state-of-the-art techniques that apply to both RDF and relational data.
 # Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
 k.github.io) - Jakub Maciejewski - [George Papadakis](https://
 gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
 ) Research and development is made under the supervision of Pr. Manolis
 Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
 of the Department of Informatics and Telecommunications at the University of
-Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
-(https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE). Copyright Â© 2023
+Athens. # License Released under the Apache-2.0 license (see [LICENSE.txt]
+(https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)). Copyright Â© 2023
 AI-Team, University of Athens
 ===============================================================================
 
   [https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png]
               [https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/
               Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png]
```

### Comparing `pyjedai-0.0.8/src/pyjedai.egg-info/SOURCES.txt` & `pyjedai-0.0.9/src/pyjedai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/tests/test_block_building.py` & `pyjedai-0.0.9/tests/test_block_building.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/tests/test_block_cleaning.py` & `pyjedai-0.0.9/tests/test_block_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/tests/test_clustering.py` & `pyjedai-0.0.9/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.8/tests/test_comparison_cleaning.py` & `pyjedai-0.0.9/tests/test_comparison_cleaning.py`

 * *Files identical despite different names*

