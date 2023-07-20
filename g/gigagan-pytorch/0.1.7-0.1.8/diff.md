# Comparing `tmp/gigagan-pytorch-0.1.7.tar.gz` & `tmp/gigagan-pytorch-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.1.7.tar", last modified: Thu Jul 20 18:42:01 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.1.8.tar", last modified: Thu Jul 20 19:21:33 2023, max compression
```

## Comparing `gigagan-pytorch-0.1.7.tar` & `gigagan-pytorch-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    71646 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:42:01.000000 gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:42:01.839456 gigagan-pytorch-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 18:41:51.000000 gigagan-pytorch-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71724 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/setup.py
```

### Comparing `gigagan-pytorch-0.1.7/LICENSE` & `gigagan-pytorch-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.7/PKG-INFO` & `gigagan-pytorch-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.7
+Version: 0.1.8
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.7/README.md` & `gigagan-pytorch-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -144,14 +144,30 @@
 * `GP` - Gradient Penalty
 * `SSL` - Auxiliary Reconstruction in Discriminator (from Lightweight GAN)
 
 A healthy run would have `G`, `MSG`, `D`, `MSD` with values hovering between `0` to `10`, and usually staying pretty constant. If at any time after 1k training steps these values persist at triple digits, that would mean something is wrong. It is ok for generator and discriminator values to occasionally dip negative, but it should swing back up to the range above.
 
 `GP` and `SSL` should be pushed towards `0`. `GP` can occasionally spike; I like to imagine it as the networks undergoing some epiphany
 
+## Multi-GPU Training
+
+The `GigaGAN` class is now equipped with <a href="https://huggingface.co/docs/accelerate/accelerator">🤗 Accelerator</a>. You can easily do multi-gpu training in two steps using their `accelerate` CLI
+
+At the project root directory, where the training script is, run
+
+```python
+$ accelerate config
+```
+
+Then, in the same directory
+
+```python
+$ accelerate launch train.py
+```
+
 ## Todo
 
 - [x] make sure it can be trained unconditionally
 - [x] read the relevant papers and knock out all 3 auxiliary losses
     - [x] matching aware loss
     - [x] clip loss
     - [x] vision-aided discriminator loss
@@ -169,15 +185,15 @@
 - [x] make text conditioned training work for both base and upsampler
 - [x] make recon more efficient by random sampling patches
 - [x] make sure generator and discriminator can also accept pre-encoded CLIP text encodings
 
 - [ ] add accelerate
     - [x] works single machine
     - [x] works for mixed precision (make sure gradient penalty is scaled correctly), take care of manual scaler saving and reloading, borrow from imagen-pytorch
-    - [ ] make sure it works multi-GPU for one machine
+    - [x] make sure it works multi-GPU for one machine
     - [ ] have someone else try multiple machines
 
 - [ ] add ability to select a random subset from multiscale dimension, for efficiency
 
 - [ ] add some differentiable augmentations, proven technique from the old GAN days
     - [ ] remove any magic being done with automatic rgbs processing, and have it explicitly passed in - offer functions on the discriminator that can process real images into the right multi-scales
     - [ ] add horizontal flip for starters
```

#### html2text {}

```diff
@@ -40,54 +40,59 @@
 `GP` - Gradient Penalty * `SSL` - Auxiliary Reconstruction in Discriminator
 (from Lightweight GAN) A healthy run would have `G`, `MSG`, `D`, `MSD` with
 values hovering between `0` to `10`, and usually staying pretty constant. If at
 any time after 1k training steps these values persist at triple digits, that
 would mean something is wrong. It is ok for generator and discriminator values
 to occasionally dip negative, but it should swing back up to the range above.
 `GP` and `SSL` should be pushed towards `0`. `GP` can occasionally spike; I
-like to imagine it as the networks undergoing some epiphany ## Todo - [x] make
-sure it can be trained unconditionally - [x] read the relevant papers and knock
-out all 3 auxiliary losses - [x] matching aware loss - [x] clip loss - [x]
-vision-aided discriminator loss - [x] add reconstruction losses on arbitrary
-stages in the discriminator (lightweight gan) - [x] figure out how the random
-projections are used from projected-gan - [x] vision aided discriminator needs
-to extract N layers from the vision model in CLIP - [x] figure out whether to
-discard CLS token and reshape into image dimensions for convolution, or stick
-with attention and condition with adaptive layernorm - also turn off vision
-aided gan in unconditional case - [x] unet upsampler - [x] add adaptive conv -
-[x] modify latter stage of unet to also output rgb residuals, and pass the rgb
-into discriminator. make discriminator agnostic to rgb being passed in - [x] do
-pixel shuffle upsamples for unet - [x] get a code review for the multi-scale
-inputs and outputs, as the paper was a bit vague - [x] add upsampling network
-architecture - [x] make unconditional work for both base generator and
-upsampler - [x] make text conditioned training work for both base and upsampler
-- [x] make recon more efficient by random sampling patches - [x] make sure
-generator and discriminator can also accept pre-encoded CLIP text encodings -
-[ ] add accelerate - [x] works single machine - [x] works for mixed precision
-(make sure gradient penalty is scaled correctly), take care of manual scaler
-saving and reloading, borrow from imagen-pytorch - [ ] make sure it works
-multi-GPU for one machine - [ ] have someone else try multiple machines - [ ]
-add ability to select a random subset from multiscale dimension, for efficiency
-- [ ] add some differentiable augmentations, proven technique from the old GAN
-days - [ ] remove any magic being done with automatic rgbs processing, and have
-it explicitly passed in - offer functions on the discriminator that can process
-real images into the right multi-scales - [ ] add horizontal flip for starters
-- [ ] do a review of the auxiliary losses - [ ] add vision aided loss and make
-sure it trains, inspect output - [ ] port over CLI from lightweight|stylegan2-
-pytorch - [ ] hook up laion dataset for text-image ## Citations ```bibtex @misc
-{https://doi.org/10.48550/arxiv.2303.05511, url = {https://arxiv.org/abs/
-2303.05511}, author = {Kang, Minguk and Zhu, Jun-Yan and Zhang, Richard and
-Park, Jaesik and Shechtman, Eli and Paris, Sylvain and Park, Taesung}, title =
-{Scaling up GANs for Text-to-Image Synthesis}, publisher = {arXiv}, year =
-{2023}, copyright = {arXiv.org perpetual, non-exclusive license} } ```
-```bibtex @article{Liu2021TowardsFA, title = {Towards Faster and Stabilized GAN
-Training for High-fidelity Few-shot Image Synthesis}, author = {Bingchen Liu
-and Yizhe Zhu and Kunpeng Song and A. Elgammal}, journal = {ArXiv}, year =
-{2021}, volume = {abs/2101.04775} } ``` ```bibtex @inproceedings
-{dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
-Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
-Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
-in Neural Information Processing Systems}, year = {2022} } ``` ```bibtex
-@inproceedings{Heusel2017GANsTB, title = {GANs Trained by a Two Time-Scale
-Update Rule Converge to a Local Nash Equilibrium}, author = {Martin Heusel and
-Hubert Ramsauer and Thomas Unterthiner and Bernhard Nessler and Sepp
-Hochreiter}, booktitle = {NIPS}, year = {2017} } ```
+like to imagine it as the networks undergoing some epiphany ## Multi-GPU
+Training The `GigaGAN` class is now equipped with ð¤_Accelerator. You can
+easily do multi-gpu training in two steps using their `accelerate` CLI At the
+project root directory, where the training script is, run ```python $
+accelerate config ``` Then, in the same directory ```python $ accelerate launch
+train.py ``` ## Todo - [x] make sure it can be trained unconditionally - [x]
+read the relevant papers and knock out all 3 auxiliary losses - [x] matching
+aware loss - [x] clip loss - [x] vision-aided discriminator loss - [x] add
+reconstruction losses on arbitrary stages in the discriminator (lightweight
+gan) - [x] figure out how the random projections are used from projected-gan -
+[x] vision aided discriminator needs to extract N layers from the vision model
+in CLIP - [x] figure out whether to discard CLS token and reshape into image
+dimensions for convolution, or stick with attention and condition with adaptive
+layernorm - also turn off vision aided gan in unconditional case - [x] unet
+upsampler - [x] add adaptive conv - [x] modify latter stage of unet to also
+output rgb residuals, and pass the rgb into discriminator. make discriminator
+agnostic to rgb being passed in - [x] do pixel shuffle upsamples for unet - [x]
+get a code review for the multi-scale inputs and outputs, as the paper was a
+bit vague - [x] add upsampling network architecture - [x] make unconditional
+work for both base generator and upsampler - [x] make text conditioned training
+work for both base and upsampler - [x] make recon more efficient by random
+sampling patches - [x] make sure generator and discriminator can also accept
+pre-encoded CLIP text encodings - [ ] add accelerate - [x] works single machine
+- [x] works for mixed precision (make sure gradient penalty is scaled
+correctly), take care of manual scaler saving and reloading, borrow from
+imagen-pytorch - [x] make sure it works multi-GPU for one machine - [ ] have
+someone else try multiple machines - [ ] add ability to select a random subset
+from multiscale dimension, for efficiency - [ ] add some differentiable
+augmentations, proven technique from the old GAN days - [ ] remove any magic
+being done with automatic rgbs processing, and have it explicitly passed in -
+offer functions on the discriminator that can process real images into the
+right multi-scales - [ ] add horizontal flip for starters - [ ] do a review of
+the auxiliary losses - [ ] add vision aided loss and make sure it trains,
+inspect output - [ ] port over CLI from lightweight|stylegan2-pytorch - [ ]
+hook up laion dataset for text-image ## Citations ```bibtex @misc{https://
+doi.org/10.48550/arxiv.2303.05511, url = {https://arxiv.org/abs/2303.05511},
+author = {Kang, Minguk and Zhu, Jun-Yan and Zhang, Richard and Park, Jaesik and
+Shechtman, Eli and Paris, Sylvain and Park, Taesung}, title = {Scaling up GANs
+for Text-to-Image Synthesis}, publisher = {arXiv}, year = {2023}, copyright =
+{arXiv.org perpetual, non-exclusive license} } ``` ```bibtex @article
+{Liu2021TowardsFA, title = {Towards Faster and Stabilized GAN Training for
+High-fidelity Few-shot Image Synthesis}, author = {Bingchen Liu and Yizhe Zhu
+and Kunpeng Song and A. Elgammal}, journal = {ArXiv}, year = {2021}, volume =
+{abs/2101.04775} } ``` ```bibtex @inproceedings{dao2022flashattention, title =
+{Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
+Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
+Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
+Processing Systems}, year = {2022} } ``` ```bibtex @inproceedings
+{Heusel2017GANsTB, title = {GANs Trained by a Two Time-Scale Update Rule
+Converge to a Local Nash Equilibrium}, author = {Martin Heusel and Hubert
+Ramsauer and Thomas Unterthiner and Bernhard Nessler and Sepp Hochreiter},
+booktitle = {NIPS}, year = {2017} } ```
```

### Comparing `gigagan-pytorch-0.1.7/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.1.8/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.7/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.1.8/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.7/gigagan_pytorch/data.py` & `gigagan-pytorch-0.1.8/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.7/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.1.8/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1664,26 +1664,27 @@
         early_save_and_sample_every = 100,
         num_samples = 25,
         model_folder = './gigagan-models',
         results_folder = './gigagan-results',
         sample_upsampler_dl: Optional[DataLoader] = None,
         accelerator: Optional[Accelerator] = None,
         accelerate_kwargs: dict = {},
+        find_unused_parameters = False,
         amp = False,
         mixed_precision_type = 'fp16'
     ):
         super().__init__()
 
         # create accelerator
 
         if accelerator:
             self.accelerator = accelerator
             assert is_empty(accelerate_kwargs)
         else:
-            kwargs = DistributedDataParallelKwargs(find_unused_parameters = True)
+            kwargs = DistributedDataParallelKwargs(find_unused_parameters = find_unused_parameters)
 
             self.accelerator = Accelerator(
                 kwargs_handlers = [kwargs],
                 mixed_precision = mixed_precision_type if amp else 'no',
                 **accelerate_kwargs
             )
 
@@ -1722,16 +1723,16 @@
         self.has_ema_generator = False
 
         if self.is_main and create_ema_generator_at_init:
             self.create_ema_generator()
 
         # print number of parameters
 
-        print(f'Generator parameters: {numerize.numerize(generator.total_params)}')
-        print(f'Discriminator parameters: {numerize.numerize(discriminator.total_params)}')
+        self.print(f'Generator parameters: {numerize.numerize(generator.total_params)}')
+        self.print(f'Discriminator parameters: {numerize.numerize(discriminator.total_params)}')
 
         # text encoder
 
         if exists(text_encoder):
             if isinstance(text_encoder, dict):
                 text_encoder = TextEncoder(**text_encoder)
 
@@ -1928,15 +1929,15 @@
         else:
             assert exists(batch_size)
 
             G_kwargs = dict(batch_size = batch_size)
 
         # create noise
 
-        noise = torch.randn(batch_size, self.G.style_network.dim, device = self.device)
+        noise = torch.randn(batch_size, self.unwrapped_G.style_network.dim, device = self.device)
 
         G_kwargs.update(noise = noise)
 
         return G_kwargs, maybe_text_kwargs
     
     @beartype
     def train_discriminator_step(
```

### Comparing `gigagan-pytorch-0.1.7/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.1.8/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.7/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.1.8/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.7/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.1.8/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.7/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.7
+Version: 0.1.8
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.7/setup.py` & `gigagan-pytorch-0.1.8/setup.py`

 * *Files identical despite different names*

