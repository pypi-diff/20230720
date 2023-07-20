# Comparing `tmp/chex-0.1.81.tar.gz` & `tmp/chex-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chex-0.1.81.tar", last modified: Thu Jun 29 10:59:31 2023, max compression
+gzip compressed data, was "chex-0.1.82.tar", last modified: Thu Jul 20 10:24:24 2023, max compression
```

## Comparing `chex-0.1.81.tar` & `chex-0.1.82.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.849064 chex-0.1.81/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-29 10:59:21.000000 chex-0.1.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 10:59:21.000000 chex-0.1.81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-06-29 10:59:31.849064 chex-0.1.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-06-29 10:59:21.000000 chex-0.1.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.841064 chex-0.1.81/chex/
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-29 10:59:21.000000 chex-0.1.81/chex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.849064 chex-0.1.81/chex/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64909 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_chexify.py
--rw-r--r--   0 runner    (1001) docker     (123)    23171 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_chexify_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_internal_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    73097 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/dataclass_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/dimensions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/fake_set_n_cpu_devices_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/pytypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/restrict_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/restrict_backends_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20448 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/variants_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-29 10:59:21.000000 chex-0.1.81/chex/chex_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:21.000000 chex-0.1.81/chex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.841064 chex-0.1.81/chex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.849064 chex-0.1.81/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 10:59:21.000000 chex-0.1.81/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 10:59:21.000000 chex-0.1.81/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 10:59:21.000000 chex-0.1.81/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:59:31.849064 chex-0.1.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-29 10:59:21.000000 chex-0.1.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:24:24.935601 chex-0.1.82/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 10:24:02.000000 chex-0.1.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 10:24:02.000000 chex-0.1.82/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-07-20 10:24:24.935601 chex-0.1.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-07-20 10:24:02.000000 chex-0.1.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:24:24.931601 chex-0.1.82/chex/
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-07-20 10:24:02.000000 chex-0.1.82/chex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:24:24.931601 chex-0.1.82/chex/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64245 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/asserts_chexify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23171 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/asserts_chexify_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/asserts_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/asserts_internal_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68914 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/asserts_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22591 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/dataclass_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/dimensions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/fake_set_n_cpu_devices_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/restrict_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/restrict_backends_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20448 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-07-20 10:24:02.000000 chex-0.1.82/chex/_src/variants_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-20 10:24:02.000000 chex-0.1.82/chex/chex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:24:02.000000 chex-0.1.82/chex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:24:24.931601 chex-0.1.82/chex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-07-20 10:24:24.000000 chex-0.1.82/chex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-20 10:24:24.000000 chex-0.1.82/chex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:24:24.000000 chex-0.1.82/chex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:24:24.000000 chex-0.1.82/chex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 10:24:24.000000 chex-0.1.82/chex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 10:24:24.000000 chex-0.1.82/chex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:24:24.935601 chex-0.1.82/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-20 10:24:02.000000 chex-0.1.82/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 10:24:02.000000 chex-0.1.82/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 10:24:02.000000 chex-0.1.82/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:24:24.935601 chex-0.1.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-20 10:24:02.000000 chex-0.1.82/setup.py
```

### Comparing `chex-0.1.81/LICENSE` & `chex-0.1.82/LICENSE`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/PKG-INFO` & `chex-0.1.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chex
-Version: 0.1.81
+Version: 0.1.82
 Summary: Chex: Testing made fun, in JAX!
 Home-page: https://github.com/deepmind/chex
 Author: DeepMind
 Author-email: chex-dev@google.com
 License: Apache 2.0
 Keywords: jax testing debugging python machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chex-0.1.81/README.md` & `chex-0.1.82/README.md`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/__init__.py` & `chex-0.1.82/chex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 from chex._src.variants import all_variants
 from chex._src.variants import ChexVariantType
 from chex._src.variants import params_product
 from chex._src.variants import TestCase
 from chex._src.variants import variants
 
 
-__version__ = "0.1.81"
+__version__ = "0.1.82"
 
 __all__ = (
     "all_variants",
     "Array",
     "ArrayBatched",
     "ArrayDevice",
     "ArrayDeviceTree",
```

### Comparing `chex-0.1.81/chex/_src/__init__.py` & `chex-0.1.82/chex/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/asserts.py` & `chex-0.1.82/chex/_src/asserts.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,32 +19,39 @@
 import functools
 import inspect
 import traceback
 from typing import Any, Callable, List, Optional, Sequence, Set, Type, Union, cast
 import unittest
 from unittest import mock
 
+from absl import logging
 from chex._src import asserts_internal as _ai
 from chex._src import pytypes
 import jax
 from jax.experimental import checkify
 import jax.numpy as jnp
 import jax.test_util as jax_test
 import numpy as np
-import tree as dm_tree
 
 Scalar = pytypes.Scalar
 Array = pytypes.Array
 ArrayTree = pytypes.ArrayTree
 
 _value_assertion = _ai.chex_assertion
 _static_assertion = functools.partial(
     _ai.chex_assertion, jittable_assert_fn=None)
 
 
+def _ignore_nones_deprecation() -> None:
+  logging.warning(
+      "`ignore_nones` argument is non-functional since v0.1.82 and will be"
+      " removed in the next version, please update your usages."
+  )
+
+
 def disable_asserts() -> None:
   """Disables all Chex assertions.
 
   Use wisely.
   """
   _ai.DISABLE_ASSERTIONS = True
 
@@ -418,15 +425,15 @@
 
   if isinstance(expected_sizes, int):
     expected_sizes = [expected_sizes] * len(inputs)
 
   if not isinstance(expected_sizes, (list, tuple)):
     raise AssertionError(
         "Error in size compatibility check: expected sizes should be an int, "
-        f"list, or tuple of ints, got {expected_sizes}.")  
+        f"list, or tuple of ints, got {expected_sizes}.")
 
   if len(inputs) != len(expected_sizes):
     raise AssertionError(
         "Length of `inputs` and `expected_sizes` must match: "
         f"{len(inputs)} is not equal to {len(expected_sizes)}.")
 
   errors = []
@@ -1005,54 +1012,54 @@
 
   Args:
     tree: A tree to assert.
 
   Raises:
     AssertionError: If the tree contains at least one `None`.
   """
-  errors = []
+  has_nones = False
 
-  def _assert_fn(path, leaf):
-    if leaf is None:
-      nonlocal errors
-      errors.append(f"`None` detected at '{_ai.format_tree_path(path)}'.")
+  def _is_leaf(value):
+    if value is None:
+      nonlocal has_nones
+      has_nones = True
+    return False
 
-  for path, leaf in dm_tree.flatten_with_path(tree):
-    _assert_fn(path, leaf)
-  if errors:
-    raise AssertionError("\n".join(errors))
+  treedef = jax.tree_util.tree_structure(tree, is_leaf=_is_leaf)
+  if has_nones:
+    raise AssertionError(f"Tree contains `None`(s): {treedef}.")
 
 
 @_static_assertion
 def assert_tree_has_only_ndarrays(tree: ArrayTree,
                                   *,
                                   ignore_nones: bool = False) -> None:
   """Checks that all `tree`'s leaves are n-dimensional arrays (tensors).
 
   Args:
     tree: A tree to assert.
-    ignore_nones: Whether to ignore `None` in the tree.
+    ignore_nones: Deprecated.
 
   Raises:
     AssertionError: If the tree contains an object which is not an ndarray.
   """
-  if not ignore_nones:
-    assert_tree_no_nones(tree)
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   errors = []
 
   def _assert_fn(path, leaf):
     if leaf is not None:
       if not isinstance(leaf, (np.ndarray, jnp.ndarray)):
         nonlocal errors
         errors.append((f"Tree leaf '{_ai.format_tree_path(path)}' is not an "
                        f"ndarray (type={type(leaf)})."))
 
-  for path, leaf in dm_tree.flatten_with_path(tree):
-    _assert_fn(path, leaf)
+  for path, leaf in jax.tree_util.tree_flatten_with_path(tree)[0]:
+    _assert_fn(_ai.convert_jax_path_to_dm_path(path), leaf)
   if errors:
     raise AssertionError("\n".join(errors))
 
 
 # Only look the sharding attribute after jax version >= 0.3.22 i.e. remove this
 # function and use `isinstance(x.sharding, jax.sharding.PmapSharding)` after
 # jax version >= 0.3.22.
@@ -1086,21 +1093,24 @@
 
   Args:
     tree: A tree to assert.
     allow_cpu_device: Whether to allow JAX arrays that reside on a CPU device.
     allow_sharded_arrays: Whether to allow sharded JAX arrays. Sharded arrays
       are considered "on host" only if they are sharded across CPU devices and
       `allow_cpu_device` is `True`.
-    ignore_nones: Whether to ignore `None` in the tree.
+    ignore_nones: Deprecated.
 
   Raises:
     AssertionError: If the tree contains a leaf that is not an ndarray or does
       not reside on host.
   """
-  assert_tree_has_only_ndarrays(tree, ignore_nones=ignore_nones)
+  if ignore_nones:
+    _ignore_nones_deprecation()
+
+  assert_tree_has_only_ndarrays(tree)
   errors = []
 
   def _assert_fn(path, leaf):
     if leaf is not None:
       if not isinstance(leaf, np.ndarray):
         nonlocal errors
 
@@ -1135,16 +1145,16 @@
             errors.append((f"Tree leaf '{_ai.format_tree_path(path)}' resides "
                            f"on {leaf.device()} (CPU devices are disallowed)."))
         else:
           # Not a jax.Array.
           errors.append((f"Tree leaf '{_ai.format_tree_path(path)}' has "
                          f"unexpected type: {type(leaf)}."))
 
-  for path, leaf in dm_tree.flatten_with_path(tree):
-    _assert_fn(path, leaf)
+  for path, leaf in jax.tree_util.tree_flatten_with_path(tree)[0]:
+    _assert_fn(_ai.convert_jax_path_to_dm_path(path), leaf)
   if errors:
     raise AssertionError("\n".join(errors))
 
 
 @_static_assertion
 def assert_tree_is_on_device(tree: ArrayTree,
                              *,
@@ -1158,21 +1168,24 @@
 
   Args:
     tree: A tree to assert.
     platform: A platform or a list of platforms where the leaves are expected to
       reside. Ignored if `device` is specified.
     device: An optional device where the tree's arrays are expected to reside.
       Any device (except CPU) is accepted if not specified.
-    ignore_nones: Whether to ignore `None` in the tree.
+    ignore_nones: Deprecated.
 
   Raises:
     AssertionError: If the tree contains a leaf that is not an ndarray or does
       not reside on the specified device or platform.
   """
-  assert_tree_has_only_ndarrays(tree, ignore_nones=ignore_nones)
+  if ignore_nones:
+    _ignore_nones_deprecation()
+
+  assert_tree_has_only_ndarrays(tree)
 
   # If device is specified, require its platform.
   if device is not None:
     platform = (device.platform,)
   elif not isinstance(platform, collections.abc.Sequence):
     platform = (platform,)
 
@@ -1200,16 +1213,16 @@
             errors.append(
                 (f"Tree leaf '{_ai.format_tree_path(path)}' resides on "
                  f"{leaf.device()}, expected {device}."))
       else:
         errors.append((f"Tree leaf '{_ai.format_tree_path(path)}' has "
                        f"unexpected type: {type(leaf)}."))
 
-  for path, leaf in dm_tree.flatten_with_path(tree):
-    _assert_fn(path, leaf)
+  for path, leaf in jax.tree_util.tree_flatten_with_path(tree)[0]:
+    _assert_fn(_ai.convert_jax_path_to_dm_path(path), leaf)
   if errors:
     raise AssertionError("\n".join(errors))
 
 
 @_static_assertion
 def assert_tree_is_sharded(tree: ArrayTree,
                            *,
@@ -1217,21 +1230,24 @@
                            ignore_nones: bool = False) -> None:
   """Checks that all leaves are ndarrays sharded across the specified devices.
 
   Args:
     tree: A tree to assert.
     devices: A list of devices which the tree's leaves are expected to be
       sharded across. This list is order-sensitive.
-    ignore_nones: Whether to ignore `None` in the tree.
+    ignore_nones: Deprecated.
 
   Raises:
     AssertionError: If the tree contains a leaf that is not a device array
       sharded across the specified devices.
   """
-  assert_tree_has_only_ndarrays(tree, ignore_nones=ignore_nones)
+  if ignore_nones:
+    _ignore_nones_deprecation()
+
+  assert_tree_has_only_ndarrays(tree)
 
   errors = []
   devices = tuple(devices)
 
   def _assert_fn(path, leaf):
     if leaf is not None:
       nonlocal errors
@@ -1252,51 +1268,47 @@
           )
       else:
         errors.append(
             f"Tree leaf '{_ai.format_tree_path(path)}' is not a "
             f"jax.Array (type={type(leaf)})."
         )
 
-  for path, leaf in dm_tree.flatten_with_path(tree):
-    _assert_fn(path, leaf)
+  for path, leaf in jax.tree_util.tree_flatten_with_path(tree)[0]:
+    _assert_fn(_ai.convert_jax_path_to_dm_path(path), leaf)
   if errors:
     raise AssertionError("\n".join(errors))
 
 
 @_static_assertion
 def assert_tree_shape_prefix(tree: ArrayTree,
                              shape_prefix: Sequence[int],
                              *,
                              ignore_nones: bool = False) -> None:
   """Checks that all ``tree`` leaves' shapes have the same prefix.
 
   Args:
     tree: A tree to check.
     shape_prefix: An expected shape prefix.
-    ignore_nones: Whether to ignore `None` in the tree.
+    ignore_nones: Deprecated.
 
   Raises:
-    AssertionError: If some leaf's shape doesn't start with ``shape_prefix``;
-      if ``ignore_nones`` isn't set and the tree contains `None`.
+    AssertionError: If some leaf's shape doesn't start with ``shape_prefix``.
   """
-  if not ignore_nones:
-    assert_tree_no_nones(tree)
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   # To compare with the leaf's `shape`, convert int sequence to tuple.
   shape_prefix = tuple(shape_prefix)
 
   if not shape_prefix:
     return  # No prefix, this is trivially true.
 
   errors = []
 
   def _assert_fn(path, leaf):
-    if leaf is None:
-      return
-
     nonlocal errors
     if len(shape_prefix) > len(leaf.shape):
       errors.append(
           (f"Tree leaf '{_ai.format_tree_path(path)}' has a shape "
            f"of length {leaf.ndim} (shape={leaf.shape}) which is smaller "
            f"than the expected prefix of length {len(shape_prefix)} "
            f"(prefix={shape_prefix})."))
@@ -1304,51 +1316,47 @@
 
     suffix = leaf.shape[:len(shape_prefix)]
     if suffix != shape_prefix:
       errors.append(
           (f"Tree leaf '{_ai.format_tree_path(path)}' has a shape prefix "
            f"different from expected: {suffix} != {shape_prefix}."))
 
-  for path, leaf in dm_tree.flatten_with_path(tree):
-    _assert_fn(path, leaf)
+  for path, leaf in jax.tree_util.tree_flatten_with_path(tree)[0]:
+    _assert_fn(_ai.convert_jax_path_to_dm_path(path), leaf)
   if errors:
     raise AssertionError("\n".join(errors))
 
 
 @_static_assertion
 def assert_tree_shape_suffix(tree: ArrayTree,
                              shape_suffix: Sequence[int],
                              *,
                              ignore_nones: bool = False) -> None:
   """Checks that all ``tree`` leaves' shapes have the same suffix.
 
   Args:
     tree: A tree to check.
     shape_suffix: An expected shape suffix.
-    ignore_nones: Whether to ignore `None` in the tree.
+    ignore_nones: Deprecated.
 
   Raises:
-    AssertionError: If some leaf's shape doesn't start with ``shape_suffix``;
-      if ``ignore_nones`` isn't set and the tree contains `None`.
+    AssertionError: If some leaf's shape doesn't start with ``shape_suffix``.
   """
-  if not ignore_nones:
-    assert_tree_no_nones(tree)
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   # To compare with the leaf's `shape`, convert int sequence to tuple.
   shape_suffix = tuple(shape_suffix)
 
   if not shape_suffix:
     return  # No suffix, this is trivially true.
 
   errors = []
 
   def _assert_fn(path, leaf):
-    if leaf is None:
-      return
-
     nonlocal errors
     if len(shape_suffix) > len(leaf.shape):
       errors.append(
           (f"Tree leaf '{_ai.format_tree_path(path)}' has a shape "
            f"of length {len(leaf.shape)} (shape={leaf.shape}) which is smaller "
            f"than the expected suffix of length {len(shape_suffix)} "
            f"(suffix={shape_suffix})."))
@@ -1356,26 +1364,24 @@
 
     suffix = leaf.shape[-len(shape_suffix):]
     if suffix != shape_suffix:
       errors.append(
           (f"Tree leaf '{_ai.format_tree_path(path)}' has a shape suffix "
            f"different from expected: {suffix} != {shape_suffix}."))
 
-  for path, leaf in dm_tree.flatten_with_path(tree):
-    _assert_fn(path, leaf)
+  for path, leaf in jax.tree_util.tree_flatten_with_path(tree)[0]:
+    _assert_fn(_ai.convert_jax_path_to_dm_path(path), leaf)
   if errors:
     raise AssertionError("\n".join(errors))
 
 
 @_static_assertion
 def assert_trees_all_equal_structs(*trees: ArrayTree) -> None:
   """Checks that trees have the same structure.
 
-  Note that `None` is treated as a PyTree node.
-
   Args:
     *trees: A sequence of (at least 2) trees to assert equal structure between.
 
   Raises:
     ValueError: If ``trees`` does not contain at least 2 elements.
     AssertionError: If structures of any two trees are different.
   """
@@ -1411,54 +1417,47 @@
   Args:
     equality_comparator: A custom function that accepts two leaves and checks
       whether they are equal. Expected to be transitive.
     error_msg_fn: A function accepting two unequal as per
       ``equality_comparator`` leaves and returning an error message.
     *trees: A sequence of (at least 2) trees to check on equality as per
       ``equality_comparator``.
-    ignore_nones: Whether to ignore `None` in the trees.
+    ignore_nones: Deprecated.
 
   Raises:
     ValueError: If ``trees`` does not contain at least 2 elements.
     AssertionError: if ``equality_comparator`` returns `False` for any pair of
                     trees from ``trees``.
   """
+  if ignore_nones:
+    _ignore_nones_deprecation()
+
   if len(trees) < 2:
     raise ValueError(
         "Assertions over only one tree does not make sense. Maybe you wrote "
         "`assert_trees_xxx([a, b])` instead of `assert_trees_xxx(a, b)`, or "
         "forgot the `error_msg_fn` arg to `assert_trees_all_equal_comparator`?")
   assert_trees_all_equal_structs(*trees)
-  if not ignore_nones:
-    assert_tree_no_nones(trees)
 
   def tree_error_msg_fn(l_1: _ai.TLeaf, l_2: _ai.TLeaf, path: str, i_1: int,
                         i_2: int):
     msg = error_msg_fn(l_1, l_2)
     if path:
       return f"Trees {i_1} and {i_2} differ in leaves '{path}': {msg}."
     else:
       return f"Trees (arrays) {i_1} and {i_2} differ: {msg}."
 
-  def wrapped_equality_comparator(leaf_1, leaf_2):
-    if leaf_1 is None or leaf_1 is None:
-      # Either both or none of leaves can be `None`.
-      assert leaf_1 is None and leaf_2 is None, (
-          "non-mutual cases must be caught by assert_trees_all_equal_structs")
-      if ignore_nones:
-        return True
-
-    return equality_comparator(leaf_1, leaf_2)
-
   cmp_fn = functools.partial(_ai.assert_leaves_all_eq_comparator,
-                             wrapped_equality_comparator, tree_error_msg_fn)
+                             equality_comparator, tree_error_msg_fn)
 
   # Trees are guaranteed to have the same structure.
-  paths = [path for path, _ in dm_tree.flatten_with_path(trees[0])]
-  trees_leaves = [dm_tree.flatten(tree) for tree in trees]
+  paths = [
+      _ai.convert_jax_path_to_dm_path(path)
+      for path, _ in jax.tree_util.tree_flatten_with_path(trees[0])[0]]
+  trees_leaves = [jax.tree_util.tree_leaves(tree) for tree in trees]
   for leaf_i, path in enumerate(paths):
     cmp_fn(path, *[leaves[leaf_i] for leaves in trees_leaves])
 
 
 assert_tree_all_equal_comparator = _ai.deprecation_wrapper(
     assert_trees_all_equal_comparator,
     old_name="assert_tree_all_equal_comparator",
@@ -1466,100 +1465,98 @@
 
 
 @_static_assertion
 def assert_trees_all_equal_dtypes(*trees: ArrayTree,
                                   ignore_nones: bool = False) -> None:
   """Checks that trees' leaves have the same dtype.
 
-  Note that `None` is treated as a PyTree nodes.
-
   Args:
     *trees: A sequence of (at least 2) trees to check.
-    ignore_nones: Whether to ignore `None` in the trees.
+    ignore_nones: Deprecated.
 
   Raises:
     AssertionError: If leaves' dtypes for any two trees differ.
   """
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   def cmp_fn(arr_1, arr_2):
     return (hasattr(arr_1, "dtype") and hasattr(arr_2, "dtype") and
             arr_1.dtype == arr_2.dtype)
 
   def err_msg_fn(arr_1, arr_2):
     if not hasattr(arr_1, "dtype"):
       return f"{type(arr_1)} is not a (j-)np array (has no `dtype` property)"
     if not hasattr(arr_2, "dtype"):
       return f"{type(arr_2)} is not a (j-)np array (has no `dtype` property)"
     return f"types: {arr_1.dtype} != {arr_2.dtype}"
 
-  assert_trees_all_equal_comparator(
-      cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones)
+  assert_trees_all_equal_comparator(cmp_fn, err_msg_fn, *trees)
 
 
 @_static_assertion
 def assert_trees_all_equal_sizes(*trees: ArrayTree,
                                  ignore_nones: bool = False) -> None:
   """Checks that trees have the same structure and leaves' sizes.
 
   Args:
     *trees: A sequence of (at least 2) trees with array leaves.
-    ignore_nones: Whether to ignore `None` in the trees.
+    ignore_nones: Deprecated.
 
   Raises:
-    AssertionError: If trees' structures or leaves' sizes are different;
-      if the trees contain `None` (with ``ignore_nones=False``).
+    AssertionError: If trees' structures or leaves' sizes are different.
   """
+  if ignore_nones:
+    _ignore_nones_deprecation()
   cmp_fn = lambda arr_1, arr_2: arr_1.size == arr_2.size
   err_msg_fn = lambda arr_1, arr_2: f"sizes: {arr_1.size} != {arr_2.size}"
-  assert_trees_all_equal_comparator(
-      cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones
-  )
+  assert_trees_all_equal_comparator(cmp_fn, err_msg_fn, *trees)
 
 
 @_static_assertion
 def assert_trees_all_equal_shapes(*trees: ArrayTree,
                                   ignore_nones: bool = False) -> None:
   """Checks that trees have the same structure and leaves' shapes.
 
   Args:
     *trees: A sequence of (at least 2) trees with array leaves.
-    ignore_nones: Whether to ignore `None` in the trees.
+    ignore_nones: Deprecated
 
   Raises:
-    AssertionError: If trees' structures or leaves' shapes are different;
-      if the trees contain `None` (with ``ignore_nones=False``).
+    AssertionError: If trees' structures or leaves' shapes are different.
   """
+  if ignore_nones:
+    _ignore_nones_deprecation()
   cmp_fn = lambda arr_1, arr_2: arr_1.shape == arr_2.shape
   err_msg_fn = lambda arr_1, arr_2: f"shapes: {arr_1.shape} != {arr_2.shape}"
-  assert_trees_all_equal_comparator(
-      cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones)
+  assert_trees_all_equal_comparator(cmp_fn, err_msg_fn, *trees)
 
 
 assert_tree_all_equal_shapes = _ai.deprecation_wrapper(
     assert_trees_all_equal_shapes,
     old_name="assert_tree_all_equal_shapes",
     new_name="assert_trees_all_equal_shapes")
 
 
 @_static_assertion
 def assert_trees_all_equal_shapes_and_dtypes(
     *trees: ArrayTree, ignore_nones: bool = False) -> None:
   """Checks that trees' leaves have the same shape and dtype.
 
-  Note that `None` is treated as a PyTree nodes.
-
   Args:
     *trees: A sequence of (at least 2) trees to check.
-    ignore_nones: Whether to ignore `None` in the trees.
+    ignore_nones: Deprecated.
 
   Raises:
     AssertionError: If leaves' shapes or dtypes for any two trees differ.
   """
-  assert_trees_all_equal_shapes(*trees, ignore_nones=ignore_nones)
-  assert_trees_all_equal_dtypes(*trees, ignore_nones=ignore_nones)
+  if ignore_nones:
+    _ignore_nones_deprecation()
+  assert_trees_all_equal_shapes(*trees)
+  assert_trees_all_equal_dtypes(*trees)
 
 
 ############# Value assertions. #############
 
 
 def _assert_tree_all_finite_static(tree_like: ArrayTree) -> None:
   """Checks that all leaves in a tree are finite.
@@ -1609,22 +1606,23 @@
   """Checks that all trees have leaves with *exactly* equal values.
 
   If you are comparing floating point numbers, an exact equality check may not
   be appropriate; consider using ``assert_trees_all_close``.
 
   Args:
     *trees: A sequence of (at least 2) trees with array leaves.
-    ignore_nones: Whether to ignore `None` in the trees.
+    ignore_nones: Deprecated.
     strict: If True, disable special scalar handling as described in
       `np.testing.assert_array_equals` notes section.
 
   Raises:
-    AssertionError: If the leaf values actual and desired are not exactly equal,
-      or the trees contain `None` (with ``ignore_nones=False``).
+    AssertionError: If the leaf values actual and desired are not exactly equal.
   """
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   def assert_fn(arr_1, arr_2):
     np.testing.assert_array_equal(
         _ai.jnp_to_np_array(arr_1),
         _ai.jnp_to_np_array(arr_2),
         err_msg="Error in value equality check: Values not exactly equal",
         strict=strict)
@@ -1641,16 +1639,15 @@
     try:
       assert_fn(arr_1, arr_2)
     except AssertionError as e:
       return (f"{str(e)} \nOriginal dtypes: "
               f"{np.asarray(arr_1).dtype}, {np.asarray(arr_2).dtype}")
     return ""
 
-  assert_trees_all_equal_comparator(
-      cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones)
+  assert_trees_all_equal_comparator(cmp_fn, err_msg_fn, *trees)
 
 
 def _assert_trees_all_equal_jittable(
     *trees: ArrayTree, ignore_nones: bool = False, strict: bool = True,
 ) -> Array:
   """A jittable version of `_assert_trees_all_equal_static`."""
   if not strict:
@@ -1658,16 +1655,16 @@
         "`strict=False` is not implemented by"
         " `_assert_trees_all_equal_jittable`. This is a feature of"
         " `np.testing.assert_array_equal` used in the static implementation of"
         " `assert_trees_all_equal` that we do not implement in the jittable"
         " version."
     )
 
-  if not ignore_nones:
-    assert_tree_no_nones(trees)
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   err_msg_template = "Values not exactly equal: {arr_1} != {arr_2}."
   cmp_fn = lambda x, y: jnp.array_equal(x, y, equal_nan=True)
   return _ai.assert_trees_all_eq_comparator_jittable(
       cmp_fn, err_msg_template, *trees
   )
 
@@ -1688,21 +1685,22 @@
   This compares the difference between values of actual and desired up to
    ``atol + rtol * abs(desired)``.
 
   Args:
     *trees: A sequence of (at least 2) trees with array leaves.
     rtol: A relative tolerance.
     atol: An absolute tolerance.
-    ignore_nones: Whether to ignore `None` in the trees.
+    ignore_nones: Deprecated.
 
   Raises:
     AssertionError: If actual and desired values are not equal up to
-      specified tolerance; if the trees contain `None` (with
-      ``ignore_nones=False``).
+      specified tolerance.
   """
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   def assert_fn(arr_1, arr_2):
     np.testing.assert_allclose(
         _ai.jnp_to_np_array(arr_1),
         _ai.jnp_to_np_array(arr_2),
         rtol=rtol,
         atol=atol,
@@ -1720,25 +1718,24 @@
     try:
       assert_fn(arr_1, arr_2)
     except AssertionError as e:
       return (f"{str(e)} \nOriginal dtypes: "
               f"{np.asarray(arr_1).dtype}, {np.asarray(arr_2).dtype}")
     return ""
 
-  assert_trees_all_equal_comparator(
-      cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones)
+  assert_trees_all_equal_comparator(cmp_fn, err_msg_fn, *trees)
 
 
 def _assert_trees_all_close_jittable(*trees: ArrayTree,
                                      rtol: float = 1e-06,
                                      atol: float = .0,
                                      ignore_nones: bool = False) -> Array:
   """A jittable version of `_assert_trees_all_close_static`."""
-  if not ignore_nones:
-    assert_tree_no_nones(trees)
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   err_msg_template = (
       f"Values not approximately equal ({rtol=}, {atol=}): "
       + "{arr_1} != {arr_2}."
   )
   cmp_fn = lambda x, y: jnp.isclose(x, y, rtol=rtol, atol=atol).all()
   return _ai.assert_trees_all_eq_comparator_jittable(
@@ -1794,21 +1791,22 @@
 
   Note that this function is not currently supported within JIT contexts,
   and does not currently support bfloat16 dtypes.
 
   Args:
     *trees: A sequence of (at least 2) trees with array leaves.
     maxulp: The maximum number of ULPs by which leaves may differ.
-    ignore_nones: Whether to ignore `None` in the trees.
+    ignore_nones: Deprecated.
 
   Raises:
     AssertionError: If actual and desired values are not equal up to
-      specified tolerance; if the trees contain `None` (with
-      ``ignore_nones=False``).
+      specified tolerance.
   """
+  if ignore_nones:
+    _ignore_nones_deprecation()
 
   def assert_fn(arr_1, arr_2):
     if (
         getattr(arr_1, "dtype", None) == jnp.bfloat16
         or getattr(arr_2, "dtype", None) == jnp.bfloat16
     ):
       # jnp_to_np_array currently converts bfloat16 to float32, which will cause
@@ -1839,17 +1837,15 @@
     except AssertionError as e:
       return (
           f"{str(e)} \nOriginal dtypes: "
           f"{np.asarray(arr_1).dtype}, {np.asarray(arr_2).dtype}"
       )
     return ""
 
-  assert_trees_all_equal_comparator(
-      cmp_fn, err_msg_fn, *trees, ignore_nones=ignore_nones
-  )
+  assert_trees_all_equal_comparator(cmp_fn, err_msg_fn, *trees)
 
 
 # The return should be typing.NoReturn, but that would significantly complicate
 # the signature of _value_assertion, so we pretend the return is jax.Array.
 def _assert_trees_all_close_ulp_jittable(
     *trees: ArrayTree,
     maxulp: int = 1,
@@ -1860,22 +1856,26 @@
   JAX does not yet have a native version of assert_array_max_ulp, so at the
   moment making ULP assertions on tracer objects simply isn't supported.
   This function exists only to make sure a sensible error is given.
 
   Args:
     *trees: Ignored.
     maxulp: Ignored.
-    ignore_nones: Ignored.
+    ignore_nones: Deprecated.
 
   Raises:
     NotImplementedError: unconditionally.
 
   Returns:
     Never returns. (We pretend jax.Array to satisfy the type checker.)
   """
+  del trees, maxulp
+  if ignore_nones:
+    _ignore_nones_deprecation()
+
   raise NotImplementedError(
       f"{_ai.ERR_PREFIX}assert_trees_all_close_ulp is not supported within JIT "
       "contexts."
   )
 
 
 assert_trees_all_close_ulp = _value_assertion(
```

### Comparing `chex-0.1.81/chex/_src/asserts_chexify.py` & `chex-0.1.82/chex/_src/asserts_chexify.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/asserts_chexify_test.py` & `chex-0.1.82/chex/_src/asserts_chexify_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/asserts_internal.py` & `chex-0.1.82/chex/_src/asserts_internal.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,22 @@
 
 import collections
 import collections.abc
 import functools
 import re
 import threading
 import traceback
-from typing import Any, Sequence, Union, Callable, List, Optional, Set, Tuple, Type
+from typing import Any, Sequence, Union, Callable, Hashable, List, Optional, Set, Tuple, Type
 
 from absl import logging
 from chex._src import pytypes
 import jax
 from jax.experimental import checkify
 import jax.numpy as jnp
 import numpy as np
-import tree as dm_tree
 
 # Custom pytypes.
 TLeaf = Any
 TLeavesEqCmpFn = Callable[[TLeaf, TLeaf], bool]
 TLeavesEqCmpErrorFn = Callable[[TLeaf, TLeaf], str]
 
 # TODO(iukemaev): define a typing protocol for TChexAssertion.
@@ -408,15 +407,16 @@
 
   if len(trees) < 2:
     raise ValueError(
         "Assertions over only one tree does not make sense. Maybe you wrote "
         "`assert_trees_xxx([a, b])` instead of `assert_trees_xxx(a, b)`, or "
         "forgot the `error_msg_fn` arg to `assert_trees_xxx`?")
 
-  def _tree_error_msg_fn(path: str, i_1: int, i_2: int):
+  def _tree_error_msg_fn(
+      path: Tuple[Union[int, str, Hashable]], i_1: int, i_2: int):
     if path:
       return (
           f"Trees {i_1} and {i_2} differ in leaves '{path}':"
           f" {error_msg_template}"
       )
     else:
       return f"Trees (arrays) {i_1} and {i_2} differ: {error_msg_template}."
@@ -431,17 +431,53 @@
           arr_1=leaves[0],
           arr_2=leaves[i],
       )
       verdict = jnp.logical_and(verdict, check_res)
     return verdict
 
   # Trees are guaranteed to have the same structure.
-  paths = [path for path, _ in dm_tree.flatten_with_path(trees[0])]
-  trees_leaves = [dm_tree.flatten(tree) for tree in trees]
+  paths = [
+      convert_jax_path_to_dm_path(path)
+      for path, _ in jax.tree_util.tree_flatten_with_path(trees[0])[0]]
+  trees_leaves = [jax.tree_util.tree_leaves(tree) for tree in trees]
 
   verdict = jnp.array(True)
   for leaf_i, path in enumerate(paths):
     verdict = jnp.logical_and(
         verdict, _cmp_leaves(path, *[leaves[leaf_i] for leaves in trees_leaves])
     )
 
   return verdict
+
+
+JaxKeyType = Union[
+    int,
+    str,
+    Hashable,
+    jax.tree_util.SequenceKey,
+    jax.tree_util.DictKey,
+    jax.tree_util.FlattenedIndexKey,
+    jax.tree_util.GetAttrKey,
+]
+
+
+def convert_jax_path_to_dm_path(
+    jax_tree_path: Sequence[JaxKeyType],
+) -> Tuple[Union[int, str, Hashable]]:
+  """Converts a path from jax.tree_util to one from dm-tree."""
+
+  # pytype:disable=attribute-error
+  def _convert_key_fn(key: JaxKeyType) -> Union[int, str, Hashable]:
+    if isinstance(key, (str, int)):
+      return key  # int | str.
+    if isinstance(key, jax.tree_util.SequenceKey):
+      return key.idx  # int.
+    if isinstance(key, jax.tree_util.DictKey):
+      return key.key  # Hashable
+    if isinstance(key, jax.tree_util.FlattenedIndexKey):
+      return key.key  # int.
+    if isinstance(key, jax.tree_util.GetAttrKey):
+      return key.name  # str.
+    raise ValueError(f"Jax tree key '{key}' of type '{type(key)}' not valid.")
+  # pytype:enable=attribute-error
+
+  return tuple(_convert_key_fn(key) for key in jax_tree_path)
```

### Comparing `chex-0.1.81/chex/_src/asserts_internal_test.py` & `chex-0.1.82/chex/_src/asserts_internal_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/asserts_test.py` & `chex-0.1.82/chex/_src/asserts_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -888,14 +888,33 @@
 
     # Test `None`s.
     with self.assertRaisesRegex(
         AssertionError,
         _get_err_regex('Error in tree structs equality check.*trees 0 and 1')):
       assert_fn(tree5, tree6)
 
+  def test_assert_tree_no_nones(self):
+    with self.subTest('tree_no_nones'):
+      tree_ok = {'a': [jnp.zeros((1,))], 'b': 1}
+      asserts.assert_tree_no_nones(tree_ok)
+
+    with self.subTest('tree_with_nones'):
+      tree_with_none = {'a': [jnp.zeros((1,))], 'b': None}
+      with self.assertRaisesRegex(
+          AssertionError, _get_err_regex('Tree contains `None`')
+      ):
+        asserts.assert_tree_no_nones(tree_with_none)
+
+    # Check `None`.
+    with self.subTest('input_none'):
+      with self.assertRaisesRegex(
+          AssertionError, _get_err_regex('Tree contains `None`')
+      ):
+        asserts.assert_tree_no_nones(None)
+
   def test_tree_all_finite_passes_finite(self):
     finite_tree = {'a': jnp.ones((3,)), 'b': jnp.array([0.0, 0.0])}
     asserts.assert_tree_all_finite(finite_tree)
     self.assertTrue(asserts._assert_tree_all_finite_jittable(finite_tree))
 
   def test_tree_all_finite_should_fail_inf(self):
     inf_tree = {
@@ -929,24 +948,14 @@
     tree2 = (jnp.array([1.0, 1.0 + 5e-7]),)
     error_msg = 'Values not exactly equal'
     with self.assertRaisesRegex(AssertionError, _get_err_regex(error_msg)):
       asserts.assert_trees_all_equal(tree1, tree2)
     with self.assertRaisesRegex(ValueError, error_msg):
       asserts._assert_trees_all_equal_jittable(tree1, tree2)
 
-  def test_assert_trees_all_equal_nones(self):
-    tree = {'a': [jnp.zeros((1,))], 'b': None}
-    asserts.assert_trees_all_equal(tree, tree, ignore_nones=True)
-    err_regex = _get_err_regex('`None` detected')
-    with self.assertRaisesRegex(AssertionError, err_regex):
-      asserts.assert_trees_all_equal(tree, tree, ignore_nones=False)
-
-    with self.assertRaisesRegex(AssertionError, err_regex):
-      asserts._assert_trees_all_equal_jittable(tree, tree, ignore_nones=False)
-
   def test_assert_trees_all_equal_strict_mode(self):
     # See 'notes' section of
     # https://numpy.org/doc/stable/reference/generated/numpy.testing.assert_array_equal.html
     # for details about the 'strict' mode of `numpy.testing.assert_array_equal`.
     # tldr; it has special handling for scalar values (by default).
     tree1 = {'a': jnp.array([1.0], dtype=jnp.float32), 'b': 0.0}
     tree2 = {'a': jnp.array(1.0, dtype=jnp.float32), 'b': 0.0}
@@ -985,23 +994,14 @@
   def test_assert_trees_all_close_passes_values_close_but_not_equal(self):
     tree1 = (jnp.array([1.0, 1.0]),)
     tree2 = (jnp.array([1.0, 1.0 + 5e-7]),)
     asserts.assert_trees_all_close(tree1, tree2, rtol=1e-6)
     self.assertTrue(
         asserts._assert_trees_all_close_jittable(tree1, tree2, rtol=1e-6))
 
-  def test_assert_trees_all_close_nones(self):
-    tree = {'a': [jnp.zeros((1,))], 'b': None}
-    asserts.assert_trees_all_close(tree, tree, ignore_nones=True)
-    err_regex = _get_err_regex('`None` detected')
-    with self.assertRaisesRegex(AssertionError, err_regex):
-      asserts.assert_trees_all_close(tree, tree, ignore_nones=False)
-    with self.assertRaisesRegex(AssertionError, err_regex):
-      asserts._assert_trees_all_close_jittable(tree, tree, ignore_nones=False)
-
   def test_assert_trees_all_close_bfloat16(self):
     tree1 = {'a': jnp.asarray([0.8, 1.6], dtype=jnp.bfloat16)}
     tree2 = {
         'a': jnp.asarray([0.8, 1.6], dtype=jnp.bfloat16).astype(jnp.float32)
     }
     tree3 = {'a': jnp.asarray([0.8, 1.7], dtype=jnp.bfloat16)}
     asserts.assert_trees_all_close(tree1, tree1)
@@ -1074,59 +1074,38 @@
     err_msg = re.escape(
         'not almost equal up to 1 ULP (max difference is 2 ULP)'
     )
     err_regex = _get_err_regex(err_msg)
     with self.assertRaisesRegex(AssertionError, err_regex):
       asserts.assert_trees_all_close_ulp(tree1, tree2, maxulp=1)
 
-  def test_assert_trees_all_close_ulp_nones(self):
-    tree = {'a': [jnp.zeros((1,))], 'b': None}
-    asserts.assert_trees_all_close_ulp(tree, tree, ignore_nones=True)
-    err_regex = _get_err_regex('`None` detected')
-    with self.assertRaisesRegex(AssertionError, err_regex):
-      asserts.assert_trees_all_close_ulp(tree, tree, ignore_nones=False)
-
   def test_assert_trees_all_close_ulp_fails_bfloat16(self):
     tree_f32 = (jnp.array([0.0]),)
     tree_bf16 = (jnp.array([0.0], dtype=jnp.bfloat16),)
     err_msg = 'ULP assertions are not currently supported for bfloat16.'
     err_regex = _get_err_regex(err_msg)
     with self.assertRaisesRegex(ValueError, err_regex):  # pylint: disable=g-error-prone-assert-raises
       asserts.assert_trees_all_close_ulp(tree_bf16, tree_bf16)
     with self.assertRaisesRegex(ValueError, err_regex):  # pylint: disable=g-error-prone-assert-raises
       asserts.assert_trees_all_close_ulp(tree_bf16, tree_f32)
 
-  def test_assert_trees_all_equal_shapes_nones(self):
-    tree = {'a': [jnp.zeros((1,))], 'b': None}
-    asserts.assert_trees_all_equal_shapes(tree, tree, ignore_nones=True)
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_trees_all_equal_shapes(tree, tree, ignore_nones=False)
-
   def test_assert_tree_has_only_ndarrays(self):
     # Check correct inputs.
     asserts.assert_tree_has_only_ndarrays({'a': jnp.zeros(1), 'b': np.ones(3)})
     asserts.assert_tree_has_only_ndarrays(np.zeros(4))
     asserts.assert_tree_has_only_ndarrays(())
 
     # Check incorrect inputs.
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('\'b\' is not an ndarray')):
       asserts.assert_tree_has_only_ndarrays({'a': jnp.zeros((1,)), 'b': 1})
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('\'b/1\' is not an ndarray')):
       asserts.assert_tree_has_only_ndarrays({'a': jnp.zeros(101), 'b': [1, 2]})
 
-    # Check `None`.
-    tree_with_none = (np.array([2]), None)
-    asserts.assert_tree_has_only_ndarrays(tree_with_none, ignore_nones=True)
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_has_only_ndarrays(tree_with_none)
-
   def test_assert_tree_is_on_host(self):
     cpu = jax.devices('cpu')[0]
 
     # Check Numpy arrays.
     for flag in (False, True):
       asserts.assert_tree_is_on_host({'a': np.zeros(1), 'b': np.ones(3)},
                                      allow_cpu_device=flag)
@@ -1188,21 +1167,14 @@
     ):
       asserts.assert_tree_is_on_host(
           {'a': jax.device_put_replicated(np.zeros(1), (cpu,))},
           allow_cpu_device=False,
           allow_sharded_arrays=True,
       )
 
-    # Check `None`.
-    tree_with_none = (np.array([2]), None)
-    asserts.assert_tree_is_on_host(tree_with_none, ignore_nones=True)
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_is_on_host(tree_with_none)
-
   def test_assert_tree_is_on_device(self):
     # Check CPU platform.
     cpu = jax.devices('cpu')[0]
     to_cpu = lambda x: jax.device_put(x, cpu)
 
     cpu_tree = {'a': to_cpu(np.zeros(1)), 'b': to_cpu(np.ones(3))}
     asserts.assert_tree_is_on_device(cpu_tree, device=cpu)
@@ -1279,20 +1251,14 @@
 
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('\'a\' is a ShardedDeviceArra')):
       # ShardedArrays are disallowed.
       asserts.assert_tree_is_on_device(
           {'a': jax.device_put_replicated(np.zeros(1), (cpu,))}, device=cpu)
 
-    # Check `None`.
-    asserts.assert_tree_is_on_device((None,), ignore_nones=True)
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_is_on_device((None,))
-
   def test_assert_tree_is_sharded(self):
     np_tree = {'a': np.zeros(1), 'b': np.ones(3)}
 
     def _format(*devs):
       return re.escape(f'{devs}')
 
     # Check single-device case.
@@ -1392,34 +1358,14 @@
       asserts.assert_tree_is_sharded({'a': jnp.zeros(1)}, devices=(cpu,))
 
     with self.assertRaisesRegex(
         AssertionError, _get_err_regex('\'a\' is not sharded.*CPU')):
       asserts.assert_tree_is_sharded({'a': jax.device_put(np.zeros(1), cpu)},
                                      devices=(cpu,))
 
-    # Check `None`.
-    asserts.assert_tree_is_sharded((None,), devices=(cpu,), ignore_nones=True)
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_is_sharded((None,), devices=(cpu,))
-
-  def test_assert_tree_no_nones(self):
-    tree_ok = {'a': [jnp.zeros((1,))], 'b': 1}
-    asserts.assert_tree_no_nones(tree_ok)
-
-    tree_with_none = {'a': [jnp.zeros((1,))], 'b': None}
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_no_nones(tree_with_none)
-
-    # Check `None`.
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_no_nones(None)
-
   def test_assert_trees_all_close_fails_different_structure(self):
     self._assert_tree_structs_validation(asserts.assert_trees_all_close)
 
   def test_assert_trees_all_close_fails_values_differ(self):
     tree1 = jnp.array([0.0, 2.0])
     tree2 = jnp.array([0.0, 2.1])
     asserts.assert_trees_all_close(tree1, tree2, atol=0.1)
@@ -1509,27 +1455,14 @@
         _get_err_regex(r'leaf \'x/y\' has a shape of length 2')):
       asserts.assert_tree_shape_prefix(tree, (3, 2, 1))
     with self.assertRaisesRegex(
         AssertionError,
         _get_err_regex(r'leaf \'x/y\' has a shape of length 2')):
       asserts.assert_tree_shape_prefix(tree, [3, 2, 1])
 
-  def test_assert_tree_shape_prefix_none(self):
-    tree = {'x': np.zeros([3]), 'n': None}
-    asserts.assert_tree_shape_prefix(tree, (3,), ignore_nones=True)
-    asserts.assert_tree_shape_prefix(tree, [3], ignore_nones=True)
-
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_shape_prefix(tree, (3,), ignore_nones=False)
-
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_shape_prefix(tree, [3], ignore_nones=False)
-
   @parameterized.named_parameters(
       ('scalars', ()),
       ('vectors', (1,)),
       ('matrices', (2, 1)),
   )
   def test_assert_tree_shape_suffix_matching(self, shape):
     tree = {'x': {'y': np.zeros([4, 2, 1])}, 'z': np.zeros([2, 1])}
@@ -1572,27 +1505,14 @@
         AssertionError, _get_err_regex('which is smaller than the expected')):
       asserts.assert_tree_shape_suffix(tree, (3, 4, 2, 1))
 
     with self.assertRaisesRegex(
         AssertionError, _get_err_regex('which is smaller than the expected')):
       asserts.assert_tree_shape_suffix(tree, [3, 4, 2, 1])
 
-  def test_assert_tree_shape_suffix_none(self):
-    tree = {'x': np.zeros([3]), 'n': None}
-    asserts.assert_tree_shape_suffix(tree, (3,), ignore_nones=True)
-    asserts.assert_tree_shape_suffix(tree, [3], ignore_nones=True)
-
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_shape_suffix(tree, (3,), ignore_nones=False)
-
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_tree_shape_suffix(tree, [3], ignore_nones=False)
-
   def test_assert_trees_all_equal_dtypes(self):
     t_0 = {'x': np.zeros(3, dtype=np.int16), 'y': np.ones(2, dtype=np.float32)}
     t_1 = {'x': np.zeros(5, dtype=np.uint16), 'y': np.ones(4, dtype=np.float32)}
 
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('Trees 0 and 1 differ')):
       asserts.assert_trees_all_equal_dtypes(t_0, t_1)
@@ -1657,26 +1577,22 @@
   def test_assert_trees_all_equal_none(self):
     t_0 = {'x': None, 'y': np.array(2, dtype=np.int32)}
     t_1 = {'x': None, 'y': np.array([23], dtype=np.int32)}
     t_2 = {'x': None, 'y': np.array(3, dtype=np.float32)}
     t_3 = {'y': np.array([23], dtype=np.int32)}
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('Trees 0 and 2 differ')):
-      asserts.assert_trees_all_equal_dtypes(t_0, t_1, t_2, ignore_nones=True)
-    asserts.assert_trees_all_equal_dtypes(t_0, t_1, ignore_nones=True)
-    with self.assertRaisesRegex(AssertionError,
-                                _get_err_regex('`None` detected')):
-      asserts.assert_trees_all_equal_dtypes(t_0, t_1, ignore_nones=False)
-
+      asserts.assert_trees_all_equal_dtypes(t_0, t_1, t_2)
+    asserts.assert_trees_all_equal_dtypes(t_0, t_1)
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('trees 0 and 1 do not match')):
-      asserts.assert_trees_all_equal_dtypes(t_0, t_3, ignore_nones=True)
+      asserts.assert_trees_all_equal_dtypes(t_0, t_3)
     with self.assertRaisesRegex(AssertionError,
                                 _get_err_regex('trees 0 and 1 do not match')):
-      asserts.assert_trees_all_equal_dtypes(t_0, t_3, ignore_nones=False)
+      asserts.assert_trees_all_equal_dtypes(t_0, t_3)
 
 
 class DevicesAssertTest(parameterized.TestCase):
 
   def _device_count(self, backend):
     try:
       return jax.device_count(backend)
```

### Comparing `chex-0.1.81/chex/_src/dataclass.py` & `chex-0.1.82/chex/_src/dataclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """JAX/dm-tree friendly dataclass implementation reusing Python dataclasses."""
 
 import collections
 import dataclasses
 import functools
+import sys
 
 from absl import logging
 import jax
 from typing_extensions import dataclass_transform  # pytype: disable=not-supported-yet
 
 
 FrozenInstanceError = dataclasses.FrozenInstanceError
@@ -89,14 +90,15 @@
     *,
     init=True,
     repr=True,  # pylint: disable=redefined-builtin
     eq=True,
     order=False,
     unsafe_hash=False,
     frozen=False,
+    kw_only: bool = False,
     mappable_dataclass=True,  # pylint: disable=redefined-outer-name
 ):
   """JAX-friendly wrapper for :py:func:`dataclasses.dataclass`.
 
   This wrapper class registers new dataclasses with JAX so that tree utils
   operate correctly. Additionally a replace method is provided making it easy
   to operate on the class when made immutable (frozen=True).
@@ -105,14 +107,15 @@
     cls: A class to decorate.
     init: See :py:func:`dataclasses.dataclass`.
     repr: See :py:func:`dataclasses.dataclass`.
     eq: See :py:func:`dataclasses.dataclass`.
     order: See :py:func:`dataclasses.dataclass`.
     unsafe_hash: See :py:func:`dataclasses.dataclass`.
     frozen: See :py:func:`dataclasses.dataclass`.
+    kw_only: See :py:func:`dataclasses.dataclass`.
     mappable_dataclass: If True (the default), methods to make the class
       implement the :py:class:`collections.abc.Mapping` interface will be
       generated and the class will include :py:class:`collections.abc.Mapping`
       in its base classes.
       `True` is the default, because being an instance of `Mapping` makes
       `chex.dataclass` compatible with e.g. `jax.tree_util.tree_*` methods, the
       `tree` library, or methods related to tensorflow/python/utils/nest.py.
@@ -122,15 +125,15 @@
 
   Returns:
     A JAX-friendly dataclass.
   """
   def dcls(cls):
     # Make sure to create a separate _Dataclass instance for each `cls`.
     return _Dataclass(
-        init, repr, eq, order, unsafe_hash, frozen, mappable_dataclass
+        init, repr, eq, order, unsafe_hash, frozen, kw_only, mappable_dataclass
     )(cls)
 
   if cls is None:
     return dcls
   return dcls(cls)
 
 
@@ -141,43 +144,52 @@
       self,
       init=True,
       repr=True,  # pylint: disable=redefined-builtin
       eq=True,
       order=False,
       unsafe_hash=False,
       frozen=False,
+      kw_only=False,
       mappable_dataclass=True,  # pylint: disable=redefined-outer-name
   ):
     self.init = init
     self.repr = repr  # pylint: disable=redefined-builtin
     self.eq = eq
     self.order = order
     self.unsafe_hash = unsafe_hash
     self.frozen = frozen
+    self.kw_only = kw_only
     self.mappable_dataclass = mappable_dataclass
     self.registered = False
 
   def __call__(self, cls):
     """Forwards class to dataclasses's wrapper and registers it with JAX."""
 
     # Remove once https://github.com/python/cpython/pull/24484 is merged.
     for base in cls.__bases__:
       if (dataclasses.is_dataclass(base) and
           getattr(base, "__dataclass_params__").frozen and not self.frozen):
         raise TypeError("cannot inherit non-frozen dataclass from a frozen one")
 
+    # `kw_only` is only available starting from 3.10.
+    version_dependent_args = {}
+    version = sys.version_info
+    if version.major == 3 and version.minor >= 10:
+      version_dependent_args = {"kw_only": self.kw_only}
     # pytype: disable=wrong-keyword-args
     dcls = dataclasses.dataclass(
         cls,
         init=self.init,
         repr=self.repr,
         eq=self.eq,
         order=self.order,
         unsafe_hash=self.unsafe_hash,
-        frozen=self.frozen)
+        frozen=self.frozen,
+        **version_dependent_args,
+    )
     # pytype: enable=wrong-keyword-args
 
     fields_names = set(f.name for f in dataclasses.fields(dcls))
     invalid_fields = fields_names.intersection(_RESERVED_DCLS_FIELD_NAMES)
     if invalid_fields:
       raise ValueError(f"The following dataclass fields are disallowed: "
                        f"{invalid_fields} ({dcls}).")
```

### Comparing `chex-0.1.81/chex/_src/dataclass_test.py` & `chex-0.1.82/chex/_src/dataclass_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for `dataclass.py`."""
 import copy
 import dataclasses
 import pickle
+import sys
 from typing import Any, Generic, Mapping, TypeVar
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from chex._src import asserts
 from chex._src import dataclass
 from chex._src import pytypes
@@ -379,14 +380,58 @@
     obj = dummy_dataclass(frozen=frozen)
     obj = obj.replace(a=obj.a.replace(c=factor * obj.a.c))
     obj = obj.replace(a=obj.a.replace(d=factor * obj.a.d))
     obj = obj.replace(b=factor * obj.b)
     target_obj = dummy_dataclass(factor=factor, frozen=frozen)
     asserts.assert_trees_all_close(obj, target_obj)
 
+  def test_dataclass_requires_kwargs_by_default(self):
+    factor = 1.0
+    with self.assertRaisesRegex(
+        ValueError,
+        "Mappable dataclass constructor doesn't support positional args.",
+    ):
+      Dataclass(
+          NestedDataclass(
+              c=factor * np.ones((3,), dtype=np.float32),
+              d=factor * np.ones((4,), dtype=np.float32),
+          ),
+          factor * 2 * np.ones((5,), dtype=np.float32),
+      )
+
+  def test_dataclass_mappable_dataclass_false(self):
+    factor = 1.0
+
+    @chex_dataclass(mappable_dataclass=False)
+    class NonMappableDataclass:
+      a: NestedDataclass
+      b: pytypes.ArrayDevice
+
+    NonMappableDataclass(
+        NestedDataclass(
+            c=factor * np.ones((3,), dtype=np.float32),
+            d=factor * np.ones((4,), dtype=np.float32),
+        ),
+        factor * 2 * np.ones((5,), dtype=np.float32),
+    )
+
+  def test_inheritance_is_possible_thanks_to_kw_only(self):
+    if sys.version_info.minor < 10:  # Feature only available for Python >= 3.10
+      return
+
+    @chex_dataclass(kw_only=True)
+    class Base:
+      default: int = 1
+
+    @chex_dataclass(kw_only=True)
+    class Child(Base):
+      non_default: int
+
+    Child(non_default=2)
+
   def test_unfrozen_dataclass_is_mutable(self):
     factor = 5.
     obj = dummy_dataclass(frozen=False)
     obj.a.c = factor * obj.a.c
     obj.a.d = factor * obj.a.d
     obj.b = factor * obj.b
     target_obj = dummy_dataclass(factor=factor, frozen=False)
```

### Comparing `chex-0.1.81/chex/_src/dimensions.py` & `chex-0.1.82/chex/_src/dimensions.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/dimensions_test.py` & `chex-0.1.82/chex/_src/dimensions_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/fake.py` & `chex-0.1.82/chex/_src/fake.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/fake_set_n_cpu_devices_test.py` & `chex-0.1.82/chex/_src/fake_set_n_cpu_devices_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/fake_test.py` & `chex-0.1.82/chex/_src/fake_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/pytypes.py` & `chex-0.1.82/chex/_src/pytypes.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/restrict_backends.py` & `chex-0.1.82/chex/_src/restrict_backends.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/restrict_backends_test.py` & `chex-0.1.82/chex/_src/restrict_backends_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/variants.py` & `chex-0.1.82/chex/_src/variants.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/_src/variants_test.py` & `chex-0.1.82/chex/_src/variants_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex/chex_test.py` & `chex-0.1.82/chex/chex_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/chex.egg-info/PKG-INFO` & `chex-0.1.82/chex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chex
-Version: 0.1.81
+Version: 0.1.82
 Summary: Chex: Testing made fun, in JAX!
 Home-page: https://github.com/deepmind/chex
 Author: DeepMind
 Author-email: chex-dev@google.com
 License: Apache 2.0
 Keywords: jax testing debugging python machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chex-0.1.81/chex.egg-info/SOURCES.txt` & `chex-0.1.82/chex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chex-0.1.81/setup.py` & `chex-0.1.82/setup.py`

 * *Files identical despite different names*

