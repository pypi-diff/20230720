# Comparing `tmp/enstat-0.9.5.tar.gz` & `tmp/enstat-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstat-0.9.5.tar", last modified: Tue Jul  4 13:38:25 2023, max compression
+gzip compressed data, was "enstat-0.9.6.tar", last modified: Thu Jul 20 13:36:36 2023, max compression
```

## Comparing `enstat-0.9.5.tar` & `enstat-0.9.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-04 13:38:15.000000 enstat-0.9.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 13:38:15.000000 enstat-0.9.5/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-04 13:38:15.000000 enstat-0.9.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-04 13:38:15.000000 enstat-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-04 13:38:15.000000 enstat-0.9.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 13:38:15.000000 enstat-0.9.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 13:38:15.000000 enstat-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 13:38:25.924010 enstat-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-04 13:38:15.000000 enstat-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/enstat/
--rw-r--r--   0 runner    (1001) docker     (123)    30684 2023-07-04 13:38:15.000000 enstat-0.9.5/enstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-04 13:38:15.000000 enstat-0.9.5/enstat/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-04 13:38:15.000000 enstat-0.9.5/enstat/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/enstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 13:38:15.000000 enstat-0.9.5/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-04 13:38:15.000000 enstat-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:38:25.924010 enstat-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:15.000000 enstat-0.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-07-04 13:38:15.000000 enstat-0.9.5/tests/test_binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-07-04 13:38:15.000000 enstat-0.9.5/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-07-04 13:38:15.000000 enstat-0.9.5/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:36:36.576896 enstat-0.9.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:36:36.568896 enstat-0.9.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:36:36.568896 enstat-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-20 13:36:24.000000 enstat-0.9.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-20 13:36:24.000000 enstat-0.9.6/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-20 13:36:24.000000 enstat-0.9.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-20 13:36:24.000000 enstat-0.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-20 13:36:24.000000 enstat-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-20 13:36:24.000000 enstat-0.9.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-20 13:36:24.000000 enstat-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-20 13:36:36.572896 enstat-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-20 13:36:24.000000 enstat-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:36:36.572896 enstat-0.9.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 13:36:24.000000 enstat-0.9.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 13:36:24.000000 enstat-0.9.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-20 13:36:24.000000 enstat-0.9.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 13:36:24.000000 enstat-0.9.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 13:36:24.000000 enstat-0.9.6/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:36:36.572896 enstat-0.9.6/enstat/
+-rw-r--r--   0 runner    (1001) docker     (123)    30932 2023-07-20 13:36:24.000000 enstat-0.9.6/enstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-20 13:36:36.000000 enstat-0.9.6/enstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-20 13:36:24.000000 enstat-0.9.6/enstat/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-20 13:36:24.000000 enstat-0.9.6/enstat/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:36:36.572896 enstat-0.9.6/enstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-20 13:36:36.000000 enstat-0.9.6/enstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 13:36:36.000000 enstat-0.9.6/enstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:36:36.000000 enstat-0.9.6/enstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 13:36:36.000000 enstat-0.9.6/enstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 13:36:36.000000 enstat-0.9.6/enstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 13:36:24.000000 enstat-0.9.6/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 13:36:24.000000 enstat-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:36:36.576896 enstat-0.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:36:36.572896 enstat-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:36:24.000000 enstat-0.9.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-07-20 13:36:24.000000 enstat-0.9.6/tests/test_binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-07-20 13:36:24.000000 enstat-0.9.6/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-07-20 13:36:24.000000 enstat-0.9.6/tests/test_main.py
```

### Comparing `enstat-0.9.5/.github/workflows/ci.yml` & `enstat-0.9.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/.github/workflows/python-publish.yml` & `enstat-0.9.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/.gitignore` & `enstat-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/.pre-commit-config.yaml` & `enstat-0.9.6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,46 +4,46 @@
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-yaml
   - id: check-toml
   - id: debug-statements
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.9.0
+  rev: v2.10.0
   hooks:
   - id: pretty-format-yaml
     args: [--preserve-quotes, --autofix, --indent, '2']
   - id: pretty-format-toml
     args: [--autofix]
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
     args: [--safe, --quiet, --line-length=100]
 - repo: https://github.com/humitos/mirrors-autoflake.git
   rev: v1.1
   hooks:
   - id: autoflake
     args: [--in-place, --remove-unused-variable, --remove-all-unused-imports]
 - repo: https://github.com/asottile/reorder_python_imports
   rev: v3.10.0
   hooks:
   - id: reorder-python-imports
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.7.0
+  rev: v3.9.0
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
   - id: flake8
     args: [--max-line-length=100, "--ignore=F811,W503"]
 - repo: https://github.com/asottile/setup-cfg-fmt
-  rev: v2.3.0
+  rev: v2.4.0
   hooks:
   - id: setup-cfg-fmt
 - repo: https://github.com/tdegeus/conda_envfile
   rev: v0.4.2
   hooks:
   - id: conda_envfile_parse
     files: environment.yaml
```

### Comparing `enstat-0.9.5/LICENSE` & `enstat-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/PKG-INFO` & `enstat-0.9.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.5
+Version: 0.9.6
 Summary: Ensemble averages
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/enstat
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,33 +16,32 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/enstat.svg)](https://anaconda.org/conda-forge/enstat)
 [![PyPi release](https://img.shields.io/pypi/v/enstat.svg)](https://pypi.org/project/enstat/)
 
 Documentation: [enstat.readthedocs.io](https://enstat.readthedocs.io)
 
 ## Hallmark feature
 
-*enstat* is a library to facilitate the computation of
+*enstat* is a library to compute ensemble statistics **without storing the entire ensemble in memory**.
+In particular, it allows you to compute:
 
 *   [Ensemble averages (and their variance)](#readme-average);
 *   [Ensemble averages (and their variance) based on a certain binning of a quantity](#readme-binned);
 *   [Histograms of an ensemble](#readme-histogram).
 
-**without storing the entire ensemble in memory**.
-
-> Below you find a quick-start.
-> For more information, see the [documentation](https://enstat.readthedocs.io).
+Below you find a quick-start.
+For more information, see the [documentation](https://enstat.readthedocs.io).
 
 <div id="readme-average"></div>
 
 ## Ensemble average
 
-> The key feature is to store the sum of the first and second statistical moments and the number of samples.
-> This gives access to the mean (and variance) at all times, while you can keep adding samples.
+The key feature is to store the sum of the first and second statistical moments and the number of samples.
+This gives access to the mean (and variance) at all times, while you can keep adding samples.
 
-Suppose that we have 100 realisations, each with 1000 'blocks', and we want to know the ensemble average of each block:
+Suppose that we have 100 realisations, each with 1000 'items', and we want to know the ensemble average of each item:
 
 ```python
 import enstat
 import numpy as np
 
 ensemble = enstat.static()
 
@@ -58,15 +57,15 @@
 This is the equivalent of
 
 ```python
 import numpy as np
 
 container = np.empty((100, 1000))
 
-
+for realisation in range(100):
     sample = np.random.random(1000)
     container[realisation, :] = sample
 
 print(np.mean(container, axis=0))
 ```
 
 The key difference is that *enstat* only requires you to have `4 * N` values in memory for a sample of size `N`: the sample itself, the sums of the first and second moment, and the normalisation.
```

### Comparing `enstat-0.9.5/README.md` & `enstat-0.9.6/enstat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,47 @@
+Metadata-Version: 2.1
+Name: enstat
+Version: 0.9.6
+Summary: Ensemble averages
+Author-email: Tom de Geus <tom@geus.me>
+Project-URL: Source, https://github.com/tdegeus/enstat
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # enstat
 
 [![CI](https://github.com/tdegeus/enstat/workflows/CI/badge.svg)](https://github.com/tdegeus/enstat/actions)
 [![Documentation Status](https://readthedocs.org/projects/enstat/badge/?version=latest)](https://enstat.readthedocs.io)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/enstat.svg)](https://anaconda.org/conda-forge/enstat)
 [![PyPi release](https://img.shields.io/pypi/v/enstat.svg)](https://pypi.org/project/enstat/)
 
 Documentation: [enstat.readthedocs.io](https://enstat.readthedocs.io)
 
 ## Hallmark feature
 
-*enstat* is a library to facilitate the computation of
+*enstat* is a library to compute ensemble statistics **without storing the entire ensemble in memory**.
+In particular, it allows you to compute:
 
 *   [Ensemble averages (and their variance)](#readme-average);
 *   [Ensemble averages (and their variance) based on a certain binning of a quantity](#readme-binned);
 *   [Histograms of an ensemble](#readme-histogram).
 
-**without storing the entire ensemble in memory**.
-
-> Below you find a quick-start.
-> For more information, see the [documentation](https://enstat.readthedocs.io).
+Below you find a quick-start.
+For more information, see the [documentation](https://enstat.readthedocs.io).
 
 <div id="readme-average"></div>
 
 ## Ensemble average
 
-> The key feature is to store the sum of the first and second statistical moments and the number of samples.
-> This gives access to the mean (and variance) at all times, while you can keep adding samples.
+The key feature is to store the sum of the first and second statistical moments and the number of samples.
+This gives access to the mean (and variance) at all times, while you can keep adding samples.
 
-Suppose that we have 100 realisations, each with 1000 'blocks', and we want to know the ensemble average of each block:
+Suppose that we have 100 realisations, each with 1000 'items', and we want to know the ensemble average of each item:
 
 ```python
 import enstat
 import numpy as np
 
 ensemble = enstat.static()
 
@@ -47,15 +57,15 @@
 This is the equivalent of
 
 ```python
 import numpy as np
 
 container = np.empty((100, 1000))
 
-
+for realisation in range(100):
     sample = np.random.random(1000)
     container[realisation, :] = sample
 
 print(np.mean(container, axis=0))
 ```
 
 The key difference is that *enstat* only requires you to have `4 * N` values in memory for a sample of size `N`: the sample itself, the sums of the first and second moment, and the normalisation.
```

### Comparing `enstat-0.9.5/docs/Makefile` & `enstat-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/docs/make.bat` & `enstat-0.9.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/docs/module.rst` & `enstat-0.9.6/docs/module.rst`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/enstat/__init__.py` & `enstat-0.9.6/enstat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,24 @@
 
     *   :py:attr:`scalar.first`: Sum of the first statistical moment.
     *   :py:attr:`scalar.second`: Sum of the second statistical moment.
     *   :py:attr:`scalar.norm`: Number of samples.
 
     To restore data: use :py:func:`scalar.restore`.
     In short: `restored = enstat.scalar.restore(**dict(average))`.
+
+    :param dtype:
+        The type to use for the sum of the first (and second) statistical moment.
+        Tip: Python's ``int`` is unbounded, but e.g. ``np.int64`` is not.
     """
 
-    def __init__(self):
-        self.first = 0.0
-        self.second = 0.0
-        self.norm = 0.0
+    def __init__(self, dtype=float):
+        self.first = dtype(0)
+        self.second = dtype(0)
+        self.norm = int(0)
 
     def __iter__(self):
         yield "first", self.first
         yield "second", self.second
         yield "norm", self.norm
 
     @classmethod
@@ -84,46 +88,45 @@
         Add a sample.
         Internally changes the sums of the first and second statistical moments and normalisation.
 
         :param datum: Sample.
         """
 
         datum = np.array(datum)
-        self.first += np.sum(datum)
-        self.second += np.sum(datum**2)
-        self.norm += datum.size
+        self.first += type(self.first)(np.sum(datum))
+        self.second += type(self.second)(np.sum(datum**2))
+        self.norm += type(self.norm)(datum.size)
 
     def mean(self) -> float:
         r"""
         Current mean.
         Samples can be added afterwards without any problems.
 
         :return: Mean.
         """
 
         if self.norm == 0:
             return np.NaN
 
-        return self.first / self.norm
+        return self.first / float(self.norm)
 
     def variance(self) -> float:
         r"""
         Current variance.
         Samples can be added afterwards without any problems.
 
         :return: Variance.
         """
 
         if self.norm <= 1:
             return np.NaN
 
-        d = (self.second / self.norm - (self.first / self.norm) ** 2) * self.norm
-        n = self.norm - 1
-
-        return d / n
+        n = float(self.norm)
+        d = (self.second / n - (self.first / n) ** 2) * n
+        return d / (n - 1.0)
 
     def std(self) -> float:
         r"""
         Current standard deviation.
         Samples can be added afterwards without any problems.
 
         :return: Standard deviation.
```

### Comparing `enstat-0.9.5/enstat/detail.py` & `enstat-0.9.6/enstat/detail.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/enstat/mean.py` & `enstat-0.9.6/enstat/mean.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/enstat.egg-info/PKG-INFO` & `enstat-0.9.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,36 @@
-Metadata-Version: 2.1
-Name: enstat
-Version: 0.9.5
-Summary: Ensemble averages
-Author-email: Tom de Geus <tom@geus.me>
-Project-URL: Source, https://github.com/tdegeus/enstat
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # enstat
 
 [![CI](https://github.com/tdegeus/enstat/workflows/CI/badge.svg)](https://github.com/tdegeus/enstat/actions)
 [![Documentation Status](https://readthedocs.org/projects/enstat/badge/?version=latest)](https://enstat.readthedocs.io)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/enstat.svg)](https://anaconda.org/conda-forge/enstat)
 [![PyPi release](https://img.shields.io/pypi/v/enstat.svg)](https://pypi.org/project/enstat/)
 
 Documentation: [enstat.readthedocs.io](https://enstat.readthedocs.io)
 
 ## Hallmark feature
 
-*enstat* is a library to facilitate the computation of
+*enstat* is a library to compute ensemble statistics **without storing the entire ensemble in memory**.
+In particular, it allows you to compute:
 
 *   [Ensemble averages (and their variance)](#readme-average);
 *   [Ensemble averages (and their variance) based on a certain binning of a quantity](#readme-binned);
 *   [Histograms of an ensemble](#readme-histogram).
 
-**without storing the entire ensemble in memory**.
-
-> Below you find a quick-start.
-> For more information, see the [documentation](https://enstat.readthedocs.io).
+Below you find a quick-start.
+For more information, see the [documentation](https://enstat.readthedocs.io).
 
 <div id="readme-average"></div>
 
 ## Ensemble average
 
-> The key feature is to store the sum of the first and second statistical moments and the number of samples.
-> This gives access to the mean (and variance) at all times, while you can keep adding samples.
+The key feature is to store the sum of the first and second statistical moments and the number of samples.
+This gives access to the mean (and variance) at all times, while you can keep adding samples.
 
-Suppose that we have 100 realisations, each with 1000 'blocks', and we want to know the ensemble average of each block:
+Suppose that we have 100 realisations, each with 1000 'items', and we want to know the ensemble average of each item:
 
 ```python
 import enstat
 import numpy as np
 
 ensemble = enstat.static()
 
@@ -58,15 +46,15 @@
 This is the equivalent of
 
 ```python
 import numpy as np
 
 container = np.empty((100, 1000))
 
-
+for realisation in range(100):
     sample = np.random.random(1000)
     container[realisation, :] = sample
 
 print(np.mean(container, axis=0))
 ```
 
 The key difference is that *enstat* only requires you to have `4 * N` values in memory for a sample of size `N`: the sample itself, the sums of the first and second moment, and the normalisation.
```

### Comparing `enstat-0.9.5/enstat.egg-info/SOURCES.txt` & `enstat-0.9.6/enstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/tests/test_binned.py` & `enstat-0.9.6/tests/test_binned.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/tests/test_histogram.py` & `enstat-0.9.6/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.5/tests/test_main.py` & `enstat-0.9.6/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,21 @@
         for i in range(a.shape[0]):
             average += a[i, :]
 
         average *= factor
         self.assertTrue(np.isclose(average.mean(), np.mean(aprime)))
         self.assertTrue(np.isclose(average.std(), np.std(aprime), rtol=1e-3))
 
+    def test_scalar_large(self):
+        v = int(np.iinfo(np.uint64).max)
+        data = [v * i for i in range(1000)]
+        average = enstat.scalar(dtype=int)
+        average += data
+        self.assertAlmostEqual(average.mean(), np.mean(data))
+
     def test_static(self):
         """
         Basic test of "mean" and "std" using a random sample.
         """
 
         average = enstat.static()
```

