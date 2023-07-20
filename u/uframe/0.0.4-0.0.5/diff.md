# Comparing `tmp/uframe-0.0.4.tar.gz` & `tmp/uframe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uframe-0.0.4.tar", last modified: Thu Jul 20 08:31:44 2023, max compression
+gzip compressed data, was "uframe-0.0.5.tar", last modified: Thu Jul 20 14:33:44 2023, max compression
```

## Comparing `uframe-0.0.4.tar` & `uframe-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.735144 uframe-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-07-20 08:31:44.735144 uframe-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.4/README.md
--rw-rw-rw-   0        0        0     1053 2023-07-20 08:30:55.000000 uframe-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      462 2023-07-20 08:31:44.735144 uframe-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-07-11 11:16:34.000000 uframe-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.697028 uframe-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.719509 uframe-0.0.4/src/uframe/
--rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.4/src/uframe/__init__.py
--rw-rw-rw-   0        0        0    61174 2023-07-20 08:30:39.000000 uframe-0.0.4/src/uframe/uframe.py
--rw-rw-rw-   0        0        0     7066 2023-07-11 11:16:34.000000 uframe-0.0.4/src/uframe/uframe_from_mice.py
--rw-rw-rw-   0        0        0    12408 2023-07-11 11:16:34.000000 uframe-0.0.4/src/uframe/uframe_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.735144 uframe-0.0.4/src/uframe.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.4/src/uframe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       85 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.735144 uframe-0.0.4/tests/
--rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.4/tests/test_uframe.py
--rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.4/tests/test_uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.578837 uframe-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-07-20 14:33:44.578837 uframe-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1055 2023-07-20 14:33:01.000000 uframe-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      462 2023-07-20 14:33:44.578837 uframe-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.545908 uframe-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.563156 uframe-0.0.5/src/uframe/
+-rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.5/src/uframe/__init__.py
+-rw-rw-rw-   0        0        0    61223 2023-07-20 11:22:06.000000 uframe-0.0.5/src/uframe/uframe.py
+-rw-rw-rw-   0        0        0     7071 2023-07-20 09:00:36.000000 uframe-0.0.5/src/uframe/uframe_from_mice.py
+-rw-rw-rw-   0        0        0    12958 2023-07-20 11:30:18.000000 uframe-0.0.5/src/uframe/uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.578837 uframe-0.0.5/src/uframe.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.5/src/uframe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      142 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.578837 uframe-0.0.5/tests/
+-rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.5/tests/test_uframe.py
+-rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.5/tests/test_uframe_instance.py
```

### Comparing `uframe-0.0.4/LICENSE` & `uframe-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uframe-0.0.4/PKG-INFO` & `uframe-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.4/README.md` & `uframe-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `uframe-0.0.4/pyproject.toml` & `uframe-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 [build-system]
 requires = ["setuptools>=42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
@@ -20,15 +21,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
 
 [project]
 name = "uframe"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Christian Amesoder", email="christian.amesoeder@informatik.uni-regensburg.de" },
   { name="Michael Hagn", email="michael.hagn@stud.uni-regensburg.de" }
 ]
 description = "Package for handling uncertain data"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `uframe-0.0.4/src/uframe/__init__.py` & `uframe-0.0.5/src/uframe/__init__.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.4/src/uframe/uframe.py` & `uframe-0.0.5/src/uframe/uframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -865,17 +865,17 @@
 
         raise NotImplementedError()
 
     def mode(self):
 
         return np.concatenate([inst.mode() for inst in self.data], axis=0)
 
-    def sample(self, n=1, seed=None):
+    def sample(self, n=1, seed=None, threshold = 1):
 
-        return np.concatenate([inst.sample(n, seed) for inst in self.data], axis=0)
+        return np.concatenate([inst.sample(n = n, seed = seed, threshold = threshold) for inst in self.data], axis=0)
 
     def ev(self):
         
         evs = [inst.ev() for inst in self.data]
         if 'categorical' not in self._col_dtype:
             
             #print([(ev, type(ev)) for ev in evs])
```

### Comparing `uframe-0.0.4/src/uframe/uframe_from_mice.py` & `uframe-0.0.5/src/uframe/uframe_from_mice.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     missing = np.random.binomial(1, p, shape)
     
     y[missing.astype('bool')] = np.nan
     return y, missing
 
 
 def uframe_from_array_mice_2(a: np.ndarray, p=0.1, mice_iterations=5, kernel="stats.gaussian_kde",
-                           scaler= "min_max", cat_indices=[]):
+                           scaler= "min_max", cat_indices=[], **kwargs):
 
     x, missing = generate_missing_values(a, p)
 
     distr = {}
     cat_distr = {}
     index_dict={}
 
@@ -159,15 +159,15 @@
         #print("Shape of imp array", imp_array.shape)
 
         if kernel == "stats.gaussian_kde":
             kde = stats.gaussian_kde(imp_array)
 
         else:
             imp_array = imp_array.T
-            kde = KernelDensity(kernel=kernel, bandwidth=1.0).fit(imp_array)
+            kde = KernelDensity(kernel=kernel, **kwargs).fit(imp_array)
             #print("Dimension of kde", kde.n_features_in_)
 
         imp_distr = kde
 
         distr[i] = imp_distr
 
     #print(x)
```

### Comparing `uframe-0.0.4/src/uframe/uframe_instance.py` & `uframe-0.0.5/src/uframe/uframe_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,18 +176,31 @@
 
     def __mode_categorical(self):
         if self.n_categorical == 0:
             return np.array([])
         return np.array([list(dist.keys())[np.argmax([*dist.values()])] for dist in self.categorical]).reshape(1, -1)
 
     # sampling functions
-    def sample(self, n: int = 1, seed: Optional[int] = None):
-
-        return self.__align(self.sample_continuous(n, seed), self.sample_categorical(n, seed), n)
-
+    def sample(self, n: int = 1, seed: Optional[int] = None, threshold: Optional[float] = 1):
+        if threshold == 1:
+            return self.__align(self.sample_continuous(n, seed), self.sample_categorical(n, seed), n)
+        else: 
+            
+            samples = self.__align(self.sample_continuous(n, seed), self.sample_categorical(n, seed), n)
+            
+            pdfs = self.pdf(samples)
+            
+            sort_ind = np.argsort(pdfs, axis = 0)
+            sort_ind = np.squeeze(sort_ind[:])
+            sort_ind = sort_ind[sort_ind < round(n*threshold)]
+                
+            return samples[sort_ind,:]             
+                
+                
+                
     def sample_categorical(self, n: int = 1, seed: Optional[int] = None):
         if self.n_categorical == 0:
             return np.array([])
         return np.array([self.__sample_categorical_dist(dist, n, seed) for dist in self.categorical]).transpose()
 
     def __sample_categorical_dist(self, dist, n, seed: Optional[int] = None):
         return np.random.choice(list(dist.keys()), size=n, p=[*dist.values()])
```

### Comparing `uframe-0.0.4/src/uframe.egg-info/PKG-INFO` & `uframe-0.0.5/src/uframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.4/tests/test_uframe_instance.py` & `uframe-0.0.5/tests/test_uframe_instance.py`

 * *Files identical despite different names*

