# Comparing `tmp/aisee-0.0.2.tar.gz` & `tmp/aisee-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisee-0.0.2.tar", max compression
+gzip compressed data, was "aisee-0.1.0.tar", max compression
```

## Comparing `aisee-0.0.2.tar` & `aisee-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1098 2023-04-26 12:18:08.386683 aisee-0.0.2/LICENSE
--rw-r--r--   0        0        0     3795 2023-04-26 12:18:08.386683 aisee-0.0.2/README.md
--rw-r--r--   0        0        0      211 2023-04-26 12:18:08.658690 aisee-0.0.2/aisee/__init__.py
--rw-r--r--   0        0        0     9624 2023-04-26 12:18:08.386683 aisee-0.0.2/aisee/custom_datasets.py
--rw-r--r--   0        0        0    15087 2023-04-26 12:18:08.386683 aisee-0.0.2/aisee/trainer.py
--rw-r--r--   0        0        0     6033 2023-04-26 12:18:08.386683 aisee-0.0.2/aisee/utils.py
--rw-r--r--   0        0        0    21393 2023-04-26 12:18:08.386683 aisee-0.0.2/aisee/vision_classifier.py
--rw-r--r--   0        0        0     3245 2023-04-26 12:18:23.635061 aisee-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 aisee-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-07-20 09:48:43.273147 aisee-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4294 2023-07-20 09:48:43.273147 aisee-0.1.0/README.md
+-rw-r--r--   0        0        0      211 2023-07-20 09:48:43.561145 aisee-0.1.0/aisee/__init__.py
+-rw-r--r--   0        0        0     9624 2023-07-20 09:48:43.273147 aisee-0.1.0/aisee/custom_datasets.py
+-rw-r--r--   0        0        0    15152 2023-07-20 09:48:43.273147 aisee-0.1.0/aisee/trainer.py
+-rw-r--r--   0        0        0     6033 2023-07-20 09:48:43.273147 aisee-0.1.0/aisee/utils.py
+-rw-r--r--   0        0        0    27487 2023-07-20 09:48:43.273147 aisee-0.1.0/aisee/vision_classifier.py
+-rw-r--r--   0        0        0     3262 2023-07-20 09:48:56.793064 aisee-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5628 1970-01-01 00:00:00.000000 aisee-0.1.0/PKG-INFO
```

### Comparing `aisee-0.0.2/LICENSE` & `aisee-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aisee-0.0.2/README.md` & `aisee-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 [![AISee Logo](./docs/source/_resources/aisee-logo.png)](https://iiconocimiento.github.io/aisee/stable/)
 
 ---
 
-[![License: MIT](https://img.shields.io/github/license/iiconocimiento/aisee)](https://github.com/iiconocimiento/aisee/blob/main/LICENSE) ![GitHub Stars](https://img.shields.io/github/stars/iiconocimiento/aisee?style=social) [![Latest Version on Pypi](https://img.shields.io/pypi/v/aisee)](https://pypi.org/project/aisee/) ![Supported Python versions](https://img.shields.io/pypi/pyversions/aisee) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) ![Unit tests](https://github.com/iiconocimiento/aisee/actions/workflows/unit-tests.yml/badge.svg) ![Docs](https://github.com/iiconocimiento/aisee/actions/workflows/documentation.yml/badge.svg)
+[![License: MIT](https://img.shields.io/github/license/iiconocimiento/aisee)](https://github.com/iiconocimiento/aisee/blob/main/LICENSE) ![GitHub Stars](https://img.shields.io/github/stars/iiconocimiento/aisee?style=social) [![Latest Version on Pypi](https://img.shields.io/pypi/v/aisee)](https://pypi.org/project/aisee/) ![Supported Python versions](https://img.shields.io/pypi/pyversions/aisee) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) ![Unit tests](https://github.com/iiconocimiento/aisee/actions/workflows/unit-tests.yml/badge.svg) [![codecov](https://codecov.io/github/iiconocimiento/aisee/branch/main/graph/badge.svg?token=YA7QJ8FOIM)](https://codecov.io/github/iiconocimiento/aisee) [![Docs](https://github.com/iiconocimiento/aisee/actions/workflows/documentation.yml/badge.svg)](https://iiconocimiento.github.io/aisee/stable/)
 
 An open-source library for computer vision built on top of PyTorch and Timm libraries. It provides an easy-to-use interface for training and predicting with State-of-the-Art neural networks.
 
 ## AISee key features 
 
 - 🤗 Simple interface for training and predicting using timm library models.
 - 📁 Easily load images from a folder, a pandas `DataFrame` or a single image path.
 - 🏋🏽‍♂️ Train SOTA neural networks from pre-trained weights or from scratch in very few lines of code.  
 - 🖼️ Supports multiclass and multilabel image classification tasks.
 - 🔨 We take care of `DataLoaders`, image transformations and training and inference loops.
 
 
+## Installation
+
+Install AISee using pip.
+
+```bash
+pip install aisee
+```
+
+
 ## Quick tour
 
 Here's an example of how to quickly train a model using AISee. We just have to initialize a `VisionClassifier` model and create a `Trainer`. As easy as it gets!
 
 ```python
 from aisee import Trainer, VisionClassifier
 
@@ -43,21 +52,19 @@
 
 ```python
 # Predict 
 trainer.base_model.predict("animals/without_label")
 ```
 
 
-## Installation
-
-Install AISee using pip.
+## Try it on Google Colab
+<a target="_blank" href="https://colab.research.google.com/github/iiconocimiento/aisee/blob/main/notebooks/multi_class_classification.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
-```bash
-pip install aisee
-```
 
 ## Getting started
 
 - Visit [AISee Getting started](https://iiconocimiento.github.io/aisee/stable/_getting_started/getting_started.html) to get an overview of how AISee works.
 
 - Explore [AISee Documentation](https://iiconocimiento.github.io/aisee/stable/) page for a detailed guide and comprehensive API reference.
 
@@ -69,10 +76,10 @@
 
 We also appreciate your feedback which helps us develop a robust and efficient solution for computer vision tasks. Together, let's make AISee the go-to library for AI practitioners and enthusiasts alike.
 
 ## Contact Us
 For any questions or inquiries regarding the AISee library or potential collaborations, please feel free to contact us in marketing@iic.uam.es. 
 
 ## Instituto de Ingeniería del Conocimiento (IIC)
-IIC is a non-profit R&D centre founded in 1989 that has been working on Big Data analysis and Artificial Intelligence for more than 30 years. Its value proposition is the development of algorithms and analytical solutions based on applied research tailored to different businesses in different sectors such as energy, health, insurance and talent analytics.
+[IIC](https://www.iic.uam.es/) is a non-profit R&D centre founded in 1989 that has been working on Big Data analysis and Artificial Intelligence for more than 30 years. Its value proposition is the development of algorithms and analytical solutions based on applied research tailored to different businesses in different sectors such as energy, health, insurance and talent analytics.
 
 ---
```

### Comparing `aisee-0.0.2/aisee/custom_datasets.py` & `aisee-0.1.0/aisee/custom_datasets.py`

 * *Files identical despite different names*

### Comparing `aisee-0.0.2/aisee/trainer.py` & `aisee-0.1.0/aisee/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,18 +378,19 @@
                 self.hist[epoch][phase + "_acc"] = epoch_acc
                 self.hist[epoch][phase + "_f1"] = epoch_f1
 
                 epoch_sm = self.hist[epoch][phase + "_" + self.checkpointing_metric] * factor
 
                 if phase == "val" and epoch_sm > best_sm:
                     best_sm = epoch_sm
+                    best_epoch = epoch + 1
                     best_model_wts = copy.deepcopy(self.base_model.model.state_dict())
                     torch.save(self.base_model.model.state_dict(), self.output_dir)
 
         best_sm = best_sm * factor
         time_elapsed = time.time() - since
 
         if self.verbose > 0:
             LOGGER.info(f"Training complete in {time_elapsed // 60:.0f}m {time_elapsed % 60:.0f}s")
-            LOGGER.info(f"Best val {self.checkpointing_metric}: {best_sm:4f}")
+            LOGGER.info(f"Best val {self.checkpointing_metric}: {best_sm:4f} in epoch {best_epoch}")
 
         self.base_model.model.load_state_dict(best_model_wts)
```

### Comparing `aisee-0.0.2/aisee/utils.py` & `aisee-0.1.0/aisee/utils.py`

 * *Files identical despite different names*

### Comparing `aisee-0.0.2/aisee/vision_classifier.py` & `aisee-0.1.0/aisee/vision_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import inspect
 import logging
 import operator
 from collections.abc import Mapping
 from pathlib import Path
-from typing import TypeVar, Union
+from typing import Any, Callable, TypeVar, Union
 
+import numpy as np
 import pandas as pd
 import timm
 import torch
 from torch import nn
 from torchvision import transforms
 
 from .custom_datasets import (
@@ -597,7 +599,163 @@
 
                 all_probabilities = torch.cat((all_probabilities, probabilities), 0)
                 all_predictions = torch.cat((all_predictions, predictions), 0)
                 all_real_labels = torch.cat((all_real_labels, labels), 0)
                 all_paths.extend(paths)
 
         return all_paths, all_probabilities, all_predictions, all_real_labels
+
+    def evaluate(
+        self,
+        data: Union[pd.Series, pd.DataFrame, str],
+        metrics: list[Callable],
+        metrics_kwargs: dict[str, dict[str, Any]],
+        num_workers: int = 2,
+        data_transform: transforms.Compose = None,
+        batch_size: int = 8,
+    ) -> dict[str, Any]:
+        """
+        Evaluate `data` over the metrics indicated in the `metrics` parameter.
+
+        Parameters
+        ----------
+        data : pandas.DataFrame or str
+            A DataFrame or a string which contains the training data:
+
+        - If it is a dataframe:
+            - If it is a multiclass problem: the dataframe must contain a `path`
+            column with the full path of the image and a `label` column (optional) with
+            the label assigned to the image. This `label` can be a number or a string.
+
+            Example:
+
+            +-------------------+------------+
+            |       path        |   label    |
+            +===================+============+
+            |"sample/cat1.png"  |   "cat"    |
+            +-------------------+------------+
+            |"sample/cat2.png"  |   "cat"    |
+            +-------------------+------------+
+            |"sample/dog1.png"  |   "dog"    |
+            +-------------------+------------+
+            |"sample/cat3.png"  |   "cat"    |
+            +-------------------+------------+
+
+            or
+
+            +-----------------+
+            |        path     |
+            +=================+
+            |"sample/cat1.png"|
+            +-----------------+
+            |"sample/cat2.png"|
+            +-----------------+
+            |"sample/dog1.png"|
+            +-----------------+
+            |"sample/cat3.png"|
+            +-----------------+
+
+            - If it is a multilabel problem: the dataframe must contain a "path"
+            column with the full path of the image and one column for each
+            class in the problem. The classes that belong to that image will be
+            indicated with a "1" and those that do not with a "0".
+
+            Example:
+
+            +------------------------+---------+---------------+--------+
+            |        path            |   car   |   motorbike   |   bus  |
+            +========================+=========+===============+========+
+            |"sample/vehicles1.png"  |    1    |       1       |    0   |
+            +------------------------+---------+---------------+--------+
+            |"sample/vehicles2.png"  |    0    |       0       |    1   |
+            +------------------------+---------+---------------+--------+
+            |"sample/vehicles3.png"  |    1    |       0       |    1   |
+            +------------------------+---------+---------------+--------+
+            |"sample/vehicles4.png"  |    1    |       0       |    0   |
+            +------------------------+---------+---------------+--------+
+
+        - If it is a string, it must be:
+            - A path to an image.
+
+            Example
+
+            .. code-block:: console
+
+                /data/cat.png
+
+            - A directory where each folder is a class, and inside that class are the
+            images.
+
+            Example:
+
+            .. code-block:: console
+
+                ├── animals
+                ├── cat
+                │  ├── cat1.jpg
+                │  └── cat2.jpg
+                └── dog
+                    ├── dog1.jpg
+                    └── dog2.jpg
+
+        metrics : List[Callable]
+            Each element of the list is a function that at least has the parameters
+            `y_pred` and `y_true`, and each parameter accepts pure predictions as 1D array-like.
+
+            For example, you can import `accuracy_score` from `sklearn.metrics`.
+        metrics_kwargs : Dict[str, Dict[str, Any]]
+            Each key of the dictionary represents the name of one of the functions
+            indicated in the `metrics` parameter. The value is a dictionary with the
+            arguments of thath function.
+
+            For example, if your `metrics` parameter has the function `f1_score` from
+            `sklearn.metrics` and you want to use the parameter `average` with `micro` value,
+            your kwargs will be:
+
+                .. code-block:: python
+
+                metrics_kwargs = {"f1_score": {"average": "micro"}}
+
+        num_workers : int, default=2
+            Subprocesses to use for data loading.
+        data_transform : torchvision.transforms.Compose, default=None
+        batch_size : int, default=8
+
+        Returns
+        -------
+        evaluation_results : Dict[str, Any]
+            The resulting dictionary has a key for each function in the `metrics` parameter.
+            The values are the results of each function.
+        """
+        for metric in metrics:
+            func_params = inspect.signature(metric).parameters
+            if not all(
+                required_param in func_params
+                for required_param in [
+                    "y_true",
+                    "y_pred",
+                ]
+            ):
+                raise TypeError(
+                    f"Parameters y_true and y_pred are required in function {metric.__name__}",
+                )
+
+        predictions = self.predict(data, num_workers, data_transform, batch_size)
+        predictions = pd.DataFrame(predictions, columns=["prediction", "real_label"])
+
+        if self.task == "single_label":
+            y_pred = predictions["prediction"].astype("int")
+            y_true = predictions["real_label"].astype("int")
+        else:
+            y_pred = np.concatenate(predictions["prediction"].to_numpy())
+            y_true = np.concatenate(predictions["real_label"].to_numpy())
+
+        return {
+            metric.__name__: metric(
+                y_pred=y_pred,
+                y_true=y_true,
+                **metrics_kwargs[metric.__name__],
+            )
+            if metric.__name__ in metrics_kwargs
+            else metric(y_pred=y_pred, y_true=y_true)
+            for metric in metrics
+        }
```

### Comparing `aisee-0.0.2/pyproject.toml` & `aisee-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aisee"
-version = "0.0.2"
+version = "0.1.0"
 description = "aisee is a Python package for image classification using PyTorch and timm created by Instituto de Ingeniería del Conocimiento"
 authors = ["IIC"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://iiconocimiento.github.io/aisee"
 repository = "https://github.com/iiconocimiento/aisee"
 documentation = "https://iiconocimiento.github.io/aisee"
@@ -25,15 +25,15 @@
 python = ">=3.9, <3.12"
 datasets = ">= 2"
 huggingface-hub = ">= 0.13"
 pandas = ">= 1"
 Pillow = ">= 8.4.0"
 scikit-learn = ">= 1"
 timm = ">= 0.5.4"
-torch = ">= 1.13.1"
+torch = ">= 1.13.1, <=2.0.0"
 torchvision = ">= 0.11.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.3.1"
 pytest-cov = "3.0.0"
 coverage = {extras = ["toml"], version ="6.5.0"}
 pytest-ruff = "0.0.5"
@@ -48,16 +48,16 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
     "--cov-report", "html:cover",
     "--cov-report", "term",
+    "--cov-report", "xml",
     "--cov-config=pyproject.toml",
-    "--junitxml=report.xml",
     "--cov=aisee",
     "--durations=20",
     "--ignore=docs/",
 ]
 filterwarnings = [
     "ignore::PendingDeprecationWarning",
     "ignore::RuntimeWarning",
@@ -100,15 +100,15 @@
     "PTH",
     "ERA",
     "PD",
     "PL",
     "RUF",
 ]
 unfixable = ["B007"]
-ignore = ["E501", "D100", "D103", "D104", "PLR0913", "PLR0915", "PLR2004", "S101", "ANN101"]
+ignore = ["E501", "D100", "D103", "D104", "PLR0913", "PLR0915", "PLR2004", "RUF013", "S101", "ANN101"]
 
 src = ["aisee", "tests"]
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
```

### Comparing `aisee-0.0.2/PKG-INFO` & `aisee-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisee
-Version: 0.0.2
+Version: 0.1.0
 Summary: aisee is a Python package for image classification using PyTorch and timm created by Instituto de Ingeniería del Conocimiento
 Home-page: https://iiconocimiento.github.io/aisee
 License: MIT
 Keywords: aisee,computer vision,vision,timm,pytorch
 Author: IIC
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,47 +13,53 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: Pillow (>=8.4.0)
 Requires-Dist: datasets (>=2)
 Requires-Dist: huggingface-hub (>=0.13)
 Requires-Dist: pandas (>=1)
 Requires-Dist: scikit-learn (>=1)
 Requires-Dist: timm (>=0.5.4)
-Requires-Dist: torch (>=1.13.1)
+Requires-Dist: torch (>=1.13.1,<=2.0.0)
 Requires-Dist: torchvision (>=0.11.3)
 Project-URL: Documentation, https://iiconocimiento.github.io/aisee
 Project-URL: Repository, https://github.com/iiconocimiento/aisee
 Description-Content-Type: text/markdown
 
 [![AISee Logo](./docs/source/_resources/aisee-logo.png)](https://iiconocimiento.github.io/aisee/stable/)
 
 ---
 
-[![License: MIT](https://img.shields.io/github/license/iiconocimiento/aisee)](https://github.com/iiconocimiento/aisee/blob/main/LICENSE) ![GitHub Stars](https://img.shields.io/github/stars/iiconocimiento/aisee?style=social) [![Latest Version on Pypi](https://img.shields.io/pypi/v/aisee)](https://pypi.org/project/aisee/) ![Supported Python versions](https://img.shields.io/pypi/pyversions/aisee) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) ![Unit tests](https://github.com/iiconocimiento/aisee/actions/workflows/unit-tests.yml/badge.svg) ![Docs](https://github.com/iiconocimiento/aisee/actions/workflows/documentation.yml/badge.svg)
+[![License: MIT](https://img.shields.io/github/license/iiconocimiento/aisee)](https://github.com/iiconocimiento/aisee/blob/main/LICENSE) ![GitHub Stars](https://img.shields.io/github/stars/iiconocimiento/aisee?style=social) [![Latest Version on Pypi](https://img.shields.io/pypi/v/aisee)](https://pypi.org/project/aisee/) ![Supported Python versions](https://img.shields.io/pypi/pyversions/aisee) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) ![Unit tests](https://github.com/iiconocimiento/aisee/actions/workflows/unit-tests.yml/badge.svg) [![codecov](https://codecov.io/github/iiconocimiento/aisee/branch/main/graph/badge.svg?token=YA7QJ8FOIM)](https://codecov.io/github/iiconocimiento/aisee) [![Docs](https://github.com/iiconocimiento/aisee/actions/workflows/documentation.yml/badge.svg)](https://iiconocimiento.github.io/aisee/stable/)
 
 An open-source library for computer vision built on top of PyTorch and Timm libraries. It provides an easy-to-use interface for training and predicting with State-of-the-Art neural networks.
 
 ## AISee key features 
 
 - 🤗 Simple interface for training and predicting using timm library models.
 - 📁 Easily load images from a folder, a pandas `DataFrame` or a single image path.
 - 🏋🏽‍♂️ Train SOTA neural networks from pre-trained weights or from scratch in very few lines of code.  
 - 🖼️ Supports multiclass and multilabel image classification tasks.
 - 🔨 We take care of `DataLoaders`, image transformations and training and inference loops.
 
 
+## Installation
+
+Install AISee using pip.
+
+```bash
+pip install aisee
+```
+
+
 ## Quick tour
 
 Here's an example of how to quickly train a model using AISee. We just have to initialize a `VisionClassifier` model and create a `Trainer`. As easy as it gets!
 
 ```python
 from aisee import Trainer, VisionClassifier
 
@@ -78,21 +84,19 @@
 
 ```python
 # Predict 
 trainer.base_model.predict("animals/without_label")
 ```
 
 
-## Installation
+## Try it on Google Colab
+<a target="_blank" href="https://colab.research.google.com/github/iiconocimiento/aisee/blob/main/notebooks/multi_class_classification.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
-Install AISee using pip.
-
-```bash
-pip install aisee
-```
 
 ## Getting started
 
 - Visit [AISee Getting started](https://iiconocimiento.github.io/aisee/stable/_getting_started/getting_started.html) to get an overview of how AISee works.
 
 - Explore [AISee Documentation](https://iiconocimiento.github.io/aisee/stable/) page for a detailed guide and comprehensive API reference.
 
@@ -104,11 +108,11 @@
 
 We also appreciate your feedback which helps us develop a robust and efficient solution for computer vision tasks. Together, let's make AISee the go-to library for AI practitioners and enthusiasts alike.
 
 ## Contact Us
 For any questions or inquiries regarding the AISee library or potential collaborations, please feel free to contact us in marketing@iic.uam.es. 
 
 ## Instituto de Ingeniería del Conocimiento (IIC)
-IIC is a non-profit R&D centre founded in 1989 that has been working on Big Data analysis and Artificial Intelligence for more than 30 years. Its value proposition is the development of algorithms and analytical solutions based on applied research tailored to different businesses in different sectors such as energy, health, insurance and talent analytics.
+[IIC](https://www.iic.uam.es/) is a non-profit R&D centre founded in 1989 that has been working on Big Data analysis and Artificial Intelligence for more than 30 years. Its value proposition is the development of algorithms and analytical solutions based on applied research tailored to different businesses in different sectors such as energy, health, insurance and talent analytics.
 
 ---
```

