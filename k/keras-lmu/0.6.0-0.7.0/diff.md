# Comparing `tmp/keras-lmu-0.6.0.tar.gz` & `tmp/keras-lmu-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-lmu-0.6.0.tar", last modified: Tue May  9 15:13:55 2023, max compression
+gzip compressed data, was "keras-lmu-0.7.0.tar", last modified: Thu Jul 20 21:54:38 2023, max compression
```

## Comparing `keras-lmu-0.6.0.tar` & `keras-lmu-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.288609 keras-lmu-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/.nengobones.yml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-09 15:13:55.288609 keras-lmu-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/api-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/basic-usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/examples/psMNIST-training.png
--rw-r--r--   0 runner    (1001) docker     (123)  1252848 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/examples/psMNIST-weights.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/examples/psMNIST.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/docs/project.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/keras_lmu/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42115 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.288609 keras-lmu-0.6.0/keras_lmu/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/keras_lmu/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:13:55.284609 keras-lmu-0.6.0/keras_lmu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:12:45.000000 keras-lmu-0.6.0/keras_lmu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 15:13:55.000000 keras-lmu-0.6.0/keras_lmu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 15:13:55.288609 keras-lmu-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-09 15:11:42.000000 keras-lmu-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:54:38.349441 keras-lmu-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/.nengobones.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-07-20 21:54:38.349441 keras-lmu-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:54:38.345441 keras-lmu-0.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:54:38.345441 keras-lmu-0.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/basic-usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:54:38.349441 keras-lmu-0.7.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/examples/psMNIST-training.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1252848 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/examples/psMNIST-weights.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/examples/psMNIST.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/docs/project.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:54:38.349441 keras-lmu-0.7.0/keras_lmu/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/keras_lmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42658 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/keras_lmu/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:54:38.349441 keras-lmu-0.7.0/keras_lmu/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/keras_lmu/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/keras_lmu/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/keras_lmu/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/keras_lmu/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/keras_lmu/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:54:38.349441 keras-lmu-0.7.0/keras_lmu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-07-20 21:54:38.000000 keras-lmu-0.7.0/keras_lmu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-20 21:54:38.000000 keras-lmu-0.7.0/keras_lmu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:54:38.000000 keras-lmu-0.7.0/keras_lmu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:53:41.000000 keras-lmu-0.7.0/keras_lmu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 21:54:38.000000 keras-lmu-0.7.0/keras_lmu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 21:54:38.000000 keras-lmu-0.7.0/keras_lmu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-20 21:54:38.353441 keras-lmu-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-20 21:52:18.000000 keras-lmu-0.7.0/setup.py
```

### Comparing `keras-lmu-0.6.0/.nengobones.yml` & `keras-lmu-0.7.0/.nengobones.yml`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,18 @@
     - nengo_sphinx_theme>=1.2.0
     - numpydoc>=0.6
   classifiers:
     - "Development Status :: 3 - Alpha"
     - "Intended Audience :: Science/Research"
     - "Operating System :: OS Independent"
     - "Programming Language :: Python "
-    - "Programming Language :: Python :: 3.7"
     - "Programming Language :: Python :: 3.8"
     - "Programming Language :: Python :: 3.9"
+    - "Programming Language :: Python :: 3.10"
+    - "Programming Language :: Python :: 3.11"
     - "Topic :: Scientific/Engineering "
     - "Topic :: Scientific/Engineering :: Artificial Intelligence"
 
 setup_cfg: {}
 
 docs_conf_py:
   intersphinx_mapping:
@@ -104,10 +105,10 @@
 pre_commit_config_yaml: {}
 
 pyproject_toml: {}
 
 version_py:
   type: semver
   major: 0
-  minor: 6
+  minor: 7
   patch: 0
-  release: True
+  release: true
```

### Comparing `keras-lmu-0.6.0/CHANGES.rst` & `keras-lmu-0.7.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,26 @@
 
    - Added
    - Changed
    - Deprecated
    - Removed
    - Fixed
 
+0.7.0 (July 20, 2023)
+=====================
+
+*Compatible with TensorFlow 2.4 - 2.13*
+
+**Changed**
+
+- Minimum supported Python version is now 3.8 (3.7 reached end of life in June 2023).
+  (`#54`_)
+
+.. _#54: https://github.com/nengo/keras-lmu/pull/54
+
 0.6.0 (May 5, 2023)
 ===================
 
 *Compatible with TensorFlow 2.4 - 2.11*
 
 **Changed**
```

### Comparing `keras-lmu-0.6.0/CONTRIBUTING.rst` & `keras-lmu-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/LICENSE.rst` & `keras-lmu-0.7.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/MANIFEST.in` & `keras-lmu-0.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/PKG-INFO` & `keras-lmu-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: keras-lmu
-Version: 0.6.0
+Version: 0.7.0
 Summary: Keras implementation of Legendre Memory Units
 Home-page: https://www.nengo.ai/keras-lmu
 Author: Applied Brain Research
 Author-email: info@appliedbrainresearch.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python 
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering 
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: optional
 Provides-Extra: tests
 License-File: LICENSE.rst
 
 KerasLMU: Recurrent neural networks using Legendre Memory Units
@@ -114,14 +115,26 @@
 
    - Added
    - Changed
    - Deprecated
    - Removed
    - Fixed
 
+0.7.0 (July 20, 2023)
+=====================
+
+*Compatible with TensorFlow 2.4 - 2.13*
+
+**Changed**
+
+- Minimum supported Python version is now 3.8 (3.7 reached end of life in June 2023).
+  (`#54`_)
+
+.. _#54: https://github.com/nengo/keras-lmu/pull/54
+
 0.6.0 (May 5, 2023)
 ===================
 
 *Compatible with TensorFlow 2.4 - 2.11*
 
 **Changed**
```

### Comparing `keras-lmu-0.6.0/README.rst` & `keras-lmu-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/docs/_static/favicon.ico` & `keras-lmu-0.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/docs/basic-usage.rst` & `keras-lmu-0.7.0/docs/basic-usage.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/docs/citation.rst` & `keras-lmu-0.7.0/docs/citation.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/docs/examples/psMNIST-training.png` & `keras-lmu-0.7.0/docs/examples/psMNIST-training.png`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/docs/examples/psMNIST-weights.hdf5` & `keras-lmu-0.7.0/docs/examples/psMNIST-weights.hdf5`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/docs/examples/psMNIST.ipynb` & `keras-lmu-0.7.0/docs/examples/psMNIST.ipynb`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/docs/examples.rst` & `keras-lmu-0.7.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/docs/getting-started.rst` & `keras-lmu-0.7.0/docs/getting-started.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 .. code:: bash
 
    pip install keras-lmu
 
 Requirements
 ------------
 
-KerasLMU works with Python 3.6 or later.  After installing NumPy and TensorFlow, ``pip``
+KerasLMU works with Python 3.8 or later.  After installing NumPy and TensorFlow, ``pip``
 will do its best to install all of the package's other requirements when it installs
 KerasLMU. However, if anything goes wrong during this process, you can install each
 required package manually and then try to ``pip install keras-lmu`` again.
 
 Developer installation
 ----------------------
 If you want to modify KerasLMU, or get the very latest updates, you will need to
```

### Comparing `keras-lmu-0.6.0/keras_lmu/layers.py` & `keras-lmu-0.7.0/keras_lmu/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 from packaging import version
 
 # pylint: disable=ungrouped-imports
 if version.parse(tf.__version__) < version.parse("2.6.0rc0"):
     from tensorflow.python.keras.layers.recurrent import DropoutRNNCellMixin
 elif version.parse(tf.__version__) < version.parse("2.9.0rc0"):
     from keras.layers.recurrent import DropoutRNNCellMixin
-else:
+elif version.parse(tf.__version__) < version.parse("2.13.0rc0"):
     from keras.layers.rnn.dropout_rnn_cell_mixin import DropoutRNNCellMixin
+else:
+    from keras.src.layers.rnn.dropout_rnn_cell_mixin import DropoutRNNCellMixin
 
 if version.parse(tf.__version__) < version.parse("2.8.0rc0"):
     from tensorflow.keras.layers import Layer as BaseRandomLayer
-else:
+elif version.parse(tf.__version__) < version.parse("2.13.0rc0"):
     from keras.engine.base_layer import BaseRandomLayer
+else:
+    from keras.src.engine.base_layer import BaseRandomLayer
 
 
 @tf.keras.utils.register_keras_serializable("keras-lmu")
 class LMUCell(DropoutRNNCellMixin, BaseRandomLayer):
     """
     Implementation of LMU cell (to be used within Keras RNN wrapper).
 
@@ -446,15 +450,19 @@
 
         return config
 
     @classmethod
     def from_config(cls, config):
         """Load model from serialized config."""
 
-        config["hidden_cell"] = tf.keras.layers.deserialize(config["hidden_cell"])
+        config["hidden_cell"] = (
+            None
+            if config["hidden_cell"] is None
+            else tf.keras.layers.deserialize(config["hidden_cell"])
+        )
         return super().from_config(config)
 
 
 @tf.keras.utils.register_keras_serializable("keras-lmu")
 class LMU(tf.keras.layers.Layer):
     """
     A layer of trainable low-dimensional delay systems.
@@ -710,15 +718,19 @@
 
         return config
 
     @classmethod
     def from_config(cls, config):
         """Load model from serialized config."""
 
-        config["hidden_cell"] = tf.keras.layers.deserialize(config["hidden_cell"])
+        config["hidden_cell"] = (
+            None
+            if config["hidden_cell"] is None
+            else tf.keras.layers.deserialize(config["hidden_cell"])
+        )
         return super().from_config(config)
 
 
 @tf.keras.utils.register_keras_serializable("keras-lmu")
 class LMUFeedforward(tf.keras.layers.Layer):
     """
     Layer class for the feedforward variant of the LMU.
@@ -1061,9 +1073,13 @@
 
         return config
 
     @classmethod
     def from_config(cls, config):
         """Load model from serialized config."""
 
-        config["hidden_cell"] = tf.keras.layers.deserialize(config["hidden_cell"])
+        config["hidden_cell"] = (
+            None
+            if config["hidden_cell"] is None
+            else tf.keras.layers.deserialize(config["hidden_cell"])
+        )
         return super().from_config(config)
```

### Comparing `keras-lmu-0.6.0/keras_lmu/tests/test_benchmarks.py` & `keras-lmu-0.7.0/keras_lmu/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/keras_lmu/tests/test_layers.py` & `keras-lmu-0.7.0/keras_lmu/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/keras_lmu/version.py` & `keras-lmu-0.7.0/keras_lmu/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 We use semantic versioning (see http://semver.org/) and conform to PEP440 (see
 https://www.python.org/dev/peps/pep-0440/). '.dev0' will be added to the version
 unless the code base represents a release version. Release versions are git
 tagged with the version.
 """
 
-version_info = (0, 6, 0)
+version_info = (0, 7, 0)
 
 name = "keras-lmu"
 dev = None
 
 # use old string formatting, so that this can still run in Python <= 3.5
 # (since this file is parsed in setup.py, before python_requires is applied)
 version = ".".join(str(v) for v in version_info)
```

### Comparing `keras-lmu-0.6.0/keras_lmu.egg-info/PKG-INFO` & `keras-lmu-0.7.0/keras_lmu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: keras-lmu
-Version: 0.6.0
+Version: 0.7.0
 Summary: Keras implementation of Legendre Memory Units
 Home-page: https://www.nengo.ai/keras-lmu
 Author: Applied Brain Research
 Author-email: info@appliedbrainresearch.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python 
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering 
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: optional
 Provides-Extra: tests
 License-File: LICENSE.rst
 
 KerasLMU: Recurrent neural networks using Legendre Memory Units
@@ -114,14 +115,26 @@
 
    - Added
    - Changed
    - Deprecated
    - Removed
    - Fixed
 
+0.7.0 (July 20, 2023)
+=====================
+
+*Compatible with TensorFlow 2.4 - 2.13*
+
+**Changed**
+
+- Minimum supported Python version is now 3.8 (3.7 reached end of life in June 2023).
+  (`#54`_)
+
+.. _#54: https://github.com/nengo/keras-lmu/pull/54
+
 0.6.0 (May 5, 2023)
 ===================
 
 *Compatible with TensorFlow 2.4 - 2.11*
 
 **Changed**
```

### Comparing `keras-lmu-0.6.0/keras_lmu.egg-info/SOURCES.txt` & `keras-lmu-0.7.0/keras_lmu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/setup.cfg` & `keras-lmu-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-lmu-0.6.0/setup.py` & `keras-lmu-0.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -64,21 +64,22 @@
     install_requires=install_req,
     extras_require={
         "all": docs_req + optional_req + tests_req,
         "docs": docs_req,
         "optional": optional_req,
         "tests": tests_req,
     },
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: Free for non-commercial use",
         "Operating System :: OS Independent",
         "Programming Language :: Python ",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering ",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
```

