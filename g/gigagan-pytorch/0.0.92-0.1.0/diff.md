# Comparing `tmp/gigagan-pytorch-0.0.92.tar.gz` & `tmp/gigagan-pytorch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.0.92.tar", last modified: Thu Jul 20 04:08:35 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.1.0.tar", last modified: Thu Jul 20 15:21:14 2023, max compression
```

## Comparing `gigagan-pytorch-0.0.92.tar` & `gigagan-pytorch-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:08:35.726359 gigagan-pytorch-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-20 04:08:35.726359 gigagan-pytorch-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:08:35.726359 gigagan-pytorch-0.0.92/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:08:35.726359 gigagan-pytorch-0.0.92/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-20 04:08:35.000000 gigagan-pytorch-0.0.92/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 04:08:35.000000 gigagan-pytorch-0.0.92/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:08:35.000000 gigagan-pytorch-0.0.92/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 04:08:35.000000 gigagan-pytorch-0.0.92/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 04:08:35.000000 gigagan-pytorch-0.0.92/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:08:35.726359 gigagan-pytorch-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 04:08:23.000000 gigagan-pytorch-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:14.500859 gigagan-pytorch-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 15:21:14.500859 gigagan-pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:14.496859 gigagan-pytorch-0.1.0/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68870 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:14.500859 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 15:21:14.000000 gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:14.500859 gigagan-pytorch-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 15:21:04.000000 gigagan-pytorch-0.1.0/setup.py
```

### Comparing `gigagan-pytorch-0.0.92/LICENSE` & `gigagan-pytorch-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.0.92/PKG-INFO` & `gigagan-pytorch-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.0.92
+Version: 0.1.0
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.0.92/README.md` & `gigagan-pytorch-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img src="./gigagan-sample.png" width="500px"></img>
 
 <img src="./gigagan-architecture.png" width="500px"></img>
 
-## GigaGAN - Pytorch (wip)
+## GigaGAN - Pytorch
 
 Implementation of <a href="https://arxiv.org/abs/2303.05511v2">GigaGAN</a> <a href="https://mingukkang.github.io/GigaGAN/">(project page)</a>, new SOTA GAN out of Adobe.
 
 I will also add a few findings from <a href="https://github.com/lucidrains/lightweight-gan">lightweight gan</a>, for faster convergence (skip layer excitation) and better stability (reconstruction auxiliary loss in discriminator).
 
 It will also contain the code for the 1k - 4k upsamplers, which I find to be the highlight of this paper.
 
@@ -20,14 +20,20 @@
 
 - All the maintainers at <a href="https://github.com/mlfoundations/open_clip">OpenClip</a>, for their SOTA open sourced contrastive learning text-image models
 
 - <a href="https://github.com/XavierXiao">Xavier</a> for reviewing the discriminator code and pointing out that the scale invariance was not correctly built!
 
 - <a href="https://github.com/CerebralSeed">@CerebralSeed</a> for pull requesting the initial sampling code for both the generator and upsampler!
 
+## Install
+
+```bash
+$ pip install gigagan-pytorch
+```
+
 ## Usage
 
 Simple unconditional GAN, for starters
 
 ```python
 import torch
 
@@ -125,17 +131,17 @@
 * `G` - Generator
 * `MSG` - Multiscale Generator
 * `D` - Discriminator
 * `MSD` - Multiscale Discriminator
 * `GP` - Gradient Penalty
 * `SSL` - Auxiliary Reconstruction in Discriminator (from Lightweight GAN)
 
-A healthy run would have `G`, `MSG`, `D`, `MSD` with values hovering between `-10` to `10`, and usually staying pretty constant. If at any time after 1k training steps these values persist at triple digits, that would mean something is wrong.
+A healthy run would have `G`, `MSG`, `D`, `MSD` with values hovering between `0` to `10`, and usually staying pretty constant. If at any time after 1k training steps these values persist at triple digits, that would mean something is wrong. It is ok for generator and discriminator values to occasionally dip negative, but it should swing back up to the range above.
 
-`GP` and `SSL` should be pushed towards `0`. `GP` can occasionally spike; I like to imagine it as the networks undergoing some phase shift.
+`GP` and `SSL` should be pushed towards `0`. `GP` can occasionally spike; I like to imagine it as the networks undergoing some epiphany
 
 ## Todo
 
 - [x] make sure it can be trained unconditionally
 - [x] read the relevant papers and knock out all 3 auxiliary losses
     - [x] matching aware loss
     - [x] clip loss
```

#### html2text {}

```diff
@@ -1,76 +1,79 @@
-[./gigagan-sample.png] [./gigagan-architecture.png] ## GigaGAN - Pytorch (wip)
+[./gigagan-sample.png] [./gigagan-architecture.png] ## GigaGAN - Pytorch
 Implementation of GigaGAN (project_page), new SOTA GAN out of Adobe. I will
 also add a few findings from lightweight_gan, for faster convergence (skip
 layer excitation) and better stability (reconstruction auxiliary loss in
 discriminator). It will also contain the code for the 1k - 4k upsamplers, which
 I find to be the highlight of this paper. Please join [Join_us_on_Discord] if
 you are interested in helping out with the replication with the LAION community
 ## Appreciation - StabilityAI for the sponsorship, as well as my other
 sponsors, for affording me the independence to open source artificial
 intelligence. - ð¤_Huggingface for their accelerate library - All the
 maintainers at OpenClip, for their SOTA open sourced contrastive learning text-
 image models - Xavier for reviewing the discriminator code and pointing out
 that the scale invariance was not correctly built! - @CerebralSeed for pull
 requesting the initial sampling code for both the generator and upsampler! ##
-Usage Simple unconditional GAN, for starters ```python import torch from
-gigagan_pytorch import ( GigaGAN, ImageDataset ) gan = GigaGAN( generator =
-dict( dim_capacity = 8, style_network = dict( dim = 64, depth = 4 ), image_size
-= 256, dim_max = 512, num_skip_layers_excite = 4, unconditional = True ),
-discriminator = dict( dim_capacity = 16, dim_max = 512, image_size = 256,
-num_skip_layers_excite = 4, unconditional = True ) ).cuda() # dataset dataset =
-ImageDataset( folder = '/path/to/your/data', image_size = 256 ) dataloader =
-dataset.get_dataloader(batch_size = 1) # training the discriminator and
-generator alternating # for 100 steps in this example, batch size 1, gradient
-accumulated 8 times gan( dataloader = dataloader, steps = 100, grad_accum_every
-= 8 ) ``` For unconditional Unet Upsampler ```python import torch from
-gigagan_pytorch import GigaGAN, ImageDataset gan = GigaGAN( train_upsampler =
-True, # set this to True generator = dict( style_network = dict( dim = 64,
-depth = 4 ), dim = 32, image_size = 256, input_image_size = 128, unconditional
-= True ), discriminator = dict( dim_capacity = 16, dim_max = 512, image_size =
-256, num_skip_layers_excite = 4, unconditional = True ) ).cuda() dataset =
+Install ```bash $ pip install gigagan-pytorch ``` ## Usage Simple unconditional
+GAN, for starters ```python import torch from gigagan_pytorch import ( GigaGAN,
+ImageDataset ) gan = GigaGAN( generator = dict( dim_capacity = 8, style_network
+= dict( dim = 64, depth = 4 ), image_size = 256, dim_max = 512,
+num_skip_layers_excite = 4, unconditional = True ), discriminator = dict
+( dim_capacity = 16, dim_max = 512, image_size = 256, num_skip_layers_excite =
+4, unconditional = True ) ).cuda() # dataset dataset = ImageDataset( folder =
+'/path/to/your/data', image_size = 256 ) dataloader = dataset.get_dataloader
+(batch_size = 1) # training the discriminator and generator alternating # for
+100 steps in this example, batch size 1, gradient accumulated 8 times gan
+( dataloader = dataloader, steps = 100, grad_accum_every = 8 ) ``` For
+unconditional Unet Upsampler ```python import torch from gigagan_pytorch import
+GigaGAN, ImageDataset gan = GigaGAN( train_upsampler = True, # set this to True
+generator = dict( style_network = dict( dim = 64, depth = 4 ), dim = 32,
+image_size = 256, input_image_size = 128, unconditional = True ), discriminator
+= dict( dim_capacity = 16, dim_max = 512, image_size = 256,
+num_skip_layers_excite = 4, unconditional = True ) ).cuda() dataset =
 ImageDataset( folder = '/path/to/your/data', image_size = 256 ) dataloader =
 dataset.get_dataloader(batch_size = 1) # training the discriminator and
 generator alternating # for 100 steps in this example, batch size 1, gradient
 accumulated 8 times gan( dataloader = dataloader, steps = 100, grad_accum_every
 = 8 ) ``` ## Losses (wip) * `G` - Generator * `MSG` - Multiscale Generator *
 `D` - Discriminator * `MSD` - Multiscale Discriminator * `GP` - Gradient
 Penalty * `SSL` - Auxiliary Reconstruction in Discriminator (from Lightweight
 GAN) A healthy run would have `G`, `MSG`, `D`, `MSD` with values hovering
-between `-10` to `10`, and usually staying pretty constant. If at any time
-after 1k training steps these values persist at triple digits, that would mean
-something is wrong. `GP` and `SSL` should be pushed towards `0`. `GP` can
-occasionally spike; I like to imagine it as the networks undergoing some phase
-shift. ## Todo - [x] make sure it can be trained unconditionally - [x] read the
-relevant papers and knock out all 3 auxiliary losses - [x] matching aware loss
-- [x] clip loss - [x] vision-aided discriminator loss - [x] add reconstruction
-losses on arbitrary stages in the discriminator (lightweight gan) - [x] figure
-out how the random projections are used from projected-gan - [x] vision aided
-discriminator needs to extract N layers from the vision model in CLIP - [x]
-figure out whether to discard CLS token and reshape into image dimensions for
-convolution, or stick with attention and condition with adaptive layernorm -
-also turn off vision aided gan in unconditional case - [x] unet upsampler - [x]
-add adaptive conv - [x] modify latter stage of unet to also output rgb
-residuals, and pass the rgb into discriminator. make discriminator agnostic to
-rgb being passed in - [x] do pixel shuffle upsamples for unet - [x] get a code
-review for the multi-scale inputs and outputs, as the paper was a bit vague -
-[x] add upsampling network architecture - [x] make unconditional work for both
-base generator and upsampler - [x] make text conditioned training work for both
-base and upsampler - [x] make recon more efficient by random sampling patches -
-[ ] add accelerate - [ ] do a review of the auxiliary losses - [ ] port over
-CLI from lightweight|stylegan2-pytorch - [ ] hook up laion dataset for text-
-image ## Citations ```bibtex @misc{https://doi.org/10.48550/arxiv.2303.05511,
-url = {https://arxiv.org/abs/2303.05511}, author = {Kang, Minguk and Zhu, Jun-
-Yan and Zhang, Richard and Park, Jaesik and Shechtman, Eli and Paris, Sylvain
-and Park, Taesung}, title = {Scaling up GANs for Text-to-Image Synthesis},
-publisher = {arXiv}, year = {2023}, copyright = {arXiv.org perpetual, non-
-exclusive license} } ``` ```bibtex @article{Liu2021TowardsFA, title = {Towards
-Faster and Stabilized GAN Training for High-fidelity Few-shot Image Synthesis},
-author = {Bingchen Liu and Yizhe Zhu and Kunpeng Song and A. Elgammal}, journal
-= {ArXiv}, year = {2021}, volume = {abs/2101.04775} } ``` ```bibtex
+between `0` to `10`, and usually staying pretty constant. If at any time after
+1k training steps these values persist at triple digits, that would mean
+something is wrong. It is ok for generator and discriminator values to
+occasionally dip negative, but it should swing back up to the range above. `GP`
+and `SSL` should be pushed towards `0`. `GP` can occasionally spike; I like to
+imagine it as the networks undergoing some epiphany ## Todo - [x] make sure it
+can be trained unconditionally - [x] read the relevant papers and knock out all
+3 auxiliary losses - [x] matching aware loss - [x] clip loss - [x] vision-aided
+discriminator loss - [x] add reconstruction losses on arbitrary stages in the
+discriminator (lightweight gan) - [x] figure out how the random projections are
+used from projected-gan - [x] vision aided discriminator needs to extract N
+layers from the vision model in CLIP - [x] figure out whether to discard CLS
+token and reshape into image dimensions for convolution, or stick with
+attention and condition with adaptive layernorm - also turn off vision aided
+gan in unconditional case - [x] unet upsampler - [x] add adaptive conv - [x]
+modify latter stage of unet to also output rgb residuals, and pass the rgb into
+discriminator. make discriminator agnostic to rgb being passed in - [x] do
+pixel shuffle upsamples for unet - [x] get a code review for the multi-scale
+inputs and outputs, as the paper was a bit vague - [x] add upsampling network
+architecture - [x] make unconditional work for both base generator and
+upsampler - [x] make text conditioned training work for both base and upsampler
+- [x] make recon more efficient by random sampling patches - [ ] add accelerate
+- [ ] do a review of the auxiliary losses - [ ] port over CLI from
+lightweight|stylegan2-pytorch - [ ] hook up laion dataset for text-image ##
+Citations ```bibtex @misc{https://doi.org/10.48550/arxiv.2303.05511, url =
+{https://arxiv.org/abs/2303.05511}, author = {Kang, Minguk and Zhu, Jun-Yan and
+Zhang, Richard and Park, Jaesik and Shechtman, Eli and Paris, Sylvain and Park,
+Taesung}, title = {Scaling up GANs for Text-to-Image Synthesis}, publisher =
+{arXiv}, year = {2023}, copyright = {arXiv.org perpetual, non-exclusive
+license} } ``` ```bibtex @article{Liu2021TowardsFA, title = {Towards Faster and
+Stabilized GAN Training for High-fidelity Few-shot Image Synthesis}, author =
+{Bingchen Liu and Yizhe Zhu and Kunpeng Song and A. Elgammal}, journal =
+{ArXiv}, year = {2021}, volume = {abs/2101.04775} } ``` ```bibtex
 @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
 Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
 Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
 booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
 } ``` ```bibtex @inproceedings{Heusel2017GANsTB, title = {GANs Trained by a Two
 Time-Scale Update Rule Converge to a Local Nash Equilibrium}, author = {Martin
 Heusel and Hubert Ramsauer and Thomas Unterthiner and Bernhard Nessler and Sepp
```

### Comparing `gigagan-pytorch-0.0.92/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.1.0/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.0.92/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.1.0/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.0.92/gigagan_pytorch/data.py` & `gigagan-pytorch-0.1.0/gigagan_pytorch/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             T.Resize(image_size),
             T.RandomHorizontalFlip() if augment_horizontal_flip else nn.Identity(),
             T.CenterCrop(image_size),
             T.ToTensor()
         ])
 
     def get_dataloader(self, *args, **kwargs):
-        return DataLoader(self, *args, shuffle = True, **kwargs)
+        return DataLoader(self, *args, shuffle = True, drop_last = True, **kwargs)
 
     def __len__(self):
         return len(self.paths)
 
     def __getitem__(self, index):
         path = self.paths[index]
         img = Image.open(path)
```

### Comparing `gigagan-pytorch-0.0.92/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.1.0/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,26 @@
 from gigagan_pytorch.open_clip import OpenClipAdapter
 from gigagan_pytorch.optimizer import get_optimizer
 
 from tqdm import tqdm
 
 from numerize import numerize
 
+from accelerate import Accelerator, DistributedType
+from accelerate.utils import DistributedDataParallelKwargs
+
 # helpers
 
 def exists(val):
     return val is not None
 
+@beartype
+def is_empty(arr: Union[Tuple, Dict, List]):
+    return len(arr) == 0
+
 def default(*vals):
     for val in vals:
         if exists(val):
             return val
     return None
 
 def cast_tuple(t, length = 1):
@@ -66,14 +73,22 @@
     if remainder > 0:
         arr.append(remainder)
     return arr
 
 def mkdir_if_not_exists(path):
     path.mkdir(exist_ok = True, parents = True)
 
+@beartype
+def set_requires_grad_(
+    m: nn.Module,
+    requires_grad: bool
+):
+    for p in m.parameters():
+        p.requires_grad = requires_grad
+
 # activation functions
 
 def leaky_relu(neg_slope = 0.1):
     return nn.LeakyReLU(neg_slope)
 
 def conv2d_3x3(dim_in, dim_out):
     return nn.Conv2d(dim_in, dim_out, 3, padding = 1)
@@ -613,14 +628,16 @@
         super().__init__()
         self.dim = dim
 
         if not exists(clip):
             clip = OpenClipAdapter()
 
         self.clip = clip
+        set_requires_grad_(clip, False)
+
         self.learned_global_token = nn.Parameter(torch.randn(dim))
 
         self.project_in = nn.Linear(clip.dim_latent, dim) if clip.dim_latent != dim else nn.Identity()
 
         self.transformer = Transformer(
             dim = dim,
             depth = depth,
@@ -1007,15 +1024,15 @@
             rgbs.append(rgb)
 
             if exists(upsample_rgb):
                 rgb = upsample_rgb(rgb)
 
         # sanity check
 
-        assert len([*conv_mods]) == 0, 'convolutions were incorrectly modulated'
+        assert is_empty([*conv_mods]), 'convolutions were incorrectly modulated'
 
         if return_all_rgbs:
             return rgb, rgbs
 
         return rgb
 
 # discriminator
@@ -1200,20 +1217,21 @@
     ):
         super().__init__()
         self.unconditional = unconditional
         self.residual_fn = nn.Conv2d(dim, dim, 1)
         self.layers = nn.ModuleList([])
 
         klass = nn.Conv2d if unconditional else partial(AdaptiveConv2DMod, num_conv_kernels = num_conv_kernels)
+        klass_kwargs = dict(padding = 1) if unconditional else dict()
 
         for ind in range(depth):
             self.layers.append(nn.ModuleList([
-                klass(dim, dim, 3, padding = 1),
+                klass(dim, dim, 3, **klass_kwargs),
                 leaky_relu(),
-                klass(dim, dim, 3, padding = 1),
+                klass(dim, dim, 3, **klass_kwargs),
                 leaky_relu()
             ]))
 
         self.to_logits = nn.Conv2d(dim, 1, 1)
 
     def forward(
         self,
@@ -1562,15 +1580,15 @@
                 # for efficiency
 
                 aux_recon_loss = recon_decoder(recon_output, aux_recon_target)
                 aux_recon_losses.append(aux_recon_loss)
 
         # sanity check
 
-        assert self.unconditional or len([*conv_mods]) == 0, 'convolutions were incorrectly modulated'
+        assert self.unconditional or is_empty([*conv_mods]), 'convolutions were incorrectly modulated'
 
         # to logits
 
         logits = self.to_logits(x)   
         logits = rearrange(logits, '(s b) ... -> s b ...', b = batch)
 
         return logits, multiscale_outputs, aux_recon_losses
@@ -1611,41 +1629,58 @@
         create_ema_generator_at_init = True,
         save_and_sample_every = 1000,
         early_save_thres_steps = 2500,
         early_save_and_sample_every = 100,
         num_samples = 25,
         model_folder = './gigagan-models',
         results_folder = './gigagan-results',
-        val_upsampler_dl: DataLoader = None
+        sample_upsampler_dl: Optional[DataLoader] = None,
+        accelerator: Optional[Accelerator] = None,
+        accelerate_kwargs: dict = {}
     ):
         super().__init__()
 
-        self.train_upsampler = train_upsampler
+        # create accelerator
 
-        self.upsampler_replace_rgb_with_input_lowres_image = upsampler_replace_rgb_with_input_lowres_image
+        if accelerator:
+            self.accelerator = accelerator
+            assert is_empty(accelerate_kwargs)
+        else:
+            kwargs = DistributedDataParallelKwargs(find_unused_parameters = True)
+            self.accelerator = Accelerator(kwargs_handlers = [kwargs], **accelerate_kwargs)
 
-        self.apply_gradient_penalty_every = apply_gradient_penalty_every
-        self.calc_multiscale_loss_every = calc_multiscale_loss_every
+        # whether to train upsampler or not
+
+        self.train_upsampler = train_upsampler
 
         if train_upsampler:
             from gigagan_pytorch.unet_upsampler import UnetUpsampler
             generator_klass = UnetUpsampler
         else:
             generator_klass = Generator
 
+        self.upsampler_replace_rgb_with_input_lowres_image = upsampler_replace_rgb_with_input_lowres_image
+
+        # gradient penalty and auxiliary recon loss
+
+        self.apply_gradient_penalty_every = apply_gradient_penalty_every
+        self.calc_multiscale_loss_every = calc_multiscale_loss_every
+
         if isinstance(generator, dict):
             generator = generator_klass(**generator)
 
         if isinstance(discriminator, dict):
             discriminator = Discriminator(**discriminator)
 
         assert isinstance(generator, generator_klass)
 
-        self.G = generator
-        self.D = discriminator
+        # use _base to designate unwrapped models
+
+        self.G_base = generator
+        self.D_base = discriminator
 
         # print number of parameters
 
         print(f'Generator parameters: {numerize.numerize(generator.total_params)}')
         print(f'Discriminator parameters: {numerize.numerize(discriminator.total_params)}')
 
         # text encoder
@@ -1658,27 +1693,31 @@
 
         assert generator.unconditional == discriminator.unconditional
 
         self.unconditional = generator.unconditional
 
         # optimizers
 
-        self.G_opt = get_optimizer(self.G.parameters(), lr = learning_rate, betas = betas, weight_decay = weight_decay)
-        self.D_opt = get_optimizer(self.D.parameters(), lr = learning_rate * ttur_mult, betas = betas, weight_decay = weight_decay)
+        self.G_opt = get_optimizer(self.G_base.parameters(), lr = learning_rate, betas = betas, weight_decay = weight_decay)
+        self.D_opt = get_optimizer(self.D_base.parameters(), lr = learning_rate * ttur_mult, betas = betas, weight_decay = weight_decay)
+
+        # prepare for distributed
+
+        self.G, self.D, self.G_opt, self.D_opt = self.accelerator.prepare(self.G_base, self.D_base, self.G_opt, self.D_opt)
 
         # loss related
 
         self.discr_aux_recon_loss_weight = discr_aux_recon_loss_weight
         self.multiscale_divergence_loss_weight = multiscale_divergence_loss_weight
 
         # ema
 
         self.has_ema_generator = False
 
-        if create_ema_generator_at_init:
+        if self.is_main and create_ema_generator_at_init:
             self.create_ema_generator()
 
         # steps
 
         self.log_steps_every = log_steps_every
 
         self.register_buffer('steps', torch.ones(1, dtype = torch.long))
@@ -1687,31 +1726,35 @@
 
         self.save_and_sample_every = save_and_sample_every
         self.early_save_thres_steps = early_save_thres_steps
         self.early_save_and_sample_every = early_save_and_sample_every
 
         self.num_samples = num_samples
 
-        self.val_dl_iter = val_upsampler_dl
+        self.train_dl = None
+
+        self.sample_upsampler_dl_iter = None
+        if exists(sample_upsampler_dl):
+            self.sample_upsampler_dl_iter = cycle(self.sample_upsampler_dl)
 
         self.results_folder = Path(results_folder)
         self.model_folder = Path(model_folder)
 
         mkdir_if_not_exists(self.results_folder)
         mkdir_if_not_exists(self.model_folder)
 
     def save(self, path, overwrite = True):
         path = Path(path)
         mkdir_if_not_exists(path.parents[0])
 
         assert overwrite or not path.exists()
 
         pkg = dict(
-            G = self.G.state_dict(),
-            D = self.D.state_dict(),
+            G = self.G_base.state_dict(),
+            D = self.D_base.state_dict(),
             G_opt = self.G_opt.state_dict(),
             D_opt = self.D_opt.state_dict(),
             steps = self.steps.item(),
             version = __version__
         )
 
         if self.has_ema_generator:
@@ -1724,16 +1767,16 @@
         assert path.exists()
 
         pkg = torch.load(str(path))
 
         if 'version' in pkg and pkg['version'] != __version__:
             print(f"trying to load from version {pkg['version']}")
 
-        self.G.load_state_dict(pkg['G'], strict = strict)
-        self.D.load_state_dict(pkg['D'], strict = strict)
+        self.G_base.load_state_dict(pkg['G'], strict = strict)
+        self.D_base.load_state_dict(pkg['D'], strict = strict)
 
         if self.has_ema_generator:
             self.G_ema.load_state_dict(pkg['G_ema'])
 
         if 'steps' in pkg:
             self.steps.copy_(torch.tensor([pkg['steps']]))
 
@@ -1743,32 +1786,60 @@
         try:
             self.G_opt.load_state_dict(pkg['G_opt'])
             self.D_opt.load_state_dict(pkg['D_opt'])
         except Exception as e:
             self.print(f'unable to load optimizers {e.msg}- optimizer states will be reset')
             pass
 
+    # accelerate related
+
     @property
     def device(self):
-        return self.steps.device
+        return self.accelerator.device
+
+    def print(self, msg):
+        self.accelerator.print(msg)
+
+    @property
+    def is_distributed(self):
+        return not (self.accelerator.distributed_type == DistributedType.NO and self.accelerator.num_processes == 1)
+
+    @property
+    def is_main(self):
+        return self.accelerator.is_main_process
+
+    @property
+    def is_local_main(self):
+        return self.accelerator.is_local_main_process
+
+    @beartype
+    def set_dataloader(self, dl: DataLoader):
+        assert not exists(self.train_dl), 'training dataloader has already been set'
+
+        self.train_dl = dl
+        self.train_dl_batch_size = dl.batch_size
+
+        self.train_dl = self.accelerator.prepare(self.train_dl)
+
+    # create EMA generator
 
     def create_ema_generator(
         self,
         update_every = 10,
         update_after_step = 100,
         decay = 0.995
     ):
+        if not self.is_main:
+            return
+
         assert not self.has_ema_generator, 'EMA generator has already been created'
 
         self.has_ema_generator = True
         self.G_ema = EMA(self.G, update_every = update_every, update_after_step = update_after_step, beta = decay)
 
-    def print(self, msg):
-        print(msg)
-
     def generate_kwargs(self, dl_iter, batch_size):
         # what to pass into the generator
         # depends on whether training upsampler or not
 
         maybe_text_kwargs = dict()
         if self.train_upsampler or not self.unconditional:
             assert exists(dl_iter)
@@ -1919,15 +1990,15 @@
 
                 total_aux_loss += (aux_loss.item() / grad_accum_every)
 
                 total_loss = total_loss + aux_loss * self.discr_aux_recon_loss_weight
 
             # backwards
 
-            (total_loss / grad_accum_every).backward()
+            self.accelerator.backward(total_loss / grad_accum_every)
 
         self.D_opt.step()
 
         return TrainDiscrLosses(total_divergence, total_multiscale_divergence, total_gp_loss, total_aux_loss)
 
     def train_generator_step(
         self,
@@ -1981,15 +2052,15 @@
                 for multiscale_logit in multiscale_logits:
                     multiscale_divergence = multiscale_divergence + generator_hinge_loss(multiscale_logit)
 
                 total_multiscale_divergence += (multiscale_divergence.item() / grad_accum_every)
 
                 total_loss = total_loss + multiscale_divergence * self.multiscale_divergence_loss_weight
 
-            (total_loss / grad_accum_every).backward()
+            self.accelerator.backward(total_loss / grad_accum_every)
 
         self.G_opt.step()
 
         # update exponentially moving averaged generator
 
         if self.has_ema_generator:
             self.G_ema.update()
@@ -2016,15 +2087,16 @@
         batch_size,
         dl_iter = None
     ):
         milestone = self.steps.item() // self.save_and_sample_every
         nrow_mult = 2 if self.train_upsampler else 1
         batches = num_to_groups(self.num_samples, batch_size)
 
-        dl_iter = default(self.val_dl_iter, dl_iter)
+        if self.train_upsampler:
+            dl_iter = default(self.sample_upsampler_dl_iter, dl_iter)
 
         assert exists(dl_iter)
 
         sample_models_and_output_file_name = [(self.G, f'sample-{milestone}.png')]
 
         if self.has_ema_generator:
             sample_models_and_output_file_name.append((self.G_ema, f'ema-sample-{milestone}.png'))
@@ -2047,38 +2119,41 @@
         self.save(str(self.model_folder / f'model-{milestone}.ckpt'))
         
     @beartype
     def forward(
         self,
         *,
         steps,
-        dataloader: DataLoader,
         grad_accum_every = 1
     ):
-        batch_size = dataloader.batch_size
-        dl_iter = cycle(dataloader)
+        assert exists(self.train_dl), 'you need to set the dataloader by running .set_dataloader(dl: Dataloader)'
+
+        batch_size = self.train_dl_batch_size
+        dl_iter = cycle(self.train_dl)
 
         last_gp_loss = 0.
         last_multiscale_d_loss = 0.
         last_multiscale_g_loss = 0.
 
         for _ in tqdm(range(steps), initial = self.steps.item()):
             steps = self.steps.item()
             is_first_step = steps == 1
 
             apply_gradient_penalty = self.apply_gradient_penalty_every > 0 and divisible_by(steps, self.apply_gradient_penalty_every)
             calc_multiscale_loss =  self.calc_multiscale_loss_every > 0 and divisible_by(steps, self.calc_multiscale_loss_every)
 
             d_loss, multiscale_d_loss, gp_loss, recon_loss = self.train_discriminator_step(
-                dl_iter,
+                dl_iter = dl_iter,
                 grad_accum_every = grad_accum_every,
                 apply_gradient_penalty = apply_gradient_penalty,
                 calc_multiscale_loss = calc_multiscale_loss
             )
 
+            self.accelerator.wait_for_everyone()
+
             g_loss, multiscale_g_loss = self.train_generator_step(
                 dl_iter = dl_iter,
                 batch_size = batch_size,
                 grad_accum_every = grad_accum_every,
                 calc_multiscale_loss = calc_multiscale_loss
             )
 
@@ -2090,13 +2165,15 @@
 
             if exists(multiscale_g_loss):
                 last_multiscale_g_loss = multiscale_g_loss
 
             if is_first_step or divisible_by(steps, self.log_steps_every):
                 self.print(f' G: {g_loss:.2f} | MSG: {last_multiscale_g_loss:.2f} | D: {d_loss:.2f} | MSD: {last_multiscale_d_loss:.2f} | GP: {last_gp_loss:.2f} | SSL: {recon_loss:.2f}')
 
-            if is_first_step or divisible_by(steps, self.save_and_sample_every) or (steps <= self.early_save_thres_steps and divisible_by(steps, self.early_save_and_sample_every)):
+            self.accelerator.wait_for_everyone()
+
+            if self.is_main and (is_first_step or divisible_by(steps, self.save_and_sample_every) or (steps <= self.early_save_thres_steps and divisible_by(steps, self.early_save_and_sample_every))):
                 self.save_sample(batch_size, dl_iter)
             
             self.steps += 1
 
         self.print(f'complete {steps} training steps')
```

### Comparing `gigagan-pytorch-0.0.92/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.1.0/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.0.92/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.1.0/gigagan_pytorch/optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def get_optimizer(
     params,
     lr = 1e-4,
     wd = 1e-2,
     betas = (0.9, 0.99),
     eps = 1e-8,
-    filter_by_requires_grad = False,
+    filter_by_requires_grad = True,
     group_wd_params = True,
     **kwargs
 ):
     if filter_by_requires_grad:
         params = list(filter(lambda t: t.requires_grad, params))
 
     if group_wd_params and wd > 0:
```

### Comparing `gigagan-pytorch-0.0.92/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.1.0/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.0.92/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.1.0/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.0.92
+Version: 0.1.0
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.0.92/setup.py` & `gigagan-pytorch-0.1.0/setup.py`

 * *Files identical despite different names*

