# Comparing `tmp/fastervit-0.9.2.tar.gz` & `tmp/fastervit-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-rbstb00d/fastervit-0.9.2.tar", last modified: Fri Jul  7 22:30:07 2023, max compression
+gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-g4tgee92/fastervit-0.9.3.tar", last modified: Thu Jul 20 14:32:02 2023, max compression
```

## Comparing `fastervit-0.9.2.tar` & `fastervit-0.9.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/
--rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-07-07 22:05:20.000000 fastervit-0.9.2/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-07-07 22:05:20.000000 fastervit-0.9.2/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)    10232 2023-07-07 22:30:07.000000 fastervit-0.9.2/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     9282 2023-07-07 22:29:03.000000 fastervit-0.9.2/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/
--rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/__init__.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/assets/
--rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/assets/hierarchial_attn.png
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/models/
--rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/models/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49072 2023-07-07 22:14:53.000000 fastervit-0.9.2/fastervit/models/faster_vit.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    50830 2023-07-07 22:20:22.000000 fastervit-0.9.2/fastervit/models/faster_vit_any_res.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/models/registry.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/scheduler/
--rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/cosine_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/multistep_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/plateau_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/poly_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/scheduler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/scheduler_factory.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/step_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/tanh_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/tensorboard.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49422 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/train.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/utils/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/utils/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/utils/datasets.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16159 2023-07-07 22:17:54.000000 fastervit-0.9.2/fastervit/validate.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)    10232 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      824 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-07-07 22:30:07.000000 fastervit-0.9.2/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-07-07 22:29:54.000000 fastervit-0.9.2/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-07-07 22:05:20.000000 fastervit-0.9.3/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-07-07 22:05:20.000000 fastervit-0.9.3/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)     8238 2023-07-20 14:32:02.000000 fastervit-0.9.3/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7287 2023-07-20 14:31:18.000000 fastervit-0.9.3/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/__init__.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/assets/
+-rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/assets/hierarchial_attn.png
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/models/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/models/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49072 2023-07-07 22:14:53.000000 fastervit-0.9.3/fastervit/models/faster_vit.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    50830 2023-07-07 22:20:22.000000 fastervit-0.9.3/fastervit/models/faster_vit_any_res.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/models/registry.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/scheduler/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/cosine_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/multistep_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/plateau_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/poly_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/scheduler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/scheduler_factory.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/step_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/tanh_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/tensorboard.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49422 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/train.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/utils/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/utils/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/utils/datasets.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16159 2023-07-07 22:17:54.000000 fastervit-0.9.3/fastervit/validate.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     8238 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      824 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-07-20 14:32:02.000000 fastervit-0.9.3/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-07-20 14:30:03.000000 fastervit-0.9.3/setup.py
```

### Comparing `fastervit-0.9.2/LICENSE` & `fastervit-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/README.md` & `fastervit-0.9.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-# FasterViT: Fast Vision Transformers with Hierarchical Attention
+Metadata-Version: 2.1
+Name: fastervit
+Version: 0.9.3
+Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
+Home-page: https://github.com/NVlabs/FasterViT
+Author: Ali Hatamizadeh
+Author-email: ahatamiz123@gmail.com
+License: NVIDIA Source Code License-NC
+Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-Official PyTorch implementation of [**FasterViT: Fast Vision Transformers with Hierarchical Attention**](https://arxiv.org/abs/2306.06189).
+[**FasterViT: Fast Vision Transformers with Hierarchical Attention**](https://arxiv.org/abs/2306.06189).
 
-[Ali Hatamizadeh](https://research.nvidia.com/person/ali-hatamizadeh),
-[Greg Heinrich](https://developer.nvidia.com/blog/author/gheinrich/),
-[Hongxu (Danny) Yin](https://scholar.princeton.edu/hongxu),
-[Andrew Tao](https://developer.nvidia.com/blog/author/atao/),
-[Jose M. Alvarez](https://alvarezlopezjosem.github.io/),
-[Jan Kautz](https://jankautz.com/), 
-[Pavlo Molchanov](https://www.pmolchanov.com/).
-
-For business inquiries, please visit our website and submit the form: [NVIDIA Research Licensing](https://www.nvidia.com/en-us/research/inquiries/)
-
-
---- 
 
 FasterViT achieves a new SOTA Pareto-front in
 terms of accuracy vs. image throughput without extra training data !
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
+Note: Please use the [**latest NVIDIA TensorRT release**](https://docs.nvidia.com/deeplearning/tensorrt/container-release-notes/index.html) to enjoy the benefits of optimized FasterViT ops. 
+
 
 ## Quick Start
 
 We can import pre-trained FasterViT models with **1 line of code**. First, FasterViT can be simply installed by:
 
 ```bash
 pip install fastervit
@@ -263,57 +273,14 @@
     <td>76.1</td>
     <td>93.0</td>
 </tr>
 
 </table>
 
 A, R and V2 denote ImageNet-A, ImageNet-R and ImageNet-V2 respectively. 
-## Training
-
-Please see [TRAINING.md](TRAINING.md) for detailed training instructions of all models. 
-
-## Evaluation
-
-The FasterViT models can be evaluated on ImageNet-1K validation set using the following: 
-
-```
-python validate.py \
---model <model-name>
---checkpoint <checkpoint-path>
---data_dir <imagenet-path>
---batch-size <batch-size-per-gpu
-``` 
-
-Here `--model` is the FasterViT variant (e.g. `faster_vit_0_224_1k`), `--checkpoint` is the path to pretrained model weights, `--data_dir` is the path to ImageNet-1K validation set and `--batch-size` is the number of batch size. We also provide a sample script [here](./fastervit/validate.sh). 
-
-## ONNX Conversion
-
-We provide ONNX conversion script to enable dynamic batch size inference. For instance, to generate ONNX model for `faster_vit_0_any_res` with resolution 576 x 960 and ONNX opset number 17, the following can be used. 
-
-```bash 
-python onnx_convert --model-name faster_vit_0_any_res --resolution-h 576 --resolution-w 960 --onnx-opset 17
-
-```
-
-
-## Installation
-
-The dependencies can be installed by running:
-
-```bash
-pip install -r requirements.txt
-```
-
-## Star History
-
-[![Star History Chart](https://api.star-history.com/svg?repos=NVlabs/FasterViT&type=Date)](https://star-history.com/#NVlabs/FasterViT&Date)
-
-
-## Third-party Extentions
-We always welcome third-party extentions/implementations and usage for other purposes. If you would like your work to be listed in this repository, please raise and issue and provide us with detailed information.  
 
 ## Citation
 
 Please consider citing FasterViT if this repository is useful for your work. 
 
 ```
 @article{hatamizadeh2023fastervit,
@@ -332,9 +299,8 @@
 This work is made available under the NVIDIA Source Code License-NC. Click [here](LICENSE) to view a copy of this license.
 
 For license information regarding the timm repository, please refer to its [repository](https://github.com/rwightman/pytorch-image-models).
 
 For license information regarding the ImageNet dataset, please see the [ImageNet official website](https://www.image-net.org/). 
 
 ## Acknowledgement
-This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.  
-
+This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.
```

#### html2text {}

```diff
@@ -1,46 +1,52 @@
-# FasterViT: Fast Vision Transformers with Hierarchical Attention Official
-PyTorch implementation of [**FasterViT: Fast Vision Transformers with
-Hierarchical Attention**](https://arxiv.org/abs/2306.06189). [Ali Hatamizadeh]
-(https://research.nvidia.com/person/ali-hatamizadeh), [Greg Heinrich](https://
-developer.nvidia.com/blog/author/gheinrich/), [Hongxu (Danny) Yin](https://
-scholar.princeton.edu/hongxu), [Andrew Tao](https://developer.nvidia.com/blog/
-author/atao/), [Jose M. Alvarez](https://alvarezlopezjosem.github.io/), [Jan
-Kautz](https://jankautz.com/), [Pavlo Molchanov](https://www.pmolchanov.com/).
-For business inquiries, please visit our website and submit the form: [NVIDIA
-Research Licensing](https://www.nvidia.com/en-us/research/inquiries/) --
-- FasterViT achieves a new SOTA Pareto-front in terms of accuracy vs. image
-throughput without extra training data !
+Metadata-Version: 2.1 Name: fastervit Version: 0.9.3 Summary: FasterViT: Fast
+Vision Transformers with Hierarchical Attention Home-page: https://github.com/
+NVlabs/FasterViT Author: Ali Hatamizadeh Author-email: ahatamiz123@gmail.com
+License: NVIDIA Source Code License-NC Keywords: pytorch pretrained models
+efficientnet mobilenetv3 mnasnet resnet vision transformer vit Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Python: >=3.7 Description-Content-Type:
+text/markdown License-File: LICENSE [**FasterViT: Fast Vision Transformers with
+Hierarchical Attention**](https://arxiv.org/abs/2306.06189). FasterViT achieves
+a new SOTA Pareto-front in terms of accuracy vs. image throughput without extra
+training data !
  [https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-
                                  6cdd16bfccc1]
-## Quick Start We can import pre-trained FasterViT models with **1 line of
-code**. First, FasterViT can be simply installed by: ```bash pip install
-fastervit ``` A pretrained FasterViT model with default hyper-parameters can be
-created as in the following: ```python >>> from fastervit import create_model #
-Define fastervit-0 model with 224 x 224 resolution >>> model = create_model
-('faster_vit_0_224', pretrained=True, model_path="/tmp/faster_vit_0.pth.tar")
-``` `model_path` is used to set the directory to download the model. We can
-also simply test the model by passing a dummy input image. The output is the
-logits: ```python >>> import torch >>> image = torch.rand(1, 3, 224, 224) >>>
-output = model(image) # torch.Size([1, 1000]) ``` We can also use the any-
-resolution FasterViT model to accommodate arbitrary image resolutions. In the
-following, we define an any-resolution FasterViT-0 model with input resolution
-of 576 x 960, window sizes of 12 and 6 in 3rd and 4th stages, carrier token
-size of 2 and embedding dimension of 64: ```python >>> from fastervit import
-create_model # Define any-resolution FasterViT-0 model with 576 x 960
-resolution >>> model = create_model('faster_vit_0_any_res', resolution=[576,
-960], window_size=[7, 7, 12, 6], ct_size=2, dim=64, pretrained=True) ``` Note
-that the above model is intiliazed from the original ImageNet pre-trained
-FasterViT with original resolution of 224 x 224. As a result, missing keys and
-mis-matches could be expected since we are addign new layers (e.g. addition of
-new carrier tokens, etc.) We can simply test the model by passing a dummy input
-image. The output is the logits: ```python >>> import torch >>> image =
-torch.rand(1, 3, 576, 960) >>> output = model(image) # torch.Size([1, 1000])
-``` --- ## Results + Pretrained Models ### ImageNet-1K **FasterViT ImageNet-1K
-Pretrained Models**
+Note: Please use the [**latest NVIDIA TensorRT release**](https://
+docs.nvidia.com/deeplearning/tensorrt/container-release-notes/index.html) to
+enjoy the benefits of optimized FasterViT ops. ## Quick Start We can import
+pre-trained FasterViT models with **1 line of code**. First, FasterViT can be
+simply installed by: ```bash pip install fastervit ``` A pretrained FasterViT
+model with default hyper-parameters can be created as in the following:
+```python >>> from fastervit import create_model # Define fastervit-0 model
+with 224 x 224 resolution >>> model = create_model('faster_vit_0_224',
+pretrained=True, model_path="/tmp/faster_vit_0.pth.tar") ``` `model_path` is
+used to set the directory to download the model. We can also simply test the
+model by passing a dummy input image. The output is the logits: ```python >>>
+import torch >>> image = torch.rand(1, 3, 224, 224) >>> output = model(image) #
+torch.Size([1, 1000]) ``` We can also use the any-resolution FasterViT model to
+accommodate arbitrary image resolutions. In the following, we define an any-
+resolution FasterViT-0 model with input resolution of 576 x 960, window sizes
+of 12 and 6 in 3rd and 4th stages, carrier token size of 2 and embedding
+dimension of 64: ```python >>> from fastervit import create_model # Define any-
+resolution FasterViT-0 model with 576 x 960 resolution >>> model = create_model
+('faster_vit_0_any_res', resolution=[576, 960], window_size=[7, 7, 12, 6],
+ct_size=2, dim=64, pretrained=True) ``` Note that the above model is intiliazed
+from the original ImageNet pre-trained FasterViT with original resolution of
+224 x 224. As a result, missing keys and mis-matches could be expected since we
+are addign new layers (e.g. addition of new carrier tokens, etc.) We can simply
+test the model by passing a dummy input image. The output is the logits:
+```python >>> import torch >>> image = torch.rand(1, 3, 576, 960) >>> output =
+model(image) # torch.Size([1, 1000]) ``` --- ## Results + Pretrained Models ###
+ImageNet-1K **FasterViT ImageNet-1K Pretrained Models**
 Name       Acc@1(%) Acc@5(%) Throughput Resolution #Params(M) FLOPs(G) Download
                              (Img/Sec)
 FasterViT- 82.1     95.9     5802       224x224    31.4       3.3      model
 0
 FasterViT- 83.2     96.5     4188       224x224    53.4       5.3      model
 1
 FasterViT- 84.2     96.8     3161       224x224    75.9       8.7      model
@@ -61,41 +67,22 @@
 FasterViT-1 31.2       63.3       47.5       61.9       72.6        91.0
 FasterViT-2 38.2       68.9       49.6       63.4       73.7        91.6
 FasterViT-3 44.2       73.0       51.9       65.6       75.0        92.2
 FasterViT-4 49.0       75.4       56.0       69.6       75.7        92.7
 FasterViT-5 52.7       77.6       56.9       70.0       76.0        93.0
 FasterViT-6 53.7       78.4       57.1       70.1       76.1        93.0
 A, R and V2 denote ImageNet-A, ImageNet-R and ImageNet-V2 respectively. ##
-Training Please see [TRAINING.md](TRAINING.md) for detailed training
-instructions of all models. ## Evaluation The FasterViT models can be evaluated
-on ImageNet-1K validation set using the following: ``` python validate.py \ --
-model  --checkpoint  --data_dir  --batch-size
-`` Here `--model` is the FasterViT variant (e.g. `faster_vit_0_224_1k`), `--
-checkpoint` is the path to pretrained model weights, `--data_dir` is the path
-to ImageNet-1K validation set and `--batch-size` is the number of batch size.
-We also provide a sample script [here](./fastervit/validate.sh). ## ONNX
-Conversion We provide ONNX conversion script to enable dynamic batch size
-inference. For instance, to generate ONNX model for `faster_vit_0_any_res` with
-resolution 576 x 960 and ONNX opset number 17, the following can be used.
-```bash python onnx_convert --model-name faster_vit_0_any_res --resolution-
-h 576 --resolution-w 960 --onnx-opset 17 ``` ## Installation The dependencies
-can be installed by running: ```bash pip install -r requirements.txt ``` ##
-Star History [![Star History Chart](https://api.star-history.com/
-svg?repos=NVlabs/FasterViT&type=Date)](https://star-history.com/#NVlabs/
-FasterViT&Date) ## Third-party Extentions We always welcome third-party
-extentions/implementations and usage for other purposes. If you would like your
-work to be listed in this repository, please raise and issue and provide us
-with detailed information. ## Citation Please consider citing FasterViT if this
-repository is useful for your work. ``` @article{hatamizadeh2023fastervit,
-title={FasterViT: Fast Vision Transformers with Hierarchical Attention},
-author={Hatamizadeh, Ali and Heinrich, Greg and Yin, Hongxu and Tao, Andrew and
-Alvarez, Jose M and Kautz, Jan and Molchanov, Pavlo}, journal={arXiv preprint
-arXiv:2306.06189}, year={2023} } ``` ## Licenses Copyright Â© 2023, NVIDIA
-Corporation. All rights reserved. This work is made available under the NVIDIA
-Source Code License-NC. Click [here](LICENSE) to view a copy of this license.
-For license information regarding the timm repository, please refer to its
-[repository](https://github.com/rwightman/pytorch-image-models). For license
-information regarding the ImageNet dataset, please see the [ImageNet official
-website](https://www.image-net.org/). ## Acknowledgement This repository is
-built on top of the [timm](https://github.com/huggingface/pytorch-image-models)
-repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and
-maintaining this high-quality library.
+Citation Please consider citing FasterViT if this repository is useful for your
+work. ``` @article{hatamizadeh2023fastervit, title={FasterViT: Fast Vision
+Transformers with Hierarchical Attention}, author={Hatamizadeh, Ali and
+Heinrich, Greg and Yin, Hongxu and Tao, Andrew and Alvarez, Jose M and Kautz,
+Jan and Molchanov, Pavlo}, journal={arXiv preprint arXiv:2306.06189}, year=
+{2023} } ``` ## Licenses Copyright Â© 2023, NVIDIA Corporation. All rights
+reserved. This work is made available under the NVIDIA Source Code License-NC.
+Click [here](LICENSE) to view a copy of this license. For license information
+regarding the timm repository, please refer to its [repository](https://
+github.com/rwightman/pytorch-image-models). For license information regarding
+the ImageNet dataset, please see the [ImageNet official website](https://
+www.image-net.org/). ## Acknowledgement This repository is built on top of the
+[timm](https://github.com/huggingface/pytorch-image-models) repository. We
+thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining
+this high-quality library.
```

### Comparing `fastervit-0.9.2/fastervit/assets/hierarchial_attn.png` & `fastervit-0.9.3/fastervit/assets/hierarchial_attn.png`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/models/faster_vit.py` & `fastervit-0.9.3/fastervit/models/faster_vit.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/models/faster_vit_any_res.py` & `fastervit-0.9.3/fastervit/models/faster_vit_any_res.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/models/registry.py` & `fastervit-0.9.3/fastervit/models/registry.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/scheduler/cosine_lr.py` & `fastervit-0.9.3/fastervit/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/scheduler/multistep_lr.py` & `fastervit-0.9.3/fastervit/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/scheduler/plateau_lr.py` & `fastervit-0.9.3/fastervit/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/scheduler/poly_lr.py` & `fastervit-0.9.3/fastervit/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/scheduler/scheduler.py` & `fastervit-0.9.3/fastervit/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/scheduler/scheduler_factory.py` & `fastervit-0.9.3/fastervit/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/scheduler/step_lr.py` & `fastervit-0.9.3/fastervit/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/scheduler/tanh_lr.py` & `fastervit-0.9.3/fastervit/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/tensorboard.py` & `fastervit-0.9.3/fastervit/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/train.py` & `fastervit-0.9.3/fastervit/train.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/utils/datasets.py` & `fastervit-0.9.3/fastervit/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit/validate.py` & `fastervit-0.9.3/fastervit/validate.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/fastervit.egg-info/SOURCES.txt` & `fastervit-0.9.3/fastervit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.2/setup.py` & `fastervit-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='fastervit',
-    version='0.9.2',
+    version='0.9.3',
     description='FasterViT: Fast Vision Transformers with Hierarchical Attention',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NVlabs/FasterViT',
     author='Ali Hatamizadeh',
     author_email='ahatamiz123@gmail.com',
     classifiers=[
```

