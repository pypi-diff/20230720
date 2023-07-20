# Comparing `tmp/gigagan-pytorch-0.1.1.tar.gz` & `tmp/gigagan-pytorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.1.1.tar", last modified: Thu Jul 20 16:49:59 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.1.2.tar", last modified: Thu Jul 20 17:18:43 2023, max compression
```

## Comparing `gigagan-pytorch-0.1.1.tar` & `gigagan-pytorch-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    69663 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:18:43.314976 gigagan-pytorch-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 17:18:43.314976 gigagan-pytorch-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:18:43.314976 gigagan-pytorch-0.1.2/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70468 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:18:43.314976 gigagan-pytorch-0.1.2/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 17:18:43.000000 gigagan-pytorch-0.1.2/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 17:18:43.000000 gigagan-pytorch-0.1.2/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:18:43.000000 gigagan-pytorch-0.1.2/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 17:18:43.000000 gigagan-pytorch-0.1.2/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 17:18:43.000000 gigagan-pytorch-0.1.2/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:18:43.314976 gigagan-pytorch-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 17:18:31.000000 gigagan-pytorch-0.1.2/setup.py
```

### Comparing `gigagan-pytorch-0.1.1/LICENSE` & `gigagan-pytorch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.1/PKG-INFO` & `gigagan-pytorch-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.1/README.md` & `gigagan-pytorch-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,22 @@
 dataset = ImageDataset(
     folder = '/path/to/your/data',
     image_size = 256
 )
 
 dataloader = dataset.get_dataloader(batch_size = 1)
 
+# you must then set the dataloader for the GAN before training
+
+gan.set_dataloader(dataloader)
+
 # training the discriminator and generator alternating
 # for 100 steps in this example, batch size 1, gradient accumulated 8 times
 
 gan(
-    dataloader = dataloader,
     steps = 100,
     grad_accum_every = 8
 )
 ```
 
 For unconditional Unet Upsampler
 
@@ -112,19 +115,20 @@
 dataset = ImageDataset(
     folder = '/path/to/your/data',
     image_size = 256
 )
 
 dataloader = dataset.get_dataloader(batch_size = 1)
 
+gan.set_dataloader(dataloader)
+
 # training the discriminator and generator alternating
 # for 100 steps in this example, batch size 1, gradient accumulated 8 times
 
 gan(
-    dataloader = dataloader,
     steps = 100,
     grad_accum_every = 8
 )
 ```
 
 ## Losses (wip)
 
@@ -158,15 +162,15 @@
 - [x] add upsampling network architecture
 - [x] make unconditional work for both base generator and upsampler
 - [x] make text conditioned training work for both base and upsampler
 - [x] make recon more efficient by random sampling patches
 
 - [ ] add accelerate
     - [x] works single machine
-    - [ ] works for mixed precision (make sure gradient penalty is scaled correctly), take care of manual scaler saving and reloading, borrow from imagen-pytorch
+    - [x] works for mixed precision (make sure gradient penalty is scaled correctly), take care of manual scaler saving and reloading, borrow from imagen-pytorch
     - [ ] make sure it works multi-GPU for one machine
     - [ ] have someone else try multiple machines
 
 - [ ] add ability to select a random subset from multiscale dimension, for efficiency
 - [ ] make sure text encoder can also accept pre-encoded CLIP embeddings
 
 - [ ] do a review of the auxiliary losses
```

#### html2text {}

```diff
@@ -16,54 +16,55 @@
 GAN, for starters ```python import torch from gigagan_pytorch import ( GigaGAN,
 ImageDataset ) gan = GigaGAN( generator = dict( dim_capacity = 8, style_network
 = dict( dim = 64, depth = 4 ), image_size = 256, dim_max = 512,
 num_skip_layers_excite = 4, unconditional = True ), discriminator = dict
 ( dim_capacity = 16, dim_max = 512, image_size = 256, num_skip_layers_excite =
 4, unconditional = True ) ).cuda() # dataset dataset = ImageDataset( folder =
 '/path/to/your/data', image_size = 256 ) dataloader = dataset.get_dataloader
-(batch_size = 1) # training the discriminator and generator alternating # for
-100 steps in this example, batch size 1, gradient accumulated 8 times gan
-( dataloader = dataloader, steps = 100, grad_accum_every = 8 ) ``` For
-unconditional Unet Upsampler ```python import torch from gigagan_pytorch import
-GigaGAN, ImageDataset gan = GigaGAN( train_upsampler = True, # set this to True
+(batch_size = 1) # you must then set the dataloader for the GAN before training
+gan.set_dataloader(dataloader) # training the discriminator and generator
+alternating # for 100 steps in this example, batch size 1, gradient accumulated
+8 times gan( steps = 100, grad_accum_every = 8 ) ``` For unconditional Unet
+Upsampler ```python import torch from gigagan_pytorch import GigaGAN,
+ImageDataset gan = GigaGAN( train_upsampler = True, # set this to True
 generator = dict( style_network = dict( dim = 64, depth = 4 ), dim = 32,
 image_size = 256, input_image_size = 128, unconditional = True ), discriminator
 = dict( dim_capacity = 16, dim_max = 512, image_size = 256,
 num_skip_layers_excite = 4, unconditional = True ) ).cuda() dataset =
 ImageDataset( folder = '/path/to/your/data', image_size = 256 ) dataloader =
-dataset.get_dataloader(batch_size = 1) # training the discriminator and
-generator alternating # for 100 steps in this example, batch size 1, gradient
-accumulated 8 times gan( dataloader = dataloader, steps = 100, grad_accum_every
-= 8 ) ``` ## Losses (wip) * `G` - Generator * `MSG` - Multiscale Generator *
-`D` - Discriminator * `MSD` - Multiscale Discriminator * `GP` - Gradient
-Penalty * `SSL` - Auxiliary Reconstruction in Discriminator (from Lightweight
-GAN) A healthy run would have `G`, `MSG`, `D`, `MSD` with values hovering
-between `0` to `10`, and usually staying pretty constant. If at any time after
-1k training steps these values persist at triple digits, that would mean
-something is wrong. It is ok for generator and discriminator values to
-occasionally dip negative, but it should swing back up to the range above. `GP`
-and `SSL` should be pushed towards `0`. `GP` can occasionally spike; I like to
-imagine it as the networks undergoing some epiphany ## Todo - [x] make sure it
-can be trained unconditionally - [x] read the relevant papers and knock out all
-3 auxiliary losses - [x] matching aware loss - [x] clip loss - [x] vision-aided
-discriminator loss - [x] add reconstruction losses on arbitrary stages in the
-discriminator (lightweight gan) - [x] figure out how the random projections are
-used from projected-gan - [x] vision aided discriminator needs to extract N
-layers from the vision model in CLIP - [x] figure out whether to discard CLS
-token and reshape into image dimensions for convolution, or stick with
-attention and condition with adaptive layernorm - also turn off vision aided
-gan in unconditional case - [x] unet upsampler - [x] add adaptive conv - [x]
-modify latter stage of unet to also output rgb residuals, and pass the rgb into
-discriminator. make discriminator agnostic to rgb being passed in - [x] do
+dataset.get_dataloader(batch_size = 1) gan.set_dataloader(dataloader) #
+training the discriminator and generator alternating # for 100 steps in this
+example, batch size 1, gradient accumulated 8 times gan( steps = 100,
+grad_accum_every = 8 ) ``` ## Losses (wip) * `G` - Generator * `MSG` -
+Multiscale Generator * `D` - Discriminator * `MSD` - Multiscale Discriminator *
+`GP` - Gradient Penalty * `SSL` - Auxiliary Reconstruction in Discriminator
+(from Lightweight GAN) A healthy run would have `G`, `MSG`, `D`, `MSD` with
+values hovering between `0` to `10`, and usually staying pretty constant. If at
+any time after 1k training steps these values persist at triple digits, that
+would mean something is wrong. It is ok for generator and discriminator values
+to occasionally dip negative, but it should swing back up to the range above.
+`GP` and `SSL` should be pushed towards `0`. `GP` can occasionally spike; I
+like to imagine it as the networks undergoing some epiphany ## Todo - [x] make
+sure it can be trained unconditionally - [x] read the relevant papers and knock
+out all 3 auxiliary losses - [x] matching aware loss - [x] clip loss - [x]
+vision-aided discriminator loss - [x] add reconstruction losses on arbitrary
+stages in the discriminator (lightweight gan) - [x] figure out how the random
+projections are used from projected-gan - [x] vision aided discriminator needs
+to extract N layers from the vision model in CLIP - [x] figure out whether to
+discard CLS token and reshape into image dimensions for convolution, or stick
+with attention and condition with adaptive layernorm - also turn off vision
+aided gan in unconditional case - [x] unet upsampler - [x] add adaptive conv -
+[x] modify latter stage of unet to also output rgb residuals, and pass the rgb
+into discriminator. make discriminator agnostic to rgb being passed in - [x] do
 pixel shuffle upsamples for unet - [x] get a code review for the multi-scale
 inputs and outputs, as the paper was a bit vague - [x] add upsampling network
 architecture - [x] make unconditional work for both base generator and
 upsampler - [x] make text conditioned training work for both base and upsampler
 - [x] make recon more efficient by random sampling patches - [ ] add accelerate
-- [x] works single machine - [ ] works for mixed precision (make sure gradient
+- [x] works single machine - [x] works for mixed precision (make sure gradient
 penalty is scaled correctly), take care of manual scaler saving and reloading,
 borrow from imagen-pytorch - [ ] make sure it works multi-GPU for one machine -
 [ ] have someone else try multiple machines - [ ] add ability to select a
 random subset from multiscale dimension, for efficiency - [ ] make sure text
 encoder can also accept pre-encoded CLIP embeddings - [ ] do a review of the
 auxiliary losses - [ ] add vision aided loss and make sure it trains, inspect
 output - [ ] port over CLI from lightweight|stylegan2-pytorch - [ ] hook up
```

### Comparing `gigagan-pytorch-0.1.1/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.1.2/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.1/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.1.2/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.1/gigagan_pytorch/data.py` & `gigagan-pytorch-0.1.2/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.1/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.1.2/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from torchvision import utils
 
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum, Tensor
 from torch.autograd import grad as torch_grad
 from torch.utils.data import DataLoader
+from torch.cuda.amp import GradScaler
 
 from beartype import beartype
 from beartype.typing import List, Optional, Tuple, Dict, Union, Iterable
 
 from einops import rearrange, pack, unpack, repeat, reduce
 from einops.layers.torch import Rearrange, Reduce
 
@@ -98,31 +99,39 @@
 def log(t, eps = 1e-20):
     return t.clamp(min = eps).log()
 
 def gradient_penalty(
     images,
     outputs,
     grad_output_weights = None,
-    weight = 10
+    weight = 10,
+    scaler: Optional[GradScaler] = None
 ):
     if not isinstance(outputs, (list, tuple)):
         outputs = [outputs]
 
     if not exists(grad_output_weights):
         grad_output_weights = (1,) * len(outputs)
 
-    gradients, *_ = torch_grad(
+    maybe_scaled_gradients, *_ = torch_grad(
         outputs = outputs,
         inputs = images,
         grad_outputs = [(torch.ones_like(output) * weight) for output, weight in zip(outputs, grad_output_weights)],
         create_graph = True,
         retain_graph = True,
         only_inputs = True
     )
 
+    gradients = maybe_scaled_gradients
+
+    if exists(scaler):
+        scale = scaler.get_scale()
+        inv_scale = 1. / max(scale, 1e-5)
+        gradients = maybe_scaled_gradients * inv_scale
+
     gradients = rearrange(gradients, 'b ... -> b (...)')
     return weight * ((gradients.norm(2, dim = 1) - 1) ** 2).mean()
 
 # hinge gan losses
 
 def generator_hinge_loss(fake):
     return fake.mean()
@@ -1760,14 +1769,20 @@
             D = self.unwrapped_D.state_dict(),
             G_opt = self.G_opt.state_dict(),
             D_opt = self.D_opt.state_dict(),
             steps = self.steps.item(),
             version = __version__
         )
 
+        if exists(self.G_opt.scaler):
+            pkg['G_scaler'] = self.G_opt.scaler.state_dict()
+
+        if exists(self.D_opt.scaler):
+            pkg['D_scaler'] = self.D_opt.scaler.state_dict()
+
         if self.has_ema_generator:
             pkg['G_ema'] = self.G_ema.state_dict()
 
         torch.save(pkg, str(path))
 
     def load(self, path, strict = False):
         path = Path(path)
@@ -1789,14 +1804,21 @@
 
         if 'G_opt'not in pkg or 'D_opt' not in pkg:
             return
 
         try:
             self.G_opt.load_state_dict(pkg['G_opt'])
             self.D_opt.load_state_dict(pkg['D_opt'])
+
+            if 'G_scaler' in pkg and exists(self.G_opt.scaler):
+                self.G_opt.scaler.load_state_dict(pkg['G_scaler'])
+
+            if 'D_scaler' in pkg and exists(self.D_opt.scaler):
+                self.D_opt.scaler.load_state_dict(pkg['D_scaler'])
+
         except Exception as e:
             self.print(f'unable to load optimizers {e.msg}- optimizer states will be reset')
             pass
 
     # accelerate related
 
     @property
@@ -1985,15 +2007,16 @@
 
                 gp_loss = 0.
 
                 if apply_gradient_penalty:
                     gp_loss = gradient_penalty(
                         real_images,
                         outputs = [real_logits, *real_multiscale_logits],
-                        grad_output_weights = [1., *(self.multiscale_divergence_loss_weight,) * len(real_multiscale_logits)]
+                        grad_output_weights = [1., *(self.multiscale_divergence_loss_weight,) * len(real_multiscale_logits)],
+                        scaler = self.D_opt.scaler
                     )
 
                     total_gp_loss += (gp_loss.item() / grad_accum_every)
 
                 # sum up losses
 
                 total_loss = divergence + gp_loss
```

### Comparing `gigagan-pytorch-0.1.1/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.1.2/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.1/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.1.2/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.1/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.1.2/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.1.2/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.1/setup.py` & `gigagan-pytorch-0.1.2/setup.py`

 * *Files identical despite different names*

