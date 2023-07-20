# Comparing `tmp/smplkit-0.0.1.tar.gz` & `tmp/smplkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smplkit-0.0.1.tar", last modified: Sat Jul  8 08:43:57 2023, max compression
+gzip compressed data, was "smplkit-0.0.2.tar", last modified: Thu Jul 20 15:51:37 2023, max compression
```

## Comparing `smplkit-0.0.1.tar` & `smplkit-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:43:57.115253 smplkit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-08 08:43:46.000000 smplkit-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-08 08:43:57.115253 smplkit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-08 08:43:46.000000 smplkit-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:43:57.115253 smplkit-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-08 08:43:46.000000 smplkit-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:43:57.115253 smplkit-0.0.1/smplkit/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 08:43:47.000000 smplkit-0.0.1/smplkit/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/lbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-08 08:43:46.000000 smplkit-0.0.1/smplkit/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:43:57.115253 smplkit-0.0.1/smplkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-08 08:43:57.000000 smplkit-0.0.1/smplkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-08 08:43:57.000000 smplkit-0.0.1/smplkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:43:57.000000 smplkit-0.0.1/smplkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 08:43:57.000000 smplkit-0.0.1/smplkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:43:57.115253 smplkit-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 08:43:46.000000 smplkit-0.0.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:51:37.447269 smplkit-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 15:51:25.000000 smplkit-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 15:51:37.447269 smplkit-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-20 15:51:25.000000 smplkit-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:51:37.447269 smplkit-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-20 15:51:25.000000 smplkit-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:51:37.447269 smplkit-0.0.2/smplkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:51:26.000000 smplkit-0.0.2/smplkit/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29389 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/lbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:51:37.447269 smplkit-0.0.2/smplkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:51:37.447269 smplkit-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 15:51:25.000000 smplkit-0.0.2/test/test.py
```

### Comparing `smplkit-0.0.1/LICENSE` & `smplkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smplkit-0.0.1/PKG-INFO` & `smplkit-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smplkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: SMPL-KIT: Use SMPL models more easily.
 Home-page: https://github.com/Silverster98/smpl-kit
 Author: Zan Wang
 Author-email: zanwang98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -20,36 +20,46 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # smpl-kit
-Use SMPL more easily!
+> Use SMPL more easily! This project aims to provide a simple and easy-to-use interface for SMPL-related human body models, e.g., SMPL and SMPL-X. It also provides useful tools, e.g., SMPL parameter transformation, SMPL body mesh visualization, etc.
 
 ## Installation
 
-To install the `smplkit` package, you can either install it from PyPI or install it from source.
+1. Before installing `smplkit`, please make sure that you have installed [pytorch](https://pytorch.org/).
 
-- To install from PyPI by using `pip`:
 
-```bash
-pip install smplkit
-```
+2. To install the `smplkit` package, you can either install it from PyPI or install it from source.
 
-- Or, clone this repository and install it from source:
+   - To install from PyPI by using `pip`:
 
-```bash
-git clone git@github.com:Silverster98/smpl-kit.git
-cd smpl-kit
-pip install .
-```
+   ```bash
+   pip install smplkit
+   ```
+
+   - Or, clone this repository and install it from source:
+
+   ```bash
+   git clone git@github.com:Silverster98/smpl-kit.git
+   cd smpl-kit
+   pip install .
+   ```
 
 ## Documentation
 
+### Features
+
+- [x] SMPL/SMPL+H/SMPL-X body models
+- [x] Variable batch size
+- [x] Numerous utility functions
+- [x] Visualization tools
+
 ### Tutorial
 
 #### 1. Use the `SMPLLayer` to generate a SMPL body mesh with random translation while keeping other parameters as zero:
 
 ```python
 import torch
 import trimesh
```

### Comparing `smplkit-0.0.1/README.md` & `smplkit-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 # smpl-kit
-Use SMPL more easily!
+> Use SMPL more easily! This project aims to provide a simple and easy-to-use interface for SMPL-related human body models, e.g., SMPL and SMPL-X. It also provides useful tools, e.g., SMPL parameter transformation, SMPL body mesh visualization, etc.
 
 ## Installation
 
-To install the `smplkit` package, you can either install it from PyPI or install it from source.
+1. Before installing `smplkit`, please make sure that you have installed [pytorch](https://pytorch.org/).
 
-- To install from PyPI by using `pip`:
 
-```bash
-pip install smplkit
-```
+2. To install the `smplkit` package, you can either install it from PyPI or install it from source.
 
-- Or, clone this repository and install it from source:
+   - To install from PyPI by using `pip`:
 
-```bash
-git clone git@github.com:Silverster98/smpl-kit.git
-cd smpl-kit
-pip install .
-```
+   ```bash
+   pip install smplkit
+   ```
+
+   - Or, clone this repository and install it from source:
+
+   ```bash
+   git clone git@github.com:Silverster98/smpl-kit.git
+   cd smpl-kit
+   pip install .
+   ```
 
 ## Documentation
 
+### Features
+
+- [x] SMPL/SMPL+H/SMPL-X body models
+- [x] Variable batch size
+- [x] Numerous utility functions
+- [x] Visualization tools
+
 ### Tutorial
 
 #### 1. Use the `SMPLLayer` to generate a SMPL body mesh with random translation while keeping other parameters as zero:
 
 ```python
 import torch
 import trimesh
```

### Comparing `smplkit-0.0.1/setup.py` & `smplkit-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 URL = 'https://github.com/Silverster98/smpl-kit'
 EMAIL = 'zanwang98@gmail.com'
 AUTHOR = 'Zan Wang'
 REQUIRES_PYTHON = '>=3.6.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    # 'requests', 'maya', 'records',
+    'numpy>=1.19.0',
+    'einops>=0.3.0',
+    'torch>=1.6.0',
 ]
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

### Comparing `smplkit-0.0.1/smplkit/lbs.py` & `smplkit-0.0.2/smplkit/lbs.py`

 * *Files identical despite different names*

### Comparing `smplkit-0.0.1/smplkit/misc.py` & `smplkit-0.0.2/smplkit/misc.py`

 * *Files 22% similar despite different names*

```diff
@@ -91,14 +91,23 @@
     Return:
         The euler angles
     """
     sy = torch.sqrt(rot_mats[:, 0, 0] * rot_mats[:, 0, 0] +
                     rot_mats[:, 1, 0] * rot_mats[:, 1, 0])
     return torch.atan2(-rot_mats[:, 2, 0], sy)
 
+def find_joint_kin_chain(joint_id, kinematic_tree):
+    """ Find the kinematic chain of a given joint"""
+    kin_chain = []
+    curr_idx = joint_id
+    while curr_idx != -1:
+        kin_chain.append(curr_idx)
+        curr_idx = kinematic_tree[curr_idx]
+    return kin_chain
+
 class Struct(object):
     """ Body model parameter structure
     """
     def __init__(self, **kwargs: Dict) -> None:
         for key, val in kwargs.items():
             setattr(self, key, val)
 
@@ -119,8 +128,24 @@
     def items(self):
         return self.__dict__.items()
 
 @dataclass
 class SMPLOutput(ModelOutput):
     """ SMPL body model output structure
     """
-    
+    body_pose: Optional[Tensor] = None
+
+@dataclass
+class SMPLHOutput(SMPLOutput):
+    """ SMPLH body model output structure
+    """
+    left_hand_pose: Optional[Tensor] = None
+    right_hand_pose: Optional[Tensor] = None
+
+@dataclass
+class SMPLXOutput(SMPLHOutput):
+    """ SMPLX body model output structure
+    """
+    jaw_pose: Optional[Tensor] = None
+    leye_pose: Optional[Tensor] = None
+    reye_pose: Optional[Tensor] = None
+    landmarks: Optional[Tensor] = None
```

### Comparing `smplkit-0.0.1/smplkit.egg-info/PKG-INFO` & `smplkit-0.0.2/smplkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smplkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: SMPL-KIT: Use SMPL models more easily.
 Home-page: https://github.com/Silverster98/smpl-kit
 Author: Zan Wang
 Author-email: zanwang98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -20,36 +20,46 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # smpl-kit
-Use SMPL more easily!
+> Use SMPL more easily! This project aims to provide a simple and easy-to-use interface for SMPL-related human body models, e.g., SMPL and SMPL-X. It also provides useful tools, e.g., SMPL parameter transformation, SMPL body mesh visualization, etc.
 
 ## Installation
 
-To install the `smplkit` package, you can either install it from PyPI or install it from source.
+1. Before installing `smplkit`, please make sure that you have installed [pytorch](https://pytorch.org/).
 
-- To install from PyPI by using `pip`:
 
-```bash
-pip install smplkit
-```
+2. To install the `smplkit` package, you can either install it from PyPI or install it from source.
 
-- Or, clone this repository and install it from source:
+   - To install from PyPI by using `pip`:
 
-```bash
-git clone git@github.com:Silverster98/smpl-kit.git
-cd smpl-kit
-pip install .
-```
+   ```bash
+   pip install smplkit
+   ```
+
+   - Or, clone this repository and install it from source:
+
+   ```bash
+   git clone git@github.com:Silverster98/smpl-kit.git
+   cd smpl-kit
+   pip install .
+   ```
 
 ## Documentation
 
+### Features
+
+- [x] SMPL/SMPL+H/SMPL-X body models
+- [x] Variable batch size
+- [x] Numerous utility functions
+- [x] Visualization tools
+
 ### Tutorial
 
 #### 1. Use the `SMPLLayer` to generate a SMPL body mesh with random translation while keeping other parameters as zero:
 
 ```python
 import torch
 import trimesh
```

