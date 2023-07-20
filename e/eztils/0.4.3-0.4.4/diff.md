# Comparing `tmp/eztils-0.4.3.tar.gz` & `tmp/eztils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.3.tar", max compression
+gzip compressed data, was "eztils-0.4.4.tar", max compression
```

## Comparing `eztils-0.4.3.tar` & `eztils-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.4.3/LICENSE
--rw-r--r--   0        0        0    12815 2023-07-15 07:19:31.991773 eztils-0.4.3/README.md
--rw-r--r--   0        0        0      542 2023-07-14 02:09:17.596159 eztils-0.4.3/eztils/__init__.py
--rw-r--r--   0        0        0     2021 2023-07-15 08:36:51.511267 eztils-0.4.3/eztils/default/__init__.py
--rw-r--r--   0        0        0     3689 2023-07-15 06:11:10.377851 eztils-0.4.3/eztils/default/dict_operations.py
--rw-r--r--   0        0        0     2246 2023-07-14 21:46:13.733182 eztils-0.4.3/eztils/default/itertools.py
--rw-r--r--   0        0        0     2458 2023-07-14 23:07:36.740250 eztils-0.4.3/eztils/default/logging.py
--rw-r--r--   0        0        0     1412 2023-07-15 08:36:51.519267 eztils-0.4.3/eztils/default/math.py
--rw-r--r--   0        0        0     1091 2023-07-14 01:58:12.704178 eztils-0.4.3/eztils/default/structures.py
--rw-r--r--   0        0        0     2346 2023-07-15 08:36:50.879275 eztils-0.4.3/eztils/git/__init__.py
--rw-r--r--   0        0        0     1489 2023-07-15 08:36:51.539267 eztils-0.4.3/eztils/torch/__init__.py
--rw-r--r--   0        0        0    15657 2023-07-15 08:36:51.763264 eztils-0.4.3/eztils/torch/distributions.py
--rw-r--r--   0        0        0      155 2023-07-14 22:54:30.913527 eztils-0.4.3/eztils/torch/lightning.py
--rw-r--r--   0        0        0      173 2023-07-14 22:54:30.917527 eztils-0.4.3/eztils/torch/math.py
--rw-r--r--   0        0        0     2550 2023-07-15 08:36:51.535267 eztils-0.4.3/eztils/torch/modules.py
--rw-r--r--   0        0        0     1420 2023-07-14 22:54:30.937527 eztils-0.4.3/eztils/torch/parameters.py
--rw-r--r--   0        0        0     1668 2023-07-15 08:36:50.879275 eztils-0.4.3/eztils/torch/tensor_creators.py
--rw-r--r--   0        0        0     2858 2023-07-14 23:03:35.175106 eztils-0.4.3/eztils/torch/to.py
--rw-r--r--   0        0        0     3712 2023-07-15 08:38:50.197824 eztils-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    13848 1970-01-01 00:00:00.000000 eztils-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-20 20:08:12.299029 eztils-0.4.4/LICENSE
+-rw-r--r--   0        0        0    12741 2023-07-20 20:08:12.299029 eztils-0.4.4/README.md
+-rw-r--r--   0        0        0      542 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/__init__.py
+-rw-r--r--   0        0        0     2359 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/dict_operations.py
+-rw-r--r--   0        0        0     2246 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/itertools.py
+-rw-r--r--   0        0        0     2458 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/logging.py
+-rw-r--r--   0        0        0     1412 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/math.py
+-rw-r--r--   0        0        0     1091 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/structures.py
+-rw-r--r--   0        0        0     1992 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/typing_validator.py
+-rw-r--r--   0        0        0     2346 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/git/__init__.py
+-rw-r--r--   0        0        0     1551 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/__init__.py
+-rw-r--r--   0        0        0    15657 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/distributions.py
+-rw-r--r--   0        0        0      155 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/lightning.py
+-rw-r--r--   0        0        0      173 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/math.py
+-rw-r--r--   0        0        0     2550 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/modules.py
+-rw-r--r--   0        0        0     1420 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/parameters.py
+-rw-r--r--   0        0        0     1668 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/tensor_creators.py
+-rw-r--r--   0        0        0     2858 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/to.py
+-rw-r--r--   0        0        0     3624 2023-07-20 20:08:12.299029 eztils-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    13903 1970-01-01 00:00:00.000000 eztils-0.4.4/PKG-INFO
```

### Comparing `eztils-0.4.3/LICENSE` & `eztils-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/README.md` & `eztils-0.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # eztils
 
-# TODO add tests
-# TODO add serialization to cloud or huggingface dataset
 <div align="center">
 
 [![Build status](https://github.com/ezhang7423/eztils/workflows/build/badge.svg?branch=master&event=push)](https://github.com/ezhang7423/eztils/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/eztils.svg)](https://pypi.org/project/eztils/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ezhang7423/eztils/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `eztils-0.4.3/eztils/__init__.py` & `eztils-0.4.4/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/default/__init__.py` & `eztils-0.4.4/eztils/default/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import inspect as inspect_
 import os
 import sys
 from inspect import getsourcefile, isfunction
 
+"""
+miscellaneous functions that are often used
+"""
+
 
 def default(val, d):
     """If val exists, return it. Otherwise, return d"""
     if val is not None:
         return val
     return d() if isfunction(d) else d
 
@@ -55,12 +59,22 @@
             return valid[default]
         elif choice in valid:
             return valid[choice]
         else:
             sys.stdout.write("Please respond with 'yes' or 'no' " "(or 'y' or 'n').\n")
 
 
+"""
+often used modules
+"""
+# beartype
+from beartype import beartype
+from beartype.door import die_if_unbearable  # <-- like "assert isinstance(...)"
+from beartype.door import is_bearable  # <-------- like "isinstance(...)"
+from beartype.vale import Is
+
 from .dict_operations import *
 from .itertools import *
 from .logging import *
 from .math import *
 from .structures import *
+from .typing_validator import *
```

### Comparing `eztils-0.4.3/eztils/default/dict_operations.py` & `eztils-0.4.4/eztils/default/dict_operations.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/default/itertools.py` & `eztils-0.4.4/eztils/default/itertools.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/default/logging.py` & `eztils-0.4.4/eztils/default/logging.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/default/math.py` & `eztils-0.4.4/eztils/default/math.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/default/structures.py` & `eztils-0.4.4/eztils/default/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/git/__init__.py` & `eztils-0.4.4/eztils/git/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/torch/__init__.py` & `eztils-0.4.4/eztils/torch/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-"""eds utilities"""
-
-# import often used modules
+"""
+import often used modules
+"""
 import random
 from pathlib import Path
 
 import numpy as np
 import torch
 from einops import rearrange as rea
 from einops import reduce
-from torch import einsum, nn
+from jaxtyping import Bool, Float, Float16, Float32, Int
+from torch import einsum, nn, tensor
 from torch.nn import functional as F
 from torchvision.utils import save_image
 
-# globals
+"""
+globals
+"""
 USE_GPU = False
 DTYPE = torch.float
 GPU_ID = 0
 DEVICE = None
 
 
 def set_gpu_mode(mode, gpu_id=0):
@@ -37,15 +40,17 @@
 
 
 def soft_update_from_to(source, target, tau):
     for target_param, param in zip(target.parameters(), source.parameters()):
         target_param.data.copy_(target_param.data * (1.0 - tau) + param.data * tau)
 
 
-# helper functions
+"""
+helper functions
+"""
 
 
 def seed_everything(seed):
     """
     Set the seed for all the possible random number generators
     for global packages.
     :param seed:
```

### Comparing `eztils-0.4.3/eztils/torch/distributions.py` & `eztils-0.4.4/eztils/torch/distributions.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/torch/modules.py` & `eztils-0.4.4/eztils/torch/modules.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/torch/parameters.py` & `eztils-0.4.4/eztils/torch/parameters.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/torch/tensor_creators.py` & `eztils-0.4.4/eztils/torch/tensor_creators.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/eztils/torch/to.py` & `eztils-0.4.4/eztils/torch/to.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.3/pyproject.toml` & `eztils-0.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.3"
+version = "0.4.4"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = [] #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   #! Update me
@@ -33,14 +33,16 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.3.3"
 numpy = "^1.24.3"
 loguru = "^0.7.0"
 einops = "^0.6.1"
 tqdm = "^4.65.0"
+ezjaxtyping = { version = "^0.2.20", optional = true }
+beartype = "^0.14.1"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.2"
 coverage-badge = "^1.1.0"
 darglint = "^1.8.1"
@@ -52,17 +54,18 @@
 pylint = "^2.17.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-html = "^3.2.0"
 pyupgrade = "^3.3.1"
 ipython = "^8.11.0"
 
-# [tool.poetry.extras]
-# torch = ["torchtyping"]
-# TODO can't run this because torchtyping depends on torch. if only there was a way to get --no-deps to work: https://github.com/python-poetry/poetry/issues/3377
+
+[tool.poetry.extras]
+torch = ["ezjaxtyping"]
+
 
 [tool.black]
 # https://github.com/psf/black
 color = true
 line-length = 88
 target-version = ["py38"]
```

### Comparing `eztils-0.4.3/PKG-INFO` & `eztils-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.3
+Version: 0.4.4
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,26 +13,27 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: torch
+Requires-Dist: beartype (>=0.14.1,<0.15.0)
 Requires-Dist: einops (>=0.6.1,<0.7.0)
+Requires-Dist: ezjaxtyping (>=0.2.20,<0.3.0) ; extra == "torch"
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/ezhang7423/eztils
 Description-Content-Type: text/markdown
 
 # eztils
 
-# TODO add tests
-# TODO add serialization to cloud or huggingface dataset
 <div align="center">
 
 [![Build status](https://github.com/ezhang7423/eztils/workflows/build/badge.svg?branch=master&event=push)](https://github.com/ezhang7423/eztils/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/eztils.svg)](https://pypi.org/project/eztils/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ezhang7423/eztils/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

