# Comparing `tmp/llamatune-0.2.3.tar.gz` & `tmp/llamatune-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatune-0.2.3.tar", last modified: Thu Jul 20 17:59:26 2023, max compression
+gzip compressed data, was "llamatune-0.2.4.tar", last modified: Thu Jul 20 18:06:10 2023, max compression
```

## Comparing `llamatune-0.2.3.tar` & `llamatune-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:59:26.198291 llamatune-0.2.3/
--rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 17:59:26.198141 llamatune-0.2.3/PKG-INFO
--rw-r--r--   0 justusmattern   (501) staff       (20)     2670 2023-07-20 17:21:20.000000 llamatune-0.2.3/README.md
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:59:26.195890 llamatune-0.2.3/llamatune/
--rw-r--r--   0 justusmattern   (501) staff       (20)       32 2023-07-19 23:21:58.000000 llamatune-0.2.3/llamatune/__init__.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:59:26.197090 llamatune-0.2.3/llamatune/data/
--rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-19 22:21:05.000000 llamatune-0.2.3/llamatune/data/__init__.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     4246 2023-07-20 05:06:08.000000 llamatune-0.2.3/llamatune/data/chat_data_module.py
--rw-r--r--   0 justusmattern   (501) staff       (20)       65 2023-07-19 23:09:13.000000 llamatune-0.2.3/llamatune/data/data_module.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:59:26.197403 llamatune-0.2.3/llamatune/model_engines/
--rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-19 22:21:05.000000 llamatune-0.2.3/llamatune/model_engines/__init__.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     6739 2023-07-20 17:34:10.000000 llamatune-0.2.3/llamatune/model_engines/llama_model_engine.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:59:26.197733 llamatune-0.2.3/llamatune/telemetry/
--rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:14.000000 llamatune-0.2.3/llamatune/telemetry/__init__.py
--rw-r--r--   0 justusmattern   (501) staff       (20)      453 2023-07-20 17:59:07.000000 llamatune-0.2.3/llamatune/telemetry/send_event.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     4228 2023-07-20 17:34:08.000000 llamatune-0.2.3/llamatune/train.py
--rw-r--r--   0 justusmattern   (501) staff       (20)      868 2023-07-20 17:14:42.000000 llamatune-0.2.3/llamatune/trainer.py
--rw-r--r--   0 justusmattern   (501) staff       (20)      668 2023-07-19 22:45:47.000000 llamatune-0.2.3/llamatune/utils.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:59:26.196519 llamatune-0.2.3/llamatune.egg-info/
--rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 17:59:26.000000 llamatune-0.2.3/llamatune.egg-info/PKG-INFO
--rw-r--r--   0 justusmattern   (501) staff       (20)      503 2023-07-20 17:59:26.000000 llamatune-0.2.3/llamatune.egg-info/SOURCES.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-20 17:59:26.000000 llamatune-0.2.3/llamatune.egg-info/dependency_links.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)      154 2023-07-20 17:59:26.000000 llamatune-0.2.3/llamatune.egg-info/requires.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)       10 2023-07-20 17:59:26.000000 llamatune-0.2.3/llamatune.egg-info/top_level.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)       38 2023-07-20 17:59:26.198361 llamatune-0.2.3/setup.cfg
--rw-r--r--   0 justusmattern   (501) staff       (20)      549 2023-07-20 17:59:23.000000 llamatune-0.2.3/setup.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 18:06:10.611556 llamatune-0.2.4/
+-rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 18:06:10.611410 llamatune-0.2.4/PKG-INFO
+-rw-r--r--   0 justusmattern   (501) staff       (20)     2670 2023-07-20 17:21:20.000000 llamatune-0.2.4/README.md
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 18:06:10.607154 llamatune-0.2.4/llamatune/
+-rw-r--r--   0 justusmattern   (501) staff       (20)       32 2023-07-19 23:21:58.000000 llamatune-0.2.4/llamatune/__init__.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 18:06:10.609355 llamatune-0.2.4/llamatune/data/
+-rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-19 22:21:05.000000 llamatune-0.2.4/llamatune/data/__init__.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     4246 2023-07-20 05:06:08.000000 llamatune-0.2.4/llamatune/data/chat_data_module.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)       65 2023-07-19 23:09:13.000000 llamatune-0.2.4/llamatune/data/data_module.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 18:06:10.609803 llamatune-0.2.4/llamatune/model_engines/
+-rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-19 22:21:05.000000 llamatune-0.2.4/llamatune/model_engines/__init__.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     6739 2023-07-20 17:34:10.000000 llamatune-0.2.4/llamatune/model_engines/llama_model_engine.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 18:06:10.610629 llamatune-0.2.4/llamatune/telemetry/
+-rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:37:14.000000 llamatune-0.2.4/llamatune/telemetry/__init__.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)      452 2023-07-20 18:05:42.000000 llamatune-0.2.4/llamatune/telemetry/send_event.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     4228 2023-07-20 17:34:08.000000 llamatune-0.2.4/llamatune/train.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)      868 2023-07-20 17:14:42.000000 llamatune-0.2.4/llamatune/trainer.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)      668 2023-07-19 22:45:47.000000 llamatune-0.2.4/llamatune/utils.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 18:06:10.607912 llamatune-0.2.4/llamatune.egg-info/
+-rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 18:06:10.000000 llamatune-0.2.4/llamatune.egg-info/PKG-INFO
+-rw-r--r--   0 justusmattern   (501) staff       (20)      503 2023-07-20 18:06:10.000000 llamatune-0.2.4/llamatune.egg-info/SOURCES.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-20 18:06:10.000000 llamatune-0.2.4/llamatune.egg-info/dependency_links.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)      154 2023-07-20 18:06:10.000000 llamatune-0.2.4/llamatune.egg-info/requires.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)       10 2023-07-20 18:06:10.000000 llamatune-0.2.4/llamatune.egg-info/top_level.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)       38 2023-07-20 18:06:10.611609 llamatune-0.2.4/setup.cfg
+-rw-r--r--   0 justusmattern   (501) staff       (20)      549 2023-07-20 18:06:07.000000 llamatune-0.2.4/setup.py
```

### Comparing `llamatune-0.2.3/README.md` & `llamatune-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.3/llamatune/data/chat_data_module.py` & `llamatune-0.2.4/llamatune/data/chat_data_module.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.3/llamatune/model_engines/llama_model_engine.py` & `llamatune-0.2.4/llamatune/model_engines/llama_model_engine.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.3/llamatune/train.py` & `llamatune-0.2.4/llamatune/train.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.3/llamatune/trainer.py` & `llamatune-0.2.4/llamatune/trainer.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.3/llamatune/utils.py` & `llamatune-0.2.4/llamatune/utils.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.2.3/setup.py` & `llamatune-0.2.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='llamatune',
-    version='0.2.3',
+    version='0.2.4',
     author='Haven Technologies Inc.',
     author_email='hello@havenllm.com',
     description="Haven\'s Tuning Library for LLM finetuning",
     packages=find_packages(),
     install_requires=[
         'torch==2.0.1',
         'bitsandbytes==0.40.0',
```

