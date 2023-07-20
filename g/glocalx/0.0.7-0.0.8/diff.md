# Comparing `tmp/glocalx-0.0.7.tar.gz` & `tmp/glocalx-0.0.8.tar.gz`

## Comparing `glocalx-0.0.7.tar` & `glocalx-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 glocalx-0.0.7/PKG-INFO
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/__init__.py
--rwxr-xr-x   0        0        0     9852 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/api.py
--rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/callbacks.py
--rwxr-xr-x   0        0        0    26407 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/evaluators.py
--rwxr-xr-x   0        0        0     8618 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/generators.py
--rwxr-xr-x   0        0        0    24742 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/glocalx.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/glocax_probabilistic.py
--rwxr-xr-x   0        0        0    12664 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/models.py
--rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/requirements.txt
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/serialization.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/data/dummy/dummy_dataset.csv
--rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/data/dummy/dummy_model.h5
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/data/dummy/dummy_rules.json
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/data/loaders/adult_info.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 glocalx-0.0.7/src/glocalx/loaders/lore.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 glocalx-0.0.7/LICENSE
--rwxr-xr-x   0        0        0    11369 2020-02-02 00:00:00.000000 glocalx-0.0.7/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 glocalx-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 glocalx-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 glocalx-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/__init__.py
+-rwxr-xr-x   0        0        0     9852 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/api.py
+-rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/callbacks.py
+-rwxr-xr-x   0        0        0    26407 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/evaluators.py
+-rwxr-xr-x   0        0        0     8618 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/generators.py
+-rwxr-xr-x   0        0        0    24742 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/glocalx.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/glocax_probabilistic.py
+-rwxr-xr-x   0        0        0    12664 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/models.py
+-rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/requirements.txt
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/serialization.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/data/dummy/dummy_dataset.csv
+-rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/data/dummy/dummy_model.h5
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/data/dummy/dummy_rules.json
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/data/loaders/adult_info.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/loaders/lore.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 glocalx-0.0.8/LICENSE
+-rwxr-xr-x   0        0        0    11369 2020-02-02 00:00:00.000000 glocalx-0.0.8/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 glocalx-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 glocalx-0.0.8/PKG-INFO
```

### Comparing `glocalx-0.0.7/PKG-INFO` & `glocalx-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: glocalx
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generating global explanations from local ones.
 Project-URL: Homepage, https://github.com/msetzu/glocalx
 Project-URL: Bug Tracker, https://github.com/msetzu/glocalx/issues
 Author-email: Mattia Setzu <mattia.setzu@unipi.it>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <3.11,>=3.8
-Requires-Dist: click==7.1.2
+Requires-Dist: click
 Requires-Dist: logzero==1.6.2
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tensorflow==2.8
 Description-Content-Type: text/markdown
```

### Comparing `glocalx-0.0.7/src/glocalx/.gitignore` & `glocalx-0.0.8/src/glocalx/.gitignore`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/api.py` & `glocalx-0.0.8/src/glocalx/api.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/callbacks.py` & `glocalx-0.0.8/src/glocalx/callbacks.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/evaluators.py` & `glocalx-0.0.8/src/glocalx/evaluators.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/generators.py` & `glocalx-0.0.8/src/glocalx/generators.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/glocalx.py` & `glocalx-0.0.8/src/glocalx/glocalx.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/glocax_probabilistic.py` & `glocalx-0.0.8/src/glocalx/glocax_probabilistic.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/models.py` & `glocalx-0.0.8/src/glocalx/models.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/requirements.txt` & `glocalx-0.0.8/src/glocalx/requirements.txt`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/serialization.py` & `glocalx-0.0.8/src/glocalx/serialization.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/data/dummy/dummy_model.h5` & `glocalx-0.0.8/src/glocalx/data/dummy/dummy_model.h5`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/data/loaders/adult_info.json` & `glocalx-0.0.8/src/glocalx/data/loaders/adult_info.json`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/src/glocalx/loaders/lore.py` & `glocalx-0.0.8/src/glocalx/loaders/lore.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/LICENSE` & `glocalx-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/README.md` & `glocalx-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.7/pyproject.toml` & `glocalx-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "glocalx"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Mattia Setzu", email="mattia.setzu@unipi.it" },
 ]
 description = "Generating global explanations from local ones."
 readme = "README.md"
 requires-python = ">=3.8, <3.11"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers"
 ]
 dependencies = [
-    "click==7.1.2",
+    "click",
     "logzero==1.6.2",
     "numpy",
     "pandas",
     "scikit-learn",
     "scipy",
     "tensorflow==2.8",
 ]
```

