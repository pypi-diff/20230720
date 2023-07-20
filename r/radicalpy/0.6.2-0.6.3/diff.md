# Comparing `tmp/radicalpy-0.6.2.tar.gz` & `tmp/radicalpy-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicalpy-0.6.2.tar", last modified: Fri Jul 14 03:06:46 2023, max compression
+gzip compressed data, was "radicalpy-0.6.3.tar", last modified: Thu Jul 20 10:25:27 2023, max compression
```

## Comparing `radicalpy-0.6.2.tar` & `radicalpy-0.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-14 03:06:37.000000 radicalpy-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-14 03:06:46.491118 radicalpy-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-14 03:06:37.000000 radicalpy-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-14 03:06:37.000000 radicalpy-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.487118 radicalpy-0.6.2/radicalpy/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4924 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/classical.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/radicalpy/data/
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/constants.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/radicalpy/data/molecules/
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/2_6_aqds.json
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/adenine_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/flavin_anion.json
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/flavin_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/tryptophan_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/tyrosine_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/spin_data.json
--rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    20209 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     9710 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    25118 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    11422 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/radicalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-14 03:06:37.000000 radicalpy-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 03:06:46.491118 radicalpy-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_relaxations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.553914 radicalpy-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-20 10:25:08.000000 radicalpy-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-20 10:25:27.553914 radicalpy-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-20 10:25:08.000000 radicalpy-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-20 10:25:08.000000 radicalpy-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.549914 radicalpy-0.6.3/radicalpy/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/classical.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.553914 radicalpy-0.6.3/radicalpy/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/constants.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.553914 radicalpy-0.6.3/radicalpy/data/molecules/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/2_6_aqds.json
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/adenine_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/flavin_anion.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/flavin_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/tryptophan_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/tyrosine_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/spin_data.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20209 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9706 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31601 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11420 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.549914 radicalpy-0.6.3/radicalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-20 10:25:08.000000 radicalpy-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 10:25:27.553914 radicalpy-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.553914 radicalpy-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_relaxations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_simulation.py
```

### Comparing `radicalpy-0.6.2/LICENSE` & `radicalpy-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/PKG-INFO` & `radicalpy-0.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.6.2
+Version: 0.6.3
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.6.2/README.md` & `radicalpy-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/pyproject.toml` & `radicalpy-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/classical.py` & `radicalpy-0.6.3/radicalpy/classical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python
 
 
+from typing import Tuple
+
 import numpy as np
 import scipy as sp
 
 from . import utils
 
 
 def get_delta_r(mutual_diffusion: float, delta_T: float) -> float:
@@ -75,41 +77,48 @@
     theta = np.pi * np.random.rand()
     arg = np.random.uniform(-1, 1)
     phi = 2 * np.sign(arg) * np.arcsin(np.sqrt(np.abs(arg)))
     return theta, phi
 
 
 def randomwalk_3d(
-    n_steps: float,
+    n_steps: int,
     x_0: float,
     y_0: float,
     z_0: float,
     delta_r: float,
     r_min: float,
     r_max: float = 0,
-) -> (np.ndarray, np.ndarray, np.ndarray):
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Simulate Monte Carlo random walk.
 
     The MC random walk is simulated for radicals pairs in both
     solution (`r_max = 0`) and microreactor (`r_max > 0`)
     environments.
 
     Args:
+
             n_steps (float): The number of simulation steps.
+
             x_0 (float): The initial position in the x-axis (m).
+
             y_0 (float): The initial position in the x-axis (m).
+
             z_0 (float): The initial position in the x-axis (m).
+
             delta_r (float): The mean path between two radicals (m).
+
             r_min (float): The distance of closest approach (m).
+
             r_max (float): The diameter of the microreactor (m). Set
                 to 0 for solution-based, and to a positive value for
                 microreactor-based simulations.
 
     Returns:
-        (np.ndarray, np.ndarray, np.ndarray):
+        Tuple[np.ndarray, np.ndarray, np.ndarray]:
             - pos: The positions of the moving radical (m).
             - dist: The mutual distances between the radical pairs (m).
             - angle: The angles (theta) of the vector trajectories of
               the moving radical (m).
 
     """
     if r_max != 0 and r_min > r_max:
```

### Comparing `radicalpy-0.6.2/radicalpy/data/constants.json` & `radicalpy-0.6.3/radicalpy/data/constants.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/data/molecules/flavin_anion.json` & `radicalpy-0.6.3/radicalpy/data/molecules/flavin_anion.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/data/molecules/flavin_neutral.json` & `radicalpy-0.6.3/radicalpy/data/molecules/flavin_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/data/molecules/tryptophan_cation.json` & `radicalpy-0.6.3/radicalpy/data/molecules/tryptophan_cation.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/data/molecules/tyrosine_neutral.json` & `radicalpy-0.6.3/radicalpy/data/molecules/tyrosine_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/data/spin_data.json` & `radicalpy-0.6.3/radicalpy/data/spin_data.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/data.py` & `radicalpy-0.6.3/radicalpy/data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/estimations.py` & `radicalpy-0.6.3/radicalpy/estimations.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/kinetics.py` & `radicalpy-0.6.3/radicalpy/kinetics.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/plot.py` & `radicalpy-0.6.3/radicalpy/plot.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/relaxation.py` & `radicalpy-0.6.3/radicalpy/relaxation.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,21 +239,21 @@
             + np.kron(QT0, QTp)
         )
 
 
 class TripletTripletRelaxation(LiouvilleRelaxationBase):
     """Triplet-triplet relaxation superoperator.
 
-    Source: `Miura et al. J. Phys. Chem. A 119, 5534−5544 (2015)`_.
+    Source: `Miura et al. J. Phys. Chem. A 119, 5534-5544 (2015)`_.
 
     >>> TripletTripletRelaxation(rate_constant=1e6)
     Relaxation: TripletTripletRelaxation
     Rate constant: 1000000.0
 
-    .. _Miura et al. J. Phys. Chem. A 119, 5534−5544 (2015):
+    .. _Miura et al. J. Phys. Chem. A 119, 5534-5544 (2015):
        https://doi.org/10.1021/acs.jpca.5b02183
     """
 
     # restrict to
     # init_state=rpsim.State.TRIPLET_ZERO,
     # obs_state=rpsim.State.TRIPLET_ZERO,
     def init(self, sim: LiouvilleSimulation):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `radicalpy-0.6.2/radicalpy/shared.py` & `radicalpy-0.6.3/radicalpy/shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/radicalpy/simulation.py` & `radicalpy-0.6.3/radicalpy/simulation.py`

 * *Files 18% similar despite different names*

```diff
@@ -138,26 +138,29 @@
     @staticmethod
     def pauli(mult: int):
         """Generate Pauli matrices.
 
         Generates the Pauli matrices corresponding to a given multiplicity.
 
         Args:
+
             mult (int): The multiplicity of the element.
 
-        Return:
-            dict: A dictionary containing 6 `np.array` matrices of
-            shape `(mult, mult)`:
-
-            - the unit operator `result["u"]`,
-            - raising operator `result["p"]`,
-            - lowering operator `result["m"]`,
-            - Pauli matrix for x axis `result["x"]`,
-            - Pauli matrix for y axis `result["y"]`,
-            - Pauli matrix for z axis `result["z"]`.
+        Returns:
+            dict:
+
+                A dictionary containing 6 `np.array` matrices of
+                shape `(mult, mult)`:
+
+                - the unit operator `result["u"]`,
+                - raising operator `result["p"]`,
+                - lowering operator `result["m"]`,
+                - Pauli matrix for x axis `result["x"]`,
+                - Pauli matrix for y axis `result["y"]`,
+                - Pauli matrix for z axis `result["z"]`.
         """
         assert mult > 1
         result = {}
         if mult == 2:
             result["u"] = np.array([[1, 0], [0, 1]])
             result["p"] = np.array([[0, 1], [0, 0]])
             result["m"] = np.array([[0, 0], [1, 0]])
@@ -178,28 +181,29 @@
             result["y"] = -0.5 * 1j * (result["p"] - result["m"])
             result["z"] = sp.sparse.spdiags(prjs, 0, mult, mult).toarray()
         return result
 
     def spin_operator(self, idx: int, axis: str) -> np.ndarray:
         """Construct the spin operator.
 
+        Construct the spin operator for the particle with index `idx`
+        in the `HilbertSimulation`.
+
         Args:
 
             idx (int): Index of the particle.
 
             axis (str): Axis, i.e. ``"x"``, ``"y"`` or ``"z"``.
 
         Returns:
+            np.ndarray:
 
-            np.ndarray: Spin operator for a particle in the
-            `HilbertSimulation` system with indexing `idx` and axis
-            `axis`.
-
-        Construct the spin operator for the particle with index
-        `idx` in the `HilbertSimulation`.
+                Spin operator for a particle in the
+                `HilbertSimulation` system with indexing `idx` and
+                axis `axis`.
 
         """
         assert 0 <= idx and idx < len(self.particles)
         assert axis in "xyzpmu"
 
         sigma = self.pauli(self.particles[idx].multiplicity)[axis]
         eye_before = np.eye(prod(p.multiplicity for p in self.particles[:idx]))
@@ -207,234 +211,432 @@
 
         spinop = np.kron(np.kron(eye_before, sigma), eye_after)
         if self.basis == Basis.ST:
             return self.ST_basis(spinop)
         else:
             return spinop
 
-    def product_operator(self, idx1: int, idx2: int, h: float = 1) -> np.ndarray:
-        """Projection operator."""
+    def product_operator(self, idx1: int, idx2: int, h: float = 1.0) -> np.ndarray:
+        """Construct the (1D) product operator.
+
+        Construct the 1D (isotropic) product operator of two particles
+        in the spin system.
+
+        Args:
+
+            idx1 (int): Index of the first particle.
+
+            idx2 (int): Index of the second particle.
+
+            h (float): Isotopic interaction constant.
+
+        Returns:
+            np.ndarray:
+
+                Product operator for particles corresponding to `idx1`
+                and `idx2` with isotropic interaction constant `h`.
+
+        """
         return h * sum(
             [
                 self.spin_operator(idx1, axis).dot(self.spin_operator(idx2, axis))
                 for axis in "xyz"
             ]
         )
 
     def product_operator_3d(self, idx1: int, idx2: int, h: np.ndarray) -> np.ndarray:
-        """Projection operator."""
+        """Construct the 3D product operator.
+
+        Construct the 3D (anisotropic) product operator of two
+        particles in the spin system.
+
+        Args:
+
+            idx1 (int): Index of the first particle.
+
+            idx2 (int): Index of the second particle.
+
+            h (np.ndarray): Anisotropic interaction tensor.
+
+        Returns:
+            np.ndarray:
+
+                Product operator for particles corresponding to `idx1`
+                and `idx2` with anisotropic interaction tensor `h`.
+
+        """
         return sum(
-            [
+            (
                 h[i, j]
                 * self.spin_operator(idx1, ax1).dot(self.spin_operator(idx2, ax2))
                 for i, ax1 in enumerate("xyz")
                 for j, ax2 in enumerate("xyz")
-            ]
+            )
         )
 
     def projection_operator(self, state: State):
-        """Construct.
+        """Construct the projection operator corresponding to a `state`.
+
+        Args:
+
+            state (State): The target state which is projected out of
+                the density matrix.
+
+        Returns:
+            np.ndarray:
+
+                Projection operator corresponding to the `State`
+                `state`.
+
+        .. todo:: Write proper docs.
 
-        .. todo::     Write proper docs.
         """
         # Spin operators
         SAx, SAy, SAz = [self.spin_operator(0, ax) for ax in "xyz"]
         SBx, SBy, SBz = [self.spin_operator(1, ax) for ax in "xyz"]
 
         # Product operators
         SASB = self.product_operator(0, 1)
-
         eye = np.eye(len(SASB))
 
-        # Projection operators
-        # todo change p/m to +/-
-        match state:
-            case State.SINGLET:
-                return (1 / 4) * eye - SASB
-            case State.TRIPLET:
-                return (3 / 4) * eye + SASB
-            case State.TRIPLET_PLUS:
-                return (2 * SAz**2 + SAz) * (2 * SBz**2 + SBz)
-            case State.TRIPLET_MINUS:
-                return (2 * SAz**2 - SAz) * (2 * SBz**2 - SBz)
-            case State.TRIPLET_ZERO:
-                return (1 / 4) * eye + SAx @ SBx + SAy @ SBy - SAz @ SBz
-            case State.TRIPLET_PLUS_MINUS:
-                return (2 * SAz**2 + SAz) * (2 * SBz**2 + SBz) + (
-                    2 * SAz**2 - SAz
-                ) * (2 * SBz**2 - SBz)
-            case State.EQUILIBRIUM:
-                return 1.05459e-34 / (1.38e-23 * 298)
+        result = {
+            State.SINGLET: (1 / 4) * eye - SASB,
+            State.TRIPLET: (3 / 4) * eye + SASB,
+            State.TRIPLET_PLUS: (2 * SAz**2 + SAz) * (2 * SBz**2 + SBz),
+            State.TRIPLET_MINUS: (2 * SAz**2 - SAz) * (2 * SBz**2 - SBz),
+            State.TRIPLET_ZERO: (1 / 4) * eye + SAx @ SBx + SAy @ SBy - SAz @ SBz,
+            State.TRIPLET_PLUS_MINUS: (2 * SAz**2 + SAz) * (2 * SBz**2 + SBz)
+            + (2 * SAz**2 - SAz) * (2 * SBz**2 - SBz),
+            State.EQUILIBRIUM: 1.05459e-34 / (1.38e-23 * 298),
+        }
+        return result[state]
 
     def zeeman_hamiltonian(
         self, B0: float, theta: Optional[float] = None, phi: Optional[float] = None
     ) -> np.ndarray:
-        """Construct the Zeeman Hamiltonian.
+        """Construct the Zeeman Hamiltonian (1D or 3D).
 
         Construct the Zeeman Hamiltonian based on the external
-        magnetic field `B`.
+        magnetic field `B0`.  If the angles `theta` and `phi` are also
+        provided, the 3D Zeeman Hamiltonian is constructed (by
+        invoking the `zeeman_hamiltonian_3d`), otherwise the 1D Zeeman
+        Hamiltonian is constructed (by invoking the
+        `zeeman_hamiltonian_1d`).
 
         Args:
 
             B0 (float): External magnetic field intensity (milli
-            Tesla).
+                Tesla). See `zeeman_hamiltonian_1d` and
+                `zeeman_hamiltonian_3d`.
+
+            theta (Optional[float]): rotation (polar) angle between
+                the external magnetic field and the fixed
+                molecule. See `zeeman_hamiltonian_3d`.
+
+            phi (Optional[float]): rotation (azimuth) angle between
+                the external magnetic field and the fixed molecule.
+                See `zeeman_hamiltonian_3d`.
 
         Returns:
-            np.ndarray: The Zeeman Hamiltonian corresponding to the
-            system described by the `Quantum` simulation object and
-            the external magnetic field intensity `B`.
+            np.ndarray:
+
+                The Zeeman Hamiltonian corresponding to the system
+                described by the `HilbertSimulation` object and the
+                external magnetic field intensity `B0` and angles
+                `theta` and `phi`.
+
         """
         if theta is None and phi is None:
             return self.zeeman_hamiltonian_1d(B0)
         else:
             return self.zeeman_hamiltonian_3d(B0, theta, phi)
 
     def zeeman_hamiltonian_1d(self, B0: float) -> np.ndarray:
+        """Construct the 1D Zeeman Hamiltonian.
+
+        Construct the 1D Zeeman Hamiltonian based on the external
+        magnetic field `B0`.
+
+        Args:
+
+            B0 (float): External magnetic field intensity (milli
+                Tesla).
+
+        Returns:
+            np.ndarray:
+
+                The Zeeman Hamiltonian corresponding to the system
+                described by the `HilbertSimulation` object and the
+                external magnetic field intensity `B0`.
+
+        """
         axis = "z"
         gammas = enumerate(p.gamma_mT for p in self.particles)
         return -B0 * sum(g * self.spin_operator(i, axis) for i, g in gammas)
 
     def zeeman_hamiltonian_3d(
-        self, B0: float, theta: float = 0, phi: float = 0
+        self, B0: float, theta: Optional[float] = 0, phi: Optional[float] = 0
     ) -> np.ndarray:
+        """Construct the 3D Zeeman Hamiltonian.
+
+        Construct the 3D Zeeman Hamiltonian based on the external
+        magnetic field `B0` and angles `theta` and `phi`.
+
+        Args:
+
+            B0 (float): External magnetic field intensity (milli
+                Tesla).
+
+            theta (Optional[float]): rotation (polar) angle between
+                the external magnetic field and the fixed
+                molecule.
+
+            phi (Optional[float]): rotation (azimuth) angle between
+                the external magnetic field and the fixed molecule.
+
+        Returns:
+            np.ndarray:
+
+                The Zeeman Hamiltonian corresponding to the system
+                described by the `HilbertSimulation` object and the
+                external magnetic field intensity `B0` and angles
+                `theta` and `phi`.
+
+        """
         particles = np.array(
             [
                 [self.spin_operator(idx, axis) for axis in "xyz"]
                 for idx in range(len(self.particles))
             ]
         )
         rotation = utils.spherical_to_cartesian(theta, phi)
         omega = B0 * self.radicals[0].gamma_mT
         return omega * np.einsum("j,ijkl->kl", rotation, particles)
 
     def hyperfine_hamiltonian(self, hfc_anisotropy: bool = False) -> np.ndarray:
         """Construct the Hyperfine Hamiltonian.
 
-        Construct the Hyperfine Hamiltonian based on the magnetic
-        field.
+        Construct the Hyperfine Hamiltonian.  If `hfc_anisotropy` is
+        `False`, then the isotropic hyperfine coupling constants are
+        used. If `hfc_anisotropy` is `True` then the full hyperfine
+        tensors are used (assuming they are available for all the
+        nuclei of the molecule in the database, otherwise an exception
+        is raised).
+
+        Args:
+
+            hfc_anisotropy (bool): Use isotropic hyperfine coupling
+                constants if `False`, use full hyperfine tensors if
+                `False`.
 
         Returns:
-            np.ndarray: The Hyperfine Hamiltonian corresponding to the
-            system described by the `Quantum` simulation object.
+            np.ndarray:
+
+                The Hyperfine Hamiltonian corresponding to the system
+                described by the `HilbertSimulation` object.
+
         """
         if hfc_anisotropy:
             for h in [n.hfc for n in self.nuclei]:
                 # TODO(vatai) try except not is None
                 if h.anisotropic is None:
                     raise ValueError(
-                        "Not all molecules have anisotropic HFCs! Please use `hfc_anisotropy=False`"
+                        "Not all molecules have anisotropic HFCs! "
+                        "Please use `hfc_anisotropy=False`"
                     )
 
-        if hfc_anisotropy:
             prodop = self.product_operator_3d
             hfcs = [n.hfc.anisotropic for n in self.nuclei]
         else:
             prodop = self.product_operator
             hfcs = [n.hfc.isotropic for n in self.nuclei]
         return sum(
-            [
+            (
                 self.particles[ei].gamma_mT
                 * prodop(ei, len(self.radicals) + ni, hfcs[ni])
                 for ni, ei in enumerate(self.coupling)
-            ]
+            )
         )
 
     def exchange_hamiltonian(self, J: float) -> np.ndarray:
-        """Construct the Exchange Hamiltonian.
+        """Construct the exchange Hamiltonian.
 
-        Construct the Exchange (J-coupling) Hamiltonian based on the
-        coupling constant J between two electrons, which can be obtain
-        from the radical pair separation `r` using `TODO` method.
+        Construct the exchange (J-coupling) Hamiltonian based on the
+        coupling constant J between two electrons.
 
-        .. todo::
-            Write proper docs.
+        The J-coupling constant can be obtained using:
+
+        - `radicalpy.estimations.exchange_interaction_in_protein`
+        - `radicalpy.estimations.exchange_interaction_in_solution`
+
+        Args:
+
+            J (float): Exchange coupling constant.
 
         Returns:
-            np.ndarray: The Exchange (J-coupling) Hamiltonian
-            corresponding to the system described by the `Quantum`
-            simulation object and the coupling constant `J`.
+            np.ndarray:
+
+                The exchange (J-coupling) Hamiltonian corresponding to
+                the system described by the `HilbertSimulation` object
+                and the coupling constant `J`.
+
         """
-        Jcoupling = self.radicals[0].gamma_mT * J
+        Jcoupling = J * self.radicals[0].gamma_mT
         SASB = self.product_operator(0, 1)
-        return Jcoupling * (2 * SASB + 0.5 * np.eye(*SASB.shape))
+        return Jcoupling * (2 * SASB + 0.5 * np.eye(SASB.shape[0]))
 
-    def dipolar_hamiltonian(self, D: float or np.ndarray) -> np.ndarray:
+    def dipolar_hamiltonian(self, D: float | np.ndarray) -> np.ndarray:
         """Construct the Dipolar Hamiltonian.
 
         Construct the Dipolar Hamiltonian based on dipolar coupling
-        constant `D` between two electrons.
+        constant or dipolar interaction tensor `D` between two
+        electrons.  Depending on the `type` of `D`, the 1D or the 3D
+        version is invoked.
+
+        See:
+
+        - `dipolar_hamiltonian_1d`
+        - `dipolar_hamiltonian_3d`
+
+        Args:
 
-        .. todo::
-            Write proper docs.
+            D (float | np.ndarray): dipolar coupling constant or
+                dipolar interaction tensor.
 
         Returns:
-            np.ndarray: The Dipolar Hamiltonian corresponding to the
-            system described by the `Quantum` simulation object and
-            dipolar coupling constant `D`.
+            np.ndarray:
+
+                The Dipolar Hamiltonian corresponding to the system
+                described by the `HilbertSimulation` object and
+                dipolar coupling constant or dipolar interaction
+                tensor `D`.
+
         """
         if isinstance(D, np.ndarray):
             return self.dipolar_hamiltonian_3d(D)
         else:
             return self.dipolar_hamiltonian_1d(D)
 
     def dipolar_hamiltonian_1d(self, D: float) -> np.ndarray:
+        """Construct the 1D Dipolar Hamiltonian.
+
+        Construct the Dipolar Hamiltonian based on dipolar coupling
+        constant `D` between two electrons.
+
+        The dipolar coupling constant can be obtained using
+        `radicalpy.estimations.dipolar_interaction_isotropic`.
+
+        Args:
+
+            D (float): dipolar coupling constant.
+
+        Returns:
+            np.ndarray:
+
+                The 1D Dipolar Hamiltonian corresponding to the system
+                described by the `HilbertSimulation` object and
+                dipolar coupling constant `D`.
+
+        """
         SASB = self.product_operator(0, 1)
         SAz = self.spin_operator(0, "z")
         SBz = self.spin_operator(1, "z")
         omega = (2 / 3) * self.radicals[0].gamma_mT * D
         return omega * (3 * SAz * SBz - SASB)
 
     def dipolar_hamiltonian_3d(self, dipolar_tensor: np.ndarray) -> np.ndarray:
+        """Construct the 3D Dipolar Hamiltonian.
+
+        Construct the Dipolar Hamiltonian based on dipolar interaction
+        tensor `D` between two electrons.
+
+        The dipolar coupling tensor can be obtained using
+        `radicalpy.estimations.dipolar_interaction_anisotropic`.
+
+        Args:
+
+            D (np.ndarray): dipolar interaction tensor.
+
+        Returns:
+            np.ndarray:
+
+                The 3D Dipolar Hamiltonian corresponding to the system
+                described by the `HilbertSimulation` object and
+                dipolar interaction tensor `D`.
+
+        """
         ne = len(self.radicals)
         return -sum(
-            [
+            (
                 -self.radicals[0].gamma_mT
                 * self.product_operator_3d(ei, ne + ni, dipolar_tensor)
                 for ni, ei in enumerate(self.coupling)
-            ]
+            )
         )
 
     def total_hamiltonian(
         self,
-        B: float,
+        B0: float,
         J: float,
-        D: float,
+        D: float | np.ndarray,
         theta: Optional[float] = None,
         phi: Optional[float] = None,
         hfc_anisotropy: bool = False,
     ) -> np.ndarray:
-        """Construct the final (total) Hamiltonian.
+        """Construct the total Hamiltonian.
 
-        Construct the final (total)
+        The total Hamiltonian is the sum of Zeeman, Hyperfine,
+        Exchange and Dipolar Hamiltonian.
+
+        Args:
+
+            B0 (float): See `zeeman_hamiltonian`.
+
+            J (float): See `exchange_hamiltonian`.
+
+            D (float): See `dipolar_hamiltonian`.
+
+            theta (Optional[float]): See `zeeman_hamiltonian`.
+
+            phi (Optional[float]): See `zeeman_hamiltonian`.
+
+            hfc_anisotropy (bool): See `hyperfine_hamiltonian`.
+
+        Returns:
+            np.ndarray:
+
+                The total Hamiltonian.
 
-        .. todo::
-            Write proper docs.
         """
         H = (
-            self.zeeman_hamiltonian(B, theta, phi)
+            self.zeeman_hamiltonian(B0, theta, phi)
             + self.hyperfine_hamiltonian(hfc_anisotropy)
             + self.exchange_hamiltonian(J)
             + self.dipolar_hamiltonian(D)
         )
         return self.convert(H)
 
     def time_evolution(
         self, init_state: State, time: np.ndarray, H: np.ndarray
     ) -> np.ndarray:
         """Evolve the system through time.
 
         Args:
-                init_state (State): blah blah
+            init_state (State): blah blah
 
-                time (np.ndarray): blah blah
+            time (np.ndarray): blah blah
 
-                H (np.ndarray): blah blah
+            H (np.ndarray): blah blah
 
         Returns:
-                np.ndarray: blah blah
+            np.ndarray:
+
+                TODO
+
+        .. todo:: Write proper docs.
         """
         dt = time[1] - time[0]
         propagator = self.unitary_propagator(H, dt)
 
         rho0 = self.initial_density_matrix(init_state, H)
         rhos = np.zeros([len(time), *rho0.shape], dtype=complex)
         rhos[0] = rho0
@@ -475,20 +677,23 @@
         theta: Optional[float] = None,
         phi: Optional[float] = None,
         hfc_anisotropy: bool = False,
     ) -> np.ndarray:
         """Generate density matrices (rhos) for MARY.
 
         Args:
+
             init_state (State): initial state.
+
         Returns:
-            List generator.
+            np.ndarray:
 
-        .. todo::
-            Write proper docs.
+                Density matrices.
+
+        .. todo:: Write proper docs.
         """
         H_zee = self.convert(self.zeeman_hamiltonian(1, theta, phi))
         shape = self._get_rho_shape(H_zee.shape[0])
         rhos = np.zeros([len(B), len(time), *shape], dtype=complex)
         for i, B0 in enumerate(tqdm(B)):
             H = H_base + B0 * H_zee
             H_sparse = sp.sparse.csc_matrix(H)
@@ -530,15 +735,15 @@
         J: float,
         kinetics: list[HilbertIncoherentProcessBase] = [],
         relaxations: list[HilbertIncoherentProcessBase] = [],
         theta: Optional[float] = None,
         phi: Optional[float] = None,
         hfc_anisotropy: bool = False,
     ) -> dict:
-        H = self.total_hamiltonian(B=0, D=D, J=J, hfc_anisotropy=hfc_anisotropy)
+        H = self.total_hamiltonian(B0=0, D=D, J=J, hfc_anisotropy=hfc_anisotropy)
 
         self.apply_liouville_hamiltonian_modifiers(H, kinetics + relaxations)
         rhos = self.mary_loop(init_state, time, B, H, theta=theta, phi=phi)
         product_probabilities = self.product_probability(obs_state, rhos)
 
         self.apply_hilbert_kinetics(time, product_probabilities, kinetics)
         k = kinetics[0].rate_constant if kinetics else 1.0
@@ -566,16 +771,16 @@
 
     def anisotropy_loop(
         self,
         init_state: State,
         time: np.ndarray,
         B: float,
         H_base: np.ndarray,
-        theta: list[float],
-        phi: list[float],
+        theta: float | np.ndarray,
+        phi: float | np.ndarray,
     ):
         shape = self._get_rho_shape(H_base.shape[0])
         rhos = np.zeros((len(theta), len(phi), len(time), *shape), dtype=complex)
 
         iters = itertools.product(enumerate(theta), enumerate(phi))
         for (i, th), (j, ph) in tqdm(list(iters)):
             H_zee = self.zeeman_hamiltonian(B, th, ph)
@@ -584,26 +789,26 @@
         return rhos
 
     def anisotropy(
         self,
         init_state: State,
         obs_state: State,
         time: np.ndarray,
-        theta: list[float] | float,
-        phi: list[float] | float,
+        theta: np.ndarray | float,
+        phi: np.ndarray | float,
         B: float,
         D: np.ndarray,
         J: float,
         kinetics: list[HilbertIncoherentProcessBase] = [],
         relaxations: list[HilbertIncoherentProcessBase] = [],
     ) -> dict:
-        H = self.total_hamiltonian(B=0, D=D, J=J, hfc_anisotropy=True)
+        H = self.total_hamiltonian(B0=0, D=D, J=J, hfc_anisotropy=True)
 
         self.apply_liouville_hamiltonian_modifiers(H, kinetics + relaxations)
-        theta, phi = utils._anisotropy_check(theta, phi)
+        theta, phi = utils.anisotropy_check(theta, phi)
         rhos = self.anisotropy_loop(init_state, time, B, H, theta=theta, phi=phi)
         product_probabilities = self.product_probability(obs_state, rhos)
 
         self.apply_hilbert_kinetics(time, product_probabilities, kinetics)
         k = kinetics[0].rate_constant if kinetics else 1.0
         product_yields, product_yield_sums = self.product_yield(
             product_probabilities, time, k
@@ -633,15 +838,18 @@
 
         Args:
             state (State): Spin state projection operator.
 
             H (np.ndarray): Spin Hamiltonian in Hilbert space.
 
         Returns:
-            np.ndarray: A matrix in Hilbert space representing...
+            np.ndarray:
+
+                A matrix in Hilbert space representing...
+
         """
         Pi = self.projection_operator(state)
 
         if state == State.EQUILIBRIUM:
             rho0eq = sp.sparse.linalg.expm(-1j * sp.sparse.csc_matrix(H) * Pi).toarray()
             rho0 = rho0eq / rho0eq.trace()
         else:
@@ -658,22 +866,28 @@
         Arguments:
 
             H (np.ndarray): Spin Hamiltonian in Hilbert space.
 
             dt (float): Time evolution timestep.
 
         Returns:
-            np.ndarray: Two matrices (a tensor) in either Hilbert.
+            np.ndarray:
+
+                Two matrices (a tensor) in either Hilbert.
 
-        .. todo::
-            https://docs.python.org/3/library/doctest.html
+        Examples:
+
+            >>> molecules = [Molecule.fromdb("flavin_anion", ["N5"]),
+            ...              Molecule("Z")]
+            >>> sim = HilbertSimulation(molecules)
+            >>> H = sim.total_hamiltonian(B0=0, J=0, D=0)
+            >>> Up, Um = sim.unitary_propagator(H, 3e-9)
+            >>> Up.shape, Um.shape
+            ((12, 12), (12, 12))
 
-        Example:
-            >> Up, Um = UnitaryPropagator(H, 3e-9, "Hilbert")
-            >> UL = UnitaryPropagator(HL, 3e-9, "Liouville")
         """
         Up = sp.sparse.linalg.expm(1j * H * dt)
         Um = sp.sparse.linalg.expm(-1j * H * dt)
         return Up, Um
 
     def propagate(self, propagator: np.ndarray, rho: np.ndarray) -> np.ndarray:
         Up, Um = propagator
@@ -729,21 +943,32 @@
         return rho0
 
     @staticmethod
     def unitary_propagator(H, dt):
         """Create unitary propagator.
 
         Create unitary propagator matrices for time evolution of the
-        spin Hamiltonian density matrix in both Hilbert and Liouville
-        space.
+        spin Hamiltonian density matrix in Liouville space.
+
+        Examples:
+
+            >>> molecules = [Molecule.fromdb("flavin_anion", ["N5"]),
+            ...              Molecule("Z")]
+            >>> sim = LiouvilleSimulation(molecules)
+            >>> H = sim.total_hamiltonian(B0=0, J=0, D=0)
+            >>> sim.unitary_propagator(H, 3e-9).shape
+            (144, 144)
 
         Arguments:
-            H (np.ndarray): Spin Hamiltonian in Hilbert or Liouville space
-            dt (float): Time evolution timestep.
-            space (str): Select the spin space.
+            H (np.ndarray):
+
+                Spin Hamiltonian in Hilbert or Liouville space dt
+                (float): Time evolution timestep.  space (str): Select
+                the spin space.
+
         """
         return sp.sparse.linalg.expm(H * dt)
 
     def propagate(self, propagator: np.ndarray, rho: np.ndarray) -> np.ndarray:
         return propagator @ rho
```

### Comparing `radicalpy-0.6.2/radicalpy/utils.py` & `radicalpy-0.6.3/radicalpy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 
     Returns:
             float: Spectral density frequency.
     """
     return tau_c / (1 + omega**2 * tau_c**2)
 
 
-def _anisotropy_check(
+def anisotropy_check(
     theta: float | np.ndarray, phi: float | np.ndarray
 ) -> Tuple[np.ndarray, np.ndarray]:
     if isinstance(theta, float):
         theta = np.array([theta])
     if isinstance(phi, float):
         phi = np.array([phi])
     if theta.min() < 0 or np.pi < theta.max():
@@ -324,15 +324,15 @@
             phi (np.ndarray): The angles phi by which the anisotropic
                 product yields were calculated.
 
     Returns:
             float: The spherical average of the anisotropic product
                 yields.
     """
-    theta, phi = _anisotropy_check(theta, phi)
+    theta, phi = anisotropy_check(theta, phi)
     nth, nph = _check_full_sphere(theta, phi)
 
     wt = 4 * np.ones(nth)
     wt[2:-2:2] = 2
     wt[0] = wt[-1] = 1
 
     wp = 4 * np.ones(nph)
```

### Comparing `radicalpy-0.6.2/radicalpy.egg-info/PKG-INFO` & `radicalpy-0.6.3/radicalpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.6.2
+Version: 0.6.3
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.6.2/radicalpy.egg-info/SOURCES.txt` & `radicalpy-0.6.3/radicalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/tests/test_data.py` & `radicalpy-0.6.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/tests/test_estimations.py` & `radicalpy-0.6.3/tests/test_estimations.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/tests/test_shared.py` & `radicalpy-0.6.3/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.2/tests/test_simulation.py` & `radicalpy-0.6.3/tests/test_simulation.py`

 * *Files identical despite different names*

