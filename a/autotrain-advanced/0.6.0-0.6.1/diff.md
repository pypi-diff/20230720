# Comparing `tmp/autotrain-advanced-0.6.0.tar.gz` & `tmp/autotrain-advanced-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.6.0.tar", last modified: Wed Jul 19 10:43:57 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.6.1.tar", last modified: Thu Jul 20 12:00:38 2023, max compression
```

## Comparing `autotrain-advanced-0.6.0.tar` & `autotrain-advanced-0.6.1.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-19 10:43:57.096406 autotrain-advanced-0.6.0/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.0/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-19 10:43:57.096406 autotrain-advanced-0.6.0/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.0/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-19 10:43:57.096406 autotrain-advanced-0.6.0/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.0/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-19 10:43:57.092406 autotrain-advanced-0.6.0/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-19 10:43:57.092406 autotrain-advanced-0.6.0/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      816 2023-07-19 10:43:49.000000 autotrain-advanced-0.6.0/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.0/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-19 10:43:57.092406 autotrain-advanced-0.6.0/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.6.0/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1033 2023-07-19 10:07:30.000000 autotrain-advanced-0.6.0/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.0/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-13 15:03:01.000000 autotrain-advanced-0.6.0/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14456 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.0/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2178 2023-07-19 10:23:02.000000 autotrain-advanced-0.6.0/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.0/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-19 10:21:07.000000 autotrain-advanced-0.6.0/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.0/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.0/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.0/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-19 10:43:57.096406 autotrain-advanced-0.6.0/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.0/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.0/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.0/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.0/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.0/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.0/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.0/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.0/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-19 10:43:57.096406 autotrain-advanced-0.6.0/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.0/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.0/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9901 2023-07-19 10:39:25.000000 autotrain-advanced-0.6.0/src/autotrain/trainers/clm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-07-18 10:31:20.000000 autotrain-advanced-0.6.0/src/autotrain/trainers/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.0/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.0/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.0/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.0/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-19 10:14:57.000000 autotrain-advanced-0.6.0/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-19 10:43:57.096406 autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-19 10:43:57.000000 autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1254 2023-07-19 10:43:57.000000 autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-19 10:43:57.000000 autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-19 10:43:57.000000 autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-19 10:43:57.000000 autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-19 10:43:57.000000 autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.1/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.1/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.1/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      816 2023-07-20 12:00:33.000000 autotrain-advanced-0.6.1/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.1/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.6.1/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1033 2023-07-19 10:07:30.000000 autotrain-advanced-0.6.1/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.1/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-13 15:03:01.000000 autotrain-advanced-0.6.1/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-20 12:00:11.000000 autotrain-advanced-0.6.1/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2178 2023-07-19 10:23:02.000000 autotrain-advanced-0.6.1/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.1/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-19 10:21:07.000000 autotrain-advanced-0.6.1/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.1/src/autotrain/help.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/infer/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 09:08:58.000000 autotrain-advanced-0.6.1/src/autotrain/infer/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-20 12:00:25.000000 autotrain-advanced-0.6.1/src/autotrain/infer/text_generation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.1/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.1/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.1/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.1/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.1/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10663 2023-07-20 12:00:11.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/clm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-07-18 10:31:20.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-19 10:14:57.000000 autotrain-advanced-0.6.1/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.0/LICENSE` & `autotrain-advanced-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/PKG-INFO` & `autotrain-advanced-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.0/setup.py` & `autotrain-advanced-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/__init__.py` & `autotrain-advanced-0.6.1/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # pylint: enable=line-too-long
 import os
 
 
 # ignore bnb warnings
 os.environ["BITSANDBYTES_NOWELCOME"] = "1"
 os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `autotrain-advanced-0.6.0/src/autotrain/app.py` & `autotrain-advanced-0.6.1/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.6.1/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.6.1/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.6.1/src/autotrain/cli/run_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from argparse import ArgumentParser
 
 from loguru import logger
 
+from autotrain.infer.text_generation import TextGenerationInference
+
 from ..trainers.clm import train as train_llm
 from ..trainers.utils import LLMTrainingParams
 from . import BaseAutoTrainCommand
 
 
 def run_llm_command_factory(args):
     return RunAutoTrainLLMCommand(
@@ -428,14 +430,22 @@
                 raise ValueError("Data path must be specified")
             if self.model is None:
                 raise ValueError("Model must be specified")
             if self.push_to_hub:
                 if self.repo_id is None:
                     raise ValueError("Repo id must be specified for push to hub")
 
+        if self.inference:
+            tgi = TextGenerationInference(self.project_name, use_int4=self.use_int4, use_int8=self.use_int8)
+            while True:
+                prompt = input("User: ")
+                if prompt == "exit()":
+                    break
+                print(f"Bot: {tgi.chat(prompt)}")
+
     def run(self):
         logger.info("Running LLM")
         logger.info(f"Train: {self.train}")
         if self.train:
             params = LLMTrainingParams(
                 model_name=self.model,
                 data_path=self.data_path,
```

### Comparing `autotrain-advanced-0.6.0/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.6.1/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/dataset.py` & `autotrain-advanced-0.6.1/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/help.py` & `autotrain-advanced-0.6.1/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/params.py` & `autotrain-advanced-0.6.1/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.6.1/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.6.1/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.6.1/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.6.1/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/project.py` & `autotrain-advanced-0.6.1/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/tasks.py` & `autotrain-advanced-0.6.1/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.6.1/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.6.1/src/autotrain/trainers/clm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import os
 import sys
 from functools import partial
 
+import pandas as pd
 import torch
-from datasets import load_dataset
+from datasets import Dataset, load_dataset
 from huggingface_hub import HfApi
 from loguru import logger
 from peft import LoraConfig, get_peft_model, prepare_model_for_int8_training
 from transformers import (
     AutoConfig,
     AutoModelForCausalLM,
     AutoTokenizer,
@@ -21,25 +23,40 @@
 from autotrain.trainers.callbacks import LoadBestPeftModelCallback, SavePeftModelCallback
 
 
 def train(config):
     if isinstance(config, dict):
         config = utils.LLMTrainingParams(**config)
 
-    train_data = load_dataset(
-        config.data_path,
-        split=config.train_split,
-        use_auth_token=config.huggingface_token,
-    )
+    # check if config.train_split.csv exists in config.data_path
+    if config.train_split is not None:
+        train_path = f"{config.data_path}/{config.train_split}.csv"
+        if os.path.exists(train_path):
+            logger.info("loading dataset from csv")
+            train_data = pd.read_csv(train_path)
+            train_data = Dataset.from_pandas(train_data)
+        else:
+            train_data = load_dataset(
+                config.data_path,
+                split=config.train_split,
+                use_auth_token=config.huggingface_token,
+            )
+
     if config.valid_split is not None:
-        valid_data = load_dataset(
-            config.data_path,
-            split=config.valid_split,
-            use_auth_token=config.huggingface_token,
-        )
+        valid_path = f"{config.data_path}/{config.valid_split}.csv"
+        if os.path.exists(valid_path):
+            logger.info("loading dataset from csv")
+            valid_data = pd.read_csv(valid_path)
+            valid_data = Dataset.from_pandas(valid_data)
+        else:
+            valid_data = load_dataset(
+                config.data_path,
+                split=config.valid_split,
+                use_auth_token=config.huggingface_token,
+            )
 
     tokenizer = AutoTokenizer.from_pretrained(
         config.model_name,
         use_auth_token=config.huggingface_token,
         trust_remote_code=True,
     )
```

### Comparing `autotrain-advanced-0.6.0/src/autotrain/trainers/dreambooth.py` & `autotrain-advanced-0.6.1/src/autotrain/trainers/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.6.1/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.6.1/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.6.1/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.6.1/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain/utils.py` & `autotrain-advanced-0.6.1/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 src/autotrain/utils.py
 src/autotrain/cli/__init__.py
 src/autotrain/cli/autotrain.py
 src/autotrain/cli/run_app.py
 src/autotrain/cli/run_dreambooth.py
 src/autotrain/cli/run_llm.py
 src/autotrain/cli/run_setup.py
+src/autotrain/infer/__init__.py
+src/autotrain/infer/text_generation.py
 src/autotrain/preprocessor/__init__.py
 src/autotrain/preprocessor/dreambooth.py
 src/autotrain/preprocessor/tabular.py
 src/autotrain/preprocessor/text.py
 src/autotrain/preprocessor/vision.py
 src/autotrain/trainers/__init__.py
 src/autotrain/trainers/callbacks.py
```

### Comparing `autotrain-advanced-0.6.0/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

