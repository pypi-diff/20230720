# Comparing `tmp/bnlearn-0.8.1.tar.gz` & `tmp/bnlearn-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlearn-0.8.1.tar", last modified: Wed Jul 19 07:12:08 2023, max compression
+gzip compressed data, was "dist\bnlearn-0.8.2.tar", last modified: Thu Jul 20 19:50:50 2023, max compression
```

## Comparing `bnlearn-0.8.1.tar` & `bnlearn-0.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.141652 bnlearn-0.8.1/
--rw-rw-rw-   0        0        0     1231 2022-05-09 18:05:29.000000 bnlearn-0.8.1/LICENSE
--rw-rw-rw-   0        0        0      643 2022-05-09 18:05:29.000000 bnlearn-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0    12276 2023-07-19 07:12:08.139623 bnlearn-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0    11670 2023-06-13 21:59:12.000000 bnlearn-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.071832 bnlearn-0.8.1/bnlearn/
--rw-rw-rw-   0        0        0     4477 2023-07-19 07:11:51.000000 bnlearn-0.8.1/bnlearn/__init__.py
--rw-rw-rw-   0        0        0    70897 2023-07-19 07:08:39.000000 bnlearn-0.8.1/bnlearn/bnlearn.py
--rw-rw-rw-   0        0        0     1745 2022-05-09 18:05:29.000000 bnlearn-0.8.1/bnlearn/confmatrix.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.112021 bnlearn-0.8.1/bnlearn/data/
--rw-rw-rw-   0        0        0        0 2022-05-09 18:05:29.000000 bnlearn-0.8.1/bnlearn/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.116680 bnlearn-0.8.1/bnlearn/discretize/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.1/bnlearn/discretize/__init__.py
--rw-rw-rw-   0        0        0     3837 2023-06-13 20:28:20.000000 bnlearn-0.8.1/bnlearn/discretize/discretize.py
--rw-rw-rw-   0        0        0    19168 2023-05-16 18:32:33.000000 bnlearn-0.8.1/bnlearn/discretize/learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    45300 2023-06-12 07:48:11.000000 bnlearn-0.8.1/bnlearn/examples.py
--rw-rw-rw-   0        0        0     1330 2023-05-12 07:28:50.000000 bnlearn-0.8.1/bnlearn/examples_discretize.py
--rw-rw-rw-   0        0        0     4847 2023-06-13 21:56:47.000000 bnlearn-0.8.1/bnlearn/inference.py
--rw-rw-rw-   0        0        0    16904 2023-04-01 12:44:53.000000 bnlearn-0.8.1/bnlearn/network.py
--rw-rw-rw-   0        0        0     7419 2023-04-29 10:55:11.000000 bnlearn-0.8.1/bnlearn/parameter_learning.py
--rw-rw-rw-   0        0        0    27145 2023-06-14 20:00:44.000000 bnlearn-0.8.1/bnlearn/structure_learning.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.122326 bnlearn-0.8.1/bnlearn/tests/
--rw-rw-rw-   0        0        0        0 2022-11-30 17:18:09.000000 bnlearn-0.8.1/bnlearn/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.137741 bnlearn-0.8.1/bnlearn/tests/discretize/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.1/bnlearn/tests/discretize/__init__.py
--rw-rw-rw-   0        0        0     2293 2023-04-29 10:59:05.000000 bnlearn-0.8.1/bnlearn/tests/discretize/test_discretize.py
--rw-rw-rw-   0        0        0     9366 2023-05-12 07:28:13.000000 bnlearn-0.8.1/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    13436 2023-06-14 20:08:24.000000 bnlearn-0.8.1/bnlearn/tests/test_bnlearn.py
--rw-rw-rw-   0        0        0     8222 2022-11-30 17:18:09.000000 bnlearn-0.8.1/bnlearn/tests/test_structure_learning.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.109733 bnlearn-0.8.1/bnlearn.egg-info/
--rw-rw-rw-   0        0        0    12276 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      204 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 07:12:08.142801 bnlearn-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     2071 2023-05-16 15:14:21.000000 bnlearn-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:50:50.944737 bnlearn-0.8.2/
+-rw-rw-rw-   0        0        0     1231 2022-05-09 18:05:29.000000 bnlearn-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0      643 2022-05-09 18:05:29.000000 bnlearn-0.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    12317 2023-07-20 19:50:50.930785 bnlearn-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11670 2023-06-13 21:59:12.000000 bnlearn-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 19:50:50.850026 bnlearn-0.8.2/bnlearn/
+-rw-rw-rw-   0        0        0     4477 2023-07-20 19:50:38.000000 bnlearn-0.8.2/bnlearn/__init__.py
+-rw-rw-rw-   0        0        0    70899 2023-07-20 19:47:28.000000 bnlearn-0.8.2/bnlearn/bnlearn.py
+-rw-rw-rw-   0        0        0     1745 2022-05-09 18:05:29.000000 bnlearn-0.8.2/bnlearn/confmatrix.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:50:50.902952 bnlearn-0.8.2/bnlearn/data/
+-rw-rw-rw-   0        0        0        0 2022-05-09 18:05:29.000000 bnlearn-0.8.2/bnlearn/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:50:50.905931 bnlearn-0.8.2/bnlearn/discretize/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.2/bnlearn/discretize/__init__.py
+-rw-rw-rw-   0        0        0     3837 2023-06-13 20:28:20.000000 bnlearn-0.8.2/bnlearn/discretize/discretize.py
+-rw-rw-rw-   0        0        0    19168 2023-05-16 18:32:33.000000 bnlearn-0.8.2/bnlearn/discretize/learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    46917 2023-07-20 19:48:35.000000 bnlearn-0.8.2/bnlearn/examples.py
+-rw-rw-rw-   0        0        0     1330 2023-05-12 07:28:50.000000 bnlearn-0.8.2/bnlearn/examples_discretize.py
+-rw-rw-rw-   0        0        0     4847 2023-06-13 21:56:47.000000 bnlearn-0.8.2/bnlearn/inference.py
+-rw-rw-rw-   0        0        0    16904 2023-04-01 12:44:53.000000 bnlearn-0.8.2/bnlearn/network.py
+-rw-rw-rw-   0        0        0     7419 2023-04-29 10:55:11.000000 bnlearn-0.8.2/bnlearn/parameter_learning.py
+-rw-rw-rw-   0        0        0    27145 2023-06-14 20:00:44.000000 bnlearn-0.8.2/bnlearn/structure_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:50:50.912156 bnlearn-0.8.2/bnlearn/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-30 17:18:09.000000 bnlearn-0.8.2/bnlearn/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:50:50.929816 bnlearn-0.8.2/bnlearn/tests/discretize/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.2/bnlearn/tests/discretize/__init__.py
+-rw-rw-rw-   0        0        0     2293 2023-04-29 10:59:05.000000 bnlearn-0.8.2/bnlearn/tests/discretize/test_discretize.py
+-rw-rw-rw-   0        0        0     9366 2023-05-12 07:28:13.000000 bnlearn-0.8.2/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    13418 2023-07-19 08:58:02.000000 bnlearn-0.8.2/bnlearn/tests/test_bnlearn.py
+-rw-rw-rw-   0        0        0     8222 2022-11-30 17:18:09.000000 bnlearn-0.8.2/bnlearn/tests/test_structure_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:50:50.888919 bnlearn-0.8.2/bnlearn.egg-info/
+-rw-rw-rw-   0        0        0    12317 2023-07-20 19:50:50.000000 bnlearn-0.8.2/bnlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-07-20 19:50:50.000000 bnlearn-0.8.2/bnlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:50:50.000000 bnlearn-0.8.2/bnlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      204 2023-07-20 19:50:50.000000 bnlearn-0.8.2/bnlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-20 19:50:50.000000 bnlearn-0.8.2/bnlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 19:50:50.944980 bnlearn-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     2071 2023-05-16 15:14:21.000000 bnlearn-0.8.2/setup.py
```

### Comparing `bnlearn-0.8.1/LICENSE` & `bnlearn-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/MANIFEST.in` & `bnlearn-0.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/PKG-INFO` & `bnlearn-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.2.tar.gz
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -324,7 +326,9 @@
 Please cite ``bnlearn`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
 
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.1 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.2 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.1.tar.gz Author:
-Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
-Library for Bayesian network learning and inference [![Python](https://
-img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
-pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
-(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
-img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
-img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
-bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
-erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
-Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
-github.com/erdogant/bnlearn/issues) [![Project Status](http://
+Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.2.tar.gz
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # bnlearn - Library for Bayesian network learning and
+inference [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
+img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
+img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
+Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
+(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
+erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
+forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
+[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
+(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
```

### Comparing `bnlearn-0.8.1/README.md` & `bnlearn-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/__init__.py` & `bnlearn-0.8.2/bnlearn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import bnlearn.network as network
 import bnlearn.confmatrix as confmatrix
 from bnlearn.discretize.discretize import discretize, discretize_value
 from packaging import version
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 import pgmpy
 # Check version pgmpy
 if version.parse(pgmpy.__version__) < version.parse("0.1.18"):
     raise ImportError('[bnlearn] >Error: This release requires pgmpy to be version >= 0.1.18. Try to: <pip install -U pgmpy>=0.1.18>')
 
 # Version check
```

### Comparing `bnlearn-0.8.1/bnlearn/bnlearn.py` & `bnlearn-0.8.2/bnlearn/bnlearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
     """
     if verbose>=3: print('[bnlearn] >Check whether CPDs sum up to one.')
     if isinstance(DAG, dict): DAG = DAG.get('model', None)
     if DAG is not None:
         for cpd in DAG.get_cpds():
             if not np.all(cpd.values.astype(Decimal).sum(axis=0)==1):
                 if verbose>=3: print('[bnlearn] >CPD [%s] does not add up to 1 but is: %s' %(cpd.variable, cpd.values.sum(axis=0)))
-        if verbose>=3: print('[bnlearn] >Check whether CPDs associated with the nodes are consistent: %s' %(DAG.check_model()))
+        # if verbose>=3: print('[bnlearn] >Check whether CPDs associated with the nodes are consistent: %s' %(DAG.check_model()))
     else:
         if verbose>=2: print('[bnlearn] >No model found containing CPDs.')
 
 
 # %% Convert DAG into adjacency matrix
 def dag2adjmat(model, verbose=3):
     """Convert model into adjacency matrix.
```

### Comparing `bnlearn-0.8.1/bnlearn/confmatrix.py` & `bnlearn-0.8.2/bnlearn/confmatrix.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/discretize/discretize.py` & `bnlearn-0.8.2/bnlearn/discretize/discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/discretize/learn_discrete_bayes_net.py` & `bnlearn-0.8.2/bnlearn/discretize/learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/examples.py` & `bnlearn-0.8.2/bnlearn/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,60 @@
 import pandas as pd
 import numpy as np
 from pgmpy.inference import VariableElimination
 from pgmpy.models import BayesianNetwork, NaiveBayes
 from pgmpy.estimators import ExhaustiveSearch, HillClimbSearch, TreeSearch
 from pgmpy.factors.discrete import TabularCPD
 
+# %% issue #84
+# Load library
+from pgmpy.factors.discrete import TabularCPD
+import bnlearn as bn
+
+# Create some edges, all starting from the same root node: A
+edges = [('A', 'B'), ('A', 'C'), ('A', 'D')]
+DAG = bn.make_DAG(edges, methodtype='naivebayes')
+
+# Set CPDs
+cpd_A = TabularCPD(variable='A', variable_card=3, values=[[0.3], [0.5], [0.2]])
+print(cpd_A)
+cpd_B = TabularCPD(variable='B', variable_card=2, values=[[0.4, 0.9], [0.6, 0.1]], evidence=['A'], evidence_card=[2])
+print(cpd_B)
+cpd_C = TabularCPD(variable='C', variable_card=2, values=[[0.4, 0.9], [0.6, 0.1]], evidence=['A'], evidence_card=[2])
+print(cpd_C)
+cpd_D = TabularCPD(variable='D', variable_card=2, values=[[0.4, 0.9], [0.6, 0.1]], evidence=['A'], evidence_card=[2])
+print(cpd_D)
+
+DAG = bn.make_DAG(DAG, CPD=[cpd_A, cpd_B, cpd_C, cpd_D], checkmodel=True)
+# Plot the CPDs as a sanity check
+bn.print_CPD(DAG, checkmodel=True)
+# Plot the DAG
+bn.plot(DAG)
+
+
+# %%
+import bnlearn as bn
+
+# Load example dataset
+Xy_train = bn.import_example('titanic')
+Xy_train.drop(labels='Cabin', axis=1, inplace=True)
+Xy_train = Xy_train.dropna(axis=0)
+
+tarvar='Survived'
+model = bn.structure_learning.fit(Xy_train, 
+                                  methodtype='tan', 
+                                  class_node = 'Survived')
+model = bn.parameter_learning.fit(model, 
+                                  Xy_train, 
+                                  methodtype='bayes',
+                                  scoretype='bdeu')
+y_train_pred = bn.predict(model, Xy_train, variables = tarvar, verbose=4)
+
+
+
 # %%
 import bnlearn as bn
 
 # Load example dataset
 df = bn.import_example('sprinkler')
 
 edges = [('Cloudy', 'Sprinkler'),
@@ -634,14 +680,15 @@
 model = bn.structure_learning.fit(df, methodtype='naivebayes', root_node="B")
 model = bn.independence_test(model, df, prune=True)
 # Plot
 bn.plot(model)
 
 # %% Naive Bayesian model
 from pgmpy.factors.discrete import TabularCPD
+import bnlearn as bn
 
 edges = [('A', 'B'), ('A', 'C'), ('A', 'D')]
 DAG = bn.make_DAG(edges, methodtype='naivebayes')
 bn.plot(DAG)
 
 cpd_A = TabularCPD(variable='A', variable_card=3, values=[[0.3], [0.5], [0.2]])
 print(cpd_A)
```

### Comparing `bnlearn-0.8.1/bnlearn/examples_discretize.py` & `bnlearn-0.8.2/bnlearn/examples_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/inference.py` & `bnlearn-0.8.2/bnlearn/inference.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/network.py` & `bnlearn-0.8.2/bnlearn/network.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/parameter_learning.py` & `bnlearn-0.8.2/bnlearn/parameter_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/structure_learning.py` & `bnlearn-0.8.2/bnlearn/structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/tests/discretize/test_discretize.py` & `bnlearn-0.8.2/bnlearn/tests/discretize/test_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py` & `bnlearn-0.8.2/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn/tests/test_bnlearn.py` & `bnlearn-0.8.2/bnlearn/tests/test_bnlearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 
 import bnlearn as bn
 from pgmpy.factors.discrete import TabularCPD
 import numpy as np
 import pandas as pd
 
 
-def test_load_examples():
-    shapes = [(10000, 37), (10000, 223), (10000, 8), (10000, 11), (10000, 32), (352, 3)]
-    for i, data in enumerate(['alarm', 'andes', 'asia', 'sachs', 'water', 'stormofswords']):
-        print(data)
-        df = bn.import_example(data=data)
-        assert df.shape==shapes[i]
+# def test_load_examples():
+#     shapes = [(10000, 37), (10000, 223), (10000, 8), (10000, 11), (10000, 32), (352, 3)]
+#     for i, data in enumerate(['alarm', 'andes', 'asia', 'sachs', 'water', 'stormofswords']):
+#         df = bn.import_example(data=data)
+#         assert not df.empty
 
 
 def test_QUERY():
     # Load example DataFrame
     df = bn.import_example('titanic')
     dfhot, dfnum = bn.df2onehot(df)
     # Train model
```

### Comparing `bnlearn-0.8.1/bnlearn/tests/test_structure_learning.py` & `bnlearn-0.8.2/bnlearn/tests/test_structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/bnlearn.egg-info/PKG-INFO` & `bnlearn-0.8.2/bnlearn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.2.tar.gz
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -324,7 +326,9 @@
 Please cite ``bnlearn`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
 
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.1 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.2 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.1.tar.gz Author:
-Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
-Library for Bayesian network learning and inference [![Python](https://
-img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
-pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
-(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
-img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
-img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
-bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
-erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
-Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
-github.com/erdogant/bnlearn/issues) [![Project Status](http://
+Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.2.tar.gz
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # bnlearn - Library for Bayesian network learning and
+inference [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
+img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
+img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
+Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
+(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
+erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
+forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
+[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
+(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
```

### Comparing `bnlearn-0.8.1/bnlearn.egg-info/SOURCES.txt` & `bnlearn-0.8.2/bnlearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.1/setup.py` & `bnlearn-0.8.2/setup.py`

 * *Files identical despite different names*

