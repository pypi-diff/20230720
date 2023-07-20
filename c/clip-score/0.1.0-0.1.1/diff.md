# Comparing `tmp/clip-score-0.1.0.tar.gz` & `tmp/clip-score-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clip-score-0.1.0.tar", last modified: Thu Mar  9 14:24:04 2023, max compression
+gzip compressed data, was "clip-score-0.1.1.tar", last modified: Thu Jul 20 15:03:15 2023, max compression
```

## Comparing `clip-score-0.1.0.tar` & `clip-score-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tedsun    (1001) tedsun    (1001)        0 2023-03-09 14:24:04.366240 clip-score-0.1.0/
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)    11357 2023-03-09 10:28:08.000000 clip-score-0.1.0/LICENSE
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)     2953 2023-03-09 14:24:04.366240 clip-score-0.1.0/PKG-INFO
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)     2526 2023-03-09 14:14:29.000000 clip-score-0.1.0/README.md
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)      158 2023-03-09 14:24:04.370240 clip-score-0.1.0/setup.cfg
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)     1737 2023-03-09 13:38:16.000000 clip-score-0.1.0/setup.py
-drwxrwxr-x   0 tedsun    (1001) tedsun    (1001)        0 2023-03-09 14:24:04.366240 clip-score-0.1.0/src/
-drwxrwxr-x   0 tedsun    (1001) tedsun    (1001)        0 2023-03-09 14:24:04.366240 clip-score-0.1.0/src/clip_score/
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)       22 2023-03-09 10:29:31.000000 clip-score-0.1.0/src/clip_score/__init__.py
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)       59 2023-03-09 10:33:20.000000 clip-score-0.1.0/src/clip_score/__main__.py
--rwxrwxr-x   0 tedsun    (1001) tedsun    (1001)     8055 2023-03-09 13:33:37.000000 clip-score-0.1.0/src/clip_score/clip_score.py
-drwxrwxr-x   0 tedsun    (1001) tedsun    (1001)        0 2023-03-09 14:24:04.366240 clip-score-0.1.0/src/clip_score.egg-info/
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)     2953 2023-03-09 14:24:04.000000 clip-score-0.1.0/src/clip_score.egg-info/PKG-INFO
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)      374 2023-03-09 14:24:04.000000 clip-score-0.1.0/src/clip_score.egg-info/SOURCES.txt
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)        1 2023-03-09 14:24:04.000000 clip-score-0.1.0/src/clip_score.egg-info/dependency_links.txt
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)       58 2023-03-09 14:24:04.000000 clip-score-0.1.0/src/clip_score.egg-info/entry_points.txt
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)      107 2023-03-09 14:24:04.000000 clip-score-0.1.0/src/clip_score.egg-info/requires.txt
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)       11 2023-03-09 14:24:04.000000 clip-score-0.1.0/src/clip_score.egg-info/top_level.txt
-drwxrwxr-x   0 tedsun    (1001) tedsun    (1001)        0 2023-03-09 14:24:04.366240 clip-score-0.1.0/tests/
--rw-rw-r--   0 tedsun    (1001) tedsun    (1001)     3402 2023-03-09 13:29:01.000000 clip-score-0.1.0/tests/test_clip_score.py
+drwxrwxr-x   0 tedsun    (1001) conda     (1002)        0 2023-07-20 15:03:15.022299 clip-score-0.1.1/
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)    11357 2023-03-09 10:28:08.000000 clip-score-0.1.1/LICENSE
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)     2891 2023-07-20 15:03:15.022299 clip-score-0.1.1/PKG-INFO
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)     2427 2023-07-19 10:05:11.000000 clip-score-0.1.1/README.md
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)      158 2023-07-20 15:03:15.022299 clip-score-0.1.1/setup.cfg
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)     1737 2023-07-20 15:02:27.000000 clip-score-0.1.1/setup.py
+drwxrwxr-x   0 tedsun    (1001) conda     (1002)        0 2023-07-20 15:03:15.022299 clip-score-0.1.1/src/
+drwxrwxr-x   0 tedsun    (1001) conda     (1002)        0 2023-07-20 15:03:15.022299 clip-score-0.1.1/src/clip_score/
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)       22 2023-07-20 15:01:54.000000 clip-score-0.1.1/src/clip_score/__init__.py
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)       59 2023-03-09 10:33:20.000000 clip-score-0.1.1/src/clip_score/__main__.py
+-rwxrwxr-x   0 tedsun    (1001) conda     (1002)     8096 2023-07-19 10:06:29.000000 clip-score-0.1.1/src/clip_score/clip_score.py
+drwxrwxr-x   0 tedsun    (1001) conda     (1002)        0 2023-07-20 15:03:15.022299 clip-score-0.1.1/src/clip_score.egg-info/
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)     2891 2023-07-20 15:03:14.000000 clip-score-0.1.1/src/clip_score.egg-info/PKG-INFO
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)      374 2023-07-20 15:03:14.000000 clip-score-0.1.1/src/clip_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)        1 2023-07-20 15:03:14.000000 clip-score-0.1.1/src/clip_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)       58 2023-07-20 15:03:14.000000 clip-score-0.1.1/src/clip_score.egg-info/entry_points.txt
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)      107 2023-07-20 15:03:14.000000 clip-score-0.1.1/src/clip_score.egg-info/requires.txt
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)       11 2023-07-20 15:03:14.000000 clip-score-0.1.1/src/clip_score.egg-info/top_level.txt
+drwxrwxr-x   0 tedsun    (1001) conda     (1002)        0 2023-07-20 15:03:15.022299 clip-score-0.1.1/tests/
+-rw-rw-r--   0 tedsun    (1001) conda     (1002)     3402 2023-03-09 13:29:01.000000 clip-score-0.1.1/tests/test_clip_score.py
```

### Comparing `clip-score-0.1.0/LICENSE` & `clip-score-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clip-score-0.1.0/PKG-INFO` & `clip-score-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,61 @@
-Metadata-Version: 2.1
-Name: clip-score
-Version: 0.1.0
-Summary: Package for calculating Clip Score using PyTorch
-Home-page: https://github.com/taited/clip-score
-Author: Taited
-Author-email: taited9160@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
+# CLIP Score for PyTorch
 
 [![PyPI](https://img.shields.io/pypi/v/clip-score.svg)](https://pypi.org/project/clip-score/)
 
-# CLIP score for PyTorch
-
-This repository provides a batch-wise quick processing for calculating CLIP scores. 
-The project structure is adapted from (pytorch-fid)[https://github.com/mseitzer/pytorch-fid] and (CLIP)[https://github.com/openai/CLIP].
-
-The CLIP Score measures the Cosine Similarity between two embedded features.
-This repository utilizes the pretrained (CLIP Model)[https://github.com/openai/CLIP] to calculate 
-the mean average of cosine similarities between two modalities.
+This repository provides a batch-wise quick processing for calculating CLIP scores. It uses the pretrained CLIP model to measure the cosine similarity between two modalities. The project structure is adapted from [pytorch-fid](https://github.com/mseitzer/pytorch-fid) and [CLIP](https://github.com/openai/CLIP).
 
 ## Installation
 
-Install from [pip](https://pypi.org/project/clip-score/):
-
-```
-pip install clip-score
-```
-
 Requirements:
-- python3
-- pytorch
-- torchvision
-- pillow
-- numpy
+- Install PyTorch:
+  ```
+  pip install torch  # Choose a version that suits your GPU
+  ```
+- Install CLIP:
+  ```
+  pip install git+https://github.com/openai/CLIP.git
+  ```
+- Install clip-score from [PyPI](https://pypi.org/project/clip-score/):
+  ```
+  pip install clip-score
+  ```
 
 ## Usage
 
-We assume that the image and the text data are contained in two individual folders. What's more, there is the same name of each sample in two modalities. To compute the CLIP score between images and texts:
+To compute the CLIP score between images and texts, make sure that the image and text data are contained in two separate folders, and each sample has the same name in both modalities. Run the following command:
 ```
 python -m clip_score path/to/image path/to/text
 ```
 
-To run the evaluation on GPU, use the flag `--device cuda:N`, where `N` is the index of the GPU to use.
+To run the evaluation on a GPU, use the `--device cuda:N` flag, where `N` is the index of the GPU to use.
+
+## Computing CLIP Score within the Same Modality
 
-## To measure the CLIP Score within image-image or text-text:
-In case you would like to calculate the CLIP score in the same modality, the folder structure
-should follow the upper usage case. Besides, you need to specify the prefered modalities by 
-`--real_flag` and `--fake_flag`. `--real_flag` refers to the modality of the former path and the `--fake_flag` refers to the later. The default settins are `--real_flag=img` and `--fake_flag=txt`.
-For example:
+If you want to calculate the CLIP score within the same modality (e.g., image-image or text-text), follow the same folder structure as mentioned above. Additionally, specify the preferred modalities using the `--real_flag` and `--fake_flag` options. By default, `--real_flag=img` and `--fake_flag=txt`. Examples:
 ```
 python -m clip_score path/to/imageA path/to/imageB --real_flag img --fake_flag img
 python -m clip_score path/to/textA path/to/textB --real_flag txt --fake_flag txt
 ```
 
 ## Citing
 
 If you use this repository in your research, consider citing it using the following Bibtex entry:
 
 ```
 @misc{taited2023CLIPScore,
   author={SUN Zhengwentai},
-  title={{clip-score: FID Score for PyTorch}},
+  title={{clip-score: CLIP Score for PyTorch}},
   month={March},
   year={2023},
   note={Version 0.1.0},
   howpublished={\url{https://github.com/taited/clip-score}},
 }
 ```
 
 ## License
 
 This implementation is licensed under the Apache License 2.0.
 
 The project structure is adapted from [mseitzer's pytorch-fid](https://github.com/mseitzer/pytorch-fid) project. The CLIP model is adapted from [OpenAI's CLIP](https://github.com/openai/CLIP).
 
-The CLIP Score was introduced in OpenAI's [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020)
+The CLIP Score was introduced in OpenAI's [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020).
```

### Comparing `clip-score-0.1.0/README.md` & `clip-score-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,79 @@
-[![PyPI](https://img.shields.io/pypi/v/clip-score.svg)](https://pypi.org/project/clip-score/)
+Metadata-Version: 2.1
+Name: clip-score
+Version: 0.1.1
+Summary: Package for calculating CLIP-Score using PyTorch
+Home-page: https://github.com/taited/clip-score
+Author: Taited
+Author-email: taited9160@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
-# CLIP score for PyTorch
+# CLIP Score for PyTorch
 
-This repository provides a batch-wise quick processing for calculating CLIP scores. 
-The project structure is adapted from (pytorch-fid)[https://github.com/mseitzer/pytorch-fid] and (CLIP)[https://github.com/openai/CLIP].
+[![PyPI](https://img.shields.io/pypi/v/clip-score.svg)](https://pypi.org/project/clip-score/)
 
-The CLIP Score measures the Cosine Similarity between two embedded features.
-This repository utilizes the pretrained (CLIP Model)[https://github.com/openai/CLIP] to calculate 
-the mean average of cosine similarities between two modalities.
+This repository provides a batch-wise quick processing for calculating CLIP scores. It uses the pretrained CLIP model to measure the cosine similarity between two modalities. The project structure is adapted from [pytorch-fid](https://github.com/mseitzer/pytorch-fid) and [CLIP](https://github.com/openai/CLIP).
 
 ## Installation
 
-Install from [pip](https://pypi.org/project/clip-score/):
-
-```
-pip install clip-score
-```
-
 Requirements:
-- python3
-- pytorch
-- torchvision
-- pillow
-- numpy
+- Install PyTorch:
+  ```
+  pip install torch  # Choose a version that suits your GPU
+  ```
+- Install CLIP:
+  ```
+  pip install git+https://github.com/openai/CLIP.git
+  ```
+- Install clip-score from [PyPI](https://pypi.org/project/clip-score/):
+  ```
+  pip install clip-score
+  ```
 
 ## Usage
 
-We assume that the image and the text data are contained in two individual folders. What's more, there is the same name of each sample in two modalities. To compute the CLIP score between images and texts:
+To compute the CLIP score between images and texts, make sure that the image and text data are contained in two separate folders, and each sample has the same name in both modalities. Run the following command:
 ```
 python -m clip_score path/to/image path/to/text
 ```
 
-To run the evaluation on GPU, use the flag `--device cuda:N`, where `N` is the index of the GPU to use.
+To run the evaluation on a GPU, use the `--device cuda:N` flag, where `N` is the index of the GPU to use.
+
+## Computing CLIP Score within the Same Modality
 
-## To measure the CLIP Score within image-image or text-text:
-In case you would like to calculate the CLIP score in the same modality, the folder structure
-should follow the upper usage case. Besides, you need to specify the prefered modalities by 
-`--real_flag` and `--fake_flag`. `--real_flag` refers to the modality of the former path and the `--fake_flag` refers to the later. The default settins are `--real_flag=img` and `--fake_flag=txt`.
-For example:
+If you want to calculate the CLIP score within the same modality (e.g., image-image or text-text), follow the same folder structure as mentioned above. Additionally, specify the preferred modalities using the `--real_flag` and `--fake_flag` options. By default, `--real_flag=img` and `--fake_flag=txt`. Examples:
 ```
 python -m clip_score path/to/imageA path/to/imageB --real_flag img --fake_flag img
 python -m clip_score path/to/textA path/to/textB --real_flag txt --fake_flag txt
 ```
 
 ## Citing
 
 If you use this repository in your research, consider citing it using the following Bibtex entry:
 
 ```
 @misc{taited2023CLIPScore,
   author={SUN Zhengwentai},
-  title={{clip-score: FID Score for PyTorch}},
+  title={{clip-score: CLIP Score for PyTorch}},
   month={March},
   year={2023},
   note={Version 0.1.0},
   howpublished={\url{https://github.com/taited/clip-score}},
 }
 ```
 
 ## License
 
 This implementation is licensed under the Apache License 2.0.
 
 The project structure is adapted from [mseitzer's pytorch-fid](https://github.com/mseitzer/pytorch-fid) project. The CLIP model is adapted from [OpenAI's CLIP](https://github.com/openai/CLIP).
 
-The CLIP Score was introduced in OpenAI's [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020)
+The CLIP Score was introduced in OpenAI's [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020).
+
+
```

### Comparing `clip-score-0.1.0/setup.py` & `clip-score-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 if __name__ == '__main__':
     setuptools.setup(
         name='clip-score',
         version=get_version(os.path.join('src', 'clip_score', '__init__.py')),
         author='Taited',
         author_email='taited9160@gmail.com',
-        description=('Package for calculating Clip Score'
+        description=('Package for calculating CLIP-Score'
                      ' using PyTorch'),
         long_description=read('README.md'),
         long_description_content_type='text/markdown',
         url='https://github.com/taited/clip-score',
         package_dir={'': 'src'},
         packages=setuptools.find_packages(where='src'),
         classifiers=[
```

### Comparing `clip-score-0.1.0/src/clip_score/clip_score.py` & `clip-score-0.1.1/src/clip_score/clip_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Calculates the CLIP Scores
 
 The CLIP model is a contrasitively learned language-image model. There is
-an image encoder and a text encoder in one CLIP model. It is believed that
-the CLIP model could measure the similarity of cross modalities. Please find
-more information from https://github.com/openai/CLIP.
+an image encoder and a text encoder. It is believed that the CLIP model could 
+measure the similarity of cross modalities. Please find more information from 
+https://github.com/openai/CLIP.
 
 The CLIP Score measures the Cosine Similarity between two embedded features.
-This CLIP Scores repository utilizes the pretrained CLIP Model to calculate 
+This repository utilizes the pretrained CLIP Model to calculate 
 the mean average of cosine similarities. 
 
 See --help to see further details.
 
 Code apapted from https://github.com/mseitzer/pytorch-fid and https://github.com/openai/CLIP.
 
 Copyright 2023 The Hong Kong Polytechnic University
@@ -150,15 +150,15 @@
 
 
 @torch.no_grad()
 def calculate_clip_score(dataloader, model, real_flag, fake_flag):
     score_acc = 0.
     sample_num = 0.
     logit_scale = model.logit_scale.exp()
-    for batch_data in dataloader:
+    for batch_data in tqdm(dataloader):
         real = batch_data['real']
         real_features = forward_modality(model, real, real_flag)
         fake = batch_data['fake']
         fake_features = forward_modality(model, fake, fake_flag)
         
         # normalize features
         real_features = real_features / real_features.norm(dim=1, keepdim=True).to(torch.float32)
@@ -202,23 +202,24 @@
             # of CPUs).
             num_cpus = os.cpu_count()
 
         num_workers = min(num_cpus, 8) if num_cpus is not None else 0
     else:
         num_workers = args.num_workers
 
+    print('Loading CLIP model: {}'.format(args.clip_model))
     model, preprocess = clip.load(args.clip_model, device=device)
     
     dataset = DummyDataset(args.real_path, args.fake_path,
                            args.real_flag, args.fake_flag,
                            transform=preprocess, tokenizer=clip.tokenize)
     dataloader = DataLoader(dataset, args.batch_size, 
                             num_workers=num_workers, pin_memory=True)
-    dataloader = tqdm(dataloader)
     
+    print('Calculating CLIP Score:')
     clip_score = calculate_clip_score(dataloader, model,
                                       args.real_flag, args.fake_flag)
     clip_score = clip_score.cpu().item()
     print('CLIP Score: ', clip_score)
 
 
 if __name__ == '__main__':
```

### Comparing `clip-score-0.1.0/src/clip_score.egg-info/PKG-INFO` & `clip-score-0.1.1/src/clip_score.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,79 @@
 Metadata-Version: 2.1
 Name: clip-score
-Version: 0.1.0
-Summary: Package for calculating Clip Score using PyTorch
+Version: 0.1.1
+Summary: Package for calculating CLIP-Score using PyTorch
 Home-page: https://github.com/taited/clip-score
 Author: Taited
 Author-email: taited9160@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-[![PyPI](https://img.shields.io/pypi/v/clip-score.svg)](https://pypi.org/project/clip-score/)
-
-# CLIP score for PyTorch
+# CLIP Score for PyTorch
 
-This repository provides a batch-wise quick processing for calculating CLIP scores. 
-The project structure is adapted from (pytorch-fid)[https://github.com/mseitzer/pytorch-fid] and (CLIP)[https://github.com/openai/CLIP].
+[![PyPI](https://img.shields.io/pypi/v/clip-score.svg)](https://pypi.org/project/clip-score/)
 
-The CLIP Score measures the Cosine Similarity between two embedded features.
-This repository utilizes the pretrained (CLIP Model)[https://github.com/openai/CLIP] to calculate 
-the mean average of cosine similarities between two modalities.
+This repository provides a batch-wise quick processing for calculating CLIP scores. It uses the pretrained CLIP model to measure the cosine similarity between two modalities. The project structure is adapted from [pytorch-fid](https://github.com/mseitzer/pytorch-fid) and [CLIP](https://github.com/openai/CLIP).
 
 ## Installation
 
-Install from [pip](https://pypi.org/project/clip-score/):
-
-```
-pip install clip-score
-```
-
 Requirements:
-- python3
-- pytorch
-- torchvision
-- pillow
-- numpy
+- Install PyTorch:
+  ```
+  pip install torch  # Choose a version that suits your GPU
+  ```
+- Install CLIP:
+  ```
+  pip install git+https://github.com/openai/CLIP.git
+  ```
+- Install clip-score from [PyPI](https://pypi.org/project/clip-score/):
+  ```
+  pip install clip-score
+  ```
 
 ## Usage
 
-We assume that the image and the text data are contained in two individual folders. What's more, there is the same name of each sample in two modalities. To compute the CLIP score between images and texts:
+To compute the CLIP score between images and texts, make sure that the image and text data are contained in two separate folders, and each sample has the same name in both modalities. Run the following command:
 ```
 python -m clip_score path/to/image path/to/text
 ```
 
-To run the evaluation on GPU, use the flag `--device cuda:N`, where `N` is the index of the GPU to use.
+To run the evaluation on a GPU, use the `--device cuda:N` flag, where `N` is the index of the GPU to use.
+
+## Computing CLIP Score within the Same Modality
 
-## To measure the CLIP Score within image-image or text-text:
-In case you would like to calculate the CLIP score in the same modality, the folder structure
-should follow the upper usage case. Besides, you need to specify the prefered modalities by 
-`--real_flag` and `--fake_flag`. `--real_flag` refers to the modality of the former path and the `--fake_flag` refers to the later. The default settins are `--real_flag=img` and `--fake_flag=txt`.
-For example:
+If you want to calculate the CLIP score within the same modality (e.g., image-image or text-text), follow the same folder structure as mentioned above. Additionally, specify the preferred modalities using the `--real_flag` and `--fake_flag` options. By default, `--real_flag=img` and `--fake_flag=txt`. Examples:
 ```
 python -m clip_score path/to/imageA path/to/imageB --real_flag img --fake_flag img
 python -m clip_score path/to/textA path/to/textB --real_flag txt --fake_flag txt
 ```
 
 ## Citing
 
 If you use this repository in your research, consider citing it using the following Bibtex entry:
 
 ```
 @misc{taited2023CLIPScore,
   author={SUN Zhengwentai},
-  title={{clip-score: FID Score for PyTorch}},
+  title={{clip-score: CLIP Score for PyTorch}},
   month={March},
   year={2023},
   note={Version 0.1.0},
   howpublished={\url{https://github.com/taited/clip-score}},
 }
 ```
 
 ## License
 
 This implementation is licensed under the Apache License 2.0.
 
 The project structure is adapted from [mseitzer's pytorch-fid](https://github.com/mseitzer/pytorch-fid) project. The CLIP model is adapted from [OpenAI's CLIP](https://github.com/openai/CLIP).
 
-The CLIP Score was introduced in OpenAI's [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020)
+The CLIP Score was introduced in OpenAI's [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020).
+
+
```

### Comparing `clip-score-0.1.0/tests/test_clip_score.py` & `clip-score-0.1.1/tests/test_clip_score.py`

 * *Files identical despite different names*

