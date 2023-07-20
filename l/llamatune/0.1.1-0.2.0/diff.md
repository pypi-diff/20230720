# Comparing `tmp/llamatune-0.1.1.tar.gz` & `tmp/llamatune-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatune-0.1.1.tar", last modified: Thu Jul 20 05:50:36 2023, max compression
+gzip compressed data, was "llamatune-0.2.0.tar", last modified: Thu Jul 20 17:23:05 2023, max compression
```

## Comparing `llamatune-0.1.1.tar` & `llamatune-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 05:50:36.315007 llamatune-0.1.1/
--rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 05:50:36.314888 llamatune-0.1.1/PKG-INFO
--rw-r--r--   0 justusmattern   (501) staff       (20)        5 2023-07-19 22:21:05.000000 llamatune-0.1.1/README.md
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 05:50:36.313253 llamatune-0.1.1/llamatune/
--rw-r--r--   0 justusmattern   (501) staff       (20)       32 2023-07-19 23:21:58.000000 llamatune-0.1.1/llamatune/__init__.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 05:50:36.314351 llamatune-0.1.1/llamatune/data/
--rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-19 22:21:05.000000 llamatune-0.1.1/llamatune/data/__init__.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     4246 2023-07-20 05:06:08.000000 llamatune-0.1.1/llamatune/data/chat_data_module.py
--rw-r--r--   0 justusmattern   (501) staff       (20)       65 2023-07-19 23:09:13.000000 llamatune-0.1.1/llamatune/data/data_module.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 05:50:36.314634 llamatune-0.1.1/llamatune/model_engines/
--rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-19 22:21:05.000000 llamatune-0.1.1/llamatune/model_engines/__init__.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     6595 2023-07-20 05:03:39.000000 llamatune-0.1.1/llamatune/model_engines/llama_model_engine.py
--rw-r--r--   0 justusmattern   (501) staff       (20)     4227 2023-07-20 05:48:04.000000 llamatune-0.1.1/llamatune/train.py
--rw-r--r--   0 justusmattern   (501) staff       (20)      864 2023-07-20 05:21:06.000000 llamatune-0.1.1/llamatune/trainer.py
--rw-r--r--   0 justusmattern   (501) staff       (20)      668 2023-07-19 22:45:47.000000 llamatune-0.1.1/llamatune/utils.py
-drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 05:50:36.313850 llamatune-0.1.1/llamatune.egg-info/
--rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 05:50:36.000000 llamatune-0.1.1/llamatune.egg-info/PKG-INFO
--rw-r--r--   0 justusmattern   (501) staff       (20)      437 2023-07-20 05:50:36.000000 llamatune-0.1.1/llamatune.egg-info/SOURCES.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-20 05:50:36.000000 llamatune-0.1.1/llamatune.egg-info/dependency_links.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)      139 2023-07-20 05:50:36.000000 llamatune-0.1.1/llamatune.egg-info/requires.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)       10 2023-07-20 05:50:36.000000 llamatune-0.1.1/llamatune.egg-info/top_level.txt
--rw-r--r--   0 justusmattern   (501) staff       (20)       38 2023-07-20 05:50:36.315044 llamatune-0.1.1/setup.cfg
--rw-r--r--   0 justusmattern   (501) staff       (20)      524 2023-07-20 05:49:52.000000 llamatune-0.1.1/setup.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:23:05.256178 llamatune-0.2.0/
+-rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 17:23:05.256038 llamatune-0.2.0/PKG-INFO
+-rw-r--r--   0 justusmattern   (501) staff       (20)     2670 2023-07-20 17:21:20.000000 llamatune-0.2.0/README.md
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:23:05.253966 llamatune-0.2.0/llamatune/
+-rw-r--r--   0 justusmattern   (501) staff       (20)       32 2023-07-19 23:21:58.000000 llamatune-0.2.0/llamatune/__init__.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:23:05.255448 llamatune-0.2.0/llamatune/data/
+-rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-19 22:21:05.000000 llamatune-0.2.0/llamatune/data/__init__.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     4246 2023-07-20 05:06:08.000000 llamatune-0.2.0/llamatune/data/chat_data_module.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)       65 2023-07-19 23:09:13.000000 llamatune-0.2.0/llamatune/data/data_module.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:23:05.255777 llamatune-0.2.0/llamatune/model_engines/
+-rw-r--r--   0 justusmattern   (501) staff       (20)        0 2023-07-19 22:21:05.000000 llamatune-0.2.0/llamatune/model_engines/__init__.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     6763 2023-07-20 17:14:33.000000 llamatune-0.2.0/llamatune/model_engines/llama_model_engine.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)     4227 2023-07-20 05:48:04.000000 llamatune-0.2.0/llamatune/train.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)      868 2023-07-20 17:14:42.000000 llamatune-0.2.0/llamatune/trainer.py
+-rw-r--r--   0 justusmattern   (501) staff       (20)      668 2023-07-19 22:45:47.000000 llamatune-0.2.0/llamatune/utils.py
+drwxr-xr-x   0 justusmattern   (501) staff       (20)        0 2023-07-20 17:23:05.254822 llamatune-0.2.0/llamatune.egg-info/
+-rw-r--r--   0 justusmattern   (501) staff       (20)      169 2023-07-20 17:23:05.000000 llamatune-0.2.0/llamatune.egg-info/PKG-INFO
+-rw-r--r--   0 justusmattern   (501) staff       (20)      437 2023-07-20 17:23:05.000000 llamatune-0.2.0/llamatune.egg-info/SOURCES.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)        1 2023-07-20 17:23:05.000000 llamatune-0.2.0/llamatune.egg-info/dependency_links.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)      154 2023-07-20 17:23:05.000000 llamatune-0.2.0/llamatune.egg-info/requires.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)       10 2023-07-20 17:23:05.000000 llamatune-0.2.0/llamatune.egg-info/top_level.txt
+-rw-r--r--   0 justusmattern   (501) staff       (20)       38 2023-07-20 17:23:05.256214 llamatune-0.2.0/setup.cfg
+-rw-r--r--   0 justusmattern   (501) staff       (20)      549 2023-07-20 17:22:57.000000 llamatune-0.2.0/setup.py
```

### Comparing `llamatune-0.1.1/llamatune/data/chat_data_module.py` & `llamatune-0.2.0/llamatune/data/chat_data_module.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.1.1/llamatune/model_engines/llama_model_engine.py` & `llamatune-0.2.0/llamatune/model_engines/llama_model_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dataclasses import dataclass, field
 from typing import Optional, Dict
 from transformers import BitsAndBytesConfig
 from peft import prepare_model_for_kbit_training, LoraConfig, get_peft_model
 from transformers import Trainer
 
 from llamatune.utils import _get_compute_dtype, print_trainable_parameters
+from llamatune.telemetry.send_event import capture_event
 
 
 
 class LlamaEngine:
 
     def __init__(self, model_name,  training_config):
         if not training_config.training_recipe in ["lora", "full_training"]:
@@ -34,17 +35,20 @@
             tokenizer=self.tokenizer,
             train_dataset=data_module.train_dataset,
             data_collator=data_module.data_collator,
             args=training_args
         )
 
         trainer.train()
+        capture_event("end-training", {})
 
 
     def prepare_model_for_training(self):
+        capture_event("start-training", {})
+
         if self.config.training_recipe == "lora":
             self.model = transformers.AutoModelForCausalLM.from_pretrained(
                 self.model_name,
                 load_in_4bit=self.config.bits == 4,
                 load_in_8bit=self.config.bits == 8,
                 device_map=self._get_device_map(),
                 torch_dtype=self.config.compute_dtype,
@@ -68,15 +72,15 @@
                 device_map=self._get_device_map(),
                 torch_dtype=self.config.compute_dtype,
                 trust_remote_code=self.config.trust_remote_code,
                 use_auth_token=self.config.use_auth_token
             )
 
 
-        self.tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_name, padding_side="right", use_fast=self.config.use_fast, tokenizer_type=self.config.tokenizer_type, trust_remote_code=self.config.trust_remote_code, use_auth_token=self.config.use_auth_token)
+        self.tokenizer = transformers.AutoTokenizer.from_pretrained(self.model_name, padding_side="right", tokenizer_type="llama", use_fast=self.config.use_fast, tokenizer_type=self.config.tokenizer_type, trust_remote_code=self.config.trust_remote_code, use_auth_token=self.config.use_auth_token)
 
         self._smart_tokenizer_and_embedding_resize()
 
         if self.training_recipe == "lora":
             self.model = prepare_model_for_kbit_training(self.model, use_gradient_checkpointing=self.config.gradient_checkpointing)
 
         if self.config.gradient_checkpointing:
```

### Comparing `llamatune-0.1.1/llamatune/train.py` & `llamatune-0.2.0/llamatune/train.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.1.1/llamatune/trainer.py` & `llamatune-0.2.0/llamatune/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 
 class ChatTrainer:
     def __init__(self, training_config: dataclass):
         self.training_config = training_config
         self.model_engine : LlamaEngine = LlamaEngine(training_config.model_name, training_config=training_config)
         self.data_path = training_config.data_path
 
-    def train(self):     
+    def train(self):
         self.model_engine.prepare_model_for_training()
 
         self.data_module = ChatDataModule(
             tokenizer=self.model_engine.tokenizer,
             data_path_train=self.data_path,
             max_tokens=self.model_engine.config.max_tokens
         )
 
         self.model_engine.train(data_module=self.data_module)
+
```

### Comparing `llamatune-0.1.1/llamatune/utils.py` & `llamatune-0.2.0/llamatune/utils.py`

 * *Files identical despite different names*

### Comparing `llamatune-0.1.1/setup.py` & `llamatune-0.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='llamatune',
-    version='0.1.1',
+    version='0.2.0',
     author='Haven Technologies Inc.',
     author_email='hello@havenllm.com',
     description="Haven\'s Tuning Library for LLM finetuning",
     packages=find_packages(),
     install_requires=[
         'torch==2.0.1',
         'bitsandbytes==0.40.0',
         'einops==0.6.1',
         'evaluate==0.4.0',
         'scikit-learn==1.2.2',
         'sentencepiece==0.1.99',
         'wandb==0.15.3',
-        'accelerate==0.21.0'
+        'accelerate==0.21.0',
+        'posthog==2.5.0'
     ],
-
 )
```

