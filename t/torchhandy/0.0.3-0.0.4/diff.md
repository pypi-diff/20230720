# Comparing `tmp/torchhandy-0.0.3.tar.gz` & `tmp/torchhandy-0.0.4.tar.gz`

## Comparing `torchhandy-0.0.3.tar` & `torchhandy-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 torchhandy-0.0.3/.pypirc
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 torchhandy-0.0.3/torchhandy/Block.py
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 torchhandy-0.0.3/torchhandy/Conv.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 torchhandy-0.0.3/torchhandy/Diffusion.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 torchhandy-0.0.3/torchhandy/FC.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 torchhandy-0.0.3/torchhandy/Parallel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchhandy-0.0.3/torchhandy/__init__.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 torchhandy-0.0.3/torchhandy/utils.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 torchhandy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 torchhandy-0.0.3/LICENSE
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 torchhandy-0.0.3/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 torchhandy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 torchhandy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 torchhandy-0.0.4/.pypirc
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 torchhandy-0.0.4/torchhandy/Block.py
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 torchhandy-0.0.4/torchhandy/Conv.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 torchhandy-0.0.4/torchhandy/Diffusion.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 torchhandy-0.0.4/torchhandy/FC.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 torchhandy-0.0.4/torchhandy/Parallel.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 torchhandy-0.0.4/torchhandy/Train.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchhandy-0.0.4/torchhandy/__init__.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 torchhandy-0.0.4/torchhandy/utils.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 torchhandy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 torchhandy-0.0.4/LICENSE
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 torchhandy-0.0.4/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 torchhandy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 torchhandy-0.0.4/PKG-INFO
```

### Comparing `torchhandy-0.0.3/torchhandy/Block.py` & `torchhandy-0.0.4/torchhandy/Block.py`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.3/torchhandy/Conv.py` & `torchhandy-0.0.4/torchhandy/Conv.py`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.3/torchhandy/Diffusion.py` & `torchhandy-0.0.4/torchhandy/Diffusion.py`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.3/torchhandy/FC.py` & `torchhandy-0.0.4/torchhandy/FC.py`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.3/torchhandy/Parallel.py` & `torchhandy-0.0.4/torchhandy/Parallel.py`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.3/torchhandy/utils.py` & `torchhandy-0.0.4/torchhandy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import torch
 import os
 import torch.nn as nn
 import math
+import time
 
 def clear_cuda():
     '''
         This function clears out cuda for more spaces. It is extremely useful when you encounter
         an CUDA out-of-memory in the middle of your training process.
     '''
     torch.cuda.empty_cache()
     torch.cuda.empty_cache()
     torch.cuda.empty_cache()
     torch.cuda.empty_cache()
     torch.cuda.empty_cache()
-    os.sleep(5)
+    time.sleep(5)
     torch.cuda.empty_cache()
     torch.cuda.empty_cache()
     torch.cuda.empty_cache()
     torch.cuda.empty_cache()
     torch.cuda.empty_cache()
     
 def fea2cha(x):
@@ -72,15 +73,15 @@
         if normalization[0] == 1:
             norm = nn.BatchNorm1d(normalization[1])
         elif normalization[0] == 2:
             norm = nn.BatchNorm2d(normalization[1])
         elif normalization[0] == 0:
             norm = nn.LayerNorm(normalization[1])    
     except Exception as e:
-        print("warning: No or unsupported normalization type given!")
+        pass
 
     return norm
 
 def get_mask(seq_len):
     '''
         Get a typical GPT attention mask.
     '''
```

### Comparing `torchhandy-0.0.3/LICENSE` & `torchhandy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchhandy-0.0.3/pyproject.toml` & `torchhandy-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 746f 7263 6868 616e 6479 220d 0a76   "torchhandy"..v
-00000070: 6572 7369 6f6e 203d 2022 302e 302e 3322  ersion = "0.0.3"
+00000070: 6572 7369 6f6e 203d 2022 302e 302e 3422  ersion = "0.0.4"
 00000080: 0d0a 6175 7468 6f72 7320 3d20 5b0d 0a20  ..authors = [.. 
 00000090: 207b 206e 616d 653d 22e5 bca0 e88d 9fe8   { name=".......
 000000a0: 90b1 222c 2065 6d61 696c 3d22 706b 756c  ..", email="pkul
 000000b0: 656f 7a68 616e 6740 676d 6169 6c2e 636f  eozhang@gmail.co
 000000c0: 6d22 7d2c 0d0a 5d0d 0a0d 0a64 6573 6372  m"},..]....descr
 000000d0: 6970 7469 6f6e 203d 2022 746f 7263 6868  iption = "torchh
 000000e0: 616e 6479 2069 7320 6120 6861 6e64 7920  andy is a handy 
@@ -30,13 +30,13 @@
 000001d0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
 000001e0: 204d 4954 204c 6963 656e 7365 222c 0d0a   MIT License",..
 000001f0: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
 00000200: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
 00000210: 7065 6e64 656e 7422 2c0d 0a5d 0d0a 6465  pendent",..]..de
 00000220: 7065 6e64 656e 6369 6573 203d 205b 0d0a  pendencies = [..
 00000230: 2020 2020 2020 2020 2274 6f72 6368 3e3d          "torch>=
-00000240: 312e 362e 3022 2c0d 0a20 2020 205d 0d0a  1.6.0",..    ]..
+00000240: 322e 302e 3022 2c0d 0a20 2020 205d 0d0a  2.0.0",..    ]..
 00000250: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
 00000260: 0d0a 2248 6f6d 6570 6167 6522 203d 2022  .."Homepage" = "
 00000270: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00000280: 6f6d 2f4e 6963 6b59 6931 3939 302f 6a75  om/NickYi1990/ju
 00000290: 616e 7322                                ans"
```

### Comparing `torchhandy-0.0.3/PKG-INFO` & `torchhandy-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchhandy
-Version: 0.0.3
+Version: 0.0.4
 Summary: torchhandy is a handy package that implements some commonly used modules and function.
 Project-URL: Homepage, https://github.com/NickYi1990/juans
 Author-email: 张荟萱 <pkuleozhang@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Huixuan Zhang]
         
@@ -26,15 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: torch>=1.6.0
+Requires-Dist: torch>=2.0.0
 Description-Content-Type: text/markdown
 
 # TorchHandy
 
 ## Introduction
 
 This is a handy implementation of some useful pytorch modules and functions, such as fully connected layers, etc.
```

