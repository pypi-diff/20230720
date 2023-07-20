# Comparing `tmp/gigagan-pytorch-0.1.5.tar.gz` & `tmp/gigagan-pytorch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.1.5.tar", last modified: Thu Jul 20 18:07:07 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.1.6.tar", last modified: Thu Jul 20 18:26:01 2023, max compression
```

## Comparing `gigagan-pytorch-0.1.5.tar` & `gigagan-pytorch-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    71408 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/setup.py
```

### Comparing `gigagan-pytorch-0.1.5/LICENSE` & `gigagan-pytorch-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.5/PKG-INFO` & `gigagan-pytorch-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.5
+Version: 0.1.6
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.5/README.md` & `gigagan-pytorch-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.5/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.1.6/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.5/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.1.6/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.5/gigagan_pytorch/data.py` & `gigagan-pytorch-0.1.6/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.5/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.1.6/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,17 @@
     grad_output_weights = None,
     weight = 10,
     scaler: Optional[GradScaler] = None
 ):
     if not isinstance(outputs, (list, tuple)):
         outputs = [outputs]
 
+    if exists(scaler):
+        outputs = [*map(scaler.scale, outputs)]
+
     if not exists(grad_output_weights):
         grad_output_weights = (1,) * len(outputs)
 
     maybe_scaled_gradients, *_ = torch_grad(
         outputs = outputs,
         inputs = images,
         grad_outputs = [(torch.ones_like(output) * weight) for output, weight in zip(outputs, grad_output_weights)],
```

### Comparing `gigagan-pytorch-0.1.5/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.1.6/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.5/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.1.6/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.5/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.1.6/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.5
+Version: 0.1.6
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.5/setup.py` & `gigagan-pytorch-0.1.6/setup.py`

 * *Files identical despite different names*

