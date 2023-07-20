# Comparing `tmp/meld-1.0.0.tar.gz` & `tmp/meld-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/MELD/MELD/dist/tmpo0tpgad7/meld-1.0.0.tar", last modified: Thu Dec 10 17:45:06 2020, max compression
+gzip compressed data, was "meld-1.0.2.tar", last modified: Thu Jul 20 12:39:08 2023, max compression
```

## Comparing `meld-1.0.0.tar` & `meld-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 17:45:06.000000 meld-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)     4384 2020-12-10 17:45:06.000000 meld-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2838 2020-12-10 17:45:03.000000 meld-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 17:45:06.000000 meld-1.0.0/meld/
--rw-r--r--   0 runner    (1001) docker     (116)      263 2020-12-10 17:45:03.000000 meld-1.0.0/meld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6506 2020-12-10 17:45:03.000000 meld-1.0.0/meld/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (116)    12916 2020-12-10 17:45:03.000000 meld-1.0.0/meld/cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)     1795 2020-12-10 17:45:03.000000 meld-1.0.0/meld/filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     9253 2020-12-10 17:45:03.000000 meld-1.0.0/meld/meld.py
--rw-r--r--   0 runner    (1001) docker     (116)     1381 2020-12-10 17:45:03.000000 meld-1.0.0/meld/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)       78 2020-12-10 17:45:03.000000 meld-1.0.0/meld/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 17:45:06.000000 meld-1.0.0/meld.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4384 2020-12-10 17:45:06.000000 meld-1.0.0/meld.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      336 2020-12-10 17:45:06.000000 meld-1.0.0/meld.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-10 17:45:06.000000 meld-1.0.0/meld.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      225 2020-12-10 17:45:06.000000 meld-1.0.0/meld.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2020-12-10 17:45:06.000000 meld-1.0.0/meld.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      200 2020-12-10 17:45:06.000000 meld-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2020-12-10 17:45:03.000000 meld-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 17:45:06.000000 meld-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1603 2020-12-10 17:45:03.000000 meld-1.0.0/test/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (116)    12573 2020-12-10 17:45:03.000000 meld-1.0.0/test/test_meld.py
--rw-r--r--   0 runner    (1001) docker     (116)      902 2020-12-10 17:45:03.000000 meld-1.0.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:39:08.838149 meld-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-20 12:38:58.000000 meld-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    34539 2023-07-20 12:38:58.000000 meld-1.0.2/LICENSE-GPL3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-20 12:39:08.838149 meld-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-20 12:38:58.000000 meld-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:39:08.834149 meld-1.0.2/meld/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 12:38:58.000000 meld-1.0.2/meld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-20 12:38:58.000000 meld-1.0.2/meld/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-07-20 12:38:58.000000 meld-1.0.2/meld/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-20 12:38:58.000000 meld-1.0.2/meld/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-07-20 12:38:58.000000 meld-1.0.2/meld/meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-20 12:38:58.000000 meld-1.0.2/meld/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 12:38:58.000000 meld-1.0.2/meld/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:39:08.838149 meld-1.0.2/meld.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-20 12:39:08.000000 meld-1.0.2/meld.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 12:39:08.000000 meld-1.0.2/meld.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:39:08.000000 meld-1.0.2/meld.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-20 12:39:08.000000 meld-1.0.2/meld.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 12:39:08.000000 meld-1.0.2/meld.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-20 12:39:08.838149 meld-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-20 12:38:58.000000 meld-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:39:08.838149 meld-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-20 12:38:58.000000 meld-1.0.2/test/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-20 12:38:58.000000 meld-1.0.2/test/test_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-20 12:38:58.000000 meld-1.0.2/test/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `meld-1.0.0/PKG-INFO` & `meld-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 Metadata-Version: 2.1
 Name: meld
-Version: 1.0.0
+Version: 1.0.2
 Summary: MELD
 Home-page: https://github.com/KrishnaswamyLab/MELD
+Download-URL: https://github.com/KrishnaswamyLab/MELD/archive/v1.0.2.tar.gz
 Author: Daniel Burkhardt, Krishnaswamy Lab, Yale University
 Author-email: daniel.burkhardt@yale.edu
 License: Dual License - See LICENSE file
-Download-URL: https://github.com/KrishnaswamyLab/MELD/archive/v1.0.0.tar.gz
-Description: # MELD
-        ### Quantifying the effect of experimental perturbations at single-cell resolution
-        
-        
-        [![Latest PyPi version](https://img.shields.io/pypi/v/MELD.svg)](https://pypi.org/project/MELD/)
-        ![GitHub Actions](https://github.com/KrishnaswamyLab/MELD/workflows/Unit%20Tests/badge.svg)
-        [![Coverage Status](https://coveralls.io/repos/github/KrishnaswamyLab/MELD/badge.svg?branch=master)](https://coveralls.io/github/KrishnaswamyLab/MELD?branch=master)
-        [![Read the Docs](https://img.shields.io/readthedocs/meld-docs.svg)](https://meld-docs.readthedocs.io/)
-        [![bioRxiv Preprint](https://zenodo.org/badge/DOI/10.1101/532846.svg)](https://doi.org/10.1101/532846)
-        [![Twitter](https://img.shields.io/twitter/follow/KrishnaswamyLab.svg?style=social&label=Follow)](https://twitter.com/KrishnaswamyLab)
-        [![GitHub stars](https://img.shields.io/github/stars/KrishnaswamyLab/MELD.svg?style=social&label=Stars)](https://github.com/KrishnaswamyLab/MELD/)
-        
-        ### Quick Start
-        * [**Guided tutorial in Python**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/master/notebooks/Wagner2018_Chordin_Cas9_Mutagenesis.ipynb).
-        
-        ### Introduction
-        
-        MELD is a Python package for quantifying the effects of experimental perturbations. For an in depth explanation of the algorithm, read our manuscript on BioRxiv.
-        
-        [**Quantifying the effect of experimental perturbations at single-cell resolution**. Daniel B Burkhardt\*, Jay S Stanley\*, Alexander Tong, Ana Luisa Perdigoto, Scott A Gigante, Kevan C Herold, Guy Wolf, Antonio J Giraldez, David van Dijk, Smita Krishnaswamy. BioRxiv. doi:10.1101/532846.](<https://www.biorxiv.org/content/10.1101/532846v4>)
-        
-        The goal of MELD is to identify populations of cells that are most affected by an experimental perturbation. Rather than clustering the data first and calculating differential abundance of samples within clusters, MELD provides a density estimate for each scRNA-seq sample for every cell in each dataset. Comparing the ratio between the density of each sample provides a quantitative estimate the effect of a perturbation at the single-cell level. We can then identify the cells most or least affected by the perturbation.
-        
-        ### Installation
-        
-        
-        ```
-        pip install --user meld
-        ```
-        
-        ### Requirements
-        
-        MELD requires Python >= 3.6. All other requirements are installed automatically by ``pip``.
-        
-        ### Usage example
-        
-        ```
-           import numpy as np
-           import meld
-        
-           # Create toy data
-           n_samples = 500
-           n_dimensions = 100
-           data = np.random.normal(size=(n_samples, n_dimensions))
-           sample_labels = np.random.choice(['treatment', 'control'], size=n_samples)
-        
-           # Estimate density of each sample over the graph
-           sample_densities = meld.MELD().fit_transform(data, sample_labels)
-        
-           # Normalize densities to calculate sample likelihoods
-           sample_likelihoods = meld.utils.normalize_densities(sample_densities)
-        ```
-        
 Keywords: big-data,manifold-learning,computational-biology
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Framework :: Jupyter
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
+License-File: LICENSE
+License-File: LICENSE-GPL3.txt
+
+# MELD
+### Quantifying the effect of experimental perturbations at single-cell resolution
+
+
+[![Latest PyPi version](https://img.shields.io/pypi/v/MELD.svg)](https://pypi.org/project/MELD/)
+![GitHub Actions](https://github.com/KrishnaswamyLab/MELD/workflows/Unit%20Tests/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/KrishnaswamyLab/MELD/badge.svg?branch=master)](https://coveralls.io/github/KrishnaswamyLab/MELD?branch=master)
+[![Read the Docs](https://img.shields.io/readthedocs/meld-docs.svg)](https://meld-docs.readthedocs.io/)
+[![Article](https://zenodo.org/badge/DOI/10.1038/s41587-020-00803-5.svg)](https://doi.org/10.1038/s41587-020-00803-5)
+[![Twitter](https://img.shields.io/twitter/follow/KrishnaswamyLab.svg?style=social&label=Follow)](https://twitter.com/KrishnaswamyLab)
+[![GitHub stars](https://img.shields.io/github/stars/KrishnaswamyLab/MELD.svg?style=social&label=Stars)](https://github.com/KrishnaswamyLab/MELD/)
+
+### Tutorials
+For a quick-start tutorial of MELD in Google CoLab, check out this notebook from our [Machine Learning Workshop](https://krishnaswamylab.org/workshop):
+* [**MELD Quick Start - Zebrafish data**](https://colab.research.google.com/github/KrishnaswamyLab/SingleCellWorkshop/blob/master/exercises/DifferentialAbundance/Answers_Wagner2018_Chordin_Cas9_Mutagenesis.ipynb)
+
+If you're looking for an in-depth tutorial of MELD and VFC, start here:
+* [**Guided tutorial in Python - Zebrafish data**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/main/notebooks/Wagner2018_Chordin_Cas9_Mutagenesis.ipynb).
+
+If you'd like to see how to use MELD without VFC, start here:
+* [**Tutorial using MELD without VFC - T cell data**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/main/notebooks/MELD_thresholding.Tcell.ipynb).
+
+### Introduction
+
+MELD is a Python package for quantifying the effects of experimental perturbations. For an in depth explanation of the algorithm, please read the associated article:
+
+[**Quantifying the effect of experimental perturbations at single-cell resolution**. Daniel B Burkhardt\*, Jay S Stanley\*, Alexander Tong, Ana Luisa Perdigoto, Scott A Gigante, Kevan C Herold, Guy Wolf, Antonio J Giraldez, David van Dijk, Smita Krishnaswamy. Nature Biotechnology. 2021.](https://www.nature.com/articles/s41587-020-00803-5)
+
+The goal of MELD is to identify populations of cells that are most affected by an experimental perturbation. Rather than clustering the data first and calculating differential abundance of samples within clusters, MELD provides a density estimate for each scRNA-seq sample for every cell in each dataset. Comparing the ratio between the density of each sample provides a quantitative estimate the effect of a perturbation at the single-cell level. We can then identify the cells most or least affected by the perturbation.
+
+You can also watch a seminar explaining MELD given by [@dburkhardt](https://github.com/dburkhardt): [![Video](https://img.shields.io/static/v1?label=YouTube&message=Watch%20recording&color=red&logo=youtube)](https://youtu.be/PlVk1Pe0SkQ)
+
+### Installation
+
+
+```
+pip install meld
+```
+
+### Requirements
+
+MELD requires Python >= 3.6. All other requirements are installed automatically by ``pip``.
+
+### Usage example
+
+```
+   import numpy as np
+   import meld
+
+   # Create toy data
+   n_samples = 500
+   n_dimensions = 100
+   data = np.random.normal(size=(n_samples, n_dimensions))
+   sample_labels = np.random.choice(['treatment', 'control'], size=n_samples)
+
+   # Estimate density of each sample over the graph
+   sample_densities = meld.MELD().fit_transform(data, sample_labels)
+
+   # Normalize densities to calculate sample likelihoods
+   sample_likelihoods = meld.utils.normalize_densities(sample_densities)
+```
```

### Comparing `meld-1.0.0/README.md` & `meld-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,34 +2,43 @@
 ### Quantifying the effect of experimental perturbations at single-cell resolution
 
 
 [![Latest PyPi version](https://img.shields.io/pypi/v/MELD.svg)](https://pypi.org/project/MELD/)
 ![GitHub Actions](https://github.com/KrishnaswamyLab/MELD/workflows/Unit%20Tests/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/KrishnaswamyLab/MELD/badge.svg?branch=master)](https://coveralls.io/github/KrishnaswamyLab/MELD?branch=master)
 [![Read the Docs](https://img.shields.io/readthedocs/meld-docs.svg)](https://meld-docs.readthedocs.io/)
-[![bioRxiv Preprint](https://zenodo.org/badge/DOI/10.1101/532846.svg)](https://doi.org/10.1101/532846)
+[![Article](https://zenodo.org/badge/DOI/10.1038/s41587-020-00803-5.svg)](https://doi.org/10.1038/s41587-020-00803-5)
 [![Twitter](https://img.shields.io/twitter/follow/KrishnaswamyLab.svg?style=social&label=Follow)](https://twitter.com/KrishnaswamyLab)
 [![GitHub stars](https://img.shields.io/github/stars/KrishnaswamyLab/MELD.svg?style=social&label=Stars)](https://github.com/KrishnaswamyLab/MELD/)
 
-### Quick Start
-* [**Guided tutorial in Python**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/master/notebooks/Wagner2018_Chordin_Cas9_Mutagenesis.ipynb).
+### Tutorials
+For a quick-start tutorial of MELD in Google CoLab, check out this notebook from our [Machine Learning Workshop](https://krishnaswamylab.org/workshop):
+* [**MELD Quick Start - Zebrafish data**](https://colab.research.google.com/github/KrishnaswamyLab/SingleCellWorkshop/blob/master/exercises/DifferentialAbundance/Answers_Wagner2018_Chordin_Cas9_Mutagenesis.ipynb)
+
+If you're looking for an in-depth tutorial of MELD and VFC, start here:
+* [**Guided tutorial in Python - Zebrafish data**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/main/notebooks/Wagner2018_Chordin_Cas9_Mutagenesis.ipynb).
+
+If you'd like to see how to use MELD without VFC, start here:
+* [**Tutorial using MELD without VFC - T cell data**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/main/notebooks/MELD_thresholding.Tcell.ipynb).
 
 ### Introduction
 
-MELD is a Python package for quantifying the effects of experimental perturbations. For an in depth explanation of the algorithm, read our manuscript on BioRxiv.
+MELD is a Python package for quantifying the effects of experimental perturbations. For an in depth explanation of the algorithm, please read the associated article:
 
-[**Quantifying the effect of experimental perturbations at single-cell resolution**. Daniel B Burkhardt\*, Jay S Stanley\*, Alexander Tong, Ana Luisa Perdigoto, Scott A Gigante, Kevan C Herold, Guy Wolf, Antonio J Giraldez, David van Dijk, Smita Krishnaswamy. BioRxiv. doi:10.1101/532846.](<https://www.biorxiv.org/content/10.1101/532846v4>)
+[**Quantifying the effect of experimental perturbations at single-cell resolution**. Daniel B Burkhardt\*, Jay S Stanley\*, Alexander Tong, Ana Luisa Perdigoto, Scott A Gigante, Kevan C Herold, Guy Wolf, Antonio J Giraldez, David van Dijk, Smita Krishnaswamy. Nature Biotechnology. 2021.](https://www.nature.com/articles/s41587-020-00803-5)
 
 The goal of MELD is to identify populations of cells that are most affected by an experimental perturbation. Rather than clustering the data first and calculating differential abundance of samples within clusters, MELD provides a density estimate for each scRNA-seq sample for every cell in each dataset. Comparing the ratio between the density of each sample provides a quantitative estimate the effect of a perturbation at the single-cell level. We can then identify the cells most or least affected by the perturbation.
 
+You can also watch a seminar explaining MELD given by [@dburkhardt](https://github.com/dburkhardt): [![Video](https://img.shields.io/static/v1?label=YouTube&message=Watch%20recording&color=red&logo=youtube)](https://youtu.be/PlVk1Pe0SkQ)
+
 ### Installation
 
 
 ```
-pip install --user meld
+pip install meld
 ```
 
 ### Requirements
 
 MELD requires Python >= 3.6. All other requirements are installed automatically by ``pip``.
 
 ### Usage example
```

### Comparing `meld-1.0.0/meld/benchmark.py` & `meld-1.0.2/meld/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         if not data_phate.shape[1] == 3:
             raise ValueError("data_phate must have 3 dimensions")
         if not np.isclose(data_phate.mean(), 0):
             # data_phate must be mean-centered
             data_phate = scipy.stats.zscore(data_phate, axis=0)
         self.data_phate = data_phate
 
-    def fit_graph(self, data, **kwargs):
+    def fit_graph(self, data, n_pca=100, **kwargs):
         """Fits a graphtools.Graph to input data
 
         Parameters
         ----------
         data : array, shape=[n_samples, n_observations]
             Input data
         **kwargs : dict
@@ -104,15 +104,15 @@
         Returns
         -------
         graph : graphtools.Graph
             Graph fit to data
 
         """
         self.graph = gt.Graph(
-            data, n_pca=100, use_pygsp=True, random_state=self.seed, **kwargs
+            data, n_pca=n_pca, use_pygsp=True, random_state=self.seed, **kwargs
         )
         return self.graph
 
     def fit_phate(self, data, **kwargs):
         """Generates a 3D phate embedding of input data
 
         Parameters
```

### Comparing `meld-1.0.0/meld/cluster.py` & `meld-1.0.2/meld/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,16 @@
         self.N = None
         self.spec_hist = None
         self.spectrogram = None
         self.combined_spectrogram = None
         self.isfit = False
         self.likelihood = None
         self.sample_indicator = None
-        self._sklearn_params = kwargs
+        self._sklearn_params = {"n_init": 10}
+        self._sklearn_params.update(kwargs)
 
     def _activate(self, x, alpha=1):
         """Activate spectrograms for clustering
 
         Parameters
         ----------
         x : numeric
@@ -159,22 +160,22 @@
         These windows mask the signal (sample_indicator) to perform a Windowed Graph
         Fourier Transform (WGFT) as described by Shuman et al.
         (https://arxiv.org/abs/1307.5708).
 
         This function is used when the power of windows is NOT diadic
         """
         if sparse.issparse(window):
-            window = window ** t
+            window = window**t
         else:
             window = np.linalg.matrix_power(window, t)
         return preprocessing.normalize(window, "l2", axis=0).T
 
     def _power_matrix(self, a, n):
         if sparse.issparse(a):
-            a = a ** n
+            a = a**n
         else:
             a = np.linalg.matrix_power(a, n)
         return a
 
     def _compute_windows(self):
         """_compute_window
         These windows mask the signal (sample_indicator) to perform a Windowed Graph
```

### Comparing `meld-1.0.0/meld/filter.py` & `meld-1.0.2/meld/filter.py`

 * *Files identical despite different names*

### Comparing `meld-1.0.0/meld/meld.py` & `meld-1.0.2/meld/meld.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         chebyshev_order=50,
         lap_type="combinatorial",
         sample_normalize=True,
         anisotropy=1,
         n_landmark=None,
         **kwargs
     ):
-
         self.beta = beta
         self.offset = offset
         self.order = order
         self.solver = solver
         self.chebyshev_order = chebyshev_order
         self.lap_type = lap_type
         self.filter = filter
@@ -216,15 +215,15 @@
         if len(np.unique(sample_labels)) == 1:
             raise ValueError(
                 "Found only one unqiue sample label. Cannot estimate density "
                 "of a single sample."
             )
 
         # self._label_cls = type(sample_labels)
-        if isinstance(sample_labels, pd.DataFrame):
+        if hasattr(sample_labels, "index"):
             self._labels_index = sample_labels.index
         else:
             self._labels_index = None
 
         self._create_sample_indicators(sample_labels)
 
         if self.sample_normalize:
```

### Comparing `meld-1.0.0/meld/utils.py` & `meld-1.0.2/meld/utils.py`

 * *Files identical despite different names*

### Comparing `meld-1.0.0/meld.egg-info/PKG-INFO` & `meld-1.0.2/meld.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 Metadata-Version: 2.1
 Name: meld
-Version: 1.0.0
+Version: 1.0.2
 Summary: MELD
 Home-page: https://github.com/KrishnaswamyLab/MELD
+Download-URL: https://github.com/KrishnaswamyLab/MELD/archive/v1.0.2.tar.gz
 Author: Daniel Burkhardt, Krishnaswamy Lab, Yale University
 Author-email: daniel.burkhardt@yale.edu
 License: Dual License - See LICENSE file
-Download-URL: https://github.com/KrishnaswamyLab/MELD/archive/v1.0.0.tar.gz
-Description: # MELD
-        ### Quantifying the effect of experimental perturbations at single-cell resolution
-        
-        
-        [![Latest PyPi version](https://img.shields.io/pypi/v/MELD.svg)](https://pypi.org/project/MELD/)
-        ![GitHub Actions](https://github.com/KrishnaswamyLab/MELD/workflows/Unit%20Tests/badge.svg)
-        [![Coverage Status](https://coveralls.io/repos/github/KrishnaswamyLab/MELD/badge.svg?branch=master)](https://coveralls.io/github/KrishnaswamyLab/MELD?branch=master)
-        [![Read the Docs](https://img.shields.io/readthedocs/meld-docs.svg)](https://meld-docs.readthedocs.io/)
-        [![bioRxiv Preprint](https://zenodo.org/badge/DOI/10.1101/532846.svg)](https://doi.org/10.1101/532846)
-        [![Twitter](https://img.shields.io/twitter/follow/KrishnaswamyLab.svg?style=social&label=Follow)](https://twitter.com/KrishnaswamyLab)
-        [![GitHub stars](https://img.shields.io/github/stars/KrishnaswamyLab/MELD.svg?style=social&label=Stars)](https://github.com/KrishnaswamyLab/MELD/)
-        
-        ### Quick Start
-        * [**Guided tutorial in Python**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/master/notebooks/Wagner2018_Chordin_Cas9_Mutagenesis.ipynb).
-        
-        ### Introduction
-        
-        MELD is a Python package for quantifying the effects of experimental perturbations. For an in depth explanation of the algorithm, read our manuscript on BioRxiv.
-        
-        [**Quantifying the effect of experimental perturbations at single-cell resolution**. Daniel B Burkhardt\*, Jay S Stanley\*, Alexander Tong, Ana Luisa Perdigoto, Scott A Gigante, Kevan C Herold, Guy Wolf, Antonio J Giraldez, David van Dijk, Smita Krishnaswamy. BioRxiv. doi:10.1101/532846.](<https://www.biorxiv.org/content/10.1101/532846v4>)
-        
-        The goal of MELD is to identify populations of cells that are most affected by an experimental perturbation. Rather than clustering the data first and calculating differential abundance of samples within clusters, MELD provides a density estimate for each scRNA-seq sample for every cell in each dataset. Comparing the ratio between the density of each sample provides a quantitative estimate the effect of a perturbation at the single-cell level. We can then identify the cells most or least affected by the perturbation.
-        
-        ### Installation
-        
-        
-        ```
-        pip install --user meld
-        ```
-        
-        ### Requirements
-        
-        MELD requires Python >= 3.6. All other requirements are installed automatically by ``pip``.
-        
-        ### Usage example
-        
-        ```
-           import numpy as np
-           import meld
-        
-           # Create toy data
-           n_samples = 500
-           n_dimensions = 100
-           data = np.random.normal(size=(n_samples, n_dimensions))
-           sample_labels = np.random.choice(['treatment', 'control'], size=n_samples)
-        
-           # Estimate density of each sample over the graph
-           sample_densities = meld.MELD().fit_transform(data, sample_labels)
-        
-           # Normalize densities to calculate sample likelihoods
-           sample_likelihoods = meld.utils.normalize_densities(sample_densities)
-        ```
-        
 Keywords: big-data,manifold-learning,computational-biology
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Framework :: Jupyter
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
+License-File: LICENSE
+License-File: LICENSE-GPL3.txt
+
+# MELD
+### Quantifying the effect of experimental perturbations at single-cell resolution
+
+
+[![Latest PyPi version](https://img.shields.io/pypi/v/MELD.svg)](https://pypi.org/project/MELD/)
+![GitHub Actions](https://github.com/KrishnaswamyLab/MELD/workflows/Unit%20Tests/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/KrishnaswamyLab/MELD/badge.svg?branch=master)](https://coveralls.io/github/KrishnaswamyLab/MELD?branch=master)
+[![Read the Docs](https://img.shields.io/readthedocs/meld-docs.svg)](https://meld-docs.readthedocs.io/)
+[![Article](https://zenodo.org/badge/DOI/10.1038/s41587-020-00803-5.svg)](https://doi.org/10.1038/s41587-020-00803-5)
+[![Twitter](https://img.shields.io/twitter/follow/KrishnaswamyLab.svg?style=social&label=Follow)](https://twitter.com/KrishnaswamyLab)
+[![GitHub stars](https://img.shields.io/github/stars/KrishnaswamyLab/MELD.svg?style=social&label=Stars)](https://github.com/KrishnaswamyLab/MELD/)
+
+### Tutorials
+For a quick-start tutorial of MELD in Google CoLab, check out this notebook from our [Machine Learning Workshop](https://krishnaswamylab.org/workshop):
+* [**MELD Quick Start - Zebrafish data**](https://colab.research.google.com/github/KrishnaswamyLab/SingleCellWorkshop/blob/master/exercises/DifferentialAbundance/Answers_Wagner2018_Chordin_Cas9_Mutagenesis.ipynb)
+
+If you're looking for an in-depth tutorial of MELD and VFC, start here:
+* [**Guided tutorial in Python - Zebrafish data**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/main/notebooks/Wagner2018_Chordin_Cas9_Mutagenesis.ipynb).
+
+If you'd like to see how to use MELD without VFC, start here:
+* [**Tutorial using MELD without VFC - T cell data**](https://nbviewer.jupyter.org/github/KrishnaswamyLab/MELD/blob/main/notebooks/MELD_thresholding.Tcell.ipynb).
+
+### Introduction
+
+MELD is a Python package for quantifying the effects of experimental perturbations. For an in depth explanation of the algorithm, please read the associated article:
+
+[**Quantifying the effect of experimental perturbations at single-cell resolution**. Daniel B Burkhardt\*, Jay S Stanley\*, Alexander Tong, Ana Luisa Perdigoto, Scott A Gigante, Kevan C Herold, Guy Wolf, Antonio J Giraldez, David van Dijk, Smita Krishnaswamy. Nature Biotechnology. 2021.](https://www.nature.com/articles/s41587-020-00803-5)
+
+The goal of MELD is to identify populations of cells that are most affected by an experimental perturbation. Rather than clustering the data first and calculating differential abundance of samples within clusters, MELD provides a density estimate for each scRNA-seq sample for every cell in each dataset. Comparing the ratio between the density of each sample provides a quantitative estimate the effect of a perturbation at the single-cell level. We can then identify the cells most or least affected by the perturbation.
+
+You can also watch a seminar explaining MELD given by [@dburkhardt](https://github.com/dburkhardt): [![Video](https://img.shields.io/static/v1?label=YouTube&message=Watch%20recording&color=red&logo=youtube)](https://youtu.be/PlVk1Pe0SkQ)
+
+### Installation
+
+
+```
+pip install meld
+```
+
+### Requirements
+
+MELD requires Python >= 3.6. All other requirements are installed automatically by ``pip``.
+
+### Usage example
+
+```
+   import numpy as np
+   import meld
+
+   # Create toy data
+   n_samples = 500
+   n_dimensions = 100
+   data = np.random.normal(size=(n_samples, n_dimensions))
+   sample_labels = np.random.choice(['treatment', 'control'], size=n_samples)
+
+   # Estimate density of each sample over the graph
+   sample_densities = meld.MELD().fit_transform(data, sample_labels)
+
+   # Normalize densities to calculate sample likelihoods
+   sample_likelihoods = meld.utils.normalize_densities(sample_densities)
+```
```

### Comparing `meld-1.0.0/setup.py` & `meld-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = [
     "numpy>=1.14.0",
     "scipy>=1.1.0",
     "graphtools>=1.5.0",
     "pandas>=0.25",
     "scprep>=1.0",
     "pygsp",
-    "sklearn",
+    "scikit-learn",
 ]
 
 test_requires = [
     "nose",
     "nose2",
     "coverage",
     "coveralls",
@@ -52,25 +52,24 @@
     long_description_content_type="text/markdown",
     url="https://github.com/KrishnaswamyLab/MELD",
     download_url="https://github.com/KrishnaswamyLab/MELD/archive/v{}.tar.gz".format(
         version
     ),
     keywords=["big-data", "manifold-learning", "computational-biology"],
     classifiers=[
-        "Development Status :: 4 - Beta",
-        "Environment :: Console",
-        "Framework :: Jupyter",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
 )
 
 # get location of setup.py
 setup_dir = os.path.dirname(os.path.realpath(__file__))
```

### Comparing `meld-1.0.0/test/test_benchmark.py` & `meld-1.0.2/test/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `meld-1.0.0/test/test_meld.py` & `meld-1.0.2/test/test_meld.py`

 * *Files identical despite different names*

### Comparing `meld-1.0.0/test/test_utils.py` & `meld-1.0.2/test/test_utils.py`

 * *Files identical despite different names*

