# Comparing `tmp/pyBKTR-0.1.0.tar.gz` & `tmp/pyBKTR-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBKTR-0.1.0.tar", last modified: Thu Jul 20 16:29:07 2023, max compression
+gzip compressed data, was "pyBKTR-0.1.1.tar", last modified: Thu Jul 20 17:44:58 2023, max compression
```

## Comparing `pyBKTR-0.1.0.tar` & `pyBKTR-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 16:29:07.501035 pyBKTR-0.1.0/
--rw-r--r--   0 juju       (501) staff       (20)     3802 2023-07-20 16:29:07.500807 pyBKTR-0.1.0/PKG-INFO
--rw-r--r--   0 juju       (501) staff       (20)     3169 2023-07-20 15:16:49.000000 pyBKTR-0.1.0/README.md
--rw-r--r--   0 juju       (501) staff       (20)     1343 2023-07-20 16:26:45.000000 pyBKTR-0.1.0/pyproject.toml
--rw-r--r--   0 juju       (501) staff       (20)       38 2023-07-20 16:29:07.501083 pyBKTR-0.1.0/setup.cfg
-drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 16:29:07.488741 pyBKTR-0.1.0/src/
-drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 16:29:07.493185 pyBKTR-0.1.0/src/pyBKTR/
--rw-r--r--   0 juju       (501) staff       (20)        0 2022-05-23 13:24:57.000000 pyBKTR-0.1.0/src/pyBKTR/__init__.py
--rw-r--r--   0 juju       (501) staff       (20)     3708 2023-06-01 23:19:20.000000 pyBKTR-0.1.0/src/pyBKTR/_likelihood_evaluator.py
--rw-r--r--   0 juju       (501) staff       (20)    18853 2023-07-19 02:19:57.000000 pyBKTR-0.1.0/src/pyBKTR/_result_logger.py
--rw-r--r--   0 juju       (501) staff       (20)     5923 2023-07-20 15:55:10.000000 pyBKTR-0.1.0/src/pyBKTR/_samplers.py
--rw-r--r--   0 juju       (501) staff       (20)    39643 2023-07-20 06:54:42.000000 pyBKTR-0.1.0/src/pyBKTR/bktr.py
-drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 16:29:07.498683 pyBKTR-0.1.0/src/pyBKTR/data/
--rw-r--r--   0 juju       (501) staff       (20)        0 2022-05-25 08:29:04.000000 pyBKTR-0.1.0/src/pyBKTR/data/__init__.py
--rw-r--r--   0 juju       (501) staff       (20)    72118 2023-07-19 02:01:22.000000 pyBKTR-0.1.0/src/pyBKTR/data/bixi_spatial_features.csv
--rw-r--r--   0 juju       (501) staff       (20)    39489 2023-06-01 15:43:27.000000 pyBKTR-0.1.0/src/pyBKTR/data/bixi_spatial_locations.csv
--rw-r--r--   0 juju       (501) staff       (20)   527060 2023-06-01 19:47:09.000000 pyBKTR-0.1.0/src/pyBKTR/data/bixi_station_departures.csv
--rw-r--r--   0 juju       (501) staff       (20)     6407 2023-06-01 19:47:09.000000 pyBKTR-0.1.0/src/pyBKTR/data/bixi_temporal_features.csv
--rw-r--r--   0 juju       (501) staff       (20)     2846 2023-06-01 15:43:27.000000 pyBKTR-0.1.0/src/pyBKTR/data/bixi_temporal_locations.csv
-drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 16:29:07.499334 pyBKTR-0.1.0/src/pyBKTR/data/raw_data/
--rw-r--r--   0 juju       (501) staff       (20)        0 2023-06-01 19:47:09.000000 pyBKTR-0.1.0/src/pyBKTR/data/raw_data/__init__.py
--rw-r--r--   0 juju       (501) staff       (20)     2155 2023-06-01 19:47:09.000000 pyBKTR-0.1.0/src/pyBKTR/data/raw_data/_bixi_cleanup.py
--rw-r--r--   0 juju       (501) staff       (20)     3247 2023-07-19 02:01:22.000000 pyBKTR-0.1.0/src/pyBKTR/distances.py
-drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 16:29:07.499846 pyBKTR-0.1.0/src/pyBKTR/examples/
--rw-r--r--   0 juju       (501) staff       (20)        0 2022-05-25 09:20:29.000000 pyBKTR-0.1.0/src/pyBKTR/examples/__init__.py
--rw-r--r--   0 juju       (501) staff       (20)     1608 2023-07-05 02:01:18.000000 pyBKTR-0.1.0/src/pyBKTR/examples/bixi.py
--rw-r--r--   0 juju       (501) staff       (20)    11788 2023-07-19 02:01:22.000000 pyBKTR-0.1.0/src/pyBKTR/kernels.py
--rw-r--r--   0 juju       (501) staff       (20)    15812 2023-07-19 02:01:22.000000 pyBKTR-0.1.0/src/pyBKTR/plots.py
--rw-r--r--   0 juju       (501) staff       (20)     3468 2023-07-20 15:52:33.000000 pyBKTR-0.1.0/src/pyBKTR/tensor_ops.py
--rw-r--r--   0 juju       (501) staff       (20)    10265 2023-07-20 15:57:00.000000 pyBKTR-0.1.0/src/pyBKTR/utils.py
-drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 16:29:07.494138 pyBKTR-0.1.0/src/pyBKTR.egg-info/
--rw-r--r--   0 juju       (501) staff       (20)     3802 2023-07-20 16:29:07.000000 pyBKTR-0.1.0/src/pyBKTR.egg-info/PKG-INFO
--rw-r--r--   0 juju       (501) staff       (20)      818 2023-07-20 16:29:07.000000 pyBKTR-0.1.0/src/pyBKTR.egg-info/SOURCES.txt
--rw-r--r--   0 juju       (501) staff       (20)        1 2023-07-20 16:29:07.000000 pyBKTR-0.1.0/src/pyBKTR.egg-info/dependency_links.txt
--rw-r--r--   0 juju       (501) staff       (20)      198 2023-07-20 16:29:07.000000 pyBKTR-0.1.0/src/pyBKTR.egg-info/requires.txt
--rw-r--r--   0 juju       (501) staff       (20)        7 2023-07-20 16:29:07.000000 pyBKTR-0.1.0/src/pyBKTR.egg-info/top_level.txt
+drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 17:44:58.698708 pyBKTR-0.1.1/
+-rw-r--r--   0 juju       (501) staff       (20)     1072 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/LICENSE
+-rw-r--r--   0 juju       (501) staff       (20)     4322 2023-07-20 17:44:58.698537 pyBKTR-0.1.1/PKG-INFO
+-rw-r--r--   0 juju       (501) staff       (20)     3597 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/README.md
+-rw-r--r--   0 juju       (501) staff       (20)     1414 2023-07-20 17:44:53.000000 pyBKTR-0.1.1/pyproject.toml
+-rw-r--r--   0 juju       (501) staff       (20)       38 2023-07-20 17:44:58.698757 pyBKTR-0.1.1/setup.cfg
+drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 17:44:58.690507 pyBKTR-0.1.1/src/
+drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 17:44:58.694452 pyBKTR-0.1.1/src/pyBKTR/
+-rw-r--r--   0 juju       (501) staff       (20)        0 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/__init__.py
+-rw-r--r--   0 juju       (501) staff       (20)     3708 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/_likelihood_evaluator.py
+-rw-r--r--   0 juju       (501) staff       (20)    18853 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/_result_logger.py
+-rw-r--r--   0 juju       (501) staff       (20)     5923 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/_samplers.py
+-rw-r--r--   0 juju       (501) staff       (20)    39643 2023-07-20 17:44:53.000000 pyBKTR-0.1.1/src/pyBKTR/bktr.py
+drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 17:44:58.697571 pyBKTR-0.1.1/src/pyBKTR/data/
+-rw-r--r--   0 juju       (501) staff       (20)        0 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/data/__init__.py
+-rw-r--r--   0 juju       (501) staff       (20)    72118 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/data/bixi_spatial_features.csv
+-rw-r--r--   0 juju       (501) staff       (20)    39489 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/data/bixi_spatial_locations.csv
+-rw-r--r--   0 juju       (501) staff       (20)   527060 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/data/bixi_station_departures.csv
+-rw-r--r--   0 juju       (501) staff       (20)     6407 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/data/bixi_temporal_features.csv
+-rw-r--r--   0 juju       (501) staff       (20)     2846 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/data/bixi_temporal_locations.csv
+drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 17:44:58.698050 pyBKTR-0.1.1/src/pyBKTR/data/raw_data/
+-rw-r--r--   0 juju       (501) staff       (20)        0 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/data/raw_data/__init__.py
+-rw-r--r--   0 juju       (501) staff       (20)     2155 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/data/raw_data/_bixi_cleanup.py
+-rw-r--r--   0 juju       (501) staff       (20)     3247 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/distances.py
+drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 17:44:58.698306 pyBKTR-0.1.1/src/pyBKTR/examples/
+-rw-r--r--   0 juju       (501) staff       (20)        0 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/examples/__init__.py
+-rw-r--r--   0 juju       (501) staff       (20)     1608 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/examples/bixi.py
+-rw-r--r--   0 juju       (501) staff       (20)    11788 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/kernels.py
+-rw-r--r--   0 juju       (501) staff       (20)    15812 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/plots.py
+-rw-r--r--   0 juju       (501) staff       (20)     3468 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/tensor_ops.py
+-rw-r--r--   0 juju       (501) staff       (20)    10265 2023-07-20 17:20:09.000000 pyBKTR-0.1.1/src/pyBKTR/utils.py
+drwxr-xr-x   0 juju       (501) staff       (20)        0 2023-07-20 17:44:58.695257 pyBKTR-0.1.1/src/pyBKTR.egg-info/
+-rw-r--r--   0 juju       (501) staff       (20)     4322 2023-07-20 17:44:58.000000 pyBKTR-0.1.1/src/pyBKTR.egg-info/PKG-INFO
+-rw-r--r--   0 juju       (501) staff       (20)      826 2023-07-20 17:44:58.000000 pyBKTR-0.1.1/src/pyBKTR.egg-info/SOURCES.txt
+-rw-r--r--   0 juju       (501) staff       (20)        1 2023-07-20 17:44:58.000000 pyBKTR-0.1.1/src/pyBKTR.egg-info/dependency_links.txt
+-rw-r--r--   0 juju       (501) staff       (20)      198 2023-07-20 17:44:58.000000 pyBKTR-0.1.1/src/pyBKTR.egg-info/requires.txt
+-rw-r--r--   0 juju       (501) staff       (20)        7 2023-07-20 17:44:58.000000 pyBKTR-0.1.1/src/pyBKTR.egg-info/top_level.txt
```

### Comparing `pyBKTR-0.1.0/PKG-INFO` & `pyBKTR-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: pyBKTR
-Version: 0.1.0
-Summary: Python implementation of the Scalable Spatiotemporally Varying Coefficient Modelling with Bayesian Kernelized Tensor Regression
-Author: Mengying Lei, Aurelie Labbe, Lijun Sun
-Author-email: Julien Lanthier <julien.lanthier@hec.ca>
-Project-URL: Homepage, https://github.com/julien-hec/pyBKTR
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <4,>=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # pyBKTR
 
 ## Intro
 This project is a *Python* implementation of the BKTR algorithm presented by Mengying Lei, Aurélie Labbe & Lijun Sun (2023).
 The article presenting the algorithm can be found [here](https://arxiv.org/abs/2109.00046).
 
 BKTR stands for Scalable Spatiotemporally Varying Coefficient Modelling with Bayesian Kernelized Tensor Regression.
 It allows to model spatiotemporally varying coefficients using a Bayesian framework.
 We implemented the algorithm and more in a *Python* package that uses [PyTorch](https://pytorch.org/) as a tensor operation backend.
 
-For information, an alternative *R* implementation of the algorithm can be found [here](https://github.com/julien-hec/BKTR). The *Python* implementation is synchronized with this repository and development is done in parallel.
+For information, an alternative *R* implementation of the algorithm can be found [here](https://github.com/julien-hec/BKTR). The *Python* implementation is synchronized with this repository and development is done in parallel. The synchronization of features will be done at a subrevision level (x.y.0).
 
 An article presenting the *R* package in details is currently in preparation and should be available soon. The documentation for the *R* package is a work in progress and will be made available in the coming weeks.
 
 ## Installation
 
 ### Install from PyPI
 The package is available on PyPI and can be installed using pip:
@@ -42,23 +27,24 @@
 ```
 
 ## Simple Example
 To verify that everything is running smooth you can try to run a BKTR regression on the BIXI data presented in the package. (The data is already preloaded in the package in the `BixiData` class)
 
 The following code will run a BKTR regression using sensible defaults on the BIXI data and print a summary of the results.
 ```python
-library(BKTR)
 from pyBKTR.bktr import BKTRRegressor
-from pyBKTR.examples import BixiData
+from pyBKTR.examples.bixi import BixiData
 
 bixi_data = BixiData()
 bktr_regressor = BKTRRegressor(
     data_df=bixi_data.data_df,
     spatial_positions_df=bixi_data.spatial_positions_df,
-    temporal_positions_df=bixi_data.temporal_positions_df
+    temporal_positions_df=bixi_data.temporal_positions_df,
+    burn_in_iter=5,
+    sampling_iter=10
 )
 bktr_regressor.mcmc_sampling()
 print(bktr_regressor.summary)
 ```
 
 ## Contributing
 Contributions are welcome. Do not hesitate to open an issue or a pull request if you encounter any problem or have any suggestion.
@@ -94,7 +80,21 @@
 ```bash
 sphinx-apidoc -f -o . ../pyBKTR
 ```
 then
 ```bash
 make html
 ```
+
+### Publish to PyPI
+First build the package locally
+```bash
+python3 -m pip install --upgrade build
+python3 -m build
+```
+
+Then upload to PyPI
+```bash
+python3 -m pip install --upgrade twine
+python3 -m upload dist/*
+```
+Using the proper credentials, the package should be uploaded to PyPI and be available for download.
```

### Comparing `pyBKTR-0.1.0/pyproject.toml` & `pyBKTR-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyBKTR"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python implementation of the Scalable Spatiotemporally Varying Coefficient Modelling with Bayesian Kernelized Tensor Regression"
 readme = "README.md"
 authors = [
     {name = "Julien Lanthier", email = "julien.lanthier@hec.ca"},
     {name = "Mengying Lei"},
     {name = "Aurelie Labbe"},
     {name = "Lijun Sun"},
 ]
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
 ]
-urls = {Homepage = "https://github.com/julien-hec/pyBKTR"}
 requires-python = ">=3.10, <4"
 dependencies = [
     "torch>=1.12.1",
     "numpy>=1.22.3",
     "pandas>=1.4.2",
     "plotly>=5.10.0",
     "formulaic>=0.5.2",
 ]
 
+[project.urls]
+"Homepage" = "https://github.com/julien-hec/pyBKTR"
+"Bug Tracker" = "https://github.com/julien-hec/pyBKTR/issues"
+
 [project.optional-dependencies]
 dev = [
     "black==22.6.0",
     "flake8==4.0.1",
     "pre-commit==2.20.0",
     "Sphinx==6.1.3",
     "sphinx-rtd-theme==1.2.0",
```

### Comparing `pyBKTR-0.1.0/src/pyBKTR/_likelihood_evaluator.py` & `pyBKTR-0.1.1/src/pyBKTR/_likelihood_evaluator.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/_result_logger.py` & `pyBKTR-0.1.1/src/pyBKTR/_result_logger.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/_samplers.py` & `pyBKTR-0.1.1/src/pyBKTR/_samplers.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/bktr.py` & `pyBKTR-0.1.1/src/pyBKTR/bktr.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         Returns:
             tuple[pd.DataFrame, pd.DataFrame]: A tuple of two dataframes. The first
             represents the beta forecasted for all new spatial locations or temporal points.
             The second represents the forecasted response for all new spatial locations or
             temporal points.
         """
         ini_fp_type = TSR.fp_type
-        TSR.set_params(fp_type = 'float64')
+        TSR.set_params(fp_type='float64')
 
         self._pred_valid_and_sort_data(
             new_data_df, new_spatial_positions_df, new_temporal_positions_df
         )
 
         spatial_positions_df = (
             pd.concat([self.spatial_positions_df, new_spatial_positions_df], axis=0)
@@ -327,38 +327,36 @@
 
         new_betas = all_betas.mean(dim=-1)
         _, x_df = self._get_x_and_y_dfs_from_formula(data_df, self.formula)
         covariates = TSR.tensor(x_df.to_numpy()).reshape(
             [len(spatial_positions_df), len(temporal_positions_df), -1]
         )
         new_y_est = torch.einsum('ijk,ijk->ij', [new_betas, covariates])
-        data_df_index = pd.MultiIndex.from_tuples(
-            data_df_index_tups, names=['location', 'time']
-        )
+        data_df_index = pd.MultiIndex.from_tuples(data_df_index_tups, names=['location', 'time'])
         new_beta_df = pd.DataFrame(
-            new_betas.flatten(0, 1),
+            new_betas.flatten(0, 1).cpu().numpy(),
             index=data_df_index,
             columns=x_df.columns,
         )
         new_y_df = pd.DataFrame(
-            new_y_est.flatten(),
+            new_y_est.flatten().cpu().numpy(),
             index=data_df_index,
             columns=['y'],
         )
         new_locs = new_spatial_positions_df.index.get_level_values(0).unique()
         new_times = new_temporal_positions_df.index.get_level_values(0).unique()
         new_beta_df = new_beta_df[
-            (new_beta_df.index.get_level_values(0).isin(new_locs)) |
-            (new_beta_df.index.get_level_values(1).isin(new_times))
+            (new_beta_df.index.get_level_values(0).isin(new_locs))
+            | (new_beta_df.index.get_level_values(1).isin(new_times))
         ]
         new_y_df = new_y_df[
-            (new_y_df.index.get_level_values(0).isin(new_locs)) |
-            (new_y_df.index.get_level_values(1).isin(new_times))
+            (new_y_df.index.get_level_values(0).isin(new_locs))
+            | (new_y_df.index.get_level_values(1).isin(new_times))
         ]
-        TSR.set_params(fp_type = ini_fp_type)
+        TSR.set_params(fp_type=ini_fp_type)
         return new_y_df, new_beta_df
 
     @property
     def summary(self) -> str:
         """Returns a summary of the MCMC regressor results
 
         Raises:
@@ -795,15 +793,15 @@
         new_old_cov = cov_mat[-nb_new_pos:, :-nb_new_pos]
         old_new_cov = cov_mat[:-nb_new_pos, -nb_new_pos:]
         new_cov = cov_mat[-nb_new_pos:, -nb_new_pos:]
         new_decomp_mus = new_old_cov @ old_cov.inverse() @ old_decomp
         new_decomp_cov = new_cov - (new_old_cov @ old_cov.inverse() @ old_new_cov)
         new_decomp_cov = (new_decomp_cov + new_decomp_cov.T) / 2
         if jitter is not None:
-            new_decomp_cov += jitter * torch.eye(new_decomp_cov.shape[0])
+            new_decomp_cov += jitter * TSR.eye(new_decomp_cov.shape[0])
         new_decomp = (
             torch.distributions.MultivariateNormal(new_decomp_mus.T, new_decomp_cov).sample().T
         )
         return torch.concat([old_decomp, new_decomp], dim=0)
 
     @staticmethod
     def _check_pred_dfs_integrity(
```

### Comparing `pyBKTR-0.1.0/src/pyBKTR/data/bixi_spatial_features.csv` & `pyBKTR-0.1.1/src/pyBKTR/data/bixi_spatial_features.csv`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/data/bixi_spatial_locations.csv` & `pyBKTR-0.1.1/src/pyBKTR/data/bixi_spatial_locations.csv`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/data/bixi_station_departures.csv` & `pyBKTR-0.1.1/src/pyBKTR/data/bixi_station_departures.csv`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/data/bixi_temporal_features.csv` & `pyBKTR-0.1.1/src/pyBKTR/data/bixi_temporal_features.csv`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/data/bixi_temporal_locations.csv` & `pyBKTR-0.1.1/src/pyBKTR/data/bixi_temporal_locations.csv`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/data/raw_data/_bixi_cleanup.py` & `pyBKTR-0.1.1/src/pyBKTR/data/raw_data/_bixi_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/distances.py` & `pyBKTR-0.1.1/src/pyBKTR/distances.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/examples/bixi.py` & `pyBKTR-0.1.1/src/pyBKTR/examples/bixi.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/kernels.py` & `pyBKTR-0.1.1/src/pyBKTR/kernels.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/plots.py` & `pyBKTR-0.1.1/src/pyBKTR/plots.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/tensor_ops.py` & `pyBKTR-0.1.1/src/pyBKTR/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR/utils.py` & `pyBKTR-0.1.1/src/pyBKTR/utils.py`

 * *Files identical despite different names*

### Comparing `pyBKTR-0.1.0/src/pyBKTR.egg-info/PKG-INFO` & `pyBKTR-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: pyBKTR
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of the Scalable Spatiotemporally Varying Coefficient Modelling with Bayesian Kernelized Tensor Regression
 Author: Mengying Lei, Aurelie Labbe, Lijun Sun
 Author-email: Julien Lanthier <julien.lanthier@hec.ca>
 Project-URL: Homepage, https://github.com/julien-hec/pyBKTR
+Project-URL: Bug Tracker, https://github.com/julien-hec/pyBKTR/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
 
 # pyBKTR
 
 ## Intro
 This project is a *Python* implementation of the BKTR algorithm presented by Mengying Lei, Aurélie Labbe & Lijun Sun (2023).
 The article presenting the algorithm can be found [here](https://arxiv.org/abs/2109.00046).
 
 BKTR stands for Scalable Spatiotemporally Varying Coefficient Modelling with Bayesian Kernelized Tensor Regression.
 It allows to model spatiotemporally varying coefficients using a Bayesian framework.
 We implemented the algorithm and more in a *Python* package that uses [PyTorch](https://pytorch.org/) as a tensor operation backend.
 
-For information, an alternative *R* implementation of the algorithm can be found [here](https://github.com/julien-hec/BKTR). The *Python* implementation is synchronized with this repository and development is done in parallel.
+For information, an alternative *R* implementation of the algorithm can be found [here](https://github.com/julien-hec/BKTR). The *Python* implementation is synchronized with this repository and development is done in parallel. The synchronization of features will be done at a subrevision level (x.y.0).
 
 An article presenting the *R* package in details is currently in preparation and should be available soon. The documentation for the *R* package is a work in progress and will be made available in the coming weeks.
 
 ## Installation
 
 ### Install from PyPI
 The package is available on PyPI and can be installed using pip:
@@ -42,23 +44,24 @@
 ```
 
 ## Simple Example
 To verify that everything is running smooth you can try to run a BKTR regression on the BIXI data presented in the package. (The data is already preloaded in the package in the `BixiData` class)
 
 The following code will run a BKTR regression using sensible defaults on the BIXI data and print a summary of the results.
 ```python
-library(BKTR)
 from pyBKTR.bktr import BKTRRegressor
-from pyBKTR.examples import BixiData
+from pyBKTR.examples.bixi import BixiData
 
 bixi_data = BixiData()
 bktr_regressor = BKTRRegressor(
     data_df=bixi_data.data_df,
     spatial_positions_df=bixi_data.spatial_positions_df,
-    temporal_positions_df=bixi_data.temporal_positions_df
+    temporal_positions_df=bixi_data.temporal_positions_df,
+    burn_in_iter=5,
+    sampling_iter=10
 )
 bktr_regressor.mcmc_sampling()
 print(bktr_regressor.summary)
 ```
 
 ## Contributing
 Contributions are welcome. Do not hesitate to open an issue or a pull request if you encounter any problem or have any suggestion.
@@ -94,7 +97,21 @@
 ```bash
 sphinx-apidoc -f -o . ../pyBKTR
 ```
 then
 ```bash
 make html
 ```
+
+### Publish to PyPI
+First build the package locally
+```bash
+python3 -m pip install --upgrade build
+python3 -m build
+```
+
+Then upload to PyPI
+```bash
+python3 -m pip install --upgrade twine
+python3 -m upload dist/*
+```
+Using the proper credentials, the package should be uploaded to PyPI and be available for download.
```

### Comparing `pyBKTR-0.1.0/src/pyBKTR.egg-info/SOURCES.txt` & `pyBKTR-0.1.1/src/pyBKTR.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 src/pyBKTR/__init__.py
 src/pyBKTR/_likelihood_evaluator.py
 src/pyBKTR/_result_logger.py
 src/pyBKTR/_samplers.py
 src/pyBKTR/bktr.py
```

