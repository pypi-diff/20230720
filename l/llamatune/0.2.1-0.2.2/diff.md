# Comparing `tmp/llamatune-0.2.1.tar.gz` & `tmp/llamatune-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatune-0.2.1.tar", last modified: Thu Jul 20 17:35:00 2023, max compression
+gzip compressed data, was "llamatune-0.2.2.tar", last modified: Thu Jul 20 17:37:49 2023, max compression
```

## Comparing `llamatune-0.2.1.tar` & `llamatune-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:35:00.177298 llamatune-0.2.1/
--rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 17:35:00.177157 llamatune-0.2.1/PKG-INFO
--rw-r--r--   0 justusmattern   (501) staff       (20)     2670 2023-07-20 17:21:20.000000 llamatune-0.2.1/README.md
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:35:00.175289 llamatune-0.2.1/llamatune/
--rw-r--r--   0 justusmattern   (501) staff       (20)       32 2023-07-19 23:21:58.000000 llamatune-0.2.1/llamatune/__init__.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:35:00.176539 llamatune-0.2.1/llamatune/data/
--rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-19 22:21:05.000000 llamatune-0.2.1/llamatune/data/__init__.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     4246 2023-07-20 05:06:08.000000 llamatune-0.2.1/llamatune/data/chat_data_module.py
--rw-r--r--   0 justusmattern   (501) staff       (20)       65 2023-07-19 23:09:13.000000 llamatune-0.2.1/llamatune/data/data_module.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:35:00.176866 llamatune-0.2.1/llamatune/model_engines/
--rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-19 22:21:05.000000 llamatune-0.2.1/llamatune/model_engines/__init__.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     6739 2023-07-20 17:34:10.000000 llamatune-0.2.1/llamatune/model_engines/llama_model_engine.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     4228 2023-07-20 17:34:08.000000 llamatune-0.2.1/llamatune/train.py
--rw-r--r--   0 justusmattern   (501) staff       (20)      868 2023-07-20 17:14:42.000000 llamatune-0.2.1/llamatune/trainer.py
--rw-r--r--   0 justusmattern   (501) staff       (20)      668 2023-07-19 22:45:47.000000 llamatune-0.2.1/llamatune/utils.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:35:00.175907 llamatune-0.2.1/llamatune.egg-info/
--rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 17:35:00.000000 llamatune-0.2.1/llamatune.egg-info/PKG-INFO
--rw-r--r--   0 justusmattern   (501) staff       (20)      437 2023-07-20 17:35:00.000000 llamatune-0.2.1/llamatune.egg-info/SOURCES.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-20 17:35:00.000000 llamatune-0.2.1/llamatune.egg-info/dependency_links.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)      154 2023-07-20 17:35:00.000000 llamatune-0.2.1/llamatune.egg-info/requires.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)       10 2023-07-20 17:35:00.000000 llamatune-0.2.1/llamatune.egg-info/top_level.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)       38 2023-07-20 17:35:00.177351 llamatune-0.2.1/setup.cfg
--rw-r--r--   0 justusmattern   (501) staff       (20)      549 2023-07-20 17:34:55.000000 llamatune-0.2.1/setup.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:49.210335 llamatune-0.2.2/
+-rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 17:37:49.210194 llamatune-0.2.2/PKG-INFO
+-rw-r--r--   0 justusmattern   (501) staff       (20)     2670 2023-07-20 17:21:20.000000 llamatune-0.2.2/README.md
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:49.208038 llamatune-0.2.2/llamatune/
+-rw-r--r--   0 justusmattern   (501) staff       (20)       32 2023-07-19 23:21:58.000000 llamatune-0.2.2/llamatune/__init__.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:49.209309 llamatune-0.2.2/llamatune/data/
+-rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-19 22:21:05.000000 llamatune-0.2.2/llamatune/data/__init__.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     4246 2023-07-20 05:06:08.000000 llamatune-0.2.2/llamatune/data/chat_data_module.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)       65 2023-07-19 23:09:13.000000 llamatune-0.2.2/llamatune/data/data_module.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:49.209661 llamatune-0.2.2/llamatune/model_engines/
+-rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-19 22:21:05.000000 llamatune-0.2.2/llamatune/model_engines/__init__.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     6739 2023-07-20 17:34:10.000000 llamatune-0.2.2/llamatune/model_engines/llama_model_engine.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:49.210024 llamatune-0.2.2/llamatune/telemetry/
+-rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:14.000000 llamatune-0.2.2/llamatune/telemetry/__init__.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)      331 2023-07-20 17:21:41.000000 llamatune-0.2.2/llamatune/telemetry/send_event.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     4228 2023-07-20 17:34:08.000000 llamatune-0.2.2/llamatune/train.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)      868 2023-07-20 17:14:42.000000 llamatune-0.2.2/llamatune/trainer.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)      668 2023-07-19 22:45:47.000000 llamatune-0.2.2/llamatune/utils.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:49.208700 llamatune-0.2.2/llamatune.egg-info/
+-rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 17:37:49.000000 llamatune-0.2.2/llamatune.egg-info/PKG-INFO
+-rw-r--r--   0 justusmattern   (501) staff       (20)      503 2023-07-20 17:37:49.000000 llamatune-0.2.2/llamatune.egg-info/SOURCES.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-20 17:37:49.000000 llamatune-0.2.2/llamatune.egg-info/dependency_links.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)      154 2023-07-20 17:37:49.000000 llamatune-0.2.2/llamatune.egg-info/requires.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)       10 2023-07-20 17:37:49.000000 llamatune-0.2.2/llamatune.egg-info/top_level.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)       38 2023-07-20 17:37:49.210372 llamatune-0.2.2/setup.cfg
+-rw-r--r--   0 justusmattern   (501) staff       (20)      549 2023-07-20 17:37:26.000000 llamatune-0.2.2/setup.py
```

### Comparing `llamatune-0.2.1/README.md` & `llamatune-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.1/llamatune/data/chat_data_module.py` & `llamatune-0.2.2/llamatune/data/chat_data_module.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.1/llamatune/model_engines/llama_model_engine.py` & `llamatune-0.2.2/llamatune/model_engines/llama_model_engine.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.1/llamatune/train.py` & `llamatune-0.2.2/llamatune/train.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.1/llamatune/trainer.py` & `llamatune-0.2.2/llamatune/trainer.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.1/llamatune/utils.py` & `llamatune-0.2.2/llamatune/utils.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.1/setup.py` & `llamatune-0.2.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='llamatune',
-    version='0.2.1',
+    version='0.2.2',
     author='Haven Technologies Inc.',
     author_email='hello@havenllm.com',
     description="Haven\'s Tuning Library for LLM finetuning",
     packages=find_packages(),
     install_requires=[
         'torch==2.0.1',
         'bitsandbytes==0.40.0',
```

