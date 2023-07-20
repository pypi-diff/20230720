# Comparing `tmp/gigagan-pytorch-0.1.4.tar.gz` & `tmp/gigagan-pytorch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.1.4.tar", last modified: Thu Jul 20 17:39:19 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.1.5.tar", last modified: Thu Jul 20 18:07:07 2023, max compression
```

## Comparing `gigagan-pytorch-0.1.4.tar` & `gigagan-pytorch-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:19.675775 gigagan-pytorch-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 17:39:19.675775 gigagan-pytorch-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:19.675775 gigagan-pytorch-0.1.4/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    71280 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:39:19.675775 gigagan-pytorch-0.1.4/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 17:39:19.000000 gigagan-pytorch-0.1.4/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 17:39:19.000000 gigagan-pytorch-0.1.4/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:39:19.000000 gigagan-pytorch-0.1.4/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 17:39:19.000000 gigagan-pytorch-0.1.4/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 17:39:19.000000 gigagan-pytorch-0.1.4/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:39:19.675775 gigagan-pytorch-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 17:39:08.000000 gigagan-pytorch-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71408 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:07:07.000000 gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:07:07.043125 gigagan-pytorch-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 18:06:57.000000 gigagan-pytorch-0.1.5/setup.py
```

### Comparing `gigagan-pytorch-0.1.4/LICENSE` & `gigagan-pytorch-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.4/PKG-INFO` & `gigagan-pytorch-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.4/README.md` & `gigagan-pytorch-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.4/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.1.5/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.4/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.1.5/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.4/gigagan_pytorch/data.py` & `gigagan-pytorch-0.1.5/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.4/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.1.5/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1231,14 +1231,16 @@
         depth = 4,
         num_conv_kernels = 2,
         unconditional = False
     ):
         super().__init__()
         self.unconditional = unconditional
         self.residual_fn = nn.Conv2d(dim, dim, 1)
+        self.residual_scale = 2 ** -0.5
+
         self.layers = nn.ModuleList([])
 
         klass = nn.Conv2d if unconditional else partial(AdaptiveConv2DMod, num_conv_kernels = num_conv_kernels)
         klass_kwargs = dict(padding = 1) if unconditional else dict()
 
         for ind in range(depth):
             self.layers.append(nn.ModuleList([
@@ -1269,14 +1271,15 @@
 
             x = conv1(x, **kwargs)
             x = activation(x)
             x = conv2(x, **kwargs)
             x = activation(x)
 
             x = x + inner_residual
+            x = x * self.residual_scale
 
         x = x + residual
         return self.to_logits(x)
 
 class Discriminator(nn.Module):
     @beartype
     def __init__(
@@ -1636,15 +1639,15 @@
         *,
         generator: Union[BaseGenerator, Dict],
         discriminator: Union[Discriminator, Dict],
         text_encoder: Optional[Union[TextEncoder, Dict]] = None,
         learning_rate = 2e-4,
         betas = (0.5, 0.9),
         weight_decay = 0.,
-        discr_aux_recon_loss_weight = 0.25,
+        discr_aux_recon_loss_weight = 1.,
         multiscale_divergence_loss_weight = 0.1,
         calc_multiscale_loss_every = 1,
         apply_gradient_penalty_every = 4,
         ttur_mult = 1,
         train_upsampler = False,
         upsampler_replace_rgb_with_input_lowres_image = False,
         log_steps_every = 20,
@@ -2111,20 +2114,22 @@
 
             self.accelerator.backward(total_loss / grad_accum_every)
 
         self.G_opt.step()
 
         # update exponentially moving averaged generator
 
-        if self.has_ema_generator:
+        self.accelerator.wait_for_everyone()
+
+        if self.is_main and self.has_ema_generator:
             self.G_ema.update()
 
         return TrainGenLosses(total_divergence, total_multiscale_divergence)
 
-    def sample_lambda(self, dl_iter, batch_size):
+    def sample(self, dl_iter, batch_size):
         G_kwargs, maybe_text_kwargs = self.generate_kwargs(dl_iter, batch_size)
 
         with self.accelerator.autocast():
             generator_output = self.G(**G_kwargs, **maybe_text_kwargs)
 
         if not self.train_upsampler:
             return generator_output
@@ -2154,15 +2159,15 @@
 
         if self.has_ema_generator:
             sample_models_and_output_file_name.append((self.G_ema, f'ema-sample-{milestone}.png'))
 
         for model, filename in sample_models_and_output_file_name:
             model.eval()
 
-            all_images_list = list(map(lambda n: self.sample_lambda(dl_iter, n), batches))
+            all_images_list = list(map(lambda n: self.sample(dl_iter, n), batches))
             all_images = torch.cat(all_images_list, dim=0)
 
             all_images.clamp_(0., 1.)
 
             utils.save_image(
                 all_images,
                 str(self.results_folder / filename),
```

### Comparing `gigagan-pytorch-0.1.4/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.1.5/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.4/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.1.5/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.4/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.1.5/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.4/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.1.5/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.4/setup.py` & `gigagan-pytorch-0.1.5/setup.py`

 * *Files identical despite different names*

