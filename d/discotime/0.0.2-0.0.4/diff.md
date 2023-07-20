# Comparing `tmp/discotime-0.0.2.tar.gz` & `tmp/discotime-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotime-0.0.2.tar", last modified: Wed Jun 14 08:00:19 2023, max compression
+gzip compressed data, was "discotime-0.0.4.tar", last modified: Thu Jul 20 11:11:23 2023, max compression
```

## Comparing `discotime-0.0.2.tar` & `discotime-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,39 @@
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.864440 discotime-0.0.2/
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1079 2022-12-20 15:34:43.000000 discotime-0.0.2/LICENSE
--rw-r--r--   0 pechris   (1000) pechris   (1000)       62 2023-01-18 09:20:28.000000 discotime-0.0.2/MANIFEST.in
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1463 2023-06-14 08:00:19.864440 discotime-0.0.2/PKG-INFO
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1064 2023-06-14 06:33:22.000000 discotime-0.0.2/README.md
--rw-r--r--   0 pechris   (1000) pechris   (1000)      122 2023-06-13 13:32:17.000000 discotime-0.0.2/pyproject.toml
--rw-r--r--   0 pechris   (1000) pechris   (1000)     2333 2023-06-14 08:00:19.864440 discotime-0.0.2/setup.cfg
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime/
--rw-r--r--   0 pechris   (1000) pechris   (1000)      106 2023-05-20 12:38:12.000000 discotime-0.0.2/src/discotime/__init__.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime/datasets/
--rw-r--r--   0 pechris   (1000) pechris   (1000)      152 2023-06-13 13:01:51.000000 discotime-0.0.2/src/discotime/datasets/__init__.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime/datasets/_data/
--rw-r--r--   0 pechris   (1000) pechris   (1000)        1 2023-06-13 14:19:52.000000 discotime-0.0.2/src/discotime/datasets/_data/.gitignore
--rw-r--r--   0 pechris   (1000) pechris   (1000)    49998 2023-06-13 14:17:42.000000 discotime-0.0.2/src/discotime/datasets/_data/mgus2.csv
--rw-r--r--   0 pechris   (1000) pechris   (1000)     5775 2023-06-13 14:17:31.000000 discotime-0.0.2/src/discotime/datasets/from_rstats.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)    11275 2023-06-13 18:44:19.000000 discotime-0.0.2/src/discotime/datasets/utils.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime/metrics/
--rw-r--r--   0 pechris   (1000) pechris   (1000)       91 2023-02-23 14:14:46.000000 discotime-0.0.2/src/discotime/metrics/__init__.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     4635 2023-06-12 13:59:45.000000 discotime-0.0.2/src/discotime/metrics/brier_score.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1922 2023-05-30 10:17:34.000000 discotime-0.0.2/src/discotime/metrics/ipa.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.864440 discotime-0.0.2/src/discotime/models/
--rw-r--r--   0 pechris   (1000) pechris   (1000)       63 2023-05-23 08:03:53.000000 discotime-0.0.2/src/discotime/models/__init__.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     5105 2023-05-23 12:44:07.000000 discotime-0.0.2/src/discotime/models/components.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)    10384 2023-06-12 12:40:34.000000 discotime-0.0.2/src/discotime/models/models.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.864440 discotime-0.0.2/src/discotime/utils/
--rw-r--r--   0 pechris   (1000) pechris   (1000)      112 2023-03-08 13:10:12.000000 discotime-0.0.2/src/discotime/utils/__init__.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     5802 2023-06-13 17:44:35.000000 discotime-0.0.2/src/discotime/utils/estimators.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     6566 2023-06-13 17:48:04.000000 discotime-0.0.2/src/discotime/utils/misc.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1274 2023-06-13 18:42:48.000000 discotime-0.0.2/src/discotime/utils/typing.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime.egg-info/
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1463 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/PKG-INFO
--rw-r--r--   0 pechris   (1000) pechris   (1000)      913 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/SOURCES.txt
--rw-r--r--   0 pechris   (1000) pechris   (1000)        1 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/dependency_links.txt
--rw-r--r--   0 pechris   (1000) pechris   (1000)      183 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/requires.txt
--rw-r--r--   0 pechris   (1000) pechris   (1000)       10 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/top_level.txt
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.864440 discotime-0.0.2/tests/
--rw-r--r--   0 pechris   (1000) pechris   (1000)      934 2023-06-13 13:03:24.000000 discotime-0.0.2/tests/test_lightning_module.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     3521 2023-05-30 10:38:15.000000 discotime-0.0.2/tests/test_metrics.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1427 2023-06-13 17:48:41.000000 discotime-0.0.2/tests/test_mgus2.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1867 2023-06-12 11:21:21.000000 discotime-0.0.2/tests/test_models.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1989 2023-06-06 19:49:32.000000 discotime-0.0.2/tests/test_preprocessing.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     3487 2023-05-22 14:09:38.000000 discotime-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-20 11:11:08.000000 discotime-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 11:11:08.000000 discotime-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-20 11:11:23.944746 discotime-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-20 11:11:08.000000 discotime-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 11:11:08.000000 discotime-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-20 11:11:23.944746 discotime-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.940746 discotime-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.940746 discotime-0.0.4/src/discotime/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/datasets/from_rstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/metrics/brier_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/utils/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_mgus2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_utils.py
```

### Comparing `discotime-0.0.2/LICENSE` & `discotime-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discotime-0.0.2/PKG-INFO` & `discotime-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotime
-Version: 0.0.2
+Version: 0.0.4
 Summary: Discrete-time competing risk analysis with neural networks
 Home-page: https://github.com/peterchristofferholm/discotime
 Author: Peter Holm
 Author-email: "Peter Holm" <petchdk@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `discotime-0.0.2/README.md` & `discotime-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `discotime-0.0.2/setup.cfg` & `discotime-0.0.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = discotime
-version = 0.0.2
+version = 0.0.4
 url = https://github.com/peterchristofferholm/discotime
 author = Peter Holm
 author_email = "Peter Holm" <petchdk@gmail.com>
 description = Discrete-time competing risk analysis with neural networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
@@ -82,28 +82,29 @@
 	types-termcolor
 commands = 
 	mypy --allow-redefinition --ignore-missing-imports {posargs:src tests}
 
 [testenv:docs]
 deps = 
 	sphinx
-	sphinx-rtd-theme
+	pydata-sphinx-theme
 commands = 
 	sphinx-apidoc \
 	--force \
 	--implicit-namespaces \
 	--module-first \
+	--separate \
 	-o docs/reference/ \
 	src/discotime/
 	sphinx-build -n -W --keep-going -b html docs/ docs/_build/
 
 [testenv:devdocs]
 deps = 
 	sphinx
-	sphinx-rtd-theme
+	pydata-sphinx-theme
 	sphinx-autobuild
 commands = 
 	sphinx-apidoc \
 	--force \
 	--implicit-namespaces \
 	--module-first \
 	--separate \
```

### Comparing `discotime-0.0.2/src/discotime/datasets/from_rstats.py` & `discotime-0.0.4/src/discotime/datasets/from_rstats.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.2/src/discotime/datasets/utils.py` & `discotime-0.0.4/src/discotime/datasets/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,18 @@
             features=self.features[index, ...],
             event_time_disc=self.event_time_disc[index],
             event_status_disc=self.event_status_disc[index],
             event_time_cont=self.event_time_cont[index],
             event_status_cont=self.event_status_cont[index],
         )
 
+    def __iter__(self):
+        for i in range(len(self)):
+            yield self[i]
+
 
 ###############################################################################
 
 
 @dataclass(kw_only=True)
 class DataConfig:
     """Configuration class for data modules."""
@@ -124,24 +128,36 @@
         return self._config
 
     @property
     def cuts(self) -> npt.NDArray[np.float_]:
         return self.lab_transformer.cuts
 
     @property
+    def dset_fit(self) -> SurvDataset:
+        if self._dset_fit is None:
+            raise AttributeError("`self._dset_fit` has not been prepared.")
+        return self._dset_fit
+
+    @property
+    def dset_test(self) -> SurvDataset:
+        if self._dset_test is None:
+            raise AttributeError("`self._dset_test` has not been prepared.")
+        return self._dset_test
+
+    @property
     def n_time_bins(self) -> int:
         return self.config.n_time_bins
 
     @property
     def batch_size(self) -> int:
         return self.config.batch_size
 
     @property
     @abstractmethod
-    def time_range(self) -> tuple[Num, Num]:
+    def time_range(self) -> tuple[float, float]:
         ...
 
     @property
     @abstractmethod
     def n_features(self) -> int:
         ...
 
@@ -232,15 +248,15 @@
     time: Iterable[Num],
     event: Iterable[Int],
 ) -> npt.NDArray[np.float64]:
     """Makes n groups with approx. equal number of observations."""
     _time, _event = map(np.asarray, (time, event))
     km = KaplanMeier(_time, (_event != 0).astype(np.int_))
     qs = np.linspace(1, km(max_time).item(), n_bins + 1)
-    return km.percentile(qs, dtype=np.float64)
+    return np.asarray(km.percentile(qs), dtype=np.float64)
 
 
 class LabelDiscretizer:
     """Discretize continous time/event pairs.
 
     The class can either learn a discretization grid from the training data
     using one of the built-in discretization schemes, or the user can supply an
```

### Comparing `discotime-0.0.2/src/discotime/models/components.py` & `discotime-0.0.4/src/discotime/models/components.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.2/src/discotime/models/models.py` & `discotime-0.0.4/src/discotime/models/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Optional, Any, Iterable, Callable, Dict
+from typing import Optional, Any, Callable, Dict
 from dataclasses import dataclass
 import warnings
 
 import torch
 from torch.nn import functional as F
 from torch import nn
 from lightning import pytorch as pl
-import numpy as np
 
 from discotime.models.components import Net, negative_log_likelihood
-from discotime.metrics import IPA
+from discotime.metrics import BrierScoreScaled
 from discotime.datasets import LitSurvDataModule
-from discotime.utils import interpolate2d
+from discotime.utils import Interpolate2D
 
 
 @dataclass(kw_only=True)
 class ModelConfig:
     learning_rate: float = 1e-3
     activation_function: str = "SiLU"
     """Name of activation function (str). The name needs to match one of the
@@ -126,26 +125,26 @@
         if self._eval_grid is None:
             raise AssertionError(
                 (
                     "`self.eval_grid` has not been instantiated."
                     "Try calling `self.setup()` first."
                 )
             )
-        return self._eval_grid
+        return self._eval_grid.to(self.device)
 
     @property
     def data_cuts(self) -> torch.Tensor:
         if self._data_cuts is None:
             raise AssertionError(
                 (
                     "`self.data_cuts` has not been instantiated."
                     "Try calling `self.setup()` first."
                 )
             )
-        return self._data_cuts
+        return self._data_cuts.to(self.device)
 
     def setup(self, stage):
         """Called at the beginning of fit (train + validate), validate, test,
         or predict. This is where the PyTorch model gets instantiated.
 
         Args:
             stage (`str`): either ``"fit"``, ``"validate"`` ``"test"`` or
@@ -182,24 +181,34 @@
 
         if stage in {"fit", "test", "validate"}:
             self.datamodule.setup()
 
             # get attributes from the datamodule
             self._data_cuts = torch.as_tensor(self.datamodule.cuts)
             if conf.evaluation_grid_cuts is not None:
-                self._eval_grid = torch.as_tensor(conf.evaluation_grid_cuts)
+                self._eval_grid = torch.as_tensor(
+                    conf.evaluation_grid_cuts, device=self.device
+                )
             else:
                 start, end = self.datamodule.time_range
                 self._eval_grid = torch.linspace(
-                    start=start, end=end, steps=conf.evaluation_grid_size  # type: ignore
+                    start=start,
+                    end=end,
+                    steps=conf.evaluation_grid_size,
+                    device=self.device,
                 )
 
             # instantiate metrics
-            self._metrics["IPA"] = IPA(
-                np.asarray(self.eval_grid, dtype=np.float_), integrate=True
+            self._metrics["IPA"] = BrierScoreScaled(
+                survival_train=(
+                    self.datamodule.dset_fit.event_time_cont,
+                    self.datamodule.dset_fit.event_status_cont,
+                ),
+                eval_grid=self.eval_grid,
+                integrate=True,
             )
 
     def on_save_checkpoint(self, checkpoint: Dict[str, Any]) -> None:
         checkpoint["model"] = self._model
 
     def on_load_checkpoint(self, checkpoint: Dict[str, Any]) -> None:
         self._model = checkpoint["model"]
@@ -237,42 +246,42 @@
         self._test_step_outputs.append(
             (self._predict_estimates(x, self.eval_grid), ct, ce)
         )
         return test_loss
 
     def on_test_epoch_end(self) -> None:
         estimates, ct, ce = map(
-            lambda x: torch.cat(x).cpu(), zip(*self._test_step_outputs)
+            lambda x: torch.cat(x), zip(*self._test_step_outputs)
         )
         self._test_step_outputs.clear()  # empty list
         for metric, metric_fn in self._metrics.items():
-            values = metric_fn(estimates, ct, ce)
+            values = metric_fn(estimates, (ct, ce))
             for cause, value in enumerate(values, start=1):
                 self.log(f"test_{metric}_cause{cause}", value)
 
     def on_validation_epoch_end(self) -> None:
         estimates, ct, ce = map(
             lambda x: torch.cat(x).cpu(), zip(*self._validation_step_outputs)
         )
         self._validation_step_outputs.clear()  # empty list
         for metric, metric_fn in self._metrics.items():
-            values = metric_fn(estimates, ct, ce)
+            values = metric_fn(estimates, (ct, ce))
             for cause, value in enumerate(values, start=1):
                 self.log(f"val_{metric}_cause{cause}", value)
 
     def _predict_estimates(
-        self, x: torch.Tensor, timepoints: torch.Tensor
+        self, x: torch.Tensor, timepoints: Any
     ) -> torch.Tensor:
-        c_haz = F.softmax(self(x), dim=-1)
+        est = F.softmax(self(x), dim=-1)
+        surv = torch.cumprod(est[..., [0]], dim=1)
 
-        s = torch.cumprod(c_haz[..., [0]], dim=1)
-        s_lag = torch.roll(s, shifts=1, dims=1)
-        s_lag[:, 0, :] = 1
+        surv_lag = torch.roll(surv, shifts=1, dims=1)
+        surv_lag[:, 0, :] = 1  # starts with 100%
 
         # convert conditional hazards to cause-specific cumulative incidence
-        proba = torch.cumsum(s_lag * c_haz[..., 1:], dim=1)
+        proba = torch.cumsum(surv_lag * est[..., 1:], dim=1)
         proba = F.pad(proba, pad=(0, 0, 1, 0))
 
-        return interpolate2d(timepoints, self.data_cuts, proba)
+        return Interpolate2D(self.data_cuts, proba, dim=1)(timepoints)
 
     def configure_optimizers(self) -> torch.optim.Optimizer:
         return torch.optim.Adam(self.model.parameters(), self.learning_rate)
```

### Comparing `discotime-0.0.2/src/discotime/utils/estimators.py` & `discotime-0.0.4/src/discotime/metrics/brier_score.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,168 +1,176 @@
-from typing import Optional
-from collections.abc import Iterable
+from typing import TypeVar
+from itertools import pairwise
 
-import numpy as np
-import numpy.typing as npt
 import torch
-from einops import repeat
+from discotime.utils import AalenJohansen, IPCW
 
-Int = int | np.int_
-Num = Int | float | np.float_
+TensorLike = TypeVar("TensorLike")
+"Object that can be converted to a tensor"
 
 
-def _tabulate(a, v, side="left"):
-    """Count interval occurences.
-
-    As an example, if side="left" and a=[1, 2, 3], then intervals are
-    (-inf, 1), [1, 2), [2, 3) and [3, inf)
-
-    Example:
-        >>> a, v = np.array([1, 2, 3]), np.array([0.5, 1, 2.5, 4])
-        >>> _tabulate(a, v)
-        array([2, 0, 1, 1])
-    """
-    return np.bincount(np.searchsorted(a, v, side=side))
-
-
-class KaplanMeier:
-    """Simple implementation of the Kaplan-Meier estimator.
+class BrierScore:
+    """Brier score of survival model with right-censored data.
 
     Args:
-        time: event times.
-        event: event indicator (0/1) where 0 is censoring.
-
-    Example:
-        >>> km = KaplanMeier(time=[0, 1.5, 1.3, 3], event=[0, 1, 0, 0])
-        >>> km(0)
-        array([1.])
-        >>> km([0, 1.0, 1.1, 1.5])
-        array([1. , 1. , 1. , 0.5])
+        survival_train: sequence of `t` timepoints to evaluate.
     """
 
-    def __init__(self, time: Iterable[Num], event: Iterable[Int]) -> None:
-        _time, _event = map(np.asarray, (time, event))
-        order = np.argsort(_time)
-        _time, _event = _time[order], _event[order]
-
-        # observed event times
-        tj = np.unique(np.pad(_time[_event == 1], (1, 0)))
+    @torch.no_grad()
+    def __init__(self, survival_train: tuple[TensorLike, TensorLike]) -> None:
+        futime, status = survival_train
+        futime = torch.as_tensor(futime).squeeze()
+        status = torch.as_tensor(status).squeeze()
 
-        def _pad(a):
-            return np.pad(a, (0, tj.size - a.size))
+        if futime.ndim > 1 or status.ndim > 1:
+            raise ValueError("`futime` and `status` should be 1D tensors")
 
-        mj = _pad(_tabulate(tj, _time[_event == 1], side="right")[1:])
-        qj = _pad(_tabulate(tj, _time[_event == 0], side="right")[1:])
+        self.ipcw = IPCW(futime, status)
 
-        nj = np.roll(_time.size - np.cumsum(mj + qj), 1)
-        nj[0] = _time.size
-
-        self._sj = np.cumprod((nj - mj) / nj)
-        self._nj, self._tj, self._mj = nj, tj, mj
-
-    def __call__(self, time: Num | Iterable[Num]) -> npt.NDArray[np.float_]:
-        """Obtain Kaplan-Meier estimates for each timepoint.
+    @torch.no_grad()
+    def __call__(
+        self,
+        estimates: TensorLike,
+        timepoints: TensorLike,
+        survival_test: tuple[TensorLike, TensorLike],
+    ) -> torch.Tensor:
+        """Calculate Brier score of survival model.
 
         Args:
-            time (num | seq[num]): `t`'s for which `km(t)` will be returned.
+            estimates: an array with shape (`m`, `t`, `e`), where `m` is the
+                batch size, `t` is the number of time bins, and `e` is number
+                of competing causes/risks.
+            timepoints: array of timepoints with size `t` at which the
+                values in `estimates` are obtained.
+            survival_test: tuple of observed time/event data.
         """
-        _time = np.atleast_1d(np.asanyarray(time))
-        return self._sj[np.searchsorted(self._tj, _time, side="right") - 1]
 
-    def percentile(
-        self, p: Iterable[Num], dtype=np.float64
-    ) -> npt.NDArray[np.float_]:
-        """Obtain approximate timepoint t such that P(t) = p.
+        St = torch.as_tensor(estimates)
+        n_obs, n_time, n_risks = St.shape
 
-        The stepwise Kaplan-Meier estimator is piecewise linearly interpolated
-        such that unique timepoints can be obtained.
-        """
-        p = np.atleast_1d(np.asanyarray(p, dtype=dtype))
-        if not np.all((0 <= p) & (p <= 1)):
+        tau = torch.as_tensor(timepoints)
+        if len(tau) != n_time:
             raise ValueError(
-                "p is a probability and should be between 0 and 1"
+                "size of `timepoints` do not match dim 1 of estimates."
             )
-        return np.interp(1 - p, 1 - self._sj, self._tj, left=0)
 
+        futime, status = survival_test
+        futime = torch.as_tensor(futime).squeeze()
+        status = torch.as_tensor(status).squeeze()
+
+        if futime.ndim > 1 or status.ndim > 1:
+            raise ValueError("`futime` and `status` should be 1D tensors")
+
+        if len(futime) != n_obs:
+            raise ValueError("length of `futime` is not equal to batch size.")
+
+        if len(status) != n_obs:
+            raise ValueError("length of `status` is not equal to batch size.")
+
+        # has individual experienced event of interest yet?
+        I1 = torch.logical_and(
+            futime.view(-1, 1, 1) <= tau.view(1, -1, 1),
+            status.view(-1, 1, 1) == torch.arange(1, n_risks + 1),
+        )
+        # ... did something else happen?
+        # fmt: off
+        I2 = (
+            (futime.view(-1, 1, 1) <= tau.view(1, -1, 1))
+            .logical_and(status.view(-1, 1, 1) != torch.zeros_like(I1))
+            .logical_and(status.view(-1, 1, 1) != torch.arange(1, n_risks + 1))
+        )
+        # fmt: on
+        # ... or is individual still in the risk set?
+        I3 = futime.view(-1, 1, 1) > tau.view(1, -1, 1)
+
+        # The IPCW is clamped such that one individual is not "dominating" the
+        # score. see Kvamme & Borgan. "The Brier Score under Administrative
+        # Censoring: Problems and a Solution."
+        Gt = torch.clamp(self.ipcw(tau, lag=0).reshape(1, -1, 1), min=1e-4)
+        GTi = torch.clamp(self.ipcw(futime, lag=1).reshape(-1, 1, 1), min=1e-4)
+
+        results = I1 * (1 - St) ** 2 / GTi
+        results += I2 * (St**2) / GTi
+        results += I3 * (St**2) / Gt
 
-class AalenJohansen:
-    """Obtain cumulative incidence curves with the Aalen-Johansen method.
+        return torch.mean(results, dim=0)
 
-    Args:
-        time: event times
-        event: event indicator (0/1/../c) with 0=censored
-        n_causes: how many causes should be included? If None (the default)
-            then all observed causes are include.
+
+class BrierScoreScaled:
+    """Index of prediction accuracy (IPA) for right-censored survival models.
+
+    In the context of survival analysis, the IPA is also known as the Brier
+    skill score (BSS).
     """
 
+    @torch.no_grad()
     def __init__(
         self,
-        time: npt.ArrayLike,
-        event: npt.ArrayLike,
-        n_causes: Optional[Int] = None,
+        survival_train: tuple[TensorLike, TensorLike],
+        eval_grid: TensorLike,
+        integrate: bool = False,
     ) -> None:
-        time, event = map(np.asarray, (time, event))
-
-        if time.ndim != 1:
-            raise ValueError(f"`time` is a {time.ndim}D array.")
-
-        if event.ndim != 1:
-            raise ValueError(f"`event` is a {event.ndim}D array.")
+        """
+        Args:
+            timepoints: sequence of `t` timepoints to evaluate.
+            causes: causes for which the brier score is calculated.
+            integrate: should the time-dependent IPA be integrated?
+                (default: True)
+        """
+        eval_grid = torch.as_tensor(eval_grid)
 
-        order = np.argsort(time)
-        time, event = time[order], event[order]
+        if len({*eval_grid}) != len(eval_grid):
+            raise ValueError("values in `timepoints` are not unique")
 
-        # find unique event times and add t=0 if it isn't present
-        tj = np.unique(np.pad(time, (1, 0)))
+        if not all(a <= b for a, b in pairwise(eval_grid)):
+            raise ValueError("values in `timepoints` are not sorted")
 
-        # number at risk at the start of each interval
-        nj = time.size - np.cumsum(_tabulate(tj, time, side="right"))
-        nj = nj[:-1]  # drop last
+        if integrate and len(eval_grid) == 1:
+            raise ValueError(
+                "at least two values in `timepoints` are required when "
+                "self.integrate = True"
+            )
 
-        def _pad(a):
-            """Add zeros to end of array to ensure it has same size as `tj`"""
-            assert (tj.size - a.size) >= 0
-            return np.pad(a, (0, tj.size - a.size), constant_values=0)
+        self.brier_score = BrierScore(survival_train=survival_train)
+        self.eval_grid = eval_grid
+        self.integrate = integrate
 
-        # number lost in each interval to any cause
-        mj = _pad(_tabulate(tj, time[event != 0]))
+    @torch.no_grad()
+    def __call__(
+        self,
+        estimates: TensorLike,
+        survival_test: tuple[TensorLike, TensorLike],
+    ) -> torch.Tensor:
+        """Calculate the index of prediction accuracy.
 
-        # lagged survival which starts with P(0) = 1
-        sj = np.cumprod((nj - mj) / nj)[:-1]
-        sj = np.pad(sj, (1, 0), constant_values=1)
+        Args:
+            estimates: array[batch, timepoints, cause]
+                model estimates of cause probabilities.
+            time: observed follow-up.
+            event: event indicator at time with 0 as censoring.
 
-        # cause-specific incidences
-        n_risks = n_causes if n_causes else np.max(event)
-        ci = np.zeros((tj.size, n_risks))
-        for e in range(1, n_risks + 1):
-            mcj = _pad(_tabulate(tj, time[event == e]))
-            ci[:, e - 1] = np.cumsum(sj * (mcj / nj))
+        If there are multiple timepoints to consider, then the IPA is
+        numerically integrated using the trapezoidal method.
+        """
+        phi_test = torch.as_tensor(estimates)
+        n_causes = phi_test.shape[-1]
+        tau = self.eval_grid
 
-        self._tj = tj
-        self._sj = sj
-        self._ci = ci
+        futime, status = survival_test
+        futime = torch.as_tensor(futime).squeeze()
+        status = torch.as_tensor(status).squeeze()
 
-    def __call__(self, timepoints: npt.ArrayLike) -> npt.NDArray[np.float64]:
-        """Return cause-specific cumulative incidence at given timepoints."""
-        tau = np.asanyarray(timepoints).reshape(-1)
-        idx = np.searchsorted(self._tj, tau, side="right")
-        idx = np.clip(idx - 1, a_min=0, a_max=(self._tj.size - 1))
-        return self._ci[idx]
+        cic = 1 - AalenJohansen(futime, status, n_causes)(tau)
+        phi_null = cic.unsqueeze(0).expand_as(phi_test)
 
+        bs_test = self.brier_score(phi_test, tau, survival_test)
+        bs_null = self.brier_score(phi_null, tau, survival_test)
 
-def interpolate2d(x: torch.Tensor, xp: torch.Tensor, yp: torch.Tensor):
-    """Perform stepwise linear interpolation of a discrete function.
+        if self.integrate:
+            bs_null = torch.trapezoid(bs_null, tau.view(-1, 1), dim=0)
+            bs_test = torch.trapezoid(bs_test, tau.view(-1, 1), dim=0)
 
-    _xp_ and _yp_ are tensors of values used to approximate f: y = f(x). This
-    functions uses interpolation to find the value of new points x.
+        # avoid zero division
+        bs_test[bs_null == 0] += 1e-10
+        bs_null[bs_null == 0] += 1e-10
 
-    Args:
-        x (:obj:`torch.Tensor`): an 1D tensor real values.
-        xp (:obj:`torch.Tensor`): an 1D tensor of real values.
-        yp (:obj:`torch.Tensor`): an ND tensor of real values. The length of yp
-            along the second axis (dim=1) must have the same length as xp.
-    """
-    x, xp = x.to(yp), xp.to(yp)  # move to same device
-    m = torch.diff(yp, dim=1) / repeat(torch.diff(xp, dim=0), "t -> 1 t 1")
-    b = yp[:, :-1, :] - torch.einsum("btr,t->btr", m, xp[:-1])
-    idx = torch.clamp_max(torch.searchsorted(xp, x), m.shape[1] - 1)
-    return m[:, idx, :] * repeat(x, "t -> 1 t 1") + b[:, idx, :]
+        return 1 - bs_test / bs_null
```

### Comparing `discotime-0.0.2/src/discotime/utils/misc.py` & `discotime-0.0.4/src/discotime/utils/misc.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.2/src/discotime/utils/typing.py` & `discotime-0.0.4/src/discotime/utils/typing.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.2/src/discotime.egg-info/PKG-INFO` & `discotime-0.0.4/src/discotime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotime
-Version: 0.0.2
+Version: 0.0.4
 Summary: Discrete-time competing risk analysis with neural networks
 Home-page: https://github.com/peterchristofferholm/discotime
 Author: Peter Holm
 Author-email: "Peter Holm" <petchdk@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `discotime-0.0.2/src/discotime.egg-info/SOURCES.txt` & `discotime-0.0.4/src/discotime.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 src/discotime.egg-info/SOURCES.txt
 src/discotime.egg-info/dependency_links.txt
 src/discotime.egg-info/requires.txt
 src/discotime.egg-info/top_level.txt
 src/discotime/datasets/__init__.py
 src/discotime/datasets/from_rstats.py
 src/discotime/datasets/utils.py
-src/discotime/datasets/_data/.gitignore
-src/discotime/datasets/_data/mgus2.csv
 src/discotime/metrics/__init__.py
 src/discotime/metrics/brier_score.py
-src/discotime/metrics/ipa.py
 src/discotime/models/__init__.py
 src/discotime/models/components.py
 src/discotime/models/models.py
 src/discotime/utils/__init__.py
 src/discotime/utils/estimators.py
 src/discotime/utils/misc.py
 src/discotime/utils/typing.py
```

### Comparing `discotime-0.0.2/tests/test_lightning_module.py` & `discotime-0.0.4/tests/test_lightning_module.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.2/tests/test_mgus2.py` & `discotime-0.0.4/tests/test_mgus2.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.2/tests/test_models.py` & `discotime-0.0.4/tests/test_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
 from pytest import approx
 from warnings import filterwarnings
+
+from lightning import Trainer
 import torch
 import torch.nn.functional as F
 
 from discotime.models import ModelConfig, LitSurvModule
 from discotime.datasets import Mgus2, DataConfig
 from discotime.models.components import negative_log_likelihood
 
@@ -54,7 +56,31 @@
             losses = (
                 model.validation_step(batch, batch_idx) * len(batch[1])
                 for batch_idx, batch in enumerate(dataset.train_dataloader())
             )
             return sum(losses) / len(dataset.dset_train)
 
     assert get_epoch_loss(mgus_bs30) == approx(get_epoch_loss(mgus_bs60))
+
+
+def test_model_output_shape():
+    filterwarnings("ignore", message=".*`self.log")
+    model = LitSurvModule(ModelConfig())
+    model.datamodule = Mgus2(
+        DataConfig(
+            batch_size=60,
+            n_time_bins=20,
+            discretization_scheme="number",
+        )
+    )
+    model.datamodule.setup(stage="fit")
+    model.setup(stage="fit")
+
+    X = torch.vstack(
+        [torch.tensor(d.features) for d in model.datamodule.dset_fit]
+    )
+
+    n_obs, n_time_bins, n_risks = X.shape[0], model.n_time_bins, model.n_risks
+
+    assert model(X).shape == (n_obs, n_time_bins, n_risks + 1)
+    assert model.predict_step(X, 0).shape == (n_obs, n_time_bins, n_risks + 1)
+    assert model._predict_estimates(X, [2, 3]).shape == (n_obs, 2, n_risks)
```

### Comparing `discotime-0.0.2/tests/test_preprocessing.py` & `discotime-0.0.4/tests/test_preprocessing.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,30 +31,30 @@
     event = [1, 1, 1, 1, 1]
     expected = [0, 1, 2, 3, 4, 5]
     cuts = _cuts_number(n_bins=5, max_time=5, time=time, event=event)
     assert cuts == pytest.approx(expected)
 
 
 class TestLabTransDiscrete:
-    def test_interval_discretization(self, comprisk_testdata):
-        time, event = comprisk_testdata
+    def test_interval_discretization(self, survival_data_2):
+        time, event = survival_data_2
         ltd = LabelDiscretizer("interval", 10)
         dt, de = ltd.fit_transform(time, event)
         assert len(set(dt)) == 10
         assert len(set(np.round(np.diff(ltd.cuts), 4))) == 1
-        assert len(set(map(lambda x: x.size, (time, event, dt, de)))) == 1
+        assert len(set(map(lambda x: len(x), (time, event, dt, de)))) == 1
 
-    def test_quantile_discretization(self, comprisk_testdata):
-        time, event = comprisk_testdata
+    def test_quantile_discretization(self, survival_data_2):
+        time, event = survival_data_2
         ltd = LabelDiscretizer("number", 10)
         dt, de = ltd.fit_transform(time, event)
         assert len(set(dt)) == 10
         assert len(set(np.diff(ltd.cuts))) != 1
-        assert len(set(map(lambda x: x.size, (time, event, dt, de)))) == 1
+        assert len(set(map(lambda x: len(x), (time, event, dt, de)))) == 1
 
-    def test_manual_discretization(self, comprisk_testdata):
-        time, event = comprisk_testdata
+    def test_manual_discretization(self, survival_data_2):
+        time, event = survival_data_2
         ltd = LabelDiscretizer(cut_points=[0, 5, 10, 15])
         with pytest.warns(UserWarning, match="ignoring fit()"):
             dt, de = ltd.fit_transform(time, event)
         assert len(set(dt)) == 3
-        assert len(set(map(lambda x: x.size, (time, event, dt, de)))) == 1
+        assert len(set(map(lambda x: len(x), (time, event, dt, de)))) == 1
```

### Comparing `discotime-0.0.2/tests/test_utils.py` & `discotime-0.0.4/tests/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,84 @@
 import torch
 import pytest
+from pytest import approx
 import hypothesis
 import hypothesis.strategies as st
 from einops import repeat
 
-from discotime.utils import KaplanMeier, AalenJohansen, interpolate2d
+from discotime.utils import KaplanMeier, AalenJohansen, Interpolate2D, IPCW
 
-###############################################################################
-# Kaplan-Meier estimator
+### KaplanMeier ###############################################################
 
 
 @pytest.fixture
-def km_example():
+def km_estimator():
     """Example data from p. 18 in Kleinbaum & Klein (2005)"""
     data = {
         1: [6, 6, 6, 7, 10, 13, 16, 22, 23],
-        0: [6, 9, 10, 11, 17, 19, 20, 25, 32, 32, 34, 45],
+        0: [6, 9, 10, 11, 17, 19, 20, 25, 32, 32, 34, 35],
     }
-    event, time = zip(*[(e, t) for (e, ts) in data.items() for t in ts])
+    time, event = zip(*[(t, e) for (e, ts) in data.items() for t in ts])
     return KaplanMeier(time, event)
 
 
 @pytest.mark.parametrize(
     ("time", "expected"),
     [
-        # fmt: off
-        # single timepoints
-        ( 0, 1.0000),
-        ( 6, 0.8571),
-        (10, 0.7529),
-        (22, 0.5378),
-        # multiple timepoints
-        ([ 6,  7], [0.8571, 0.8067]),
-        ([10, 22], [0.7529, 0.5378]),
-        # fmt: on
+        ([0], [1]),
+        (0, [1]),
+        ([0, 0], [1, 1]),
+        (6, [0.8571]),
+        (22, [0.5378]),
+        ([6, 7], [0.8571, 0.8067]),
+        ([7, 6], [0.8067, 0.8571]),
     ],
 )
-def test_kaplan_meier_estimates(time, expected, km_example):
-    assert km_example(time) == pytest.approx(expected, abs=1e-4)
+def test_kaplan_meier_estimates(time, expected, km_estimator):
+    assert km_estimator(time) == pytest.approx(expected, abs=1e-4)
 
 
-def test_kaplan_meier_percentiles(km_example):
-    t = km_example.percentile(km_example._sj)
-    assert all(km_example(t) == km_example._sj)
+def test_kaplan_meier_percentiles(km_estimator):
+    t = km_estimator.percentile(km_estimator._sj)
+    assert all(km_estimator(t) == km_estimator._sj)
 
 
 @pytest.mark.parametrize("percentile", [-1.1, 1.1])
-def test_kaplan_meier_percentiles_errors(percentile, km_example):
+def test_kaplan_meier_percentiles_errors(percentile, km_estimator):
     with pytest.raises(ValueError):
-        km_example.percentile(percentile)
+        km_estimator.percentile(percentile)
 
 
 # km.percentile should stop giving unique timepoints if p < P(t_max)
-def test_kaplan_meier_percentiles_unobserved(km_example):
-    t_max, p_min = km_example._tj[-1], km_example._sj[-1]
-    assert km_example.percentile(p_min - 0.05) == t_max
+def test_kaplan_meier_percentiles_unobserved(km_estimator):
+    t_max, p_min = km_estimator._tj[-1], km_estimator._sj[-1]
+    assert km_estimator.percentile(p_min - 0.05) == t_max
 
 
-###############################################################################
-# Aalen-Johansen estimator
+### IPCW ######################################################################
+
+
+def test_ipcw_1(survival_data_2):
+    time = [t for t, e in zip(*survival_data_2) if e == 0]
+    ipcw = IPCW(*survival_data_2)
+
+    assert ipcw(time, lag=0) == approx(
+        [0.95, 0.87083, 0.76198, 0.63498, 0.47624, 0.0], abs=1e-5
+    )
+    assert ipcw(time, lag=1) == approx(
+        [1.0, 0.95, 0.87083, 0.76198, 0.63498, 0.47624], abs=1e-5
+    )
+
+
+### AalenJohansen #############################################################
 
 
 @pytest.fixture
-def cic(comprisk_testdata):
-    time, event = comprisk_testdata
+def cic(survival_data_2):
+    time, event = survival_data_2
     return AalenJohansen(time, event)
 
 
 @pytest.mark.parametrize(
     ("timepoint", "cause", "expected"),
     [
         # fmt: off
@@ -106,13 +117,13 @@
 def test_interpolate2d_linear(args):
     x, xp, coef = args
 
     hypothesis.assume(torch.unique(xp).size() == xp.size())
     hypothesis.assume(torch.unique(x).size() == x.size())
 
     yp = coef[0] * xp + coef[1]
-    yp = repeat(yp, "t -> b t r", b=10, r=2)
+    yp = repeat(yp, "t -> b r t", b=10, r=2)
 
     y = coef[0] * x + coef[1]
-    y = repeat(y, "t -> b t r", b=10, r=2)
+    y = repeat(y, "t -> b r t", b=10, r=2)
 
-    assert interpolate2d(x, xp, yp) == pytest.approx(y, abs=1e-3)
+    assert Interpolate2D(xp, yp)(x) == pytest.approx(y, abs=1e-3)
```

