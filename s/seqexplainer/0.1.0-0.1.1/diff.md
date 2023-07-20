# Comparing `tmp/seqexplainer-0.1.0.tar.gz` & `tmp/seqexplainer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqexplainer-0.1.0.tar", max compression
+gzip compressed data, was "seqexplainer-0.1.1.tar", max compression
```

## Comparing `seqexplainer-0.1.0.tar` & `seqexplainer-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1066 2023-03-26 17:51:58.000000 seqexplainer-0.1.0/LICENSE
--rw-r--r--   0        0        0     1992 2023-03-26 17:52:14.000000 seqexplainer-0.1.0/README.md
--rw-r--r--   0        0        0      455 2023-06-23 19:43:20.000000 seqexplainer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      211 2023-06-06 17:16:19.000000 seqexplainer-0.1.0/seqexplainer/__init__.py
--rw-r--r--   0        0        0     2529 2023-06-06 16:07:43.000000 seqexplainer-0.1.0/seqexplainer/_ism.py
--rw-r--r--   0        0        0     2815 2023-06-05 00:05:42.000000 seqexplainer-0.1.0/seqexplainer/_layer_outs.py
--rw-r--r--   0        0        0     3959 2023-06-03 00:23:20.000000 seqexplainer-0.1.0/seqexplainer/_plot.py
--rw-r--r--   0        0        0     4628 2023-06-04 23:37:23.000000 seqexplainer-0.1.0/seqexplainer/_utils.py
--rw-r--r--   0        0        0       75 2023-06-03 00:40:39.000000 seqexplainer-0.1.0/seqexplainer/attributions/__init__.py
--rw-r--r--   0        0        0     3443 2023-06-06 17:00:58.000000 seqexplainer-0.1.0/seqexplainer/attributions/_attributions.py
--rw-r--r--   0        0        0     7568 2023-06-03 00:23:20.000000 seqexplainer-0.1.0/seqexplainer/attributions/_modisco.py
--rw-r--r--   0        0        0    10017 2023-06-03 00:45:03.000000 seqexplainer-0.1.0/seqexplainer/attributions/_references.py
--rw-r--r--   0        0        0     4242 2023-06-03 00:23:20.000000 seqexplainer-0.1.0/seqexplainer/deprecated/_deprecated.py
--rw-r--r--   0        0        0    11640 2023-03-26 19:16:55.000000 seqexplainer-0.1.0/seqexplainer/experimental/_experimental.py
--rw-r--r--   0        0        0       84 2023-06-07 00:01:45.000000 seqexplainer-0.1.0/seqexplainer/filters/__init__.py
--rw-r--r--   0        0        0     3246 2023-06-08 22:08:16.000000 seqexplainer-0.1.0/seqexplainer/filters/_filters.py
--rw-r--r--   0        0        0     1892 2023-06-03 00:40:56.000000 seqexplainer-0.1.0/seqexplainer/filters/_motifs.py
--rw-r--r--   0        0        0       33 2023-06-06 05:20:04.000000 seqexplainer-0.1.0/seqexplainer/generative/__init__.py
--rw-r--r--   0        0        0     6155 2023-06-06 17:00:53.000000 seqexplainer-0.1.0/seqexplainer/generative/_evolution.py
--rw-r--r--   0        0        0       39 2023-06-06 17:09:25.000000 seqexplainer-0.1.0/seqexplainer/gia/__init__.py
--rw-r--r--   0        0        0     5178 2023-06-22 20:45:23.000000 seqexplainer-0.1.0/seqexplainer/gia/_complex_perturb.py
--rw-r--r--   0        0        0     3971 2023-06-22 17:36:55.000000 seqexplainer-0.1.0/seqexplainer/gia/_gia.py
--rw-r--r--   0        0        0        0 2023-06-22 17:08:33.000000 seqexplainer-0.1.0/seqexplainer/gia/_gia_helpers.py
--rw-r--r--   0        0        0     2459 2023-06-03 00:41:26.000000 seqexplainer-0.1.0/seqexplainer/gia/_null_models.py
--rw-r--r--   0        0        0    16623 2023-06-22 17:08:05.000000 seqexplainer-0.1.0/seqexplainer/gia/_perturb.py
--rw-r--r--   0        0        0     9445 2023-06-03 00:38:33.000000 seqexplainer-0.1.0/seqexplainer/preprocess/_helpers.py
--rw-r--r--   0        0        0    13895 2023-06-03 00:38:34.000000 seqexplainer-0.1.0/seqexplainer/preprocess/_preprocess.py
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 seqexplainer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-03-26 17:51:58.000000 seqexplainer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1992 2023-03-26 17:52:14.000000 seqexplainer-0.1.1/README.md
+-rw-r--r--   0        0        0      457 2023-07-20 19:48:33.000000 seqexplainer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/__init__.py
+-rw-r--r--   0        0        0     2959 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/_ism.py
+-rw-r--r--   0        0        0     2815 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/_layer_outs.py
+-rw-r--r--   0        0        0     4628 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/_utils.py
+-rw-r--r--   0        0        0       75 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/__init__.py
+-rw-r--r--   0        0        0     3732 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/_attributions.py
+-rw-r--r--   0        0        0     7568 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/_modisco.py
+-rw-r--r--   0        0        0     3943 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/_plot.py
+-rw-r--r--   0        0        0    11133 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/_references.py
+-rw-r--r--   0        0        0     4242 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/deprecated/_deprecated.py
+-rw-r--r--   0        0        0    12072 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/experimental/_experimental.py
+-rw-r--r--   0        0        0      180 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/__init__.py
+-rw-r--r--   0        0        0     3244 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/_activations.py
+-rw-r--r--   0        0        0      914 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/_annotate.py
+-rw-r--r--   0        0        0     1912 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/_motifs.py
+-rw-r--r--   0        0        0     1457 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/_plot.py
+-rw-r--r--   0        0        0       33 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/generative/__init__.py
+-rw-r--r--   0        0        0     6155 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/generative/_evolution.py
+-rw-r--r--   0        0        0       39 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/__init__.py
+-rw-r--r--   0        0        0     5178 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_complex_perturb.py
+-rw-r--r--   0        0        0     3971 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_gia.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_gia_helpers.py
+-rw-r--r--   0        0        0     2459 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_null_models.py
+-rw-r--r--   0        0        0    16623 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_perturb.py
+-rw-r--r--   0        0        0     9445 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/preprocess/_helpers.py
+-rw-r--r--   0        0        0    13895 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/preprocess/_preprocess.py
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 seqexplainer-0.1.1/PKG-INFO
```

### Comparing `seqexplainer-0.1.0/LICENSE` & `seqexplainer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/README.md` & `seqexplainer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/_ism.py` & `seqexplainer-0.1.1/seqexplainer/_ism.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,28 +44,40 @@
     X_idxs = inputs.argmax(axis=1)
 
     # If target not provided aggregate over all outputs
     target = np.arange(model.output_dim) if target is None else target
     
     # Get the reference output
     _model_to_device(model, device)
-    reference = model.predict(inputs, batch_size=batch_size, verbose=False)[:, target].unsqueeze(dim=1).cpu()
+    ref_batch_starts = np.arange(0, N, batch_size)
+    reference = []
+    for start in ref_batch_starts:
+        inputs_ = inputs[start : start + batch_size]
+        with torch.no_grad():
+            reference_ = model(inputs_)[:, target].unsqueeze(dim=1).cpu()
+        reference.append(reference_)
+        del inputs_, reference_
+        if device[:4] == 'cuda':
+            torch.cuda.synchronize()
+            torch.cuda.empty_cache()
+    #reference = model.predict(inputs, batch_size=batch_size, verbose=False)[:, target].unsqueeze(dim=1).cpu()
+    reference = torch.cat(reference)
 
     # Get the batch starts
     batch_starts = np.arange(0, n, batch_size)
 
     # Get the change in output for each perturbation
     isms = []
     for i in range(N):
         X = perturb_seq_torch(inputs[i])
         y = []
         for start in batch_starts:
             X_ = X[start : start + batch_size]
             with torch.no_grad():
-                y_ = model.predict(X_, batch_size=batch_size, verbose=False)[:, target].unsqueeze(dim=1).cpu()
+                y_ = model(X_)[:, target].unsqueeze(dim=1).cpu()
             y.append(y_)
             del X_, y_
             if device[:4] == 'cuda':
                 torch.cuda.synchronize()
                 torch.cuda.empty_cache()
         y = torch.cat(y)
         ism = DIFF_REGISTRY[diff_type](y, reference[i]).cpu()
```

### Comparing `seqexplainer-0.1.0/seqexplainer/_layer_outs.py` & `seqexplainer-0.1.1/seqexplainer/_layer_outs.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/_utils.py` & `seqexplainer-0.1.1/seqexplainer/_utils.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/attributions/_attributions.py` & `seqexplainer-0.1.1/seqexplainer/attributions/_attributions.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,19 @@
     one_hot,
     hypothetical_contribs,
 ):
     contr = one_hot * hypothetical_contribs
     oned_contr = contr.sum(axis=1)
     return oned_contr
 
-def _gradient_correction(
+def gradient_correction(
     grad: np.ndarray,
 ):
     grad -= np.mean(grad, axis=1, keepdims=True)
+    return grad
 
 
 ISM_REGISTRY = {
     "NaiveISM": _naive_ism,
 }
 
 def _ism_attributions(
@@ -72,20 +73,21 @@
     "GradientShap": _captum_attributions,
     "DeepLiftShap": _captum_attributions,
 }
 
 def attribute(
     model,
     inputs: torch.Tensor,
-    method: Union[str, Callable],
-    reference_type: str = None,
+    method: Union[str, Callable], 
+    references: Union[str, np.ndarray] = None,
     target: int = 0,
     batch_size: int = 128,
     device: str = "cpu",
     verbose: bool = True,
+    **kwargs
 ):
     # Disable cudnn for faster computations 
     torch.backends.cudnn.enabled = False
     
     # Put model on device
     model = _model_to_device(model, device)
 
@@ -98,23 +100,28 @@
         enumerate(starts),
         total=len(starts),
         desc=f"Computing attributions on batches of size {batch_size}",
         disable=not verbose,
     ):
         # Grab the current batch
         inputs_ = inputs[start : start + batch_size]
-        inputs_ = inputs_.requires_grad_(True).to(device)
         
         # Add reference if needed
         kwargs = {}
-        if reference_type is not None:
-            refs = get_reference(inputs_, reference_type)
-            refs = torch.tensor(refs, dtype=torch.float32).requires_grad_(True).to(device)
+        if references is not None:
+            if isinstance(references, str):
+                refs = get_reference(inputs_, references)
+                refs = torch.tensor(refs, dtype=torch.float32).requires_grad_(True).to(device)
+            else:
+                refs = torch.tensor(references, dtype=torch.float32).requires_grad_(True).to(device)
             kwargs["baselines"] = refs
 
+        # Convert to tensor and put on device
+        inputs_ = torch.tensor(inputs_, dtype=torch.float32).requires_grad_(True).to(device)
+
         # Get attributions and append
         curr_attrs = ATTRIBUTIONS_REGISTRY[method](
             model=model,
             inputs=inputs_,
             method=method,
             target=target,
             device=device,
```

### Comparing `seqexplainer-0.1.0/seqexplainer/attributions/_modisco.py` & `seqexplainer-0.1.1/seqexplainer/attributions/_modisco.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/attributions/_references.py` & `seqexplainer-0.1.1/seqexplainer/attributions/_references.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Callable, List, Tuple, Union
 import numpy as np
 from numpy.typing import NDArray
 from ..preprocess._preprocess import dinuc_shuffle_seqs
+import seqpro as sp
 
 
 def zero_ref_inputs(
     inputs: NDArray
 ) -> NDArray:
     """Return a NumPy array of zeros with the same shape as the inputs.
 
@@ -107,21 +108,51 @@
     refs : NDArray
         A NumPy array of dinucleotide shuffled sequences with the same shape as inputs.
 
     Note
     ----
     This function is a wrapper for the dinuc_shuffle_seqs function from the seqpro package and currently only works with numpy arrays.
     """
-    refs = kshuffle(inputs, **kwargs)
+    refs = dinuc_shuffle_seqs(inputs)
+    return refs
+
+def k_shuffle_ref_inputs(
+    inputs: NDArray,
+    k: int = 2,
+    alphabet: str = "DNA",
+    **kwargs
+) -> NDArray:
+    """Return a NumPy array of dinucleotide shuffled inputs with the same shape as the inputs.
+
+    Inputs are expected to be one-hot encoded sequences with shape (N, A, L)
+    where N is the number of sequences, A is the number of nucleotides, and L is the length of the sequences.
+    
+    Parameters
+    ----------
+    inputs : NDArray
+        The input sequences to be used to generate a set of dinucleotide shuffled reference sequences.
+    **kwargs
+        Additional keyword arguments to pass to the dinuc_shuffle_seqs function from the seqpro package.
+
+    Returns
+    -------
+    refs : NDArray
+        A NumPy array of dinucleotide shuffled sequences with the same shape as inputs.
+
+    Note
+    ----
+    This function is a wrapper for the dinuc_shuffle_seqs function from the seqpro package and currently only works with numpy arrays.
+    """
+    refs = sp.k_shuffle(inputs, k=k, alphabet=alphabet, **kwargs)
     return refs
 
 def gc_ref_inputs(
     inputs: NDArray,
     bg: str = "uniform",
-    uniform_dist: List[float] = [0.25, 0.25, 0.25, 0.25]
+    uniform_dist: List[float] = [0.3, 0.2, 0.3, 0.2]
 ) -> NDArray:
     """Return a NumPy array with the same GC content and shape as the inputs.
     
     Inputs are expected to be one-hot encoded sequences with shape (N, A, L)
     where N is the number of sequences, A is the number of nucleotides, and L is the length of the sequences.
 
     Parameters
@@ -203,14 +234,15 @@
     return refs 
     
 REFERENCE_REGISTRY = {
     "zero": zero_ref_inputs,
     "random": random_ref_inputs,
     "shuffle": shuffle_ref_inputs,
     "dinuc_shuffle": dinuc_shuffle_ref_inputs,
+    #TODO: "k_shuffle": k_shuffle_ref_inputs,
     "gc": gc_ref_inputs,
     "profile": profile_ref_inputs,
 }
 
 def get_reference(
     inputs: Union[NDArray, Tuple[NDArray]],
     method: Union[str, Callable],
```

### Comparing `seqexplainer-0.1.0/seqexplainer/deprecated/_deprecated.py` & `seqexplainer-0.1.1/seqexplainer/deprecated/_deprecated.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/experimental/_experimental.py` & `seqexplainer-0.1.1/seqexplainer/experimental/_experimental.py`

 * *Files 3% similar despite different names*

```diff
@@ -345,8 +345,24 @@
     """
     if normal:
         z = torch.Tensor(np.random.normal(0, 1, (num_seqs, generator.latent_dim)))
     else: 
         z = torch.rand(num_seqs, generator.latent_dim)
     z = z.to(device)
     fake = generator(z)
-    return seqs_from_tensor(fake.cpu(), num_seqs)
+    return seqs_from_tensor(fake.cpu(), num_seqs)
+
+def umap_plot(umap_data, umap1=0, umap2=1, color="b", loadings=None, labels=None, n=5):
+    xs = umap_data[:, umap1]
+    ys = umap_data[:, umap2]
+    scalex = 1.0 / (xs.max() - xs.min())
+    scaley = 1.0 / (ys.max() - ys.min())
+    ax = plt.scatter(xs * scalex, ys * scaley, c=color)
+    plt.xlim(-1, 1)
+    plt.ylim(-1, 1)
+    plt.xlabel("UMAP{}".format(1))
+    plt.ylabel("UMAP{}".format(2))
+    plt.show()
+    return ax
+    
+
+
```

### Comparing `seqexplainer-0.1.0/seqexplainer/filters/_filters.py` & `seqexplainer-0.1.1/seqexplainer/filters/_activations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
 import pandas as pd
 from tqdm.auto import tqdm
-
 from .._utils import _k_largest_index_argsort
-
 TINY = np.finfo(float).tiny
 
 def get_activators_n_seqlets(
     activations,
     sequences,
     kernel_size,
     padding=0,
```

### Comparing `seqexplainer-0.1.0/seqexplainer/filters/_motifs.py` & `seqexplainer-0.1.1/seqexplainer/filters/_motifs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ..preprocess._helpers import _get_vocab
 import numpy as np
+import pandas as pd
 TINY = np.finfo(float).tiny
 
 def pfm_to_df(
     pfm,
     vocab: str = "DNA",
 ):
     vocab = _get_vocab(vocab)
```

### Comparing `seqexplainer-0.1.0/seqexplainer/generative/_evolution.py` & `seqexplainer-0.1.1/seqexplainer/generative/_evolution.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/gia/_complex_perturb.py` & `seqexplainer-0.1.1/seqexplainer/gia/_complex_perturb.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/gia/_gia.py` & `seqexplainer-0.1.1/seqexplainer/gia/_gia.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/gia/_null_models.py` & `seqexplainer-0.1.1/seqexplainer/gia/_null_models.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/gia/_perturb.py` & `seqexplainer-0.1.1/seqexplainer/gia/_perturb.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/preprocess/_helpers.py` & `seqexplainer-0.1.1/seqexplainer/preprocess/_helpers.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/seqexplainer/preprocess/_preprocess.py` & `seqexplainer-0.1.1/seqexplainer/preprocess/_preprocess.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.0/PKG-INFO` & `seqexplainer-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: seqexplainer
-Version: 0.1.0
-Summary: nterpreting sequence-to-function machine learning models
+Version: 0.1.1
+Summary: Interpreting sequence-to-function machine learning models
 Author: adamklie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: captum (==0.5)
 Requires-Dist: logomaker (>=0.8,<0.9)
 Requires-Dist: modisco-lite (>=2.2.0,<3.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
-Requires-Dist: torch (>=1.12.0,<2.0.0)
+Requires-Dist: torch (>=1.12.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: yuzu-ism (>=0.0.1,<0.0.2)
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/seqexplainer.svg)](https://badge.fury.io/py/seqexplainer)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/seqexplainer)
```

