# Comparing `tmp/project_lighter-0.0.2a8.tar.gz` & `tmp/project_lighter-0.0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_lighter-0.0.2a8.tar", max compression
+gzip compressed data, was "project_lighter-0.0.2a9.tar", max compression
```

## Comparing `project_lighter-0.0.2a8.tar` & `project_lighter-0.0.2a9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1080 2023-07-20 10:02:32.698939 project_lighter-0.0.2a8/LICENSE
--rw-r--r--   0        0        0     2164 2023-07-20 10:02:32.698939 project_lighter-0.0.2a8/README.md
--rw-r--r--   0        0        0       67 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/__init__.py
--rw-r--r--   0        0        0      125 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/__init__.py
--rw-r--r--   0        0        0     6631 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/freezer.py
--rw-r--r--   0        0        0    17459 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/logger.py
--rw-r--r--   0        0        0     6508 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/writer/__init__.py
--rw-r--r--   0        0        0     7593 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/writer/base.py
--rw-r--r--   0        0        0     2662 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/writer/file.py
--rw-r--r--   0        0        0     2427 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/writer/table.py
--rw-r--r--   0        0        0    18288 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/system.py
--rw-r--r--   0        0        0        0 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/__init__.py
--rw-r--r--   0        0        0      627 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/cli.py
--rw-r--r--   0        0        0     2566 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/collate.py
--rw-r--r--   0        0        0     1547 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/dynamic_imports.py
--rw-r--r--   0        0        0     3896 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/misc.py
--rw-r--r--   0        0        0     5736 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/model.py
--rw-r--r--   0        0        0     2483 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/runner.py
--rw-r--r--   0        0        0       24 2023-07-20 10:02:56.247092 project_lighter-0.0.2a8/lighter/version.py
--rw-r--r--   0        0        0     4611 2023-07-20 10:02:56.183091 project_lighter-0.0.2a8/pyproject.toml
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 project_lighter-0.0.2a8/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-20 18:28:38.088984 project_lighter-0.0.2a9/LICENSE
+-rw-r--r--   0        0        0     2395 2023-07-20 18:28:38.088984 project_lighter-0.0.2a9/README.md
+-rw-r--r--   0        0        0       67 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/callbacks/__init__.py
+-rw-r--r--   0        0        0     6631 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/callbacks/freezer.py
+-rw-r--r--   0        0        0    17459 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/callbacks/logger.py
+-rw-r--r--   0        0        0     6508 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/callbacks/writer/__init__.py
+-rw-r--r--   0        0        0     7593 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/callbacks/writer/base.py
+-rw-r--r--   0        0        0     2662 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/callbacks/writer/file.py
+-rw-r--r--   0        0        0     2427 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/callbacks/writer/table.py
+-rw-r--r--   0        0        0    18288 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/system.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/utils/__init__.py
+-rw-r--r--   0        0        0      627 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/utils/cli.py
+-rw-r--r--   0        0        0     2566 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/utils/collate.py
+-rw-r--r--   0        0        0     1547 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/utils/dynamic_imports.py
+-rw-r--r--   0        0        0     3896 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/utils/misc.py
+-rw-r--r--   0        0        0     5736 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/utils/model.py
+-rw-r--r--   0        0        0     2483 2023-07-20 18:28:38.092984 project_lighter-0.0.2a9/lighter/utils/runner.py
+-rw-r--r--   0        0        0       24 2023-07-20 18:29:00.521555 project_lighter-0.0.2a9/lighter/version.py
+-rw-r--r--   0        0        0     4611 2023-07-20 18:29:00.453553 project_lighter-0.0.2a9/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 project_lighter-0.0.2a9/PKG-INFO
```

### Comparing `project_lighter-0.0.2a8/LICENSE` & `project_lighter-0.0.2a9/LICENSE`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/README.md` & `project_lighter-0.0.2a9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 - [Video Tutorials]()
 
 ## 💡 Projects
 List of projects that use `lighter`:
 
 | Project | Description |
 | --- | --- |
-| [FMCBI]() | |
+| [Foundation Models for Quantitative Imaging Biomarker Discovery in Cancer Imaging](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker) | A foundation model for CT scans trained by contrasting subvolumes with and without lesions. |
 
 
 ## 📄 Cite:
 
 If you find `lighter` useful in your research or project, please consider citing it. Here's an example BibTeX citation entry:
 
 ```bibtex
```

### Comparing `project_lighter-0.0.2a8/lighter/callbacks/freezer.py` & `project_lighter-0.0.2a9/lighter/callbacks/freezer.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/callbacks/logger.py` & `project_lighter-0.0.2a9/lighter/callbacks/logger.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/callbacks/utils.py` & `project_lighter-0.0.2a9/lighter/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/callbacks/writer/base.py` & `project_lighter-0.0.2a9/lighter/callbacks/writer/base.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/callbacks/writer/file.py` & `project_lighter-0.0.2a9/lighter/callbacks/writer/file.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/callbacks/writer/table.py` & `project_lighter-0.0.2a9/lighter/callbacks/writer/table.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/system.py` & `project_lighter-0.0.2a9/lighter/system.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/utils/cli.py` & `project_lighter-0.0.2a9/lighter/utils/cli.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/utils/collate.py` & `project_lighter-0.0.2a9/lighter/utils/collate.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/utils/dynamic_imports.py` & `project_lighter-0.0.2a9/lighter/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/utils/misc.py` & `project_lighter-0.0.2a9/lighter/utils/misc.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/utils/model.py` & `project_lighter-0.0.2a9/lighter/utils/model.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/lighter/utils/runner.py` & `project_lighter-0.0.2a9/lighter/utils/runner.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a8/pyproject.toml` & `project_lighter-0.0.2a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lighter = "lighter.utils.cli:interface"
 
 [tool.poetry]
 name = "project-lighter"
-version = "0.0.2a8"
+version = "0.0.2a9"
 description = "YAML-based automated rapid prototyping framework for deep learning experiments"
 readme = "README.md"
 authors = ["Ibrahim Hadzic <ibrahimhadzic45@gmail.com>" ,
             "Suraj Pai <b.pai@maastrichtuniversity.nl>", 
             "Keno Bressem <kbressem@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/lighter/lighter"
```

### Comparing `project_lighter-0.0.2a8/PKG-INFO` & `project_lighter-0.0.2a9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-lighter
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: YAML-based automated rapid prototyping framework for deep learning experiments
 Home-page: https://github.com/lighter/lighter
 License: MIT
 Author: Ibrahim Hadzic
 Author-email: ibrahimhadzic45@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -74,15 +74,15 @@
 - [Video Tutorials]()
 
 ## 💡 Projects
 List of projects that use `lighter`:
 
 | Project | Description |
 | --- | --- |
-| [FMCBI]() | |
+| [Foundation Models for Quantitative Imaging Biomarker Discovery in Cancer Imaging](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker) | A foundation model for CT scans trained by contrasting subvolumes with and without lesions. |
 
 
 ## 📄 Cite:
 
 If you find `lighter` useful in your research or project, please consider citing it. Here's an example BibTeX citation entry:
 
 ```bibtex
```

