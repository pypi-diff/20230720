# Comparing `tmp/robingrad-0.0.3.tar.gz` & `tmp/robingrad-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingrad-0.0.3.tar", last modified: Mon Jul 17 16:28:44 2023, max compression
+gzip compressed data, was "robingrad-0.0.4.tar", last modified: Thu Jul 20 09:40:04 2023, max compression
```

## Comparing `robingrad-0.0.3.tar` & `robingrad-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.209900 robingrad-0.0.3/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.3/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3018 2023-07-17 16:28:44.209467 robingrad-0.0.3/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1356 2023-07-17 16:28:33.000000 robingrad-0.0.3/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-17 16:28:30.000000 robingrad-0.0.3/pyproject.toml
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.203974 robingrad-0.0.3/robingrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-17 13:45:08.000000 robingrad-0.0.3/robingrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.3/robingrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2267 2023-07-13 14:47:01.000000 robingrad-0.0.3/robingrad/lab.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.207115 robingrad-0.0.3/robingrad/nn/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.3/robingrad/nn/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1659 2023-07-17 15:58:41.000000 robingrad-0.0.3/robingrad/optim.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.3/robingrad/state.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10337 2023-07-17 14:12:32.000000 robingrad-0.0.3/robingrad/tensor.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.206605 robingrad-0.0.3/robingrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3018 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      358 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-17 16:28:44.000000 robingrad-0.0.3/robingrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-17 16:28:44.210030 robingrad-0.0.3/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-17 16:28:44.208377 robingrad-0.0.3/tests/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4840 2023-07-13 15:05:49.000000 robingrad-0.0.3/tests/test_tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.430874 robingrad-0.0.4/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.4/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3018 2023-07-20 09:40:04.430528 robingrad-0.0.4/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1356 2023-07-20 09:39:28.000000 robingrad-0.0.4/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-20 09:39:25.000000 robingrad-0.0.4/pyproject.toml
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.426755 robingrad-0.0.4/robingrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-20 09:39:36.000000 robingrad-0.0.4/robingrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.4/robingrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2267 2023-07-13 14:47:01.000000 robingrad-0.0.4/robingrad/lab.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.429232 robingrad-0.0.4/robingrad/nn/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.4/robingrad/nn/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1563 2023-07-20 09:39:18.000000 robingrad-0.0.4/robingrad/optim.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.4/robingrad/state.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10337 2023-07-17 14:12:32.000000 robingrad-0.0.4/robingrad/tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.428740 robingrad-0.0.4/robingrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3018 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      358 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-20 09:40:04.430999 robingrad-0.0.4/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.429879 robingrad-0.0.4/tests/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4840 2023-07-13 15:05:49.000000 robingrad-0.0.4/tests/test_tensor.py
```

### Comparing `robingrad-0.0.3/LICENSE` & `robingrad-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.3/PKG-INFO` & `robingrad-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.3
+Version: 0.0.4
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.3
+pip install robingrad==0.0.4
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.3/README.md` & `robingrad-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.3
+pip install robingrad==0.0.4
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.3/pyproject.toml` & `robingrad-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robingrad"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Something between Tinygrad and Micrograd"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `robingrad-0.0.3/robingrad/graph.py` & `robingrad-0.0.4/robingrad/graph.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.3/robingrad/lab.py` & `robingrad-0.0.4/robingrad/lab.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.3/robingrad/optim.py` & `robingrad-0.0.4/robingrad/optim.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     def step(self) -> None:
         for param in self.params:
             param.data += -self.lr * param.grad
 
 
 # https://pytorch.org/docs/stable/generated/torch.optim.Adam.html
 class Adam(Optimizer):
-    def __init__(self, params: List[Tensor], lr: float = 0.0001, beta1: float = 0.9, beta2: float =  0.999, eps: float = 1e-08):
+    def __init__(self, params: List[Tensor], lr: float = 0.001, beta1: float = 0.9, beta2: float =  0.999, eps: float = 1e-08):
         super().__init__(params)
         self.lr, self.beta1, self.beta2, self.eps = lr, beta1, beta2, eps
-        self.first_moments = [np.zeros_like(param.data) for param in self.params]
-        self.second_moments = [np.zeros_like(param.data) for param in self.params]
+        self.m = [np.zeros_like(param.data) for param in self.params] # first moment
+        self.v = [np.zeros_like(param.data) for param in self.params] # second moment 
         self.t = 0
 
     def step(self) -> None:
         self.t += 1
         for i, param in enumerate(self.params):
-            self.first_moments[i] = self.beta1*self.first_moments[i] + (1-self.beta1)*param.grad
-            self.second_moments[i] = self.beta2*self.second_moments[i] + (1-self.beta2)*np.power(param.grad, 2)
-            first_moment_corrected = self.first_moments[i] / (1-self.beta1**self.t)
-            second_moment_corrected = self.second_moments[i] / (1-self.beta2**self.t)
-            param.data -= self.lr * first_moment_corrected / (np.sqrt(second_moment_corrected) + self.eps)
+            self.m[i] = self.beta1*self.m[i] + (1-self.beta1)*param.grad
+            self.v[i] = self.beta2*self.v[i] + (1-self.beta2)*(param.grad**2)
+            m_hat = self.m[i] / (1-self.beta1**self.t) # first moment corrected
+            v_hat = self.v[i] / (1-self.beta2**self.t) # second moment corrected
+            param.data -= (self.lr * m_hat)/(np.sqrt(v_hat) + self.eps)
```

### Comparing `robingrad-0.0.3/robingrad/state.py` & `robingrad-0.0.4/robingrad/state.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.3/robingrad/tensor.py` & `robingrad-0.0.4/robingrad/tensor.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.3/robingrad.egg-info/PKG-INFO` & `robingrad-0.0.4/robingrad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.3
+Version: 0.0.4
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.3
+pip install robingrad==0.0.4
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.3/tests/test_tensor.py` & `robingrad-0.0.4/tests/test_tensor.py`

 * *Files identical despite different names*

