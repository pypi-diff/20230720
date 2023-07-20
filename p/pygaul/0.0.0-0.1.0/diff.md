# Comparing `tmp/pygaul-0.0.0.tar.gz` & `tmp/pygaul-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygaul-0.0.0.tar", last modified: Thu Jun 29 15:48:15 2023, max compression
+gzip compressed data, was "pygaul-0.1.0.tar", last modified: Thu Jul 20 13:20:46 2023, max compression
```

## Comparing `pygaul-0.0.0.tar` & `pygaul-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 borntobealive  (1000) borntobealive  (1000)        0 2023-06-29 15:48:15.718587 pygaul-0.0.0/
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)     2708 2023-06-29 15:48:15.718587 pygaul-0.0.0/PKG-INFO
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)     1945 2023-06-29 15:09:39.000000 pygaul-0.0.0/README.rst
-drwxr-xr-x   0 borntobealive  (1000) borntobealive  (1000)        0 2023-06-29 15:48:15.708587 pygaul-0.0.0/pygaul/
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)      274 2023-06-29 15:09:01.000000 pygaul-0.0.0/pygaul/__init__.py
-drwxr-xr-x   0 borntobealive  (1000) borntobealive  (1000)        0 2023-06-29 15:48:15.708587 pygaul-0.0.0/pygaul.egg-info/
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)     2708 2023-06-29 15:48:15.000000 pygaul-0.0.0/pygaul.egg-info/PKG-INFO
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)      223 2023-06-29 15:48:15.000000 pygaul-0.0.0/pygaul.egg-info/SOURCES.txt
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)        1 2023-06-29 15:48:15.000000 pygaul-0.0.0/pygaul.egg-info/dependency_links.txt
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)      211 2023-06-29 15:48:15.000000 pygaul-0.0.0/pygaul.egg-info/requires.txt
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)        7 2023-06-29 15:48:15.000000 pygaul-0.0.0/pygaul.egg-info/top_level.txt
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)     2184 2023-06-29 15:09:57.000000 pygaul-0.0.0/pyproject.toml
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)       38 2023-06-29 15:48:15.718587 pygaul-0.0.0/setup.cfg
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)       66 2023-06-29 15:09:01.000000 pygaul-0.0.0/setup.py
-drwxr-xr-x   0 borntobealive  (1000) borntobealive  (1000)        0 2023-06-29 15:48:15.708587 pygaul-0.0.0/tests/
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)      151 2023-06-29 15:09:01.000000 pygaul-0.0.0/tests/test_pygaul.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:20:46.484388 pygaul-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-20 13:20:46.484388 pygaul-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-20 13:20:26.000000 pygaul-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:20:46.480388 pygaul-0.1.0/pygaul/
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-07-20 13:20:26.000000 pygaul-0.1.0/pygaul/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:20:46.480388 pygaul-0.1.0/pygaul.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-20 13:20:46.000000 pygaul-0.1.0/pygaul.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-20 13:20:46.000000 pygaul-0.1.0/pygaul.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:20:46.000000 pygaul-0.1.0/pygaul.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-20 13:20:46.000000 pygaul-0.1.0/pygaul.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 13:20:46.000000 pygaul-0.1.0/pygaul.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-20 13:20:26.000000 pygaul-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:20:46.484388 pygaul-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 13:20:26.000000 pygaul-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:20:46.480388 pygaul-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-20 13:20:26.000000 pygaul-0.1.0/tests/test_get_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-20 13:20:26.000000 pygaul-0.1.0/tests/test_get_name.py
```

### Comparing `pygaul-0.0.0/PKG-INFO` & `pygaul-0.1.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: pygaul
-Version: 0.0.0
-Summary: Easy access to administrative boundary defined by FAO GAUL from a Python script.
-Author-email: Pierrick Rambaud <pierrick.rambaud49@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/12rambau/pygaul
-Keywords: skeleton,Python
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.9
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: doc
-
 
 pyGAUL
 ======
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg?logo=opensourceinitiative&logoColor=white
     :target: LICENSE
     :alt: License: MIT
@@ -62,13 +41,33 @@
 .. image:: https://img.shields.io/badge/all_contributors-0-orange.svg
     :alt: All contributors
     :target: AUTHORS.rst
 
 Overview
 --------
 
-Easy access to administrative boundary defined by FAO GAUL from a Python script.
+Easy access to administrative boundary defined by FAO GAUL 2015 from Python scripts.
+
+This lib provides access to FAO GAUL 2015 datasets from a Python script. it is the best boundary dataset available for GEE at this point. We provide access to The current version (2015) administrative areas till level 2.
+
+.. note::
+
+   the dataset was generated in 2015 by the Food and Alimentation Organization (FAO). It has not been updated on Google Earthengine since then. Use with caution on disputed territories.
+
+install it using either ``pip`` or ``conda``:
+
+.. code-block:: console
+
+   pip install pygaul
+
+and then request area of interest from their name or GADM Id:
+
+.. code-block:: python
+
+   import pygaul
+
+   gdf = pygaul.get_items(name="Singapore", content_level=1)
 
 Credits
 -------
 
 This package was created with `Cookiecutter <https://github.com/cookiecutter/cookiecutter>`__ and the `12rambau/pypackage <https://github.com/12rambau/pypackage>`__ project template.
```

### Comparing `pygaul-0.0.0/pygaul.egg-info/PKG-INFO` & `pygaul-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygaul
-Version: 0.0.0
+Version: 0.1.0
 Summary: Easy access to administrative boundary defined by FAO GAUL from a Python script.
 Author-email: Pierrick Rambaud <pierrick.rambaud49@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/12rambau/pygaul
 Keywords: skeleton,Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -62,13 +62,33 @@
 .. image:: https://img.shields.io/badge/all_contributors-0-orange.svg
     :alt: All contributors
     :target: AUTHORS.rst
 
 Overview
 --------
 
-Easy access to administrative boundary defined by FAO GAUL from a Python script.
+Easy access to administrative boundary defined by FAO GAUL 2015 from Python scripts.
+
+This lib provides access to FAO GAUL 2015 datasets from a Python script. it is the best boundary dataset available for GEE at this point. We provide access to The current version (2015) administrative areas till level 2.
+
+.. note::
+
+   the dataset was generated in 2015 by the Food and Alimentation Organization (FAO). It has not been updated on Google Earthengine since then. Use with caution on disputed territories.
+
+install it using either ``pip`` or ``conda``:
+
+.. code-block:: console
+
+   pip install pygaul
+
+and then request area of interest from their name or GADM Id:
+
+.. code-block:: python
+
+   import pygaul
+
+   gdf = pygaul.get_items(name="Singapore", content_level=1)
 
 Credits
 -------
 
 This package was created with `Cookiecutter <https://github.com/cookiecutter/cookiecutter>`__ and the `12rambau/pypackage <https://github.com/12rambau/pypackage>`__ project template.
```

### Comparing `pygaul-0.0.0/pyproject.toml` & `pygaul-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygaul"
-version = "0.0.0"
+version = "0.1.0"
 description = "Easy access to administrative boundary defined by FAO GAUL from a Python script."
 keywords = ["skeleton", "Python"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.6.9"
-dependencies = ["deprecated>=1.2.14"]
+dependencies = [
+    "deprecated>=1.2.14",
+    "pandas",
+    "earthengine-api",
+    "pyarrow"
+]
 
 [[project.authors]]
 name = "Pierrick Rambaud"
 email = "pierrick.rambaud49@gmail.com"
 
 [project.license]
 text = "MIT"
@@ -32,42 +37,45 @@
 
 [project.urls]
 Homepage = "https://github.com/12rambau/pygaul"
 
 [project.optional-dependencies]
 dev = ["pre-commit", "commitizen", "nox"]
 test = ["pytest", "pytest-sugar", "pytest-cov", "pytest-deadfixtures"]
-doc = ["sphinx>=6.2.1", "pydata-sphinx-theme", "sphinx-copybutton", "sphinx-design", "sphinx-icon", "sphinx-autoapi"]
+doc = ["sphinx>=6.2.1", "pydata-sphinx-theme", "sphinx-copybutton", "sphinx-design", "sphinx-icon", "sphinx-autoapi", "geemap", "jupyter-sphinx"]
 
 [tool.setuptools]
 include-package-data = false
 license-files = ["LICENSE.txt"]
 
 [tool.setuptools.packages.find]
 include = ["pygaul*"]
 exclude = ["docs*", "tests*"]
 
 [tool.commitizen]
 tag_format = "v$major.$minor.$patch$prerelease"
 update_changelog_on_bump = false
-version = "0.0.0"
+version = "0.1.0"
 version_files = [
     "pyproject.toml:version",
     "pygaul/__init__.py:__version__",
     "docs/conf.py:release"
 ]
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 
 [tool.ruff]
 ignore-init-module-imports = true
 fix = true
 select = ["E", "F", "W", "I", "D", "RUF"]
-ignore = ["E501"]  # line too long | Black take care of it
+ignore = [
+    "E501",  # line too long | Black take care of it
+    "D212",  # Multi-line docstring | We use D213
+]
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
@@ -82,7 +90,10 @@
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
 warn_redundant_casts = true
 
 [tool.licensecheck]
 using = "PEP631:test;dev;doc"
+
+[tool.codespell]
+skip = "./pygaul/data/gaul_continent.json"
```

