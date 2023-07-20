# Comparing `tmp/xfact-0.4.71.tar.gz` & `tmp/xfact-0.4.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfact-0.4.71.tar", last modified: Thu Jul 20 04:09:43 2023, max compression
+gzip compressed data, was "xfact-0.4.74.tar", last modified: Thu Jul 20 08:08:12 2023, max compression
```

## Comparing `xfact-0.4.71.tar` & `xfact-0.4.74.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.416252 xfact-0.4.71/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 04:07:13.000000 xfact-0.4.71/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-20 04:09:43.416252 xfact-0.4.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-20 04:07:13.000000 xfact-0.4.71/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 04:07:13.000000 xfact-0.4.71/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:09:43.416252 xfact-0.4.71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 04:07:14.000000 xfact-0.4.71/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.412252 xfact-0.4.71/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.412252 xfact-0.4.71/src/xfact/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.412252 xfact-0.4.71/src/xfact/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/config/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.416252 xfact-0.4.71/src/xfact/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/logs/comet_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/logs/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/logs/wandb_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.416252 xfact-0.4.71/src/xfact/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.416252 xfact-0.4.71/src/xfact/nlp/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/datasets/fever_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/datasets/snli_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/datasets/squad_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/deardr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.416252 xfact-0.4.71/src/xfact/nlp/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/inference/prefix_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.416252 xfact-0.4.71/src/xfact/nlp/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/readers/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/nlp/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.416252 xfact-0.4.71/src/xfact/registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/registry/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/registry/registrable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-20 04:07:13.000000 xfact-0.4.71/src/xfact/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:09:43.412252 xfact-0.4.71/src/xfact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-20 04:09:43.000000 xfact-0.4.71/src/xfact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-20 04:09:43.000000 xfact-0.4.71/src/xfact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:09:43.000000 xfact-0.4.71/src/xfact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 04:09:43.000000 xfact-0.4.71/src/xfact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 04:09:43.000000 xfact-0.4.71/src/xfact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.558487 xfact-0.4.74/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 08:05:44.000000 xfact-0.4.74/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-20 08:08:12.558487 xfact-0.4.74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-20 08:05:44.000000 xfact-0.4.74/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 08:05:44.000000 xfact-0.4.74/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:08:12.558487 xfact-0.4.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 08:05:44.000000 xfact-0.4.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/config/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/logs/comet_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/logs/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/logs/wandb_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact/nlp/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/datasets/fever_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/datasets/snli_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/datasets/squad_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/deardr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact/nlp/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/inference/prefix_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact/nlp/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/readers/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/nlp/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/registry/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/registry/registrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-07-20 08:05:44.000000 xfact-0.4.74/src/xfact/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:08:12.554487 xfact-0.4.74/src/xfact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-20 08:08:12.000000 xfact-0.4.74/src/xfact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-20 08:08:12.000000 xfact-0.4.74/src/xfact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:08:12.000000 xfact-0.4.74/src/xfact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 08:08:12.000000 xfact-0.4.74/src/xfact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 08:08:12.000000 xfact-0.4.74/src/xfact.egg-info/top_level.txt
```

### Comparing `xfact-0.4.71/README.md` & `xfact-0.4.74/README.md`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/setup.py` & `xfact-0.4.74/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 install = [req for req in reqs if not req.startswith("git+git://")]
 depends = [req.replace("git+git://", "git+http://") for req in reqs if req.startswith("git+git://")]
 
 
 setup(
     name='xfact',
-    version='0.4.71',
+    version='0.4.74',
     author='James Thorne',
     author_email='james@jamesthorne.com',
     description='xfact',
     long_description="readme",
     python_requires='>=3.8',
     packages=["xfact",
               "xfact.nlp",
```

### Comparing `xfact-0.4.71/src/xfact/config/args.py` & `xfact-0.4.74/src/xfact/config/args.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/logs/comet_callback.py` & `xfact-0.4.74/src/xfact/logs/comet_callback.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/logs/logs.py` & `xfact-0.4.74/src/xfact/logs/logs.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/logs/wandb_callback.py` & `xfact-0.4.74/src/xfact/logs/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/data_utils.py` & `xfact-0.4.74/src/xfact/nlp/data_utils.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/dataset.py` & `xfact-0.4.74/src/xfact/nlp/dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/datasets/fever_dataset.py` & `xfact-0.4.74/src/xfact/nlp/datasets/fever_dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/datasets/snli_dataset.py` & `xfact-0.4.74/src/xfact/nlp/datasets/snli_dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/datasets/squad_dataset.py` & `xfact-0.4.74/src/xfact/nlp/datasets/squad_dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/deardr_trainer.py` & `xfact-0.4.74/src/xfact/nlp/deardr_trainer.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/inference/prefix_decoder.py` & `xfact-0.4.74/src/xfact/nlp/inference/prefix_decoder.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/model.py` & `xfact-0.4.74/src/xfact/nlp/model.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/post_processing.py` & `xfact-0.4.74/src/xfact/nlp/post_processing.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/reader.py` & `xfact-0.4.74/src/xfact/nlp/reader.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/readers/huggingface.py` & `xfact-0.4.74/src/xfact/nlp/readers/huggingface.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/nlp/scoring.py` & `xfact-0.4.74/src/xfact/nlp/scoring.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/registry/module.py` & `xfact-0.4.74/src/xfact/registry/module.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/registry/registrable.py` & `xfact-0.4.74/src/xfact/registry/registrable.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.71/src/xfact/train.py` & `xfact-0.4.74/src/xfact/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         params.update(asdict(model_args))
         run = wandb.init(
             # set the wandb project where this run will be logged
             project=data_args.project_name,
             # track hyperparameters and run metadata
             config=params
         )
-
-
+    else:
+        run = None
 
     if data_args.comet_key and training_args.should_log and (training_args.do_train or training_args.do_eval):
         experiment = comet_ml.Experiment(
             api_key=data_args.comet_key,
             workspace=data_args.workspace,
             project_name=data_args.project_name if data_args.project_name is not None else f"debugging-xfact",
             experiment_key=data_args.experiment_key if data_args.experiment_key is not None else None,
@@ -264,18 +264,19 @@
 
         trainer.log_metrics("eval", metrics)
         trainer.save_metrics("eval", metrics)
 
         if trainer.is_world_process_zero() and experiment:
             experiment.log_metrics({"final/" + key: value for key, value in metrics.items()})
 
-        if training_args.should_log:
-            wandb.log({"final/" + key: value for key, value in metrics.items()})
+        if training_args.should_log and run:
+            run.log({"final/" + key: value for key, value in metrics.items()})
 
-    run.finish()
+    if run:
+        run.finish()
 
 def _mp_fn(index):
     # For xla_spawn (TPUs)
     main()
 
 if __name__ == "__main__":
     main()
```

### Comparing `xfact-0.4.71/src/xfact.egg-info/SOURCES.txt` & `xfact-0.4.74/src/xfact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

