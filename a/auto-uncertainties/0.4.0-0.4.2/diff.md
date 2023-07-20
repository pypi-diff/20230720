# Comparing `tmp/auto_uncertainties-0.4.0.tar.gz` & `tmp/auto_uncertainties-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_uncertainties-0.4.0.tar", last modified: Tue Mar 14 22:47:21 2023, max compression
+gzip compressed data, was "auto_uncertainties-0.4.2.tar", last modified: Thu Jul 20 15:10:03 2023, max compression
```

## Comparing `auto_uncertainties-0.4.0.tar` & `auto_uncertainties-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:47:21.492290 auto_uncertainties-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:47:21.484290 auto_uncertainties-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:47:21.488290 auto_uncertainties-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-14 22:47:21.492290 auto_uncertainties-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:47:21.488290 auto_uncertainties-0.4.0/auto_uncertainties/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/auto_uncertainties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-14 22:47:21.000000 auto_uncertainties-0.4.0/auto_uncertainties/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/auto_uncertainties/pandas_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/auto_uncertainties/uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/auto_uncertainties/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    20448 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/auto_uncertainties/wrap_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:47:21.488290 auto_uncertainties-0.4.0/auto_uncertainties.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-14 22:47:21.000000 auto_uncertainties-0.4.0/auto_uncertainties.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-14 22:47:21.000000 auto_uncertainties-0.4.0/auto_uncertainties.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 22:47:21.000000 auto_uncertainties-0.4.0/auto_uncertainties.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-14 22:47:21.000000 auto_uncertainties-0.4.0/auto_uncertainties.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-14 22:47:21.000000 auto_uncertainties-0.4.0/auto_uncertainties.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 22:47:21.492290 auto_uncertainties-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:47:21.488290 auto_uncertainties-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/tests/test_numpy_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-03-14 22:47:05.000000 auto_uncertainties-0.4.0/tests/test_uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:10:03.509060 auto_uncertainties-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:10:03.505060 auto_uncertainties-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:10:03.505060 auto_uncertainties-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 15:10:03.509060 auto_uncertainties-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:10:03.505060 auto_uncertainties-0.4.2/auto_uncertainties/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/auto_uncertainties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 15:10:03.000000 auto_uncertainties-0.4.2/auto_uncertainties/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28043 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/auto_uncertainties/pandas_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/auto_uncertainties/uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/auto_uncertainties/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/auto_uncertainties/wrap_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:10:03.505060 auto_uncertainties-0.4.2/auto_uncertainties.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 15:10:03.000000 auto_uncertainties-0.4.2/auto_uncertainties.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-20 15:10:03.000000 auto_uncertainties-0.4.2/auto_uncertainties.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:10:03.000000 auto_uncertainties-0.4.2/auto_uncertainties.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 15:10:03.000000 auto_uncertainties-0.4.2/auto_uncertainties.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 15:10:03.000000 auto_uncertainties-0.4.2/auto_uncertainties.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:10:03.509060 auto_uncertainties-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:10:03.509060 auto_uncertainties-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/tests/test_numpy_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/tests/test_pandas_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/tests/test_pandas_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-20 15:09:48.000000 auto_uncertainties-0.4.2/tests/test_uncertainty.py
```

### Comparing `auto_uncertainties-0.4.0/.github/workflows/python-publish.yml` & `auto_uncertainties-0.4.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `auto_uncertainties-0.4.0/.github/workflows/python-test.yml` & `auto_uncertainties-0.4.2/.github/workflows/python-test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pylint pytest pytest-cov hypothesis
-          pip install .
+          pip install .[pandas]
       - name: Lint with pylint
         run: |
           pylint --fail-under=8 auto_uncertainties
       - name: Test with pytest
         run: |
-          pytest --cov=auto_uncertainties --cov-report=xml --cov-report=html
+          pytest --cov=auto_uncertainties --cov-report=xml --cov-report=html -k "not pandas"
```

### Comparing `auto_uncertainties-0.4.0/.gitignore` & `auto_uncertainties-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `auto_uncertainties-0.4.0/.pre-commit-config.yaml` & `auto_uncertainties-0.4.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 repos:
+
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.0.275
+  hooks:
+    - id: ruff
+      args: [ --fix, --exit-non-zero-on-fix ]
+
 -   repo: https://github.com/psf/black.git
     rev: 23.1.0
     hooks:
     - id: black
       language_version: python3.9
 
+- repo: https://github.com/pycqa/isort
+  rev: 5.12.0
+  hooks:
+    - id: isort
+      name: isort (python)
+
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: end-of-file-fixer
   - id: fix-encoding-pragma
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-case-conflict
   - id: check-executables-have-shebangs
   - id: check-merge-conflict
   - id: check-symlinks
   - id: debug-statements
   - id: mixed-line-ending
-
-- repo: https://github.com/pycqa/isort
-  rev: 5.12.0
-  hooks:
-    - id: isort
-      name: isort (python)
```

### Comparing `auto_uncertainties-0.4.0/LICENSE.txt` & `auto_uncertainties-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `auto_uncertainties-0.4.0/README.rst` & `auto_uncertainties-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `auto_uncertainties-0.4.0/auto_uncertainties/__init__.py` & `auto_uncertainties-0.4.2/auto_uncertainties/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import numpy as np
 
 
 class NegativeStdDevError(Exception):
     """An exception for when the standard deviation is negative"""
 
     pass
@@ -10,20 +12,20 @@
 
 class NumpyDowncastWarning(RuntimeWarning):
     """An exception for when an uncertainties array is downcast to a numpy array"""
 
     pass
 
 
-from .uncertainty import Uncertainty
+from .uncertainty import Uncertainty  # noqa: E402
 
 try:
     from .pandas_compat import UncertaintyArray
 except ImportError:
-    pass
+    UncertaintyArray = None
 
 
 def nominal_values(x):
     # Is an Uncertainty
     if hasattr(x, "_nom"):
         return x.value
     else:
@@ -41,15 +43,15 @@
                 return x
             else:
                 return x2.value
 
 
 def std_devs(x):
     # Is an Uncertainty
-    if hasattr(x, "_nom"):
+    if hasattr(x, "_err"):
         return x.error
     else:
         if np.ndim(x) > 0:
             try:
                 x2 = Uncertainty.from_sequence(x)
             except Exception:
                 return np.zeros_like(x)
```

### Comparing `auto_uncertainties-0.4.0/auto_uncertainties/uncertainty.py` & `auto_uncertainties-0.4.2/auto_uncertainties/uncertainty.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,180 +2,83 @@
 # Based heavily on the implementation of pint's Quantity object
 from __future__ import annotations
 
 import copy
 import locale
 import operator
 import warnings
-from re import match
-from types import MethodType
 
-import jax
+import joblib
 import numpy as np
-from pint import DimensionalityError, Quantity
-from pint.util import SharedRegistryObject
 
 from . import NegativeStdDevError, NumpyDowncastWarning
 from .util import (
     Display,
     ignore_numpy_downcast_warnings,
     ignore_runtime_warnings,
     is_np_duck_array,
     strip_device_array,
 )
 from .wrap_numpy import HANDLED_FUNCTIONS, HANDLED_UFUNCS, wrap_numpy
 
 
 def _check_units(value, err):
-    mag_units = hasattr(value, "units")
-    err_units = hasattr(err, "units")
-    if mag_units ^ err_units and err is not None:
-        raise DimensionalityError(
-            "",
-            "",
-            extra_msg="...Both mag and err need to have units if one of them has units!",
-        )
-    if mag_units and err is not None:
-        if value.units != err.units:
-            raise DimensionalityError(
-                value.units,
-                err.units,
-                extra_msg=f"Value units {value.units} cannot be converted to error units {err.units}",
-            )
-    if mag_units:
-        mag_units = value.units
-        ret_val = value.to(mag_units).m
+    mag_has_units = hasattr(value, "units")
+    mag_units = getattr(value, "units", None)
+    err_has_units = hasattr(err, "units")
+    err_units = getattr(err, "units", None)
+
+    if mag_has_units and mag_units is not None:
+        Q = mag_units._REGISTRY.Quantity
+        ret_val = Q(value).to(mag_units).m
         if err is not None:
-            ret_err = err.to(mag_units).m
+            ret_err = Q(err).to(mag_units).m
         else:
             ret_err = None
+        ret_units = mag_units
+    # This branch will never actually work, but its here
+    # to raise a Dimensionality error without needing to import pint
+    elif err_has_units:
+        Q = err_units._REGISTRY.Quantity
+        ret_val = Q(value).to(err_units).m
+        ret_err = Q(err).to(err_units).m
+        ret_units = err_units
     else:
-        mag_units = None
+        ret_units = None
         ret_val = value
         ret_err = err
 
-    return ret_val, ret_err, mag_units
+    return ret_val, ret_err, ret_units
 
 
 class Uncertainty(Display):
     __apply_to_both_ndarray__ = [
         "flatten",
         "real",
         "imag",
         "astype",
         "T",
         "reshape",
     ]
     __ndarray_attributes__ = ["dtype", "ndim", "size"]
 
-    # Pint comparibility
-    @property
-    def unitless(self) -> bool:
-        """ """
-        return not bool(self.to_root_units()._units)
-
-    @property
-    def dimensionless(self) -> bool:
-        """ """
-        tmp = self.to_root_units()
-
-        return not bool(tmp.dimensionality)
-
-    _dimensionality = None
-
-    @property
-    def dimensionality(self):
-        """
-        Returns
-        -------
-        dict
-            Dimensionality of the Quantity, e.g. ``{length: 1, time: -1}``
-        """
-        if self._dimensionality is None:
-            self._dimensionality = self._REGISTRY._get_dimensionality(
-                self.units
-            )
-
-        return self._dimensionality
-
-    def check(self, dimension) -> bool:
-        """Return true if the quantity's dimension matches passed dimension."""
-        return self.dimensionality == self._REGISTRY.get_dimensionality(
-            dimension
-        )
-
-    def _check(self, other) -> bool:
-        """Check if the other object use a registry and if so that it is the
-        same registry.
-        Parameters
-        ----------
-        other :
-        Returns
-        -------
-        type
-            other don't use a registry and raise ValueError if other don't use the
-            same unit registry.
-        """
-        if self._REGISTRY is getattr(other, "_REGISTRY", None):
-            return True
-
-        elif isinstance(other, SharedRegistryObject):
-            mess = "Cannot operate with {} and {} of different registries."
-            raise ValueError(
-                mess.format(self.__class__.__name__, other.__class__.__name__)
-            )
-        else:
-            return False
-
-    def to(self, other):
-        if hasattr(self.nominal_value, "units"):
-            return self.__class__(self._nom.to(other), self._err.to(other))
-        else:
-            raise AttributeError("Uncertainty has no quantity!")
-
-    @property
-    def m(self):
-        if hasattr(self.nominal_value, "units"):
-            return self.__class__(self._nom.m, self._err.m)
-        else:
-            raise AttributeError("Uncertainty has no quantity!")
-
-    @property
-    def units(self):
-        if hasattr(self.nominal_value, "units"):
-            return self._nom.units
-        else:
-            raise AttributeError("Uncertainty has no quantity!")
-
-    @property
-    def _REGISTRY(self):
-        return getattr(self._nom, "_REGISTRY", None)
-
-    def compatible_units(self, *contexts):
-        if contexts:
-            with self._REGISTRY.context(*contexts):
-                return self._REGISTRY.get_compatible_units(self._units)
-
-        return self._REGISTRY.get_compatible_units(self._units)
-
-    def _convert_magnitude_not_inplace(self, other, *contexts, **ctx_kwargs):
-        if contexts:
-            with self._REGISTRY.context(*contexts, **ctx_kwargs):
-                return self._REGISTRY.convert(
-                    self._magnitude, self._units, other
-                )
-
-        return self._REGISTRY.convert(self._magnitude, self._units, other)
+    __array_priority__ = 18
 
     @ignore_numpy_downcast_warnings
     def __init__(self, value, err=None):
+        if hasattr(value, "units") or hasattr(err, "units"):
+            raise NotImplementedError(
+                "Uncertainty cannot have units! Call Uncertainty.from_quantities instead."
+            )
 
-        value_, err_, units = _check_units(value, err)
-        value_ = strip_device_array(value_)
-        err_ = strip_device_array(err_)
+        value_ = strip_device_array(value)
+        if err is not None:
+            err_ = strip_device_array(err)
+        else:
+            err_ = None
 
         # If Uncertatity
         if isinstance(value_, self.__class__):
             magnitude_nom = value_.value
             magnitude_err = value_.error
         # If sequence
         elif isinstance(value_, list):
@@ -204,17 +107,14 @@
         # Replace NaNs in errors with zeros
         if is_np_duck_array(type(magnitude_err)):
             magnitude_err[~np.isfinite(magnitude_err)] = 0
         else:
             if not np.isfinite(magnitude_err):
                 magnitude_err = 0
 
-        if units is not None:
-            magnitude_nom *= units
-            magnitude_err *= units
         # Basic sanity checks
         if is_np_duck_array(type(magnitude_nom)):
             match_items = self.__ndarray_attributes__ + ["shape"]
             try:
                 match_items.remove("dtype")
             except ValueError:
                 pass
@@ -251,46 +151,31 @@
     def __deepcopy__(self, memo) -> Uncertainty:
         ret = self.__class__(
             copy.deepcopy(self._nom, memo), copy.deepcopy(self._err, memo)
         )
         return ret
 
     def __hash__(self) -> int:
-        return hash((self.__class__, self._nom, self._err))
+        digest = joblib.hash((self._nom, self._err), hash_name="sha1")
+        return int.from_bytes(bytes(digest, encoding="utf-8"), "big")
 
     @property
     def value(self):
         return self._nom
 
     @property
-    def nominal_value(self):
-        return self.value
-
-    @property
-    def n(self):
-        return self.value
-
-    @property
     def error(self):
         return self._err
 
     @property
-    def std_dev(self):
-        return self.error
-
-    @property
-    def s(self):
-        return self.error
-
-    @property
     def relative(self):
         if np.ndim(self._nom) == 0:
             try:
                 return self._err / self._nom
-            except (OverflowError):
+            except OverflowError:
                 return np.inf
             except ZeroDivisionError:
                 return np.NaN
         else:
             return self._err / self._nom
 
     @property
@@ -300,14 +185,39 @@
     @property
     def rel2(self):
         try:
             return self.relative**2
         except OverflowError:
             return np.inf
 
+    def plus_minus(self, err: float):
+        val = self._nom
+        old_err = self._err
+        new_err = np.sqrt(old_err**2 + err**2)
+
+        return self.__class__(val, new_err)
+
+    @classmethod
+    def from_string(cls, string: str):
+        new_str = string.replace("+/-", "±")
+        new_str = new_str.replace("+-", "±")
+        if "±" not in new_str:
+            return Uncertainty(float(string))
+        else:
+            u1, u2 = new_str.split("±")
+            return cls(float(u1), float(u2))
+
+    @classmethod
+    def from_quantities(cls, value, err):
+        value_, err_, units = _check_units(value, err)
+        inst = cls(value_, err_)
+        if units is not None:
+            inst *= units
+        return inst
+
     @classmethod
     def from_list(cls, u_list):
         return cls.from_sequence(u_list)
 
     @classmethod
     def from_sequence(cls, seq):
         _ = iter(seq)
@@ -342,119 +252,85 @@
     def __complex__(self) -> Uncertainty:
         return complex(self._nom)
 
     def __int__(self) -> Uncertainty:
         return int(self._nom)
 
     # Math Operators
-    def __iadd__(self, other):
-        new = self + other
-        if is_np_duck_array(type(self._nom)):
-            self._err = new._err
-            self._nom = new._nom
-            return self
-        else:
-            return new
-
     def __add__(self, other):
         if isinstance(other, Uncertainty):
             new_mag = self._nom + other._nom
             new_err = np.sqrt(self._err**2 + other._err**2)
         else:
             new_mag = self._nom + other
             new_err = self._err
-        return self.__class__(new_mag, new_err)
+        try:
+            return self.__class__(new_mag, new_err)
+        except NotImplementedError:
+            return NotImplemented
 
     __radd__ = __add__
 
-    def __isub__(self, other):
-        new = self - other
-        if is_np_duck_array(type(self._nom)):
-            self._err = new._err
-            self._nom = new._nom
-            return self
-        else:
-            return new
-
     def __sub__(self, other):
         if isinstance(other, Uncertainty):
             new_mag = self._nom - other._nom
             new_err = np.sqrt(self._err**2 + other._err**2)
         else:
             new_mag = self._nom - other
             new_err = self._err
-        return self.__class__(new_mag, new_err)
+        try:
+            return self.__class__(new_mag, new_err)
+        except NotImplementedError:
+            return NotImplemented
 
     def __rsub__(self, other):
         return -self.__sub__(other)
 
-    def __imul__(self, other):
-        new = self * other
-        if is_np_duck_array(type(self._nom)):
-            self._err = new._err
-            self._nom = new._nom
-            return self
-        else:
-            return new
-
     def __mul__(self, other):
         if isinstance(other, Uncertainty):
             new_mag = self._nom * other._nom
             new_err = np.abs(new_mag) * np.sqrt(self.rel2 + other.rel2)
         else:
             new_mag = self._nom * other
             new_err = np.abs(self._err * other)
-
-        return self.__class__(new_mag, new_err)
+        try:
+            return self.__class__(new_mag, new_err)
+        except NotImplementedError:
+            return NotImplemented
 
     __rmul__ = __mul__
 
     @ignore_runtime_warnings
-    def __itruediv__(self, other):
-        new = self / other
-        if is_np_duck_array(type(self._nom)):
-            self._err = new._err
-            self._nom = new._nom
-            return self
-        else:
-            return new
-
-    @ignore_runtime_warnings
     def __truediv__(self, other):
-        # Self / Other
         if isinstance(other, Uncertainty):
             new_mag = self._nom / other._nom
             new_err = np.abs(new_mag) * np.sqrt(self.rel2 + other.rel2)
         else:
             new_mag = self._nom / other
             new_err = np.abs(self._err / other)
-        return self.__class__(new_mag, new_err)
+        try:
+            return self.__class__(new_mag, new_err)
+        except NotImplementedError:
+            return NotImplemented
 
     @ignore_runtime_warnings
     def __rtruediv__(self, other):
         # Other / Self
         if isinstance(other, Uncertainty):
             raise Exception
         else:
             new_mag = other / self._nom
             new_err = np.abs(new_mag) * np.abs(self.rel)
+        try:
             return self.__class__(new_mag, new_err)
+        except NotImplementedError:
+            return NotImplemented
 
     __div__ = __truediv__
     __rdiv__ = __rtruediv__
-    __idiv__ = __itruediv__
-
-    def __ifloordiv__(self, other):
-        new = self // other
-        if is_np_duck_array(type(self._nom)):
-            self._err = new._err
-            self._nom = new._nom
-            return self
-        else:
-            return new
 
     def __floordiv__(self, other):
         if isinstance(other, Uncertainty):
             new_mag = self._nom // other._nom
             new_err = 0.0
         else:
             new_mag = self._nom // other
@@ -465,23 +341,14 @@
         if isinstance(other, Uncertainty):
             return other.__truediv__(self)
         else:
             new_mag = other // self._nom
             new_err = 0.0
             return self.__class__(new_mag, new_err)
 
-    def __imod__(self, other):
-        new = self % other
-        if is_np_duck_array(type(self._nom)):
-            self._err = new._err
-            self._nom = new._nom
-            return self
-        else:
-            return new
-
     def __mod__(self, other):
         if isinstance(other, Uncertainty):
             new_mag = self._nom % other._nom
         else:
             new_mag = self._nom % other
         if np.ndim(new_mag) == 0:
             new_err = 0.0
@@ -499,34 +366,23 @@
 
     def __divmod__(self, other):
         return self // other, self % other
 
     def __rdivmod__(self, other):
         return other // self, other % self
 
-    def __ipow__(self, other):
-        new = self**other
-        if is_np_duck_array(type(self._nom)):
-            self._err = new._err
-            self._nom = new._nom
-            return self
-        else:
-            return new
-
     @ignore_runtime_warnings
     def __pow__(self, other):
         # Self ** other
         A = self._nom
         sA = self._err
         if isinstance(other, Uncertainty):
             B = other._nom
-            sB = other._err
         else:
             B = other
-            sB = 0
         new_mag = A**B
         new_err = np.abs(new_mag) * np.sqrt((B / A * sA) ** 2)
 
         return self.__class__(new_mag, new_err)
 
     @ignore_runtime_warnings
     def __rpow__(self, other):
@@ -554,15 +410,14 @@
         return self.__class__(round(self._nom, ndigits=ndigits), self._err)
 
     def __pos__(self):
         return self.__class__(operator.pos(self._nom), self._err)
 
     def __neg__(self):
         return self.__class__(operator.neg(self._nom), self._err)
-        return self.__class__(operator.neg(self._nom), self._err)
 
     def __eq__(self, other):
         if isinstance(other, Uncertainty):
             return self._nom == other._nom
         else:
             return self._nom == other
 
@@ -575,40 +430,44 @@
 
     def compare(self, other, op):
         if isinstance(other, Uncertainty):
             return op(self._nom, other._nom)
         else:
             return op(self._nom, other)
 
-    __lt__ = lambda self, other: self.compare(other, op=operator.lt)
-    __le__ = lambda self, other: self.compare(other, op=operator.le)
-    __ge__ = lambda self, other: self.compare(other, op=operator.ge)
-    __gt__ = lambda self, other: self.compare(other, op=operator.gt)
+    __lt__ = lambda self, other: self.compare(  # noqa: E731
+        other, op=operator.lt
+    )
+    __le__ = lambda self, other: self.compare(  # noqa: E731
+        other, op=operator.le
+    )
+    __ge__ = lambda self, other: self.compare(  # noqa: E731
+        other, op=operator.ge
+    )
+    __gt__ = lambda self, other: self.compare(  # noqa: E731
+        other, op=operator.gt
+    )
 
     def __bool__(self) -> bool:
         return bool(self._nom)
 
     __nonzero__ = __bool__
 
     # NumPy function/ufunc support
-    __array_priority__ = 17
-
     @ignore_runtime_warnings
     def __array_function__(self, func, types, args, kwargs):
-        # print(func)
         if func.__name__ not in HANDLED_FUNCTIONS:
             return NotImplemented
         elif not all(issubclass(t, self.__class__) for t in types):
             return NotImplemented
         else:
             return wrap_numpy("function", func, args, kwargs)
 
     @ignore_runtime_warnings
     def __array_ufunc__(self, ufunc, method, *args, **kwargs):
-        # print(method,ufunc.__name__)
         if method != "__call__":
             raise NotImplementedError
         else:
             if ufunc.__name__ not in HANDLED_UFUNCS:
                 raise NotImplementedError(
                     f"Ufunc {ufunc.__name__} is not implemented!"
                 ) from None
@@ -637,54 +496,28 @@
             )
         elif item in HANDLED_FUNCTIONS:
             return lambda *args, **kwargs: wrap_numpy(
                 "function", item, [self] + list(args), kwargs
             )
         elif item in self.__ndarray_attributes__:
             return getattr(self._nom, item)
-        elif hasattr(Quantity, item):
-            val = getattr(self._nom, item)
-            err = getattr(self._err, item)
-            if callable(val):
-
-                def expr(*args, **kwargs):
-                    try:
-                        vexpr = val(*args, **kwargs)
-                        eexpr = err(*args, **kwargs)
-                    except Exception:
-                        raise ValueError(
-                            f"Could not execute method {item} on Uncertainty elements!"
-                        )
-                    try:
-                        ret_instance = self.__class__(vexpr, eexpr)
-                    except Exception:
-                        raise ValueError(
-                            f"Could not execute instantiate Uncertainty class with results from method {item}!"
-                        )
-                    else:
-                        return ret_instance
-
-                return expr
-            else:
-                return self.__class__(val, err)
         else:
             raise AttributeError(
-                f"Attribute {item} not available in Uncertainty, as method of a Pint Quantity, or as NumPy ufunc or function."
+                f"Attribute {item} not available in Uncertainty, or as NumPy ufunc or function."
             ) from None
 
     def __array__(self, t=None) -> np.ndarray:
         warnings.warn(
             "The uncertainty is stripped when downcasting to ndarray.",
             NumpyDowncastWarning,
             stacklevel=2,
         )
         return np.asarray(self._nom)
 
     def clip(self, min=None, max=None, out=None, **kwargs):
-
         return self.__class__(
             self._nom.clip(min, max, out, **kwargs), self._err
         )
 
     def fill(self, value) -> None:
         return self._nom.fill(value)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auto_uncertainties-0.4.0/auto_uncertainties.egg-info/SOURCES.txt` & `auto_uncertainties-0.4.2/auto_uncertainties.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,8 +13,10 @@
 auto_uncertainties/wrap_numpy.py
 auto_uncertainties.egg-info/PKG-INFO
 auto_uncertainties.egg-info/SOURCES.txt
 auto_uncertainties.egg-info/dependency_links.txt
 auto_uncertainties.egg-info/requires.txt
 auto_uncertainties.egg-info/top_level.txt
 tests/test_numpy_wrap.py
+tests/test_pandas_extension.py
+tests/test_pandas_interface.py
 tests/test_uncertainty.py
```

### Comparing `auto_uncertainties-0.4.0/pyproject.toml` & `auto_uncertainties-0.4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 [project]
 name = "auto_uncertainties"
 authors = [
     {name = "Varchas Gopalaswamy", email = "vgop@lle.rochester.edu"},
 ]
 description = "Linear Uncertainty Propagation with Auto-Differentiation"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "h5py >= 1.23.0",
+    "numpy >= 1.23.0",
     "jax >= 0.3.14",
     "jaxlib >= 0.3.14",
-    "scipy >= 1.8.1",
-    "pint >= 0.20",
-    "pandas >= 1.5.1",
+    "joblib >= 1.2.0",
+    "loguru >= 0.6.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 CI = ["pytest", "pytest-cov","hypothesis","pylint"]
+pandas = ["pandas >= 1.5.1"]
 
 [build-system]
 requires = ["setuptools >= 67.0.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "auto_uncertainties/_version.py"
 
+[tool.ruff]
+line-length = 79
+target-version = "py311"
+ignore = ["E501"]
+
+[tool.ruff.isort]
+force-sort-within-sections = true
+required-imports = ["from __future__ import annotations"]
+
 
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
@@ -74,7 +83,23 @@
 redefined-builtin,
 too-few-public-methods,
 global-statement,
 no-member,
 no-else-return
 """
 ignore = "tests"
+
+[tool.pyright]
+pythonVersion = "3.11"
+pythonPlatform = "Linux"
+stubPath = "typings"
+typeCheckingMode = "basic"
+reportUnusedImport = "none"
+reportUnusedClass = "none"
+reportUnusedFunction = "none"
+reportUnusedVariable = "none"
+reportDuplicateImport = "none"
+reportPrivateImportUsage = "none"
+reportUntypedFunctionDecorator = true
+reportUntypedClassDecorator = true
+reportMissingImports = false
+exclude = ["install*", "public*", "**/tests*", "**/resources*"]
```

### Comparing `auto_uncertainties-0.4.0/tests/test_uncertainty.py` & `auto_uncertainties-0.4.2/tests/test_uncertainty.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import operator
 import warnings
-from typing import Type
 
 import hypothesis.strategies as st
 import numpy as np
-import pint
 import pytest
-from hypothesis import given, settings
+from hypothesis import given
 from hypothesis.extra import numpy as hnp
 
 from auto_uncertainties import NegativeStdDevError, Uncertainty
 
+try:
+    from pint import DimensionalityError
+except ImportError:
+
+    class DimensionalityError(Exception):
+        pass
+
+
 BINARY_OPS = [
     operator.lt,
     operator.le,
     operator.eq,
     operator.ne,
     operator.gt,
     operator.ge,
 ]
 UNARY_OPS = [operator.not_, operator.abs]
-unit_registry = pint.UnitRegistry()
-with warnings.catch_warnings():
-    warnings.simplefilter("ignore")
-    unit_registry.Quantity([])
-warnings.filterwarnings("ignore", category=pint.UnitStrippedWarning)
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
-unit_registry.enable_contexts("boltzmann")
-unit_registry.default_format = "0.8g~P"
-unit_registry.default_system = "cgs"
-UNITS = [None, unit_registry(""), unit_registry("m"), unit_registry("s")]
+UNITS = [None]
 
 
 def check_units_and_mag(unc, units, mag, err):
     if units is not None and not hasattr(unc, "units"):
         raise ValueError
     if units is None:
         assert unc.value == mag
@@ -46,50 +44,55 @@
         assert unc.units.is_compatible_with(units)
         assert unc.value.units.is_compatible_with(units)
         assert unc.value.to(units).m == mag
         assert unc.error.units.is_compatible_with(units)
         assert unc.error.to(units).m == err
 
 
+@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 @given(
     v=st.floats(allow_subnormal=False),
     e=st.floats(allow_subnormal=False),
     units=st.sampled_from(UNITS),
 )
 def test_scalar_creation(v, e, units):
     if e < 0:
         if np.isfinite(e):
             with pytest.raises(NegativeStdDevError):
                 u = Uncertainty(v, e)
             if units is not None:
                 with pytest.raises(NegativeStdDevError):
-                    u = Uncertainty(v * units, e * units)
+                    u = Uncertainty.from_quantities(v * units, e * units)
     else:
         u = Uncertainty(v, e)
         if np.isfinite(v) and np.isfinite(e):
-            assert u.nominal_value == v
+            assert u.value == v
             assert u.error == e
             if v > 0:
                 assert u.relative == e / v
             elif v == 0:
                 assert not np.isfinite(u.relative)
 
             if units is not None:
-                u = Uncertainty(v * units, e * units)
+                with pytest.raises(NotImplementedError):
+                    u = Uncertainty(v * units, e * units)
+
+                u = Uncertainty.from_quantities(v * units, e * units)
                 check_units_and_mag(u, units, v, e)
 
                 u = Uncertainty(v, e) * units
                 check_units_and_mag(u, units, v, e)
 
-                with pytest.raises(pint.DimensionalityError):
-                    u = Uncertainty(v * units, e)
-                with pytest.raises(pint.DimensionalityError):
-                    u = Uncertainty(v, e * units)
+                with pytest.raises(DimensionalityError):
+                    u = Uncertainty.from_quantities(v * units, e)
+                with pytest.raises(DimensionalityError):
+                    u = Uncertainty.from_quantities(v, e * units)
 
 
+@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 @given(
     v1=st.floats(allow_subnormal=False),
     e1=st.floats(min_value=0, max_value=1e3, allow_subnormal=False),
     op=st.sampled_from(UNARY_OPS),
 )
 def test_scalar_unary(v1, e1, op):
     u1 = Uncertainty(v1, e1)
@@ -100,14 +103,15 @@
             assert u.value == op(u1.value)
             if np.isfinite(e1):
                 assert np.isfinite(u.error)
         else:
             assert u == op(u1.value)
 
 
+@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 @given(
     v1=st.floats(allow_subnormal=False),
     v2=st.floats(allow_subnormal=False),
     e1=st.floats(min_value=0, max_value=1e3, allow_subnormal=False),
     e2=st.floats(min_value=0, max_value=1e3, allow_subnormal=False),
     op=st.sampled_from(BINARY_OPS),
 )
@@ -120,14 +124,15 @@
         assert u.value == op(u1.value, u2.value)
         if np.isfinite(e1) and np.isfinite(e2):
             assert np.isfinite(u.error)
     else:
         assert u == op(u1.value, u2.value)
 
 
+@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 @given(
     v1=st.floats(allow_subnormal=False),
     v2=st.floats(allow_subnormal=False),
     e1=st.floats(min_value=0, max_value=1e3, allow_subnormal=False),
     e2=st.floats(min_value=0, max_value=1e3, allow_subnormal=False),
     op=st.sampled_from([operator.add, operator.sub]),
 )
@@ -138,14 +143,15 @@
     u = op(u1, u2)
     if np.isfinite(v1) and np.isfinite(v2):
         assert u.value == op(u1.value, u2.value)
     if np.isfinite(e1) and np.isfinite(e2):
         assert u.error == np.sqrt(u1.error**2 + u2.error**2)
 
 
+@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 @given(
     v1=st.floats(min_value=1, max_value=1e3, allow_subnormal=False),
     v2=st.floats(min_value=1, max_value=1e3, allow_subnormal=False),
     e1=st.floats(min_value=0, max_value=1e3, allow_subnormal=False),
     e2=st.floats(min_value=0, max_value=1e3, allow_subnormal=False),
     op=st.sampled_from([operator.mul, operator.truediv]),
 )
@@ -158,14 +164,15 @@
         assert u.value == op(u1.value, u2.value)
     if np.isfinite(e1) and np.isfinite(e2):
         np.testing.assert_almost_equal(
             u.error, u.value * np.sqrt(u1.rel**2 + u2.rel**2)
         )
 
 
+@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 @given(
     v1=st.floats(min_value=0, max_value=1e3, allow_subnormal=False),
     v2=hnp.arrays(
         dtype=st.sampled_from([np.float64]),
         shape=(11,),
         elements=st.floats(
             min_value=-10.0,
@@ -189,14 +196,15 @@
             operator.mul,
             operator.truediv,
             operator.mod,
             operator.pow,
         ]
     ),
 )
+@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 def test_mixed_arithmetic(v1, e1, v2, e2, op):
     u1 = Uncertainty(v1, e1)
     u2 = Uncertainty(v2, e2)
 
     u = op(u1, u2)
     np.testing.assert_almost_equal(u.value, op(u1.value, u2.value))
```

