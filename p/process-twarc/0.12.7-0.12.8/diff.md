# Comparing `tmp/process-twarc-0.12.7.tar.gz` & `tmp/process-twarc-0.12.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-twarc-0.12.7.tar", last modified: Thu Jul 20 18:09:14 2023, max compression
+gzip compressed data, was "process-twarc-0.12.8.tar", last modified: Thu Jul 20 18:12:53 2023, max compression
```

## Comparing `process-twarc-0.12.7.tar` & `process-twarc-0.12.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 18:09:14.142116 process-twarc-0.12.7/
--rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.7/LICENSE.txt
--rw-rw-rw-   0        0        0      693 2023-07-20 18:09:14.142116 process-twarc-0.12.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 18:09:14.121933 process-twarc-0.12.7/process_twarc/
--rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.7/process_twarc/__init__.py
--rw-rw-rw-   0        0        0     8630 2023-07-12 21:19:25.000000 process-twarc-0.12.7/process_twarc/util.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:09:14.141102 process-twarc-0.12.7/process_twarc.egg-info/
--rw-rw-rw-   0        0        0      693 2023-07-20 18:09:14.000000 process-twarc-0.12.7/process_twarc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-20 18:09:14.000000 process-twarc-0.12.7/process_twarc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 18:09:14.000000 process-twarc-0.12.7/process_twarc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-20 18:09:14.000000 process-twarc-0.12.7/process_twarc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-20 18:09:14.000000 process-twarc-0.12.7/process_twarc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-20 18:09:14.143492 process-twarc-0.12.7/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-07-20 18:09:08.000000 process-twarc-0.12.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:12:53.927267 process-twarc-0.12.8/
+-rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      693 2023-07-20 18:12:53.928329 process-twarc-0.12.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 18:12:53.913742 process-twarc-0.12.8/process_twarc/
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.8/process_twarc/__init__.py
+-rw-rw-rw-   0        0        0     9609 2023-07-20 18:12:20.000000 process-twarc-0.12.8/process_twarc/util.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:12:53.927267 process-twarc-0.12.8/process_twarc.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-07-20 18:12:53.000000 process-twarc-0.12.8/process_twarc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-20 18:12:53.000000 process-twarc-0.12.8/process_twarc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 18:12:53.000000 process-twarc-0.12.8/process_twarc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-20 18:12:53.000000 process-twarc-0.12.8/process_twarc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-20 18:12:53.000000 process-twarc-0.12.8/process_twarc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-20 18:12:53.931580 process-twarc-0.12.8/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-07-20 18:12:38.000000 process-twarc-0.12.8/setup.py
```

### Comparing `process-twarc-0.12.7/LICENSE.txt` & `process-twarc-0.12.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `process-twarc-0.12.7/PKG-INFO` & `process-twarc-0.12.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.7
+Version: 0.12.8
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.7/process_twarc/util.py` & `process-twarc-0.12.8/process_twarc/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pyarrow.parquet as pq
 from tqdm import tqdm
 from ntpath import basename
 import os
 import json
 from typing import Callable
 import itertools
+from  transformers import AutoTokenizer, AutoModel
+import torch
 
 def get_file_type(file_path):
     _, file_extension = os.path.splitext(file_path)
     return file_extension[1:].lower()  # Remove the dot and convert to lowercase
 
 def get_all_files(directory):
     """
@@ -209,28 +211,52 @@
     Args:
         dict (dict): Dictionary to be saved.
         save_path (str): Path where the JSON file will be saved.
     """
     with open(save_path, 'w', encoding="utf-8") as f:
         json.dump(dict, f, ensure_ascii=False, indent=2)
         return
+
+def save_list_to_txt(list_, path_to_output):
+    with open(path_to_output, "w", encoding="utf-8")as f:
+        f.write("\n".join(list_))
+    return
+
+def load_list_from_txt(path_to_list):
+    with open(path_to_list, "r", encoding="utf-8") as f:
+        return f.read().splitlines()
     
 def load_dict(path_to_dict):
     with open(path_to_dict, "r", encoding="utf-8") as f:
         return json.load(f)
 
+def get_characters(tokenizer):
+    vocab = list(tokenizer.get_vocab().keys())
+    merged = itertools.chain.from_iterable(vocab)
+    characters = sorted(set([character for character in merged]))
+    return characters
     
-def load_tokenizer(tokenizer_class, tokenizer_path, print_details=True):
-    def get_characters(tokenizer):
-        vocab = list(tokenizer.get_vocab().keys())
-        merged = itertools.chain.from_iterable(vocab)
-        characters = sorted(set([character for character in merged]))
-        return characters
+def load_tokenizer(tokenizer_path, tokenizer_class=AutoTokenizer, keep_newlines=True, print_details=False):
     
-    tokenizer = tokenizer_class.from_pretrained(tokenizer_path)
+    tokenizer = tokenizer_class.from_pretrained(tokenizer_path, keep_newlines=keep_newlines)
     if print_details:
-        print("Tokenizer loaded.")
-        print("Name:", tokenizer.name_or_path )
+        print()
+        print(f"{tokenizer.name_or_path} loaded." )
+        print("Type:", type(tokenizer))
         print("Vocab Size:", len(tokenizer))
         print("Unique Characters:", len(get_characters(tokenizer)))
         print("Special Tokens:", tokenizer.all_special_tokens)
     return tokenizer
+
+def load_model(model_path, model_class=AutoModel, device="", print_details=False):
+    model = model_class.from_pretrained(model_path)
+    if device:
+        model.to(device)
+    if print_details:
+        print()
+        print(f"{model.name_or_path} loaded.")
+        if device:
+            print(f"Sent to {device}.")
+        print("Type:", type(model))
+        print("Number of Parameters:", sum(p.numel() for p in model.parameters() if p.requires_grad))
+        print("Model Architecture:", model.__class__.__name__)
+    return model
```

### Comparing `process-twarc-0.12.7/process_twarc.egg-info/PKG-INFO` & `process-twarc-0.12.8/process_twarc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.7
+Version: 0.12.8
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.7/setup.py` & `process-twarc-0.12.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'process-twarc',         
   packages = ['process_twarc'],   
-  version = '0.12.7',
+  version = '0.12.8',
   license='MIT',
   description = 'Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.',   # Give a short description about your library
   author = 'Jordan Wolfgang Klein',
   author_email = 'jordan.klein.21@um.edu.mt',
   url = 'https://github.com/user/Lone-Wolfgang',
   keywords = ['Twitter', 'Deduplication', "Tokenization", "Language Modeling"],
   install_requires=[
```

