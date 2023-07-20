# Comparing `tmp/gigagan-pytorch-0.1.6.tar.gz` & `tmp/gigagan-pytorch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.1.6.tar", last modified: Thu Jul 20 18:26:01 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.1.7.tar", last modified: Thu Jul 20 18:42:01 2023, max compression
```

## Comparing `gigagan-pytorch-0.1.6.tar` & `gigagan-pytorch-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:26:01.000000 gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:26:01.389256 gigagan-pytorch-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 18:25:50.000000 gigagan-pytorch-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71646 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/setup.py
```

### Comparing `gigagan-pytorch-0.1.6/LICENSE` & `gigagan-pytorch-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.6/PKG-INFO` & `gigagan-pytorch-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.6
+Version: 0.1.7
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.6/README.md` & `gigagan-pytorch-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <img src="./gigagan-architecture.png" width="500px"></img>
 
 ## GigaGAN - Pytorch
 
 Implementation of <a href="https://arxiv.org/abs/2303.05511v2">GigaGAN</a> <a href="https://mingukkang.github.io/GigaGAN/">(project page)</a>, new SOTA GAN out of Adobe.
 
-I will also add a few findings from <a href="https://github.com/lucidrains/lightweight-gan">lightweight gan</a>, for faster convergence (skip layer excitation) and better stability (reconstruction auxiliary loss in discriminator).
+I will also add a few findings from <a href="https://github.com/lucidrains/lightweight-gan">lightweight gan</a>, for faster convergence (skip layer excitation), better stability (reconstruction auxiliary loss in discriminator), and improved generator results (GLU activations).
 
 It will also contain the code for the 1k - 4k upsamplers, which I find to be the highlight of this paper.
 
 Please join <a href="https://discord.gg/xBPBXfcFHd"><img alt="Join us on Discord" src="https://img.shields.io/discord/823813159592001537?color=5865F2&logo=discord&logoColor=white"></a> if you are interested in helping out with the replication with the <a href="https://laion.ai/">LAION</a> community
 
 ## Appreciation
 
@@ -56,15 +56,16 @@
     ),
     discriminator = dict(
         dim_capacity = 16,
         dim_max = 512,
         image_size = 256,
         num_skip_layers_excite = 4,
         unconditional = True
-    )
+    ),
+    amp = True
 ).cuda()
 
 # dataset
 
 dataset = ImageDataset(
     folder = '/path/to/your/data',
     image_size = 256
@@ -85,15 +86,18 @@
 )
 ```
 
 For unconditional Unet Upsampler
 
 ```python
 import torch
-from gigagan_pytorch import GigaGAN, ImageDataset
+from gigagan_pytorch import (
+    GigaGAN,
+    ImageDataset
+)
 
 gan = GigaGAN(
     train_upsampler = True,     # set this to True
     generator = dict(
         style_network = dict(
             dim = 64,
             depth = 4
@@ -105,15 +109,16 @@
     ),
     discriminator = dict(
         dim_capacity = 16,
         dim_max = 512,
         image_size = 256,
         num_skip_layers_excite = 4,
         unconditional = True
-    )
+    ),
+    amp = True
 ).cuda()
 
 dataset = ImageDataset(
     folder = '/path/to/your/data',
     image_size = 256
 )
 
@@ -169,14 +174,18 @@
     - [x] works single machine
     - [x] works for mixed precision (make sure gradient penalty is scaled correctly), take care of manual scaler saving and reloading, borrow from imagen-pytorch
     - [ ] make sure it works multi-GPU for one machine
     - [ ] have someone else try multiple machines
 
 - [ ] add ability to select a random subset from multiscale dimension, for efficiency
 
+- [ ] add some differentiable augmentations, proven technique from the old GAN days
+    - [ ] remove any magic being done with automatic rgbs processing, and have it explicitly passed in - offer functions on the discriminator that can process real images into the right multi-scales
+    - [ ] add horizontal flip for starters
+
 - [ ] do a review of the auxiliary losses
     - [ ] add vision aided loss and make sure it trains, inspect output
 
 - [ ] port over CLI from lightweight|stylegan2-pytorch
 - [ ] hook up laion dataset for text-image
 
 ## Citations
```

#### html2text {}

```diff
@@ -1,44 +1,45 @@
 [./gigagan-sample.png] [./gigagan-architecture.png] ## GigaGAN - Pytorch
 Implementation of GigaGAN (project_page), new SOTA GAN out of Adobe. I will
 also add a few findings from lightweight_gan, for faster convergence (skip
-layer excitation) and better stability (reconstruction auxiliary loss in
-discriminator). It will also contain the code for the 1k - 4k upsamplers, which
-I find to be the highlight of this paper. Please join [Join_us_on_Discord] if
-you are interested in helping out with the replication with the LAION community
-## Appreciation - StabilityAI and ð¤_Huggingface for the generous
-sponsorship, as well as my other sponsors, for affording me the independence to
-open source artificial intelligence. - ð¤_Huggingface for their accelerate
-library - All the maintainers at OpenClip, for their SOTA open sourced
-contrastive learning text-image models - Xavier for reviewing the discriminator
-code and pointing out that the scale invariance was not correctly built! -
-@CerebralSeed for pull requesting the initial sampling code for both the
-generator and upsampler! ## Install ```bash $ pip install gigagan-pytorch ```
-## Usage Simple unconditional GAN, for starters ```python import torch from
-gigagan_pytorch import ( GigaGAN, ImageDataset ) gan = GigaGAN( generator =
-dict( dim_capacity = 8, style_network = dict( dim = 64, depth = 4 ), image_size
-= 256, dim_max = 512, num_skip_layers_excite = 4, unconditional = True ),
-discriminator = dict( dim_capacity = 16, dim_max = 512, image_size = 256,
-num_skip_layers_excite = 4, unconditional = True ) ).cuda() # dataset dataset =
-ImageDataset( folder = '/path/to/your/data', image_size = 256 ) dataloader =
+layer excitation), better stability (reconstruction auxiliary loss in
+discriminator), and improved generator results (GLU activations). It will also
+contain the code for the 1k - 4k upsamplers, which I find to be the highlight
+of this paper. Please join [Join_us_on_Discord] if you are interested in
+helping out with the replication with the LAION community ## Appreciation -
+StabilityAI and ð¤_Huggingface for the generous sponsorship, as well as my
+other sponsors, for affording me the independence to open source artificial
+intelligence. - ð¤_Huggingface for their accelerate library - All the
+maintainers at OpenClip, for their SOTA open sourced contrastive learning text-
+image models - Xavier for reviewing the discriminator code and pointing out
+that the scale invariance was not correctly built! - @CerebralSeed for pull
+requesting the initial sampling code for both the generator and upsampler! ##
+Install ```bash $ pip install gigagan-pytorch ``` ## Usage Simple unconditional
+GAN, for starters ```python import torch from gigagan_pytorch import ( GigaGAN,
+ImageDataset ) gan = GigaGAN( generator = dict( dim_capacity = 8, style_network
+= dict( dim = 64, depth = 4 ), image_size = 256, dim_max = 512,
+num_skip_layers_excite = 4, unconditional = True ), discriminator = dict
+( dim_capacity = 16, dim_max = 512, image_size = 256, num_skip_layers_excite =
+4, unconditional = True ), amp = True ).cuda() # dataset dataset = ImageDataset
+( folder = '/path/to/your/data', image_size = 256 ) dataloader =
 dataset.get_dataloader(batch_size = 1) # you must then set the dataloader for
 the GAN before training gan.set_dataloader(dataloader) # training the
 discriminator and generator alternating # for 100 steps in this example, batch
 size 1, gradient accumulated 8 times gan( steps = 100, grad_accum_every = 8 )
 ``` For unconditional Unet Upsampler ```python import torch from
-gigagan_pytorch import GigaGAN, ImageDataset gan = GigaGAN( train_upsampler =
-True, # set this to True generator = dict( style_network = dict( dim = 64,
+gigagan_pytorch import ( GigaGAN, ImageDataset ) gan = GigaGAN( train_upsampler
+= True, # set this to True generator = dict( style_network = dict( dim = 64,
 depth = 4 ), dim = 32, image_size = 256, input_image_size = 128, unconditional
 = True ), discriminator = dict( dim_capacity = 16, dim_max = 512, image_size =
-256, num_skip_layers_excite = 4, unconditional = True ) ).cuda() dataset =
-ImageDataset( folder = '/path/to/your/data', image_size = 256 ) dataloader =
-dataset.get_dataloader(batch_size = 1) gan.set_dataloader(dataloader) #
-training the discriminator and generator alternating # for 100 steps in this
-example, batch size 1, gradient accumulated 8 times gan( steps = 100,
-grad_accum_every = 8 ) ``` ## Losses (wip) * `G` - Generator * `MSG` -
+256, num_skip_layers_excite = 4, unconditional = True ), amp = True ).cuda()
+dataset = ImageDataset( folder = '/path/to/your/data', image_size = 256 )
+dataloader = dataset.get_dataloader(batch_size = 1) gan.set_dataloader
+(dataloader) # training the discriminator and generator alternating # for 100
+steps in this example, batch size 1, gradient accumulated 8 times gan( steps =
+100, grad_accum_every = 8 ) ``` ## Losses (wip) * `G` - Generator * `MSG` -
 Multiscale Generator * `D` - Discriminator * `MSD` - Multiscale Discriminator *
 `GP` - Gradient Penalty * `SSL` - Auxiliary Reconstruction in Discriminator
 (from Lightweight GAN) A healthy run would have `G`, `MSG`, `D`, `MSD` with
 values hovering between `0` to `10`, and usually staying pretty constant. If at
 any time after 1k training steps these values persist at triple digits, that
 would mean something is wrong. It is ok for generator and discriminator values
 to occasionally dip negative, but it should swing back up to the range above.
@@ -62,14 +63,18 @@
 - [x] make recon more efficient by random sampling patches - [x] make sure
 generator and discriminator can also accept pre-encoded CLIP text encodings -
 [ ] add accelerate - [x] works single machine - [x] works for mixed precision
 (make sure gradient penalty is scaled correctly), take care of manual scaler
 saving and reloading, borrow from imagen-pytorch - [ ] make sure it works
 multi-GPU for one machine - [ ] have someone else try multiple machines - [ ]
 add ability to select a random subset from multiscale dimension, for efficiency
+- [ ] add some differentiable augmentations, proven technique from the old GAN
+days - [ ] remove any magic being done with automatic rgbs processing, and have
+it explicitly passed in - offer functions on the discriminator that can process
+real images into the right multi-scales - [ ] add horizontal flip for starters
 - [ ] do a review of the auxiliary losses - [ ] add vision aided loss and make
 sure it trains, inspect output - [ ] port over CLI from lightweight|stylegan2-
 pytorch - [ ] hook up laion dataset for text-image ## Citations ```bibtex @misc
 {https://doi.org/10.48550/arxiv.2303.05511, url = {https://arxiv.org/abs/
 2303.05511}, author = {Kang, Minguk and Zhu, Jun-Yan and Zhang, Richard and
 Park, Jaesik and Shechtman, Eli and Paris, Sylvain and Park, Taesung}, title =
 {Scaling up GANs for Text-to-Image Synthesis}, publisher = {arXiv}, year =
```

### Comparing `gigagan-pytorch-0.1.6/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.1.7/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.6/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.1.7/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.6/gigagan_pytorch/data.py` & `gigagan-pytorch-0.1.7/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.6/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.1.7/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -785,15 +785,16 @@
         self_ff_mult = 4,
         cross_attn_resolutions: Tuple[int, ...] = (32, 16),
         cross_attn_dim_head = 64,
         cross_attn_heads = 8,
         cross_ff_mult = 4,
         num_conv_kernels = 2,  # the number of adaptive conv kernels
         num_skip_layers_excite = 0,
-        unconditional = False
+        unconditional = False,
+        use_glu = True
     ):
         super().__init__()
         self.channels = channels
 
         if isinstance(style_network, dict):
             style_network = StyleNetwork(**style_network)
 
@@ -877,21 +878,24 @@
             has_cross_attn = resolution in cross_attn_resolutions and not unconditional
 
             skip_squeeze_excite = None
             if should_skip_layer_excite:
                 dim_skip_in, _ = dim_pairs[ind + num_skip_layers_excite]
                 skip_squeeze_excite = SqueezeExcite(dim_in, dim_skip_in)
 
+            dim_inner = dim_out * (2 if use_glu else 1)
+            activation = partial(nn.GLU, dim = 1) if use_glu else leaky_relu
+
             resnet_block = nn.ModuleList([
-                adaptive_conv(dim_in, dim_out),
-                Noise(dim_out),
-                leaky_relu(),
-                adaptive_conv(dim_out, dim_out),
-                Noise(dim_out),
-                leaky_relu()
+                adaptive_conv(dim_in, dim_inner),
+                Noise(dim_inner),
+                activation(),
+                adaptive_conv(dim_out, dim_inner),
+                Noise(dim_inner),
+                activation()
             ])
 
             to_rgb = adaptive_conv(dim_out, channels)
 
             self_attn = cross_attn = rgb_upsample = upsample = None
 
             upsample = Upsample(dim_in) if should_upsample else None
```

### Comparing `gigagan-pytorch-0.1.6/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.1.7/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.6/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.1.7/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.6/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.1.7/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.6/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.6
+Version: 0.1.7
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.6/setup.py` & `gigagan-pytorch-0.1.7/setup.py`

 * *Files identical despite different names*

