# Comparing `tmp/gigagan-pytorch-0.1.0.tar.gz` & `tmp/gigagan-pytorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.1.0.tar", last modified: Thu Jul 20 15:21:14 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.1.1.tar", last modified: Thu Jul 20 16:49:59 2023, max compression
```

## Comparing `gigagan-pytorch-0.1.0.tar` & `gigagan-pytorch-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:14.500859 gigagan-pytorch-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 15:21:14.500859 gigagan-pytorch-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:14.496859 gigagan-pytorch-0.1.0/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    68870 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:14.500859 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:14.500859 gigagan-pytorch-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69663 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 16:49:59.000000 gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:49:59.497492 gigagan-pytorch-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 16:49:41.000000 gigagan-pytorch-0.1.1/setup.py
```

### Comparing `gigagan-pytorch-0.1.0/LICENSE` & `gigagan-pytorch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.0/PKG-INFO` & `gigagan-pytorch-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.0/README.md` & `gigagan-pytorch-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -157,15 +157,25 @@
 - [x] get a code review for the multi-scale inputs and outputs, as the paper was a bit vague
 - [x] add upsampling network architecture
 - [x] make unconditional work for both base generator and upsampler
 - [x] make text conditioned training work for both base and upsampler
 - [x] make recon more efficient by random sampling patches
 
 - [ ] add accelerate
+    - [x] works single machine
+    - [ ] works for mixed precision (make sure gradient penalty is scaled correctly), take care of manual scaler saving and reloading, borrow from imagen-pytorch
+    - [ ] make sure it works multi-GPU for one machine
+    - [ ] have someone else try multiple machines
+
+- [ ] add ability to select a random subset from multiscale dimension, for efficiency
+- [ ] make sure text encoder can also accept pre-encoded CLIP embeddings
+
 - [ ] do a review of the auxiliary losses
+    - [ ] add vision aided loss and make sure it trains, inspect output
+
 - [ ] port over CLI from lightweight|stylegan2-pytorch
 - [ ] hook up laion dataset for text-image
 
 ## Citations
 
 ```bibtex
 @misc{https://doi.org/10.48550/arxiv.2303.05511,
```

#### html2text {}

```diff
@@ -55,26 +55,33 @@
 modify latter stage of unet to also output rgb residuals, and pass the rgb into
 discriminator. make discriminator agnostic to rgb being passed in - [x] do
 pixel shuffle upsamples for unet - [x] get a code review for the multi-scale
 inputs and outputs, as the paper was a bit vague - [x] add upsampling network
 architecture - [x] make unconditional work for both base generator and
 upsampler - [x] make text conditioned training work for both base and upsampler
 - [x] make recon more efficient by random sampling patches - [ ] add accelerate
-- [ ] do a review of the auxiliary losses - [ ] port over CLI from
-lightweight|stylegan2-pytorch - [ ] hook up laion dataset for text-image ##
-Citations ```bibtex @misc{https://doi.org/10.48550/arxiv.2303.05511, url =
-{https://arxiv.org/abs/2303.05511}, author = {Kang, Minguk and Zhu, Jun-Yan and
-Zhang, Richard and Park, Jaesik and Shechtman, Eli and Paris, Sylvain and Park,
-Taesung}, title = {Scaling up GANs for Text-to-Image Synthesis}, publisher =
-{arXiv}, year = {2023}, copyright = {arXiv.org perpetual, non-exclusive
-license} } ``` ```bibtex @article{Liu2021TowardsFA, title = {Towards Faster and
-Stabilized GAN Training for High-fidelity Few-shot Image Synthesis}, author =
-{Bingchen Liu and Yizhe Zhu and Kunpeng Song and A. Elgammal}, journal =
-{ArXiv}, year = {2021}, volume = {abs/2101.04775} } ``` ```bibtex
-@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
-Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
-Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
-booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ``` ```bibtex @inproceedings{Heusel2017GANsTB, title = {GANs Trained by a Two
-Time-Scale Update Rule Converge to a Local Nash Equilibrium}, author = {Martin
-Heusel and Hubert Ramsauer and Thomas Unterthiner and Bernhard Nessler and Sepp
-Hochreiter}, booktitle = {NIPS}, year = {2017} } ```
+- [x] works single machine - [ ] works for mixed precision (make sure gradient
+penalty is scaled correctly), take care of manual scaler saving and reloading,
+borrow from imagen-pytorch - [ ] make sure it works multi-GPU for one machine -
+[ ] have someone else try multiple machines - [ ] add ability to select a
+random subset from multiscale dimension, for efficiency - [ ] make sure text
+encoder can also accept pre-encoded CLIP embeddings - [ ] do a review of the
+auxiliary losses - [ ] add vision aided loss and make sure it trains, inspect
+output - [ ] port over CLI from lightweight|stylegan2-pytorch - [ ] hook up
+laion dataset for text-image ## Citations ```bibtex @misc{https://doi.org/
+10.48550/arxiv.2303.05511, url = {https://arxiv.org/abs/2303.05511}, author =
+{Kang, Minguk and Zhu, Jun-Yan and Zhang, Richard and Park, Jaesik and
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

### Comparing `gigagan-pytorch-0.1.0/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.1.1/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.0/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.1.1/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.0/gigagan_pytorch/data.py` & `gigagan-pytorch-0.1.1/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.0/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.1.1/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1631,26 +1631,33 @@
         early_save_thres_steps = 2500,
         early_save_and_sample_every = 100,
         num_samples = 25,
         model_folder = './gigagan-models',
         results_folder = './gigagan-results',
         sample_upsampler_dl: Optional[DataLoader] = None,
         accelerator: Optional[Accelerator] = None,
-        accelerate_kwargs: dict = {}
+        accelerate_kwargs: dict = {},
+        amp = False,
+        mixed_precision_type = 'fp16'
     ):
         super().__init__()
 
         # create accelerator
 
         if accelerator:
             self.accelerator = accelerator
             assert is_empty(accelerate_kwargs)
         else:
             kwargs = DistributedDataParallelKwargs(find_unused_parameters = True)
-            self.accelerator = Accelerator(kwargs_handlers = [kwargs], **accelerate_kwargs)
+
+            self.accelerator = Accelerator(
+                kwargs_handlers = [kwargs],
+                mixed_precision = mixed_precision_type if amp else 'no',
+                **accelerate_kwargs
+            )
 
         # whether to train upsampler or not
 
         self.train_upsampler = train_upsampler
 
         if train_upsampler:
             from gigagan_pytorch.unet_upsampler import UnetUpsampler
@@ -1671,16 +1678,23 @@
         if isinstance(discriminator, dict):
             discriminator = Discriminator(**discriminator)
 
         assert isinstance(generator, generator_klass)
 
         # use _base to designate unwrapped models
 
-        self.G_base = generator
-        self.D_base = discriminator
+        self.G = generator
+        self.D = discriminator
+
+        # ema
+
+        self.has_ema_generator = False
+
+        if self.is_main and create_ema_generator_at_init:
+            self.create_ema_generator()
 
         # print number of parameters
 
         print(f'Generator parameters: {numerize.numerize(generator.total_params)}')
         print(f'Discriminator parameters: {numerize.numerize(discriminator.total_params)}')
 
         # text encoder
@@ -1693,33 +1707,26 @@
 
         assert generator.unconditional == discriminator.unconditional
 
         self.unconditional = generator.unconditional
 
         # optimizers
 
-        self.G_opt = get_optimizer(self.G_base.parameters(), lr = learning_rate, betas = betas, weight_decay = weight_decay)
-        self.D_opt = get_optimizer(self.D_base.parameters(), lr = learning_rate * ttur_mult, betas = betas, weight_decay = weight_decay)
+        self.G_opt = get_optimizer(self.G.parameters(), lr = learning_rate, betas = betas, weight_decay = weight_decay)
+        self.D_opt = get_optimizer(self.D.parameters(), lr = learning_rate * ttur_mult, betas = betas, weight_decay = weight_decay)
 
         # prepare for distributed
 
-        self.G, self.D, self.G_opt, self.D_opt = self.accelerator.prepare(self.G_base, self.D_base, self.G_opt, self.D_opt)
+        self.G, self.D, self.G_opt, self.D_opt = self.accelerator.prepare(self.G, self.D, self.G_opt, self.D_opt)
 
         # loss related
 
         self.discr_aux_recon_loss_weight = discr_aux_recon_loss_weight
         self.multiscale_divergence_loss_weight = multiscale_divergence_loss_weight
 
-        # ema
-
-        self.has_ema_generator = False
-
-        if self.is_main and create_ema_generator_at_init:
-            self.create_ema_generator()
-
         # steps
 
         self.log_steps_every = log_steps_every
 
         self.register_buffer('steps', torch.ones(1, dtype = torch.long))
 
         # save and sample
@@ -1745,16 +1752,16 @@
     def save(self, path, overwrite = True):
         path = Path(path)
         mkdir_if_not_exists(path.parents[0])
 
         assert overwrite or not path.exists()
 
         pkg = dict(
-            G = self.G_base.state_dict(),
-            D = self.D_base.state_dict(),
+            G = self.unwrapped_G.state_dict(),
+            D = self.unwrapped_D.state_dict(),
             G_opt = self.G_opt.state_dict(),
             D_opt = self.D_opt.state_dict(),
             steps = self.steps.item(),
             version = __version__
         )
 
         if self.has_ema_generator:
@@ -1767,16 +1774,16 @@
         assert path.exists()
 
         pkg = torch.load(str(path))
 
         if 'version' in pkg and pkg['version'] != __version__:
             print(f"trying to load from version {pkg['version']}")
 
-        self.G_base.load_state_dict(pkg['G'], strict = strict)
-        self.D_base.load_state_dict(pkg['D'], strict = strict)
+        self.unwrapped_G.load_state_dict(pkg['G'], strict = strict)
+        self.unwrapped_D.load_state_dict(pkg['D'], strict = strict)
 
         if self.has_ema_generator:
             self.G_ema.load_state_dict(pkg['G_ema'])
 
         if 'steps' in pkg:
             self.steps.copy_(torch.tensor([pkg['steps']]))
 
@@ -1792,14 +1799,22 @@
 
     # accelerate related
 
     @property
     def device(self):
         return self.accelerator.device
 
+    @property
+    def unwrapped_G(self):
+        return self.accelerator.unwrap_model(self.G)
+
+    @property
+    def unwrapped_D(self):
+        return self.accelerator.unwrap_model(self.D)
+
     def print(self, msg):
         self.accelerator.print(msg)
 
     @property
     def is_distributed(self):
         return not (self.accelerator.distributed_type == DistributedType.NO and self.accelerator.num_processes == 1)
 
@@ -1829,16 +1844,16 @@
         decay = 0.995
     ):
         if not self.is_main:
             return
 
         assert not self.has_ema_generator, 'EMA generator has already been created'
 
+        self.G_ema = EMA(self.unwrapped_G, update_every = update_every, update_after_step = update_after_step, beta = decay)
         self.has_ema_generator = True
-        self.G_ema = EMA(self.G, update_every = update_every, update_after_step = update_after_step, beta = decay)
 
     def generate_kwargs(self, dl_iter, batch_size):
         # what to pass into the generator
         # depends on whether training upsampler or not
 
         maybe_text_kwargs = dict()
         if self.train_upsampler or not self.unconditional:
@@ -1915,86 +1930,87 @@
 
             # for discriminator training, fit upsampler and image synthesis logic under same function
 
             G_kwargs, maybe_text_kwargs = self.generate_kwargs(dl_iter, batch_size)
 
             # generator
 
-            with torch.no_grad():
+            with torch.no_grad(), self.accelerator.autocast():
                 images, rgbs = self.G(
                     **G_kwargs,
                     **maybe_text_kwargs,
                     return_all_rgbs = True
                 )
 
-            # detach output of generator, as training discriminator only
+                # detach output of generator, as training discriminator only
 
-            images.detach_()
+                images.detach_()
 
-            for rgb in rgbs:
-                rgb.detach_()
+                for rgb in rgbs:
+                    rgb.detach_()
 
             # main divergence loss
 
-            fake_logits, fake_multiscale_logits, _ = self.D(
-                images,
-                rgbs,
-                **maybe_text_kwargs,
-                return_multiscale_outputs = calc_multiscale_loss,
-                calc_aux_loss = False
-            )
+            with self.accelerator.autocast():
+                fake_logits, fake_multiscale_logits, _ = self.D(
+                    images,
+                    rgbs,
+                    **maybe_text_kwargs,
+                    return_multiscale_outputs = calc_multiscale_loss,
+                    calc_aux_loss = False
+                )
 
-            real_logits, real_multiscale_logits, aux_recon_losses = self.D(
-                real_images,
-                **maybe_text_kwargs,
-                return_multiscale_outputs = calc_multiscale_loss,
-                calc_aux_loss = True
-            )
+                real_logits, real_multiscale_logits, aux_recon_losses = self.D(
+                    real_images,
+                    **maybe_text_kwargs,
+                    return_multiscale_outputs = calc_multiscale_loss,
+                    calc_aux_loss = True
+                )
 
-            divergence = discriminator_hinge_loss(real_logits, fake_logits)
-            total_divergence += (divergence.item() / grad_accum_every)
+                divergence = discriminator_hinge_loss(real_logits, fake_logits)
+                total_divergence += (divergence.item() / grad_accum_every)
 
-            # handle multi-scale divergence
+                # handle multi-scale divergence
 
-            multiscale_divergence = 0.
+                multiscale_divergence = 0.
 
-            if self.multiscale_divergence_loss_weight > 0. and len(fake_multiscale_logits) > 0:
+                if self.multiscale_divergence_loss_weight > 0. and len(fake_multiscale_logits) > 0:
 
-                for multiscale_fake, multiscale_real in zip(fake_multiscale_logits, real_multiscale_logits):
-                    multiscale_loss = discriminator_hinge_loss(multiscale_real, multiscale_fake)
-                    multiscale_divergence = multiscale_divergence + multiscale_loss
+                    for multiscale_fake, multiscale_real in zip(fake_multiscale_logits, real_multiscale_logits):
+                        multiscale_loss = discriminator_hinge_loss(multiscale_real, multiscale_fake)
+                        multiscale_divergence = multiscale_divergence + multiscale_loss
 
-                total_multiscale_divergence += (multiscale_divergence.item() / grad_accum_every)
+                    total_multiscale_divergence += (multiscale_divergence.item() / grad_accum_every)
 
-            # figure out gradient penalty if needed
+                # figure out gradient penalty if needed
 
-            gp_loss = 0.
+                gp_loss = 0.
 
-            if apply_gradient_penalty:
-                gp_loss = gradient_penalty(
-                    real_images,
-                    outputs = [real_logits, *real_multiscale_logits],
-                    grad_output_weights = [1., *(self.multiscale_divergence_loss_weight,) * len(real_multiscale_logits)]
-                )
+                if apply_gradient_penalty:
+                    gp_loss = gradient_penalty(
+                        real_images,
+                        outputs = [real_logits, *real_multiscale_logits],
+                        grad_output_weights = [1., *(self.multiscale_divergence_loss_weight,) * len(real_multiscale_logits)]
+                    )
 
-                total_gp_loss += (gp_loss.item() / grad_accum_every)
+                    total_gp_loss += (gp_loss.item() / grad_accum_every)
 
-            # sum up losses
+                # sum up losses
 
-            total_loss = divergence + gp_loss
+                total_loss = divergence + gp_loss
 
-            if self.multiscale_divergence_loss_weight > 0.:
-                total_loss = total_loss + multiscale_divergence * self.multiscale_divergence_loss_weight
+                if self.multiscale_divergence_loss_weight > 0.:
+                    total_loss = total_loss + multiscale_divergence * self.multiscale_divergence_loss_weight
 
-            if self.discr_aux_recon_loss_weight > 0.:
-                aux_loss = sum(aux_recon_losses)
+                if self.discr_aux_recon_loss_weight > 0.:
+                    aux_loss = sum(aux_recon_losses)
 
-                total_aux_loss += (aux_loss.item() / grad_accum_every)
+                    total_aux_loss += (aux_loss.item() / grad_accum_every)
 
-                total_loss = total_loss + aux_loss * self.discr_aux_recon_loss_weight
+                    total_loss = total_loss + aux_loss * self.discr_aux_recon_loss_weight
 
             # backwards
 
             self.accelerator.backward(total_loss / grad_accum_every)
 
         self.D_opt.step()
 
@@ -2018,47 +2034,48 @@
 
         for _ in range(grad_accum_every):
 
             # generator
             
             G_kwargs, maybe_text_kwargs = self.generate_kwargs(dl_iter, batch_size)
 
-            image, rgbs = self.G(
-                **G_kwargs,
-                **maybe_text_kwargs,
-                return_all_rgbs = True
-            )
+            with self.accelerator.autocast():
+                image, rgbs = self.G(
+                    **G_kwargs,
+                    **maybe_text_kwargs,
+                    return_all_rgbs = True
+                )
 
-            # discriminator
+                # discriminator
 
-            logits, multiscale_logits, _ = self.D(
-                image,
-                rgbs,
-                **maybe_text_kwargs,
-                return_multiscale_outputs = calc_multiscale_loss,
-                calc_aux_loss = False
-            )
+                logits, multiscale_logits, _ = self.D(
+                    image,
+                    rgbs,
+                    **maybe_text_kwargs,
+                    return_multiscale_outputs = calc_multiscale_loss,
+                    calc_aux_loss = False
+                )
 
-            # hinge loss
+                # hinge loss
 
-            divergence = generator_hinge_loss(logits)
+                divergence = generator_hinge_loss(logits)
 
-            total_divergence += (divergence.item() / grad_accum_every)
+                total_divergence += (divergence.item() / grad_accum_every)
 
-            total_loss = divergence
+                total_loss = divergence
 
-            if self.multiscale_divergence_loss_weight > 0. and len(multiscale_logits) > 0:
-                multiscale_divergence = 0.
+                if self.multiscale_divergence_loss_weight > 0. and len(multiscale_logits) > 0:
+                    multiscale_divergence = 0.
 
-                for multiscale_logit in multiscale_logits:
-                    multiscale_divergence = multiscale_divergence + generator_hinge_loss(multiscale_logit)
+                    for multiscale_logit in multiscale_logits:
+                        multiscale_divergence = multiscale_divergence + generator_hinge_loss(multiscale_logit)
 
-                total_multiscale_divergence += (multiscale_divergence.item() / grad_accum_every)
+                    total_multiscale_divergence += (multiscale_divergence.item() / grad_accum_every)
 
-                total_loss = total_loss + multiscale_divergence * self.multiscale_divergence_loss_weight
+                    total_loss = total_loss + multiscale_divergence * self.multiscale_divergence_loss_weight
 
             self.accelerator.backward(total_loss / grad_accum_every)
 
         self.G_opt.step()
 
         # update exponentially moving averaged generator
 
@@ -2066,15 +2083,16 @@
             self.G_ema.update()
 
         return TrainGenLosses(total_divergence, total_multiscale_divergence)
 
     def sample_lambda(self, dl_iter, batch_size):
         G_kwargs, maybe_text_kwargs = self.generate_kwargs(dl_iter, batch_size)
 
-        generator_output = self.G(**G_kwargs, **maybe_text_kwargs)
+        with self.accelerator.autocast():
+            generator_output = self.G(**G_kwargs, **maybe_text_kwargs)
 
         if not self.train_upsampler:
             return generator_output
 
         output_size = generator_output.shape[-1]
         lowres_image = G_kwargs['lowres_image']
         lowres_image = F.interpolate(lowres_image, (output_size, output_size))
@@ -2113,15 +2131,15 @@
                 all_images,
                 str(self.results_folder / filename),
                 nrow = int(sqrt(self.num_samples)) * nrow_mult
             )
 
         # Possible to do: Include some metric to save if improved, include some sampler dict text entries
         self.save(str(self.model_folder / f'model-{milestone}.ckpt'))
-        
+
     @beartype
     def forward(
         self,
         *,
         steps,
         grad_accum_every = 1
     ):
```

### Comparing `gigagan-pytorch-0.1.0/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.1.1/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.0/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.1.1/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.0/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.1.1/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.1.1/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.0/setup.py` & `gigagan-pytorch-0.1.1/setup.py`

 * *Files identical despite different names*

