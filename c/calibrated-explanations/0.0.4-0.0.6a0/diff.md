# Comparing `tmp/calibrated-explanations-0.0.4.tar.gz` & `tmp/calibrated_explanations-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibrated-explanations-0.0.4.tar", last modified: Fri Jul 14 11:50:44 2023, max compression
+gzip compressed data, was "calibrated_explanations-0.0.6a0.tar", last modified: Thu Jul 20 12:54:34 2023, max compression
```

## Comparing `calibrated-explanations-0.0.4.tar` & `calibrated_explanations-0.0.6a0.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 rudy      (1080) rudy      (1080)        0 2023-07-14 11:50:44.663289 calibrated-explanations-0.0.4/
--rw-r--r--   0 rudy      (1080) rudy      (1080)     1064 2023-07-05 15:11:26.000000 calibrated-explanations-0.0.4/LICENSE
--rw-r--r--   0 rudy      (1080) rudy      (1080)     2535 2023-07-14 11:50:44.663289 calibrated-explanations-0.0.4/PKG-INFO
--rw-r--r--   0 rudy      (1080) rudy      (1080)     1907 2023-07-14 11:46:58.000000 calibrated-explanations-0.0.4/README.md
-drwxr-xr-x   0 rudy      (1080) rudy      (1080)        0 2023-07-14 11:50:44.656623 calibrated-explanations-0.0.4/calibrated_explanations/
-drwxr-xr-x   0 rudy      (1080) rudy      (1080)        0 2023-07-14 11:50:44.659956 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/
--rw-r--r--   0 rudy      (1080) rudy      (1080)     2535 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/PKG-INFO
--rw-r--r--   0 rudy      (1080) rudy      (1080)      449 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/SOURCES.txt
--rw-r--r--   0 rudy      (1080) rudy      (1080)        1 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/dependency_links.txt
--rw-r--r--   0 rudy      (1080) rudy      (1080)       67 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/requires.txt
--rw-r--r--   0 rudy      (1080) rudy      (1080)        1 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/top_level.txt
--rw-r--r--   0 rudy      (1080) rudy      (1080)      812 2023-07-14 11:50:35.000000 calibrated-explanations-0.0.4/pyproject.toml
--rw-r--r--   0 rudy      (1080) rudy      (1080)       38 2023-07-14 11:50:44.663289 calibrated-explanations-0.0.4/setup.cfg
--rw-r--r--   0 rudy      (1080) rudy      (1080)      170 2023-07-12 11:33:21.000000 calibrated-explanations-0.0.4/setup.py
-drwxr-xr-x   0 rudy      (1080) rudy      (1080)        0 2023-07-14 11:50:44.663289 calibrated-explanations-0.0.4/tests/
--rw-r--r--   0 rudy      (1080) rudy      (1080)     8488 2023-07-12 15:02:18.000000 calibrated-explanations-0.0.4/tests/test_classification.py
--rw-r--r--   0 rudy      (1080) rudy      (1080)    15237 2023-07-12 15:02:18.000000 calibrated-explanations-0.0.4/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.808170 calibrated_explanations-0.0.6a0/
+-rw-rw-rw-   0        0        0     1085 2023-07-12 12:35:31.000000 calibrated_explanations-0.0.6a0/LICENSE
+-rw-rw-rw-   0        0        0     2660 2023-07-20 12:54:34.807164 calibrated_explanations-0.0.6a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/README.md
+-rw-rw-rw-   0        0        0      979 2023-07-20 12:49:04.000000 calibrated_explanations-0.0.6a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 12:54:34.808170 calibrated_explanations-0.0.6a0/setup.cfg
+-rw-rw-rw-   0        0        0      179 2023-07-12 12:35:32.000000 calibrated_explanations-0.0.6a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.756162 calibrated_explanations-0.0.6a0/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.781161 calibrated_explanations-0.0.6a0/src/calibrated_explanations/
+-rw-rw-rw-   0        0        0     2533 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/VennAbers.py
+-rw-rw-rw-   0        0        0      509 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/__init__.py
+-rw-rw-rw-   0        0        0     1957 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/_discretizers.py
+-rw-rw-rw-   0        0        0    38940 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/_explanations.py
+-rw-rw-rw-   0        0        0    36850 2023-07-20 12:36:38.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/core.py
+-rw-rw-rw-   0        0        0     3039 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.800161 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/
+-rw-rw-rw-   0        0        0     2660 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.804163 calibrated_explanations-0.0.6a0/tests/
+-rw-rw-rw-   0        0        0     8692 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/tests/test_classification.py
+-rw-rw-rw-   0        0        0    15625 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/tests/test_regression.py
```

### Comparing `calibrated-explanations-0.0.4/LICENSE` & `calibrated_explanations-0.0.6a0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Moffran
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Moffran
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `calibrated-explanations-0.0.4/PKG-INFO` & `calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-Metadata-Version: 2.1
-Name: calibrated-explanations
-Version: 0.0.4
-Summary: Extract calibrated explanations from machine learning models.
-Author-email: Helena Löfström <helena.lofstrom@ju.se>
-Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
-Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Calibrated Explanations
-=======================
-
-[![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
-[![Build Status for Calibrated Explanations][build-status]][build-log]
-
-Calibrated Explanations is a Python library
-that is able to explain predictions of a black-box model
-using Venn Abers predictors (classification)
-or conformal predictive systems (regression) and perturbations.
-
-Install
--------
-
-First, you need a Python environment installed with pip.
-
-Calibrated Explanations can be installed from PyPI:
-
-	pip install calibrated-explanations
-
-The dependencies are:
-
-* [crepes](https://github.com/henrikbostrom/crepes)
-* [lime](https://github.com/marcotcr/lime)
-* [matplotlib](https://matplotlib.org/)
-* [NumPy](https://numpy.org/)
-* [pandas](https://pandas.pydata.org/)
-* [scikit-learn](https://scikit-learn.org/)
-* [SHAP](https://pypi.org/project/shap/)
-* [tqdm](https://tqdm.github.io/)
-
-
-Getting started
----------------
-
-```python
->>> import calibrated_explanations
-... TODO: write me...
-```
-
-
-Development
------------
-
-This project has tests that can be executed using `pytest`.
-Just run the following command from the project root.
-
-```bash
-pytest
-```
-
-
-Further reading
----------------
-
-The calibrated explanations library is based on the paper
-"Calibrated Explanations for Black-Box Predictions"
-by
-[Helena Löfström](https://github.com/Moffran),
-[Tuwe Löfström](https://github.com/tuvelofstrom),
-Ulf Johansson and
-Cecilia Sönströd.
-
-If you would like to cite this work, please cite the above paper.
-
-[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml
-[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml/badge.svg
-[pypi-version]: https://img.shields.io/pypi/v/calibrated-explanations
-[calibrated-explanations-on-pypi]: https://pypi.org/project/calibrated-explanations
+Metadata-Version: 2.1
+Name: calibrated-explanations
+Version: 0.0.6a0
+Summary: Extract calibrated explanations from machine learning models.
+Author-email: Helena Löfström <helena.lofstrom@ju.se>, Tuwe Löfström <tuwe.lofstrom@ju.se>
+Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
+Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Calibrated Explanations
+=======================
+
+[![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
+[![Build Status for Calibrated Explanations][build-status]][build-log]
+
+Calibrated Explanations is a Python library
+that is able to explain predictions of a black-box model
+using Venn Abers predictors (classification)
+or conformal predictive systems (regression) and perturbations.
+
+Install
+-------
+
+First, you need a Python environment installed with pip.
+
+Calibrated Explanations can be installed from PyPI:
+
+	pip install calibrated-explanations
+
+The dependencies are:
+
+* [crepes](https://github.com/henrikbostrom/crepes)
+* [lime](https://github.com/marcotcr/lime)
+* [matplotlib](https://matplotlib.org/)
+* [NumPy](https://numpy.org/)
+* [pandas](https://pandas.pydata.org/)
+* [scikit-learn](https://scikit-learn.org/)
+* [SHAP](https://pypi.org/project/shap/)
+* [tqdm](https://tqdm.github.io/)
+
+
+Getting started
+---------------
+
+```python
+>>> import calibrated_explanations
+... TODO: write me...
+```
+
+
+Development
+-----------
+
+This project has tests that can be executed using `pytest`.
+Just run the following command from the project root.
+
+```bash
+pytest
+```
+
+
+Further reading
+---------------
+
+The calibrated explanations library is based on the paper
+"Calibrated Explanations for Black-Box Predictions"
+by
+[Helena Löfström](https://github.com/Moffran),
+[Tuwe Löfström](https://github.com/tuvelofstrom),
+Ulf Johansson and
+Cecilia Sönströd.
+
+If you would like to cite this work, please cite the above paper.
+
+[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml
+[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml/badge.svg
+[pypi-version]: https://img.shields.io/pypi/v/calibrated-explanations
+[calibrated-explanations-on-pypi]: https://pypi.org/project/calibrated-explanations
```

### Comparing `calibrated-explanations-0.0.4/README.md` & `calibrated_explanations-0.0.6a0/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-Calibrated Explanations
-=======================
-
-[![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
-[![Build Status for Calibrated Explanations][build-status]][build-log]
-
-Calibrated Explanations is a Python library
-that is able to explain predictions of a black-box model
-using Venn Abers predictors (classification)
-or conformal predictive systems (regression) and perturbations.
-
-Install
--------
-
-First, you need a Python environment installed with pip.
-
-Calibrated Explanations can be installed from PyPI:
-
-	pip install calibrated-explanations
-
-The dependencies are:
-
-* [crepes](https://github.com/henrikbostrom/crepes)
-* [lime](https://github.com/marcotcr/lime)
-* [matplotlib](https://matplotlib.org/)
-* [NumPy](https://numpy.org/)
-* [pandas](https://pandas.pydata.org/)
-* [scikit-learn](https://scikit-learn.org/)
-* [SHAP](https://pypi.org/project/shap/)
-* [tqdm](https://tqdm.github.io/)
-
-
-Getting started
----------------
-
-```python
->>> import calibrated_explanations
-... TODO: write me...
-```
-
-
-Development
------------
-
-This project has tests that can be executed using `pytest`.
-Just run the following command from the project root.
-
-```bash
-pytest
-```
-
-
-Further reading
----------------
-
-The calibrated explanations library is based on the paper
-"Calibrated Explanations for Black-Box Predictions"
-by
-[Helena Löfström](https://github.com/Moffran),
-[Tuwe Löfström](https://github.com/tuvelofstrom),
-Ulf Johansson and
-Cecilia Sönströd.
-
-If you would like to cite this work, please cite the above paper.
-
-[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml
-[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml/badge.svg
-[pypi-version]: https://img.shields.io/pypi/v/calibrated-explanations
-[calibrated-explanations-on-pypi]: https://pypi.org/project/calibrated-explanations
+Calibrated Explanations
+=======================
+
+[![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
+[![Build Status for Calibrated Explanations][build-status]][build-log]
+
+Calibrated Explanations is a Python library
+that is able to explain predictions of a black-box model
+using Venn Abers predictors (classification)
+or conformal predictive systems (regression) and perturbations.
+
+Install
+-------
+
+First, you need a Python environment installed with pip.
+
+Calibrated Explanations can be installed from PyPI:
+
+	pip install calibrated-explanations
+
+The dependencies are:
+
+* [crepes](https://github.com/henrikbostrom/crepes)
+* [lime](https://github.com/marcotcr/lime)
+* [matplotlib](https://matplotlib.org/)
+* [NumPy](https://numpy.org/)
+* [pandas](https://pandas.pydata.org/)
+* [scikit-learn](https://scikit-learn.org/)
+* [SHAP](https://pypi.org/project/shap/)
+* [tqdm](https://tqdm.github.io/)
+
+
+Getting started
+---------------
+
+```python
+>>> import calibrated_explanations
+... TODO: write me...
+```
+
+
+Development
+-----------
+
+This project has tests that can be executed using `pytest`.
+Just run the following command from the project root.
+
+```bash
+pytest
+```
+
+
+Further reading
+---------------
+
+The calibrated explanations library is based on the paper
+"Calibrated Explanations for Black-Box Predictions"
+by
+[Helena Löfström](https://github.com/Moffran),
+[Tuwe Löfström](https://github.com/tuvelofstrom),
+Ulf Johansson and
+Cecilia Sönströd.
+
+If you would like to cite this work, please cite the above paper.
+
+[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml
+[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml/badge.svg
+[pypi-version]: https://img.shields.io/pypi/v/calibrated-explanations
+[calibrated-explanations-on-pypi]: https://pypi.org/project/calibrated-explanations
```

### Comparing `calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/PKG-INFO` & `calibrated_explanations-0.0.6a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-Metadata-Version: 2.1
-Name: calibrated-explanations
-Version: 0.0.4
-Summary: Extract calibrated explanations from machine learning models.
-Author-email: Helena Löfström <helena.lofstrom@ju.se>
-Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
-Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Calibrated Explanations
-=======================
-
-[![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
-[![Build Status for Calibrated Explanations][build-status]][build-log]
-
-Calibrated Explanations is a Python library
-that is able to explain predictions of a black-box model
-using Venn Abers predictors (classification)
-or conformal predictive systems (regression) and perturbations.
-
-Install
--------
-
-First, you need a Python environment installed with pip.
-
-Calibrated Explanations can be installed from PyPI:
-
-	pip install calibrated-explanations
-
-The dependencies are:
-
-* [crepes](https://github.com/henrikbostrom/crepes)
-* [lime](https://github.com/marcotcr/lime)
-* [matplotlib](https://matplotlib.org/)
-* [NumPy](https://numpy.org/)
-* [pandas](https://pandas.pydata.org/)
-* [scikit-learn](https://scikit-learn.org/)
-* [SHAP](https://pypi.org/project/shap/)
-* [tqdm](https://tqdm.github.io/)
-
-
-Getting started
----------------
-
-```python
->>> import calibrated_explanations
-... TODO: write me...
-```
-
-
-Development
------------
-
-This project has tests that can be executed using `pytest`.
-Just run the following command from the project root.
-
-```bash
-pytest
-```
-
-
-Further reading
----------------
-
-The calibrated explanations library is based on the paper
-"Calibrated Explanations for Black-Box Predictions"
-by
-[Helena Löfström](https://github.com/Moffran),
-[Tuwe Löfström](https://github.com/tuvelofstrom),
-Ulf Johansson and
-Cecilia Sönströd.
-
-If you would like to cite this work, please cite the above paper.
-
-[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml
-[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml/badge.svg
-[pypi-version]: https://img.shields.io/pypi/v/calibrated-explanations
-[calibrated-explanations-on-pypi]: https://pypi.org/project/calibrated-explanations
+Metadata-Version: 2.1
+Name: calibrated_explanations
+Version: 0.0.6a0
+Summary: Extract calibrated explanations from machine learning models.
+Author-email: Helena Löfström <helena.lofstrom@ju.se>, Tuwe Löfström <tuwe.lofstrom@ju.se>
+Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
+Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Calibrated Explanations
+=======================
+
+[![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
+[![Build Status for Calibrated Explanations][build-status]][build-log]
+
+Calibrated Explanations is a Python library
+that is able to explain predictions of a black-box model
+using Venn Abers predictors (classification)
+or conformal predictive systems (regression) and perturbations.
+
+Install
+-------
+
+First, you need a Python environment installed with pip.
+
+Calibrated Explanations can be installed from PyPI:
+
+	pip install calibrated-explanations
+
+The dependencies are:
+
+* [crepes](https://github.com/henrikbostrom/crepes)
+* [lime](https://github.com/marcotcr/lime)
+* [matplotlib](https://matplotlib.org/)
+* [NumPy](https://numpy.org/)
+* [pandas](https://pandas.pydata.org/)
+* [scikit-learn](https://scikit-learn.org/)
+* [SHAP](https://pypi.org/project/shap/)
+* [tqdm](https://tqdm.github.io/)
+
+
+Getting started
+---------------
+
+```python
+>>> import calibrated_explanations
+... TODO: write me...
+```
+
+
+Development
+-----------
+
+This project has tests that can be executed using `pytest`.
+Just run the following command from the project root.
+
+```bash
+pytest
+```
+
+
+Further reading
+---------------
+
+The calibrated explanations library is based on the paper
+"Calibrated Explanations for Black-Box Predictions"
+by
+[Helena Löfström](https://github.com/Moffran),
+[Tuwe Löfström](https://github.com/tuvelofstrom),
+Ulf Johansson and
+Cecilia Sönströd.
+
+If you would like to cite this work, please cite the above paper.
+
+[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml
+[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml/badge.svg
+[pypi-version]: https://img.shields.io/pypi/v/calibrated-explanations
+[calibrated-explanations-on-pypi]: https://pypi.org/project/calibrated-explanations
```

### Comparing `calibrated-explanations-0.0.4/tests/test_classification.py` & `calibrated_explanations-0.0.6a0/tests/test_classification.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-from __future__ import absolute_import
-
-import unittest
-import pytest
-
-import numpy as np
-import pandas as pd
-from sklearn.ensemble import RandomForestClassifier
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.model_selection import train_test_split
-# from sklearn.utils import shuffle
-# import matplotlib.pyplot as plt
-from lime.discretize import EntropyDiscretizer
-# from shap import Explainer
-
-from calibrated_explanations import CalibratedExplainer, BinaryDiscretizer, BinaryEntropyDiscretizer
-
-model = 'RF'
-def load_binary_dataset():
-    dataSet = 'diabetes_full'
-    delimiter = ','
-    num_to_test = 4
-    target = 'Y'
-
-    fileName = 'data/' + dataSet + ".csv"
-    df = pd.read_csv(fileName, delimiter=delimiter, dtype=np.float64)
-
-    X, y = df.drop(target,axis=1), df[target] 
-    no_of_classes = len(np.unique(y))
-    no_of_features = X.shape[1]
-    no_of_instances = X.shape[0]
-    columns = X.columns
-    categorical_features = [i for i in range(no_of_features) if len(np.unique(X.iloc[:,i])) < 10]
-    # # sort targets to make sure equal presence of both classes in test set (see definition of test_index after outer loop below)
-    idx = np.argsort(y.values).astype(int)
-    X, y = X.values[idx,:], y.values[idx]
-    # Select num_to_test/2 from top and num_to_test/2 from bottom of list of instances
-    test_index = np.array([*range(int(num_to_test/2)), *range(no_of_instances-1, no_of_instances-int(num_to_test/2)-1,-1)])
-    train_index = np.setdiff1d(np.array(range(no_of_instances)), test_index)   
-    trainCalX, testX = X[train_index,:], X[test_index,:]
-    trainCalY, testY = y[train_index], y[test_index]
-    # trainCalX,trainCalY = shuffle(trainCalX, trainCalY)
-    trainX, calX, trainY, calY = train_test_split(trainCalX, trainCalY, test_size=0.33,random_state=42, stratify=trainCalY)
-    return trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, columns
-
-def load_multiclass_dataset():
-    dataSet = 'glass'
-    delimiter = ','
-    num_to_test = 12
-    model_name = 'RF'
-    # print(dataSet)
-
-    fileName = 'data/Multiclass/' + dataSet + ".csv"
-    df = pd.read_csv(fileName, delimiter=delimiter)
-    target = 'Type'
-
-    # df.convert_objects()
-
-    df = df.dropna()
-    categorical_features = []
-    categorical_labels = {}
-    for c, col in enumerate(df.columns):
-        if df[col].dtype == object:
-            df[col] = df[col].str.replace("'", "")
-            df[col] = df[col].str.replace('"', '')
-            if col != target:
-                categorical_features.append(c)
-                categorical_labels[c] = dict(zip(range(len(np.unique(df[col]))),np.unique(df[col])))
-            else:
-                target_labels = dict(zip(range(len(np.unique(df[col]))),np.unique(df[col])))
-            mapping = dict(zip(np.unique(df[col]), range(len(np.unique(df[col])))))
-            if len(mapping) > 5:
-                counts = df[col].value_counts().sort_values(ascending=False)
-                id = 0
-                for key, count in counts.items():
-                    if count > 5:
-                        id += 1
-                        continue
-                    mapping[key] = id
-            df[col] = df[col].map(mapping)
-
-    X, y = df.drop(target,axis=1), df[target] 
-    columns = X.columns
-    no_of_classes = len(np.unique(y))
-    no_of_features = X.shape[1]
-    no_of_instances = X.shape[0]
-    categorical_features = [i for i in range(no_of_features) if len(np.unique(X.iloc[:,i])) < 10]
-    # # sort targets to make sure equal presence of both classes in test set (see definition of test_index after outer loop below)
-    idx = np.argsort(y.values).astype(int)
-    X, y = X.values[idx,:], y.values[idx]
-    test_idx = []
-    idx = list(range(no_of_instances))
-    for i in range(no_of_classes):
-        test_idx.append(np.where(y == i)[0][0:int(num_to_test/no_of_classes)])
-    test_index = np.array(test_idx).flatten()
-    # Select num_to_test/2 from top and num_to_test/2 from bottom of list of instances
-    train_index = np.setdiff1d(np.array(range(no_of_instances)), test_index)   
-    trainCalX, testX = X[train_index,:], X[test_index,:]
-    trainCalY, testY = y[train_index], y[test_index]
-    # trainCalX,trainCalY = shuffle(trainCalX, trainCalY)
-    trainX, calX, trainY, calY = train_test_split(trainCalX, trainCalY, test_size=0.33,random_state=42, stratify=trainCalY)
-    return trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, columns
-
-def get_classification_model(model_name, trainX, trainY):
-    t1 = DecisionTreeClassifier()
-    r1 = RandomForestClassifier(n_estimators=100)
-    model_dict = {'RF':(r1,"RF"),'DT': (t1,"DT")}
-
-    model, model_name = model_dict[model_name] 
-    model.fit(trainX,trainY)  
-    return model, model_name
-
-
-
-class TestCalibratedExplainer(unittest.TestCase):
-    def assertExplanation(self, exp):
-        for i, instance in enumerate(exp.x):
-            boundaries = exp.CE.rule_boundaries(instance)
-            for f in range(exp.CE.num_features):
-                # assert that instance values are covered by the rule conditions
-                assert instance[f] >= boundaries[f][0] and instance[f] <= boundaries[f][1]
-        return True
-
-    def test_binary_ce(self):
-        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, feature_names = load_binary_dataset()
-        model, model_name = get_classification_model('RF', trainX, trainY)
-        cal_exp = CalibratedExplainer(
-            model, 
-            calX, 
-            calY,
-            feature_names=feature_names, 
-            discretizer='binary', 
-            categorical_features=categorical_features, 
-            mode='classification',
-        )
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        cal_exp.set_discretizer('binaryEntropy')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, BinaryEntropyDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()    
-        
-        cal_exp.set_discretizer('entropy')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, EntropyDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()    
-
-    @unittest.skip('Test passes locally.  Skipping provisionally.')
-    def test_multiclass_ce(self):
-        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, feature_names = load_multiclass_dataset()
-        model, model_name = get_classification_model('RF', trainX, trainY)
-        cal_exp = CalibratedExplainer(
-            model, 
-            calX, 
-            calY,
-            feature_names=feature_names, 
-            discretizer='binary', 
-            categorical_features=categorical_features, 
-            mode='classification',
-        )
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()        
-        
-        cal_exp.set_discretizer('binaryEntropy')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, BinaryEntropyDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()    
-        
-        cal_exp.set_discretizer('entropy')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, EntropyDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()    
-
-
-if __name__ == '__main__':
-    # unittest.main()
-    pytest.main()
+from __future__ import absolute_import
+
+import unittest
+import pytest
+
+import numpy as np
+import pandas as pd
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.tree import DecisionTreeClassifier
+from sklearn.model_selection import train_test_split
+# from sklearn.utils import shuffle
+# import matplotlib.pyplot as plt
+from lime.discretize import EntropyDiscretizer
+# from shap import Explainer
+
+from calibrated_explanations import CalibratedExplainer, BinaryDiscretizer, BinaryEntropyDiscretizer
+
+model = 'RF'
+def load_binary_dataset():
+    dataSet = 'diabetes_full'
+    delimiter = ','
+    num_to_test = 4
+    target = 'Y'
+
+    fileName = 'data/' + dataSet + ".csv"
+    df = pd.read_csv(fileName, delimiter=delimiter, dtype=np.float64)
+
+    X, y = df.drop(target,axis=1), df[target] 
+    no_of_classes = len(np.unique(y))
+    no_of_features = X.shape[1]
+    no_of_instances = X.shape[0]
+    columns = X.columns
+    categorical_features = [i for i in range(no_of_features) if len(np.unique(X.iloc[:,i])) < 10]
+    # # sort targets to make sure equal presence of both classes in test set (see definition of test_index after outer loop below)
+    idx = np.argsort(y.values).astype(int)
+    X, y = X.values[idx,:], y.values[idx]
+    # Select num_to_test/2 from top and num_to_test/2 from bottom of list of instances
+    test_index = np.array([*range(int(num_to_test/2)), *range(no_of_instances-1, no_of_instances-int(num_to_test/2)-1,-1)])
+    train_index = np.setdiff1d(np.array(range(no_of_instances)), test_index)   
+    trainCalX, testX = X[train_index,:], X[test_index,:]
+    trainCalY, testY = y[train_index], y[test_index]
+    # trainCalX,trainCalY = shuffle(trainCalX, trainCalY)
+    trainX, calX, trainY, calY = train_test_split(trainCalX, trainCalY, test_size=0.33,random_state=42, stratify=trainCalY)
+    return trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, columns
+
+def load_multiclass_dataset():
+    dataSet = 'glass'
+    delimiter = ','
+    num_to_test = 12
+    model_name = 'RF'
+    # print(dataSet)
+
+    fileName = 'data/Multiclass/' + dataSet + ".csv"
+    df = pd.read_csv(fileName, delimiter=delimiter)
+    target = 'Type'
+
+    # df.convert_objects()
+
+    df = df.dropna()
+    categorical_features = []
+    categorical_labels = {}
+    for c, col in enumerate(df.columns):
+        if df[col].dtype == object:
+            df[col] = df[col].str.replace("'", "")
+            df[col] = df[col].str.replace('"', '')
+            if col != target:
+                categorical_features.append(c)
+                categorical_labels[c] = dict(zip(range(len(np.unique(df[col]))),np.unique(df[col])))
+            else:
+                target_labels = dict(zip(range(len(np.unique(df[col]))),np.unique(df[col])))
+            mapping = dict(zip(np.unique(df[col]), range(len(np.unique(df[col])))))
+            if len(mapping) > 5:
+                counts = df[col].value_counts().sort_values(ascending=False)
+                id = 0
+                for key, count in counts.items():
+                    if count > 5:
+                        id += 1
+                        continue
+                    mapping[key] = id
+            df[col] = df[col].map(mapping)
+
+    X, y = df.drop(target,axis=1), df[target] 
+    columns = X.columns
+    no_of_classes = len(np.unique(y))
+    no_of_features = X.shape[1]
+    no_of_instances = X.shape[0]
+    categorical_features = [i for i in range(no_of_features) if len(np.unique(X.iloc[:,i])) < 10]
+    # # sort targets to make sure equal presence of both classes in test set (see definition of test_index after outer loop below)
+    idx = np.argsort(y.values).astype(int)
+    X, y = X.values[idx,:], y.values[idx]
+    test_idx = []
+    idx = list(range(no_of_instances))
+    for i in range(no_of_classes):
+        test_idx.append(np.where(y == i)[0][0:int(num_to_test/no_of_classes)])
+    test_index = np.array(test_idx).flatten()
+    # Select num_to_test/2 from top and num_to_test/2 from bottom of list of instances
+    train_index = np.setdiff1d(np.array(range(no_of_instances)), test_index)   
+    trainCalX, testX = X[train_index,:], X[test_index,:]
+    trainCalY, testY = y[train_index], y[test_index]
+    # trainCalX,trainCalY = shuffle(trainCalX, trainCalY)
+    trainX, calX, trainY, calY = train_test_split(trainCalX, trainCalY, test_size=0.33,random_state=42, stratify=trainCalY)
+    return trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, columns
+
+def get_classification_model(model_name, trainX, trainY):
+    t1 = DecisionTreeClassifier()
+    r1 = RandomForestClassifier(n_estimators=100)
+    model_dict = {'RF':(r1,"RF"),'DT': (t1,"DT")}
+
+    model, model_name = model_dict[model_name] 
+    model.fit(trainX,trainY)  
+    return model, model_name
+
+
+
+class TestCalibratedExplainer(unittest.TestCase):
+    def assertExplanation(self, exp):
+        for i, instance in enumerate(exp.x):
+            boundaries = exp.CE.rule_boundaries(instance)
+            for f in range(exp.CE.num_features):
+                # assert that instance values are covered by the rule conditions
+                assert instance[f] >= boundaries[f][0] and instance[f] <= boundaries[f][1]
+        return True
+
+    def test_binary_ce(self):
+        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, feature_names = load_binary_dataset()
+        model, model_name = get_classification_model('RF', trainX, trainY)
+        cal_exp = CalibratedExplainer(
+            model, 
+            calX, 
+            calY,
+            feature_names=feature_names, 
+            discretizer='binary', 
+            categorical_features=categorical_features, 
+            mode='classification',
+        )
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        cal_exp.set_discretizer('binaryEntropy')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, BinaryEntropyDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()    
+        
+        cal_exp.set_discretizer('entropy')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, EntropyDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()    
+
+    @unittest.skip('Test passes locally.  Skipping provisionally.')
+    def test_multiclass_ce(self):
+        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, feature_names = load_multiclass_dataset()
+        model, model_name = get_classification_model('RF', trainX, trainY)
+        cal_exp = CalibratedExplainer(
+            model, 
+            calX, 
+            calY,
+            feature_names=feature_names, 
+            discretizer='binary', 
+            categorical_features=categorical_features, 
+            mode='classification',
+        )
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()        
+        
+        cal_exp.set_discretizer('binaryEntropy')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, BinaryEntropyDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()    
+        
+        cal_exp.set_discretizer('entropy')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, EntropyDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()    
+
+
+if __name__ == '__main__':
+    # unittest.main()
+    pytest.main()
```

### Comparing `calibrated-explanations-0.0.4/tests/test_regression.py` & `calibrated_explanations-0.0.6a0/tests/test_regression.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,388 +1,388 @@
-from __future__ import absolute_import
-
-import unittest
-import pytest
-
-import numpy as np
-import pandas as pd
-from sklearn.ensemble import RandomForestRegressor
-from sklearn.tree import DecisionTreeRegressor
-from sklearn.model_selection import train_test_split
-# from sklearn.utils import shuffle
-# import matplotlib.pyplot as plt
-from lime.discretize import EntropyDiscretizer, DecileDiscretizer, QuartileDiscretizer
-# from shap import Explainer
-
-from calibrated_explanations import CalibratedExplainer, BinaryDiscretizer, BinaryEntropyDiscretizer
-from crepes.extras import DifficultyEstimator # sigma_knn, sigma_variance, sigma_variance_oob
-
-model = 'RF'
-def load_regression_dataset():
-    dataSet = 'housing.csv'
-    delimiter = ';'
-    num_to_test = 10
-    categorical_labels = {8: {0: 'INLAND', 1: 'NEAR BAY', 2: '<1H OCEAN', 3: 'NEAR OCEAN', 4: 'ISLAND'}}
-
-    fileName = 'data/reg/' + dataSet
-    df = pd.read_csv(fileName, delimiter=delimiter, dtype=np.float64)
-
-    target = 'median_house_value'
-    # target = 'REGRESSION'
-    df.dropna(inplace=True)
-    X, y = df.drop(target,axis=1), df[target] 
-    # normalize target between 0 and 1
-    # y = (y - y.min())/(y.max() - y.min())
-    columns = df.drop(target,axis=1).columns
-    no_of_classes = len(np.unique(y))
-    no_of_features = X.shape[1]
-    no_of_instances = X.shape[0]
-    categorical_features = [i for i in range(no_of_features) if len(np.unique(X.iloc[:,i])) < 10]
-    # # sort targets to make sure equal presence of both classes in test set (see definition of test_index after outer loop below)
-
-    trainCalX, testX, trainCalY, testY = train_test_split(X.values, y.values, test_size=num_to_test,random_state=42)
-    # trainCalX,trainCalY = shuffle(trainCalX, trainCalY)
-    trainX, calX, trainY, calY = train_test_split(trainCalX, trainCalY, test_size=0.33,random_state=42)
-    return trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, categorical_labels, columns
-
-def get_regression_model(model, trainX, trainY):
-    t1 = DecisionTreeRegressor()
-    r1 = RandomForestRegressor(n_estimators=100)
-    model_dict = {'RF':(r1,"RF"),'DT': (t1,"DT")}
-
-    model, model_name = model_dict[model] 
-    model.fit(trainX,trainY)  
-    return model, model_name
-
-
-
-class TestCalibratedExplainer(unittest.TestCase):
-    def assertExplanation(self, exp):
-        for i, instance in enumerate(exp.x):
-            boundaries = exp.CE.rule_boundaries(instance)
-            for f in range(exp.CE.num_features):
-                # assert that instance values are covered by the rule conditions
-                assert instance[f] >= boundaries[f][0] and instance[f] <= boundaries[f][1]
-        return True
-    
-    
-    # NOTE: this takes takes about 70s to run
-    def test_regression_ce(self):
-        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, categorical_labels, feature_names = load_regression_dataset()
-        model, model_name = get_regression_model('RF', trainX, trainY)
-        cal_exp = CalibratedExplainer(
-            model, 
-            calX, 
-            calY,
-            feature_names=feature_names, 
-            discretizer='binary', 
-            categorical_features=categorical_features, 
-            categorical_labels=categorical_labels,
-            mode='regression'
-        )
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        
-        cal_exp.set_discretizer('quartile')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, QuartileDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        cal_exp.set_discretizer('decile')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, DecileDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules() 
-          
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-    
-    
-    @unittest.skip('Test passes but is slow, ~2 minutes.  Skipping provisionally.')
-    def test_knn_normalized_regression_ce(self):
-        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, categorical_labels, feature_names = load_regression_dataset()
-        model, model_name = get_regression_model('RF', trainX, trainY)
-        cal_exp = CalibratedExplainer(
-            model, 
-            calX, 
-            calY,
-            feature_names=feature_names, 
-            discretizer='binary', 
-            categorical_features=categorical_features, 
-            categorical_labels=categorical_labels,
-            mode='regression',
-            difficultyEstimator=DifficultyEstimator().fit(X=trainX, y=trainY, scaler=True),
-        )
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        
-        cal_exp.set_discretizer('quartile')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, QuartileDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        cal_exp.set_discretizer('decile')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, DecileDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules() 
-          
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        
-    @unittest.skip('Test passes but is slow, ~2 minutes.  Skipping provisionally.')
-    def test_var_normalized_regression_ce(self):
-        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, categorical_labels, feature_names = load_regression_dataset()
-        model, model_name = get_regression_model('RF', trainX, trainY)
-        cal_exp = CalibratedExplainer(
-            model, 
-            calX, 
-            calY,
-            feature_names=feature_names, 
-            discretizer='binary', 
-            categorical_features=categorical_features, 
-            categorical_labels=categorical_labels,
-            mode='regression',
-            difficultyEstimator=DifficultyEstimator().fit(X=trainX, learner=model, scaler=True),
-        )
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        
-        cal_exp.set_discretizer('quartile')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, QuartileDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        cal_exp.set_discretizer('decile')
-        exp = cal_exp(testX)
-        self.assertIsInstance(exp.CE.discretizer, DecileDiscretizer)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules() 
-          
-        exp = cal_exp(testX, testY)
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-        
-        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
-        self.assertExplanation(exp)
-        exp.add_conjunctive_counterfactual_rules()
-        exp.get_counterfactual_rules()
-        exp.add_conjunctive_factual_rules()
-        exp.get_factual_rules()
-   
-
-
-if __name__ == '__main__':
-    # unittest.main()
-    pytest.main()
+from __future__ import absolute_import
+
+import unittest
+import pytest
+
+import numpy as np
+import pandas as pd
+from sklearn.ensemble import RandomForestRegressor
+from sklearn.tree import DecisionTreeRegressor
+from sklearn.model_selection import train_test_split
+# from sklearn.utils import shuffle
+# import matplotlib.pyplot as plt
+from lime.discretize import EntropyDiscretizer, DecileDiscretizer, QuartileDiscretizer
+# from shap import Explainer
+
+from calibrated_explanations import CalibratedExplainer, BinaryDiscretizer, BinaryEntropyDiscretizer
+from crepes.extras import DifficultyEstimator # sigma_knn, sigma_variance, sigma_variance_oob
+
+model = 'RF'
+def load_regression_dataset():
+    dataSet = 'housing.csv'
+    delimiter = ';'
+    num_to_test = 10
+    categorical_labels = {8: {0: 'INLAND', 1: 'NEAR BAY', 2: '<1H OCEAN', 3: 'NEAR OCEAN', 4: 'ISLAND'}}
+
+    fileName = 'data/reg/' + dataSet
+    df = pd.read_csv(fileName, delimiter=delimiter, dtype=np.float64)
+
+    target = 'median_house_value'
+    # target = 'REGRESSION'
+    df.dropna(inplace=True)
+    X, y = df.drop(target,axis=1), df[target] 
+    # normalize target between 0 and 1
+    # y = (y - y.min())/(y.max() - y.min())
+    columns = df.drop(target,axis=1).columns
+    no_of_classes = len(np.unique(y))
+    no_of_features = X.shape[1]
+    no_of_instances = X.shape[0]
+    categorical_features = [i for i in range(no_of_features) if len(np.unique(X.iloc[:,i])) < 10]
+    # # sort targets to make sure equal presence of both classes in test set (see definition of test_index after outer loop below)
+
+    trainCalX, testX, trainCalY, testY = train_test_split(X.values, y.values, test_size=num_to_test,random_state=42)
+    # trainCalX,trainCalY = shuffle(trainCalX, trainCalY)
+    trainX, calX, trainY, calY = train_test_split(trainCalX, trainCalY, test_size=0.33,random_state=42)
+    return trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, categorical_labels, columns
+
+def get_regression_model(model, trainX, trainY):
+    t1 = DecisionTreeRegressor()
+    r1 = RandomForestRegressor(n_estimators=100)
+    model_dict = {'RF':(r1,"RF"),'DT': (t1,"DT")}
+
+    model, model_name = model_dict[model] 
+    model.fit(trainX,trainY)  
+    return model, model_name
+
+
+
+class TestCalibratedExplainer(unittest.TestCase):
+    def assertExplanation(self, exp):
+        for i, instance in enumerate(exp.x):
+            boundaries = exp.CE.rule_boundaries(instance)
+            for f in range(exp.CE.num_features):
+                # assert that instance values are covered by the rule conditions
+                assert instance[f] >= boundaries[f][0] and instance[f] <= boundaries[f][1]
+        return True
+    
+    
+    # NOTE: this takes takes about 70s to run
+    def test_regression_ce(self):
+        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, categorical_labels, feature_names = load_regression_dataset()
+        model, model_name = get_regression_model('RF', trainX, trainY)
+        cal_exp = CalibratedExplainer(
+            model, 
+            calX, 
+            calY,
+            feature_names=feature_names, 
+            discretizer='binary', 
+            categorical_features=categorical_features, 
+            categorical_labels=categorical_labels,
+            mode='regression'
+        )
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        
+        cal_exp.set_discretizer('quartile')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, QuartileDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        cal_exp.set_discretizer('decile')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, DecileDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules() 
+          
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+    
+    
+    @unittest.skip('Test passes but is slow, ~2 minutes.  Skipping provisionally.')
+    def test_knn_normalized_regression_ce(self):
+        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, categorical_labels, feature_names = load_regression_dataset()
+        model, model_name = get_regression_model('RF', trainX, trainY)
+        cal_exp = CalibratedExplainer(
+            model, 
+            calX, 
+            calY,
+            feature_names=feature_names, 
+            discretizer='binary', 
+            categorical_features=categorical_features, 
+            categorical_labels=categorical_labels,
+            mode='regression',
+            difficultyEstimator=DifficultyEstimator().fit(X=trainX, y=trainY, scaler=True),
+        )
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        
+        cal_exp.set_discretizer('quartile')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, QuartileDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        cal_exp.set_discretizer('decile')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, DecileDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules() 
+          
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        
+    @unittest.skip('Test passes but is slow, ~2 minutes.  Skipping provisionally.')
+    def test_var_normalized_regression_ce(self):
+        trainX, trainY, calX, calY, testX, testY, no_of_classes, no_of_features, categorical_features, categorical_labels, feature_names = load_regression_dataset()
+        model, model_name = get_regression_model('RF', trainX, trainY)
+        cal_exp = CalibratedExplainer(
+            model, 
+            calX, 
+            calY,
+            feature_names=feature_names, 
+            discretizer='binary', 
+            categorical_features=categorical_features, 
+            categorical_labels=categorical_labels,
+            mode='regression',
+            difficultyEstimator=DifficultyEstimator().fit(X=trainX, learner=model, scaler=True),
+        )
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, BinaryDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        
+        cal_exp.set_discretizer('quartile')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, QuartileDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        cal_exp.set_discretizer('decile')
+        exp = cal_exp(testX)
+        self.assertIsInstance(exp.CE.discretizer, DecileDiscretizer)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules() 
+          
+        exp = cal_exp(testX, testY)
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(0.1,np.inf))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+        
+        exp = cal_exp(testX,low_high_percentiles=(-np.inf,0.9))
+        self.assertExplanation(exp)
+        exp.add_conjunctive_counterfactual_rules()
+        exp.get_counterfactual_rules()
+        exp.add_conjunctive_factual_rules()
+        exp.get_factual_rules()
+   
+
+
+if __name__ == '__main__':
+    # unittest.main()
+    pytest.main()
```

