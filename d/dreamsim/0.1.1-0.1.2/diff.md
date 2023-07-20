# Comparing `tmp/dreamsim-0.1.1.tar.gz` & `tmp/dreamsim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamsim-0.1.1.tar", last modified: Fri Jun 16 01:07:53 2023, max compression
+gzip compressed data, was "dreamsim-0.1.2.tar", last modified: Thu Jul 20 17:21:35 2023, max compression
```

## Comparing `dreamsim-0.1.1.tar` & `dreamsim-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:07:53.784095 dreamsim-0.1.1/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1118 2023-06-15 23:35:43.000000 dreamsim-0.1.1/LICENSE
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7472 2023-06-16 01:07:53.779476 dreamsim-0.1.1/PKG-INFO
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     8642 2023-06-16 01:01:52.000000 dreamsim-0.1.1/README.md
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:07:53.608144 dreamsim-0.1.1/dreamsim/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       45 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/__init__.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      563 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/config.py
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:07:53.766266 dreamsim-0.1.1/dreamsim/feature_extraction/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/__init__.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11551 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/extractor.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1006 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/load_clip_as_dino.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     3448 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/load_mae_as_vit.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     2726 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/load_open_clip_as_dino.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11874 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/vision_transformer.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      444 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/vit_wrapper.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11462 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/model.py
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:07:53.675546 dreamsim-0.1.1/dreamsim.egg-info/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7472 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/PKG-INFO
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      567 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/SOURCES.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        1 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/dependency_links.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       83 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/requires.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       37 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/top_level.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       38 2023-06-16 01:07:53.786290 dreamsim-0.1.1/setup.cfg
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      980 2023-06-16 01:07:04.000000 dreamsim-0.1.1/setup.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-20 17:21:35.482042 dreamsim-0.1.2/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1118 2023-06-15 23:35:43.000000 dreamsim-0.1.2/LICENSE
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7270 2023-07-20 17:21:35.477307 dreamsim-0.1.2/PKG-INFO
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     8434 2023-07-20 16:55:30.000000 dreamsim-0.1.2/README.md
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-20 17:21:35.236991 dreamsim-0.1.2/dreamsim/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       45 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/__init__.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1599 2023-07-14 19:18:53.000000 dreamsim-0.1.2/dreamsim/config.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-20 17:21:35.463767 dreamsim-0.1.2/dreamsim/feature_extraction/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/__init__.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11551 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/extractor.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1006 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/load_clip_as_dino.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     3448 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/load_mae_as_vit.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     2726 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/load_open_clip_as_dino.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11874 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/vision_transformer.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      444 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/vit_wrapper.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    12310 2023-07-14 17:31:28.000000 dreamsim-0.1.2/dreamsim/model.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-20 17:21:35.305580 dreamsim-0.1.2/dreamsim.egg-info/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7270 2023-07-20 17:21:34.000000 dreamsim-0.1.2/dreamsim.egg-info/PKG-INFO
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      567 2023-07-20 17:21:35.000000 dreamsim-0.1.2/dreamsim.egg-info/SOURCES.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        1 2023-07-20 17:21:34.000000 dreamsim-0.1.2/dreamsim.egg-info/dependency_links.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       83 2023-07-20 17:21:34.000000 dreamsim-0.1.2/dreamsim.egg-info/requires.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       37 2023-07-20 17:21:34.000000 dreamsim-0.1.2/dreamsim.egg-info/top_level.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       38 2023-07-20 17:21:35.484291 dreamsim-0.1.2/setup.cfg
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      976 2023-07-20 17:17:21.000000 dreamsim-0.1.2/setup.py
```

### Comparing `dreamsim-0.1.1/LICENSE` & `dreamsim-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.1/PKG-INFO` & `dreamsim-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dreamsim
-Version: 0.1.1
+Version: 0.1.2
 Summary: DreamSim similarity metric
-Home-page: https://github.com/ssundaram21/dreamsim-dev
+Home-page: https://github.com/ssundaram21/dreamsim
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- # ![icon](images/figs/icon.png)  DreamSim Perceptual Metric -->
@@ -18,17 +18,17 @@
 [Stephanie Fu](https://stephanie-fu.github.io)\* $^{1}$, [Netanel Tamir](https://netanel-tamir.github.io)\* $^{2}$, [Shobhita Sundaram](https://ssundaram21.github.io)\* $^{1}$, [Lucy Chai](https://people.csail.mit.edu/lrchai/) $^1$, [Richard Zhang](http://richzhang.github.io) $^3$, [Tali Dekel](https://www.weizmann.ac.il/math/dekel/) $^2$, [Phillip Isola](https://web.mit.edu/phillipi/) $^1$. (*equal contribution)<br>
 $^1$ MIT, $^2$ Weizmann Institute of Science, $^3$ Adobe Research.
 
 
 
 **Summary**
 
-Current metrics for perceptual image similarity operate at the level of pixels and patches. These metrics compare images in terms of their low-level colors and textures, but fail to capture mid-level similarities/differences in image layout, object poses, and semantic content. Meanwhile, measures that use image-level embeddings such as DINO and CLIP capture high-level and semantic judgements, but may not be aligned with human perception of more finegrained attributes.
+Current metrics for perceptual image similarity operate at the level of pixels and patches. These metrics compare images in terms of their low-level colors and textures, but fail to capture mid-level differences in layout, pose, semantic content, etc. Models that use image-level embeddings such as DINO and CLIP capture high-level and semantic judgements, but may not be aligned with human perception of more finegrained attributes.
 
-DreamSim is a new metric for perceptual image similarity that bridges the gap between "low-level" metrics (e.g. LPIPS, PSNR, SSIM) and "high-level" measures (e.g. CLIP). Our model was trained by concatenating CLIP, OpenCLIP, and DINO embeddings, and then finetuning on human perceptual judgements. We gathered these judgements on a dataset of ~20k image triplets, generated by diffusion models. Our model achieves better alignment with human similarity judgements than existing metrics, and can be used for a variety of downstream applications.
+DreamSim is a new metric for perceptual image similarity that bridges the gap between "low-level" metrics (e.g. LPIPS, PSNR, SSIM) and "high-level" measures (e.g. CLIP). Our model was trained by concatenating CLIP, OpenCLIP, and DINO embeddings, and then finetuning on human perceptual judgements. We gathered these judgements on a dataset of ~20k image triplets, generated by diffusion models. Our model achieves better alignment with human similarity judgements than existing metrics, and can be used for downstream applications such as image retrieval.
 
 ## Requirements
 - Linux
 - Python 3
 - NVIDIA GPU + CUDA CuDNN (DreamSim is only supported on CUDA devices)
 
 ## Setup
@@ -37,24 +37,20 @@
 
 ```pip install dreamsim```
 
 The package is used for importing and using the DreamSim model.
 
 **Option 2:** Clone our repo and install dependencies.
 This is necessary for running our training/evaluation scripts.
-<!--  ```
-git clone https://github.com/ssundaram21/DreamSim.git
-conda env create -f environment.yml
-export PYTHONPATH="$PYTHONPATH:$(realpath ./DreamSim)"
-``` -->
+
 ```
 python3 -m venv ds
 source ds/bin/activate
 pip install -r requirements.txt
-export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsimv)"
+export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsim)"
 ```
 To install with conda:
 ```
 conda create -n ds
 conda activate ds
 conda install pip # verify with the `which pip` command
 pip install -r requirements.txt
@@ -63,28 +59,36 @@
 
 ## Usage
 **For walk-through examples of the below use-cases, check out our [Colab demo](https://colab.research.google.com/drive/1taEOMzFE9g81D9AwH27Uhy2U82tQGAVI?usp=sharing).**
 
 ### Quickstart: Perceptual similarity metric
 The basic use case is to measure the perceptual distance between two images. **A higher score means more different, lower means more similar**. 
 
-The following code snippet is all you need. The first time that you run `dreamsim` it will automatically download the model weights. The default model settings are specified in `dreamsim/dreamsim_inference_v0.yaml`.
+The following code snippet is all you need. The first time that you run `dreamsim` it will automatically download the model weights. The default model settings are specified in `./dreamsim/config.py`.
 ```
 from dreamsim import dreamsim
 from PIL import Image
 
 model, preprocess = dreamsim(pretrained=True)
 
 img1 = preprocess(Image.open("img1_path")).to("cuda")
 img2 = preprocess(Image.open("img2_path")).to("cuda")
-distance = model(img1, img2) # The model takes an RGB image from [0, 1], size 1x3x224x224
+distance = model(img1, img2) # The model takes an RGB image from [0, 1], size batch_sizex3x224x224
 ```
 
 To run on example images, run `demo.py`. The script should produce distances (0.424, 0.34). 
 
+### (new!) Single-branch models
+By default, DreamSim uses an ensemble of CLIP, DINO, and OpenCLIP (all ViT-B/16). If you need a lighter-weight model you can use *single-branch* versions of DreamSim where only a single backbone is finetuned. The available options are OpenCLIP-ViTB/32, DINO-ViTB/16, CLIP-ViTB/32, in order of performance. 
+
+To load a single-branch model, use the `dreamsim_type` argument. For example:
+```
+dreamsim_dino_model, preprocess = dreamsim(pretrained=True, dreamsim_type="dino_vitb16")
+```
+
 ### Feature extraction
 To extract a *single image embedding* using dreamsim, use the `embed` method as shown in the following snippet:
 ```
 img1 = preprocess(Image.open("img1_path")).to("cuda")
 embedding = model.embed(img1)
 ```
 The perceptual distance between two images is the cosine distance between their embeddings. If the embeddings are normalized (true by default) L2 distance can also be used.
@@ -123,28 +127,24 @@
     dist = model(predicted_image, reference_image)
     dist.backward()
     optimizer.step()
 ```
 
 
 <a name="bibtex"></a>
-# Citation
+## Citation
 
 If you find our work or any of our materials useful, please cite our paper:
 ```
 @misc{fu2023dreamsim,
       title={DreamSim: Learning New Dimensions of Human Visual Similarity using Synthetic Data}, 
       author={Stephanie Fu and Netanel Tamir and Shobhita Sundaram and Lucy Chai and Richard Zhang and Tali Dekel and Phillip Isola},
       year={2023},
       eprint={2306.09344},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
 ```
 
 ## Acknowledgements
-We thank Jim DiCarlo, Liad Mudrik, Nitzan Censor for fruitful discussions throughout the project. Additionally, we thank Narek Tumanyan for his insightful comments over the course of the project. Finally, we thank Michelle Li for proofreading sections of this paper and offering helpful comments. 
-
-This work was supported by the NSF GRFP Fellowship to Shobhita Sundaram, the Meta PhD Fellowship to Lucy Chai, the Israeli Science Foundation (grant 2303/20) to Tali Dekel, and the Packard Fellowship to Phillip Isola.
-
 Our code borrows from the ["Deep ViT Features as Dense Visual Descriptors"](https://dino-vit-features.github.io/) repository for ViT feature extraction, and takes inspiration from the [UniverSeg](https://github.com/JJGO/UniverSeg) respository for code structure.
```

### Comparing `dreamsim-0.1.1/README.md` & `dreamsim-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 [Stephanie Fu](https://stephanie-fu.github.io)\* $^{1}$, [Netanel Tamir](https://netanel-tamir.github.io)\* $^{2}$, [Shobhita Sundaram](https://ssundaram21.github.io)\* $^{1}$, [Lucy Chai](https://people.csail.mit.edu/lrchai/) $^1$, [Richard Zhang](http://richzhang.github.io) $^3$, [Tali Dekel](https://www.weizmann.ac.il/math/dekel/) $^2$, [Phillip Isola](https://web.mit.edu/phillipi/) $^1$. (*equal contribution)<br>
 $^1$ MIT, $^2$ Weizmann Institute of Science, $^3$ Adobe Research.
 
 ![teaser](images/figs/teaser.png)
 
 **Summary**
 
-Current metrics for perceptual image similarity operate at the level of pixels and patches. These metrics compare images in terms of their low-level colors and textures, but fail to capture mid-level similarities/differences in image layout, object poses, and semantic content. Meanwhile, measures that use image-level embeddings such as DINO and CLIP capture high-level and semantic judgements, but may not be aligned with human perception of more finegrained attributes.
+Current metrics for perceptual image similarity operate at the level of pixels and patches. These metrics compare images in terms of their low-level colors and textures, but fail to capture mid-level differences in layout, pose, semantic content, etc. Models that use image-level embeddings such as DINO and CLIP capture high-level and semantic judgements, but may not be aligned with human perception of more finegrained attributes.
 
-DreamSim is a new metric for perceptual image similarity that bridges the gap between "low-level" metrics (e.g. LPIPS, PSNR, SSIM) and "high-level" measures (e.g. CLIP). Our model was trained by concatenating CLIP, OpenCLIP, and DINO embeddings, and then finetuning on human perceptual judgements. We gathered these judgements on a dataset of ~20k image triplets, generated by diffusion models. Our model achieves better alignment with human similarity judgements than existing metrics, and can be used for a variety of downstream applications.
+DreamSim is a new metric for perceptual image similarity that bridges the gap between "low-level" metrics (e.g. LPIPS, PSNR, SSIM) and "high-level" measures (e.g. CLIP). Our model was trained by concatenating CLIP, OpenCLIP, and DINO embeddings, and then finetuning on human perceptual judgements. We gathered these judgements on a dataset of ~20k image triplets, generated by diffusion models. Our model achieves better alignment with human similarity judgements than existing metrics, and can be used for downstream applications such as image retrieval.
 
 ## Requirements
 - Linux
 - Python 3
 - NVIDIA GPU + CUDA CuDNN (DreamSim is only supported on CUDA devices)
 
 ## Setup
@@ -26,24 +26,20 @@
 
 ```pip install dreamsim```
 
 The package is used for importing and using the DreamSim model.
 
 **Option 2:** Clone our repo and install dependencies.
 This is necessary for running our training/evaluation scripts.
-<!--  ```
-git clone https://github.com/ssundaram21/DreamSim.git
-conda env create -f environment.yml
-export PYTHONPATH="$PYTHONPATH:$(realpath ./DreamSim)"
-``` -->
+
 ```
 python3 -m venv ds
 source ds/bin/activate
 pip install -r requirements.txt
-export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsimv)"
+export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsim)"
 ```
 To install with conda:
 ```
 conda create -n ds
 conda activate ds
 conda install pip # verify with the `which pip` command
 pip install -r requirements.txt
@@ -52,28 +48,36 @@
 
 ## Usage
 **For walk-through examples of the below use-cases, check out our [Colab demo](https://colab.research.google.com/drive/1taEOMzFE9g81D9AwH27Uhy2U82tQGAVI?usp=sharing).**
 
 ### Quickstart: Perceptual similarity metric
 The basic use case is to measure the perceptual distance between two images. **A higher score means more different, lower means more similar**. 
 
-The following code snippet is all you need. The first time that you run `dreamsim` it will automatically download the model weights. The default model settings are specified in `dreamsim/dreamsim_inference_v0.yaml`.
+The following code snippet is all you need. The first time that you run `dreamsim` it will automatically download the model weights. The default model settings are specified in `./dreamsim/config.py`.
 ```
 from dreamsim import dreamsim
 from PIL import Image
 
 model, preprocess = dreamsim(pretrained=True)
 
 img1 = preprocess(Image.open("img1_path")).to("cuda")
 img2 = preprocess(Image.open("img2_path")).to("cuda")
-distance = model(img1, img2) # The model takes an RGB image from [0, 1], size 1x3x224x224
+distance = model(img1, img2) # The model takes an RGB image from [0, 1], size batch_sizex3x224x224
 ```
 
 To run on example images, run `demo.py`. The script should produce distances (0.424, 0.34). 
 
+### (new!) Single-branch models
+By default, DreamSim uses an ensemble of CLIP, DINO, and OpenCLIP (all ViT-B/16). If you need a lighter-weight model you can use *single-branch* versions of DreamSim where only a single backbone is finetuned. The available options are OpenCLIP-ViTB/32, DINO-ViTB/16, CLIP-ViTB/32, in order of performance. 
+
+To load a single-branch model, use the `dreamsim_type` argument. For example:
+```
+dreamsim_dino_model, preprocess = dreamsim(pretrained=True, dreamsim_type="dino_vitb16")
+```
+
 ### Feature extraction
 To extract a *single image embedding* using dreamsim, use the `embed` method as shown in the following snippet:
 ```
 img1 = preprocess(Image.open("img1_path")).to("cuda")
 embedding = model.embed(img1)
 ```
 The perceptual distance between two images is the cosine distance between their embeddings. If the embeddings are normalized (true by default) L2 distance can also be used.
@@ -111,22 +115,22 @@
 for i in range(n_iters):
     dist = model(predicted_image, reference_image)
     dist.backward()
     optimizer.step()
 ```
 <!--Experiments-->
 ## NIGHTS (Novel Image Generations with Human-Tested Similarities) Dataset
-DreamSim is trained by fine-tuning on the NIGHTS dataset. For details on the dataset structure and creation, refer to the [dataset page](https://github.com/ssundaram21/dreamsim-dev/tree/main/dataset).
+DreamSim is trained by fine-tuning on the NIGHTS dataset. For details on the dataset structure and creation, refer to the [dataset page](https://github.com/ssundaram21/dreamsim/tree/main/dataset).
 
 Run `./dataset/download_dataset.sh` to download and unzip the NIGHTS dataset into `./dataset/nights`. The unzipped dataset size is 58 GB. 
 
 ## Experiments
 
 ### Download resources
-Run `./training/download_models.sh` to download and unzip necessary ViT checkpoints (for DINO, CLIP, OpenCLIP, and MAE) into `./models`. 
+Run `./training/download_models.sh` to download and unzip necessary ViT checkpoints (for CLIP, OpenCLIP, and MAE) into `./models`. 
 
 ### Training
 To finetune a perceptual model on the dataset, run `./training/train.py`. For example, to finetune an ensemble of DINO, CLIP, and OpenCLIP using LoRA, run:
 
 ```
 python ./training/train.py --config ./configs/train_ensemble_model_lora.yaml
 ```
@@ -140,28 +144,24 @@
 python ./training/evaluate.py --config ./configs/eval_baseline.yaml
 ```
 
 For an example of evaluating using a trained checkpoint, refer to `./configs/eval_checkpoint.yaml`. See `./training/evaluate.py` for a full list and description of evaluation options.
 <!--Experiments-->
 
 <a name="bibtex"></a>
-# Citation
+## Citation
 
 If you find our work or any of our materials useful, please cite our paper:
 ```
 @misc{fu2023dreamsim,
       title={DreamSim: Learning New Dimensions of Human Visual Similarity using Synthetic Data}, 
       author={Stephanie Fu and Netanel Tamir and Shobhita Sundaram and Lucy Chai and Richard Zhang and Tali Dekel and Phillip Isola},
       year={2023},
       eprint={2306.09344},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
 ```
 
 ## Acknowledgements
-We thank Jim DiCarlo, Liad Mudrik, Nitzan Censor for fruitful discussions throughout the project. Additionally, we thank Narek Tumanyan for his insightful comments over the course of the project. Finally, we thank Michelle Li for proofreading sections of this paper and offering helpful comments. 
-
-This work was supported by the NSF GRFP Fellowship to Shobhita Sundaram, the Meta PhD Fellowship to Lucy Chai, the Israeli Science Foundation (grant 2303/20) to Tali Dekel, and the Packard Fellowship to Phillip Isola.
-
 Our code borrows from the ["Deep ViT Features as Dense Visual Descriptors"](https://dino-vit-features.github.io/) repository for ViT feature extraction, and takes inspiration from the [UniverSeg](https://github.com/JJGO/UniverSeg) respository for code structure.
```

### Comparing `dreamsim-0.1.1/dreamsim/config.py` & `dreamsim-0.1.2/dreamsim/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,43 @@
 dreamsim_args = {
         "model_config": {
-            "feat_type": 'cls,embedding,embedding',
-            "model_type": "dino_vitb16,clip_vitb16,open_clip_vitb16",
-            "stride": "16,16,16",
-            "lora": True
+            "ensemble": {
+                "feat_type": 'cls,embedding,embedding',
+                "model_type": "dino_vitb16,clip_vitb16,open_clip_vitb16",
+                "stride": "16,16,16",
+                "lora": True
+            },
+            "dino_vitb16": {
+                "feat_type": 'cls',
+                "model_type": "dino_vitb16",
+                "stride": "16",
+                "lora": True
+            },
+            "clip_vitb32": {
+                "feat_type": 'embedding',
+                "model_type": "clip_vitb32",
+                "stride": "32",
+                "lora": True
+            },
+            "open_clip_vitb32": {
+                "feat_type": 'embedding',
+                "model_type": "open_clip_vitb32",
+                "stride": "32",
+                "lora": True
+            }
         },
         "lora_config": {
             "r": 16,
             "lora_alpha": 0.5,
             "lora_dropout": 0.3,
             "bias": "none",
             "target_modules": ['qkv']
         },
         "img_size": 224
     }
 
-dreamsim_weights = "https://github.com/ssundaram21/dreamsim/releases/download/v0.1.0/dreamsim_checkpoint.zip"
+dreamsim_weights = {
+    "ensemble": "https://github.com/ssundaram21/dreamsim/releases/download/v0.1.0/dreamsim_checkpoint.zip",
+    "dino_vitb16": "https://github.com/ssundaram21/dreamsim/releases/download/v0.1.2/dreamsim_dino_vitb16_checkpoint.zip",
+    "clip_vitb32": "https://github.com/ssundaram21/dreamsim/releases/download/v0.1.2/dreamsim_clip_vitb32_checkpoint.zip",
+    "open_clip_vitb32": "https://github.com/ssundaram21/dreamsim/releases/download/v0.1.2/dreamsim_open_clip_vitb32_checkpoint.zip"
+}
```

### Comparing `dreamsim-0.1.1/dreamsim/feature_extraction/extractor.py` & `dreamsim-0.1.2/dreamsim/feature_extraction/extractor.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.1/dreamsim/feature_extraction/load_clip_as_dino.py` & `dreamsim-0.1.2/dreamsim/feature_extraction/load_clip_as_dino.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.1/dreamsim/feature_extraction/load_mae_as_vit.py` & `dreamsim-0.1.2/dreamsim/feature_extraction/load_mae_as_vit.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.1/dreamsim/feature_extraction/load_open_clip_as_dino.py` & `dreamsim-0.1.2/dreamsim/feature_extraction/load_open_clip_as_dino.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.1/dreamsim/feature_extraction/vision_transformer.py` & `dreamsim-0.1.2/dreamsim/feature_extraction/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.1/dreamsim/model.py` & `dreamsim-0.1.2/dreamsim/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -153,73 +153,79 @@
 
     def forward(self, img):
         x = self.fc1(img)
         x = F.relu(x)
         return self.fc2(x) + img
 
 
-def download_weights(cache_dir):
+def download_weights(cache_dir, dreamsim_type):
     """
     Downloads and unzips DreamSim weights.
     """
+
     dreamsim_required_ckpts = {
-        "dino_vitb16_pretrain.pth",
-        "open_clip_vitb16_pretrain.pth.tar",
-        "clip_vitb16_pretrain.pth.tar",
-        "dino_vitb16_lora",
-        "open_clip_vitb16_lora",
-        "clip_vitb16_lora"
+        "ensemble": ["dino_vitb16_pretrain.pth", "dino_vitb16_lora",
+                     "open_clip_vitb32_pretrain.pth.tar", "open_clip_vitb32_lora",
+                     "clip_vitb32_pretrain.pth.tar", "clip_vitb32_lora"],
+        "dino_vitb16": ["dino_vitb16_pretrain.pth", "dino_vitb16_single_lora"],
+        "open_clip_vitb32": ["open_clip_vitb32_pretrain.pth.tar", "open_clip_vitb32_single_lora"],
+        "clip_vitb32": ["clip_vitb32_pretrain.pth.tar", "clip_vitb32_single_lora"]
     }
 
     def check(path):
-        for required_ckpt in dreamsim_required_ckpts:
+        for required_ckpt in dreamsim_required_ckpts[dreamsim_type]:
             if not os.path.exists(os.path.join(path, required_ckpt)):
                 return False
         return True
 
     if not os.path.exists(cache_dir):
         os.mkdir(cache_dir)
 
     if check(cache_dir):
         print(f"Using cached {cache_dir}")
     else:
         print("Downloading checkpoint")
-        torch.hub.download_url_to_file(url=dreamsim_weights,
+        torch.hub.download_url_to_file(url=dreamsim_weights[dreamsim_type],
                                        dst=os.path.join(cache_dir, "pretrained.zip"))
         print("Unzipping...")
         with zipfile.ZipFile(os.path.join(cache_dir, "pretrained.zip"), 'r') as zip_ref:
             zip_ref.extractall(cache_dir)
 
 
-def dreamsim(pretrained: bool = True, device="cuda", cache_dir="./models", normalize_embeds: bool = True):
-    """ Initialized the DreamSim model. When first called, downloads/caches model weights for future use.
+def dreamsim(pretrained: bool = True, device="cuda", cache_dir="./models", normalize_embeds: bool = True,
+             dreamsim_type: str = "ensemble"):
+    """ Initializes the DreamSim model. When first called, downloads/caches model weights for future use.
 
     :param pretrained: If True, downloads and loads DreamSim weights.
     :param cache_dir: Location for downloaded weights.
     :param device: Device for model.
     :param normalize_embeds: If True, normalizes embeddings (i.e. divides by norm and subtracts mean).
+    :param dreamsim_type: The type of dreamsim model to use. The default is "ensemble" (default and best-performing)
+                          which concatenates dino_vitb16, clip_vitb16, and open_clip_vitb16 embeddings. Other options
+                          are "dino_vitb16", "clip_vitb32", and "open_clip_vitb32" which are finetuned single models.
     :return:
         - PerceptualModel with DreamSim settings and weights.
         - Preprocessing function that converts a PIL image and to a (1, 3, 224, 224) tensor with values [0-1].
     """
     # Get model settings and weights
-    download_weights(cache_dir=cache_dir)
+    download_weights(cache_dir=cache_dir, dreamsim_type=dreamsim_type)
 
     # initialize PerceptualModel and load weights
-    model_list = dreamsim_args['model_config']['model_type'].split(",")
-    ours_model = PerceptualModel(**dreamsim_args['model_config'], device=device, load_dir=cache_dir,
+    model_list = dreamsim_args['model_config'][dreamsim_type]['model_type'].split(",")
+    ours_model = PerceptualModel(**dreamsim_args['model_config'][dreamsim_type], device=device, load_dir=cache_dir,
                                  normalize_embeds=normalize_embeds)
     for extractor in ours_model.extractor_list:
         lora_config = LoraConfig(**dreamsim_args['lora_config'])
         model = get_peft_model(ViTModel(extractor.model, ViTConfig()), lora_config)
         extractor.model = model
 
+    tag = "" if dreamsim_type == "ensemble" else "single_"
     if pretrained:
         for extractor, name in zip(ours_model.extractor_list, model_list):
-            load_dir = os.path.join(cache_dir, f"{name}_lora")
+            load_dir = os.path.join(cache_dir, f"{name}_{tag}lora")
             extractor.model = PeftModel.from_pretrained(extractor.model, load_dir).to(device)
             extractor.model.eval().requires_grad_(False)
 
     ours_model.eval().requires_grad_(False)
 
     # Define preprocessing function
     t = transforms.Compose([
@@ -252,7 +258,8 @@
     'mae_vitb16': {'cls': 768, 'last_layer': 768},
     'mae_vitl16': {'cls': 1024, 'last_layer': 1024},
     'mae_vith14': {'cls': 1280, 'last_layer': 1280},
     'open_clip_vitb16': {'cls': 768, 'embedding': 512, 'last_layer': 768},
     'open_clip_vitb32': {'cls': 768, 'embedding': 512, 'last_layer': 768},
     'open_clip_vitl14': {'cls': 1024, 'embedding': 768, 'last_layer': 768}
 }
+
```

### Comparing `dreamsim-0.1.1/dreamsim.egg-info/PKG-INFO` & `dreamsim-0.1.2/dreamsim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dreamsim
-Version: 0.1.1
+Version: 0.1.2
 Summary: DreamSim similarity metric
-Home-page: https://github.com/ssundaram21/dreamsim-dev
+Home-page: https://github.com/ssundaram21/dreamsim
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- # ![icon](images/figs/icon.png)  DreamSim Perceptual Metric -->
@@ -18,17 +18,17 @@
 [Stephanie Fu](https://stephanie-fu.github.io)\* $^{1}$, [Netanel Tamir](https://netanel-tamir.github.io)\* $^{2}$, [Shobhita Sundaram](https://ssundaram21.github.io)\* $^{1}$, [Lucy Chai](https://people.csail.mit.edu/lrchai/) $^1$, [Richard Zhang](http://richzhang.github.io) $^3$, [Tali Dekel](https://www.weizmann.ac.il/math/dekel/) $^2$, [Phillip Isola](https://web.mit.edu/phillipi/) $^1$. (*equal contribution)<br>
 $^1$ MIT, $^2$ Weizmann Institute of Science, $^3$ Adobe Research.
 
 
 
 **Summary**
 
-Current metrics for perceptual image similarity operate at the level of pixels and patches. These metrics compare images in terms of their low-level colors and textures, but fail to capture mid-level similarities/differences in image layout, object poses, and semantic content. Meanwhile, measures that use image-level embeddings such as DINO and CLIP capture high-level and semantic judgements, but may not be aligned with human perception of more finegrained attributes.
+Current metrics for perceptual image similarity operate at the level of pixels and patches. These metrics compare images in terms of their low-level colors and textures, but fail to capture mid-level differences in layout, pose, semantic content, etc. Models that use image-level embeddings such as DINO and CLIP capture high-level and semantic judgements, but may not be aligned with human perception of more finegrained attributes.
 
-DreamSim is a new metric for perceptual image similarity that bridges the gap between "low-level" metrics (e.g. LPIPS, PSNR, SSIM) and "high-level" measures (e.g. CLIP). Our model was trained by concatenating CLIP, OpenCLIP, and DINO embeddings, and then finetuning on human perceptual judgements. We gathered these judgements on a dataset of ~20k image triplets, generated by diffusion models. Our model achieves better alignment with human similarity judgements than existing metrics, and can be used for a variety of downstream applications.
+DreamSim is a new metric for perceptual image similarity that bridges the gap between "low-level" metrics (e.g. LPIPS, PSNR, SSIM) and "high-level" measures (e.g. CLIP). Our model was trained by concatenating CLIP, OpenCLIP, and DINO embeddings, and then finetuning on human perceptual judgements. We gathered these judgements on a dataset of ~20k image triplets, generated by diffusion models. Our model achieves better alignment with human similarity judgements than existing metrics, and can be used for downstream applications such as image retrieval.
 
 ## Requirements
 - Linux
 - Python 3
 - NVIDIA GPU + CUDA CuDNN (DreamSim is only supported on CUDA devices)
 
 ## Setup
@@ -37,24 +37,20 @@
 
 ```pip install dreamsim```
 
 The package is used for importing and using the DreamSim model.
 
 **Option 2:** Clone our repo and install dependencies.
 This is necessary for running our training/evaluation scripts.
-<!--  ```
-git clone https://github.com/ssundaram21/DreamSim.git
-conda env create -f environment.yml
-export PYTHONPATH="$PYTHONPATH:$(realpath ./DreamSim)"
-``` -->
+
 ```
 python3 -m venv ds
 source ds/bin/activate
 pip install -r requirements.txt
-export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsimv)"
+export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsim)"
 ```
 To install with conda:
 ```
 conda create -n ds
 conda activate ds
 conda install pip # verify with the `which pip` command
 pip install -r requirements.txt
@@ -63,28 +59,36 @@
 
 ## Usage
 **For walk-through examples of the below use-cases, check out our [Colab demo](https://colab.research.google.com/drive/1taEOMzFE9g81D9AwH27Uhy2U82tQGAVI?usp=sharing).**
 
 ### Quickstart: Perceptual similarity metric
 The basic use case is to measure the perceptual distance between two images. **A higher score means more different, lower means more similar**. 
 
-The following code snippet is all you need. The first time that you run `dreamsim` it will automatically download the model weights. The default model settings are specified in `dreamsim/dreamsim_inference_v0.yaml`.
+The following code snippet is all you need. The first time that you run `dreamsim` it will automatically download the model weights. The default model settings are specified in `./dreamsim/config.py`.
 ```
 from dreamsim import dreamsim
 from PIL import Image
 
 model, preprocess = dreamsim(pretrained=True)
 
 img1 = preprocess(Image.open("img1_path")).to("cuda")
 img2 = preprocess(Image.open("img2_path")).to("cuda")
-distance = model(img1, img2) # The model takes an RGB image from [0, 1], size 1x3x224x224
+distance = model(img1, img2) # The model takes an RGB image from [0, 1], size batch_sizex3x224x224
 ```
 
 To run on example images, run `demo.py`. The script should produce distances (0.424, 0.34). 
 
+### (new!) Single-branch models
+By default, DreamSim uses an ensemble of CLIP, DINO, and OpenCLIP (all ViT-B/16). If you need a lighter-weight model you can use *single-branch* versions of DreamSim where only a single backbone is finetuned. The available options are OpenCLIP-ViTB/32, DINO-ViTB/16, CLIP-ViTB/32, in order of performance. 
+
+To load a single-branch model, use the `dreamsim_type` argument. For example:
+```
+dreamsim_dino_model, preprocess = dreamsim(pretrained=True, dreamsim_type="dino_vitb16")
+```
+
 ### Feature extraction
 To extract a *single image embedding* using dreamsim, use the `embed` method as shown in the following snippet:
 ```
 img1 = preprocess(Image.open("img1_path")).to("cuda")
 embedding = model.embed(img1)
 ```
 The perceptual distance between two images is the cosine distance between their embeddings. If the embeddings are normalized (true by default) L2 distance can also be used.
@@ -123,28 +127,24 @@
     dist = model(predicted_image, reference_image)
     dist.backward()
     optimizer.step()
 ```
 
 
 <a name="bibtex"></a>
-# Citation
+## Citation
 
 If you find our work or any of our materials useful, please cite our paper:
 ```
 @misc{fu2023dreamsim,
       title={DreamSim: Learning New Dimensions of Human Visual Similarity using Synthetic Data}, 
       author={Stephanie Fu and Netanel Tamir and Shobhita Sundaram and Lucy Chai and Richard Zhang and Tali Dekel and Phillip Isola},
       year={2023},
       eprint={2306.09344},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
 ```
 
 ## Acknowledgements
-We thank Jim DiCarlo, Liad Mudrik, Nitzan Censor for fruitful discussions throughout the project. Additionally, we thank Narek Tumanyan for his insightful comments over the course of the project. Finally, we thank Michelle Li for proofreading sections of this paper and offering helpful comments. 
-
-This work was supported by the NSF GRFP Fellowship to Shobhita Sundaram, the Meta PhD Fellowship to Lucy Chai, the Israeli Science Foundation (grant 2303/20) to Tali Dekel, and the Packard Fellowship to Phillip Isola.
-
 Our code borrows from the ["Deep ViT Features as Dense Visual Descriptors"](https://dino-vit-features.github.io/) repository for ViT feature extraction, and takes inspiration from the [UniverSeg](https://github.com/JJGO/UniverSeg) respository for code structure.
```

### Comparing `dreamsim-0.1.1/dreamsim.egg-info/SOURCES.txt` & `dreamsim-0.1.2/dreamsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.1/setup.py` & `dreamsim-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 long_description = "".join(long_description.split("<!--Experiments-->")[::2])
 long_description = "".join(long_description.split("![teaser](images/figs/teaser.png)"))
 
 setuptools.setup(
     name="dreamsim",
-    version="0.1.1",
+    version="0.1.2",
     description="DreamSim similarity metric",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ssundaram21/dreamsim-dev",
+    url="https://github.com/ssundaram21/dreamsim",
     packages=['dreamsim', 'dreamsim/feature_extraction'],
     install_requires=[
         "numpy",
         "open-clip-torch",
         "peft==0.1.0",
         "Pillow",
         "torch",
```

