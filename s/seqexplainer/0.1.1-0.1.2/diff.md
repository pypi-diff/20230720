# Comparing `tmp/seqexplainer-0.1.1.tar.gz` & `tmp/seqexplainer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqexplainer-0.1.1.tar", max compression
+gzip compressed data, was "seqexplainer-0.1.2.tar", max compression
```

## Comparing `seqexplainer-0.1.1.tar` & `seqexplainer-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1066 2023-03-26 17:51:58.000000 seqexplainer-0.1.1/LICENSE
--rw-r--r--   0        0        0     1992 2023-03-26 17:52:14.000000 seqexplainer-0.1.1/README.md
--rw-r--r--   0        0        0      457 2023-07-20 19:48:33.000000 seqexplainer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      263 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/__init__.py
--rw-r--r--   0        0        0     2959 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/_ism.py
--rw-r--r--   0        0        0     2815 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/_layer_outs.py
--rw-r--r--   0        0        0     4628 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/_utils.py
--rw-r--r--   0        0        0       75 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/__init__.py
--rw-r--r--   0        0        0     3732 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/_attributions.py
--rw-r--r--   0        0        0     7568 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/_modisco.py
--rw-r--r--   0        0        0     3943 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/_plot.py
--rw-r--r--   0        0        0    11133 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/attributions/_references.py
--rw-r--r--   0        0        0     4242 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/deprecated/_deprecated.py
--rw-r--r--   0        0        0    12072 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/experimental/_experimental.py
--rw-r--r--   0        0        0      180 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/__init__.py
--rw-r--r--   0        0        0     3244 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/_activations.py
--rw-r--r--   0        0        0      914 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/_annotate.py
--rw-r--r--   0        0        0     1912 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/_motifs.py
--rw-r--r--   0        0        0     1457 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/filters/_plot.py
--rw-r--r--   0        0        0       33 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/generative/__init__.py
--rw-r--r--   0        0        0     6155 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/generative/_evolution.py
--rw-r--r--   0        0        0       39 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/__init__.py
--rw-r--r--   0        0        0     5178 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_complex_perturb.py
--rw-r--r--   0        0        0     3971 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_gia.py
--rw-r--r--   0        0        0        0 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_gia_helpers.py
--rw-r--r--   0        0        0     2459 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_null_models.py
--rw-r--r--   0        0        0    16623 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/gia/_perturb.py
--rw-r--r--   0        0        0     9445 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/preprocess/_helpers.py
--rw-r--r--   0        0        0    13895 2023-07-20 18:27:42.000000 seqexplainer-0.1.1/seqexplainer/preprocess/_preprocess.py
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 seqexplainer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-03-26 17:51:58.000000 seqexplainer-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1992 2023-03-26 17:52:14.000000 seqexplainer-0.1.2/README.md
+-rw-r--r--   0        0        0      457 2023-07-20 19:56:50.000000 seqexplainer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/__init__.py
+-rw-r--r--   0        0        0     2959 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/_ism.py
+-rw-r--r--   0        0        0     2815 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/_layer_outs.py
+-rw-r--r--   0        0        0     4628 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/_utils.py
+-rw-r--r--   0        0        0       75 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/attributions/__init__.py
+-rw-r--r--   0        0        0     3732 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/attributions/_attributions.py
+-rw-r--r--   0        0        0     7568 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/attributions/_modisco.py
+-rw-r--r--   0        0        0     3943 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/attributions/_plot.py
+-rw-r--r--   0        0        0    11133 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/attributions/_references.py
+-rw-r--r--   0        0        0     4242 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/deprecated/_deprecated.py
+-rw-r--r--   0        0        0    12072 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/experimental/_experimental.py
+-rw-r--r--   0        0        0      180 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/filters/__init__.py
+-rw-r--r--   0        0        0     3244 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/filters/_activations.py
+-rw-r--r--   0        0        0      914 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/filters/_annotate.py
+-rw-r--r--   0        0        0     1912 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/filters/_motifs.py
+-rw-r--r--   0        0        0     1457 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/filters/_plot.py
+-rw-r--r--   0        0        0       33 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/generative/__init__.py
+-rw-r--r--   0        0        0     6155 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/generative/_evolution.py
+-rw-r--r--   0        0        0       39 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/gia/__init__.py
+-rw-r--r--   0        0        0     5178 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/gia/_complex_perturb.py
+-rw-r--r--   0        0        0     3971 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/gia/_gia.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/gia/_gia_helpers.py
+-rw-r--r--   0        0        0     2459 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/gia/_null_models.py
+-rw-r--r--   0        0        0    16623 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/gia/_perturb.py
+-rw-r--r--   0        0        0     9445 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/preprocess/_helpers.py
+-rw-r--r--   0        0        0    13895 2023-07-20 18:27:42.000000 seqexplainer-0.1.2/seqexplainer/preprocess/_preprocess.py
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 seqexplainer-0.1.2/PKG-INFO
```

### Comparing `seqexplainer-0.1.1/LICENSE` & `seqexplainer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/README.md` & `seqexplainer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/_ism.py` & `seqexplainer-0.1.2/seqexplainer/_ism.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/_layer_outs.py` & `seqexplainer-0.1.2/seqexplainer/_layer_outs.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/_utils.py` & `seqexplainer-0.1.2/seqexplainer/_utils.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/attributions/_attributions.py` & `seqexplainer-0.1.2/seqexplainer/attributions/_attributions.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/attributions/_modisco.py` & `seqexplainer-0.1.2/seqexplainer/attributions/_modisco.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/attributions/_plot.py` & `seqexplainer-0.1.2/seqexplainer/attributions/_plot.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/attributions/_references.py` & `seqexplainer-0.1.2/seqexplainer/attributions/_references.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/deprecated/_deprecated.py` & `seqexplainer-0.1.2/seqexplainer/deprecated/_deprecated.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/experimental/_experimental.py` & `seqexplainer-0.1.2/seqexplainer/experimental/_experimental.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/filters/_activations.py` & `seqexplainer-0.1.2/seqexplainer/filters/_activations.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/filters/_annotate.py` & `seqexplainer-0.1.2/seqexplainer/filters/_annotate.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/filters/_motifs.py` & `seqexplainer-0.1.2/seqexplainer/filters/_motifs.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/filters/_plot.py` & `seqexplainer-0.1.2/seqexplainer/filters/_plot.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/generative/_evolution.py` & `seqexplainer-0.1.2/seqexplainer/generative/_evolution.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/gia/_complex_perturb.py` & `seqexplainer-0.1.2/seqexplainer/gia/_complex_perturb.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/gia/_gia.py` & `seqexplainer-0.1.2/seqexplainer/gia/_gia.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/gia/_null_models.py` & `seqexplainer-0.1.2/seqexplainer/gia/_null_models.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/gia/_perturb.py` & `seqexplainer-0.1.2/seqexplainer/gia/_perturb.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/preprocess/_helpers.py` & `seqexplainer-0.1.2/seqexplainer/preprocess/_helpers.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/seqexplainer/preprocess/_preprocess.py` & `seqexplainer-0.1.2/seqexplainer/preprocess/_preprocess.py`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.1.1/PKG-INFO` & `seqexplainer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqexplainer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interpreting sequence-to-function machine learning models
 Author: adamklie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

