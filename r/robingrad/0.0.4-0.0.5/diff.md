# Comparing `tmp/robingrad-0.0.4.tar.gz` & `tmp/robingrad-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingrad-0.0.4.tar", last modified: Thu Jul 20 09:40:04 2023, max compression
+gzip compressed data, was "robingrad-0.0.5.tar", last modified: Thu Jul 20 13:31:42 2023, max compression
```

## Comparing `robingrad-0.0.4.tar` & `robingrad-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.430874 robingrad-0.0.4/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.4/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3018 2023-07-20 09:40:04.430528 robingrad-0.0.4/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1356 2023-07-20 09:39:28.000000 robingrad-0.0.4/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-20 09:39:25.000000 robingrad-0.0.4/pyproject.toml
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.426755 robingrad-0.0.4/robingrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-20 09:39:36.000000 robingrad-0.0.4/robingrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.4/robingrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2267 2023-07-13 14:47:01.000000 robingrad-0.0.4/robingrad/lab.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.429232 robingrad-0.0.4/robingrad/nn/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.4/robingrad/nn/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1563 2023-07-20 09:39:18.000000 robingrad-0.0.4/robingrad/optim.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.4/robingrad/state.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10337 2023-07-17 14:12:32.000000 robingrad-0.0.4/robingrad/tensor.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.428740 robingrad-0.0.4/robingrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3018 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      358 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-20 09:40:04.000000 robingrad-0.0.4/robingrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-20 09:40:04.430999 robingrad-0.0.4/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 09:40:04.429879 robingrad-0.0.4/tests/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4840 2023-07-13 15:05:49.000000 robingrad-0.0.4/tests/test_tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.201097 robingrad-0.0.5/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.5/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-20 13:31:42.200420 robingrad-0.0.5/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1289 2023-07-20 13:31:13.000000 robingrad-0.0.5/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-20 13:30:46.000000 robingrad-0.0.5/pyproject.toml
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.194384 robingrad-0.0.5/robingrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-20 13:30:55.000000 robingrad-0.0.5/robingrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.5/robingrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2267 2023-07-13 14:47:01.000000 robingrad-0.0.5/robingrad/lab.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.197286 robingrad-0.0.5/robingrad/nn/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.5/robingrad/nn/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1564 2023-07-20 13:31:06.000000 robingrad-0.0.5/robingrad/optim.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.5/robingrad/state.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10337 2023-07-17 14:12:32.000000 robingrad-0.0.5/robingrad/tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.196792 robingrad-0.0.5/robingrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      358 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-20 13:31:42.201269 robingrad-0.0.5/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.198469 robingrad-0.0.5/tests/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4840 2023-07-13 15:05:49.000000 robingrad-0.0.5/tests/test_tensor.py
```

### Comparing `robingrad-0.0.4/LICENSE` & `robingrad-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.4/PKG-INFO` & `robingrad-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.4
+Version: 0.0.5
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.4
+pip install robingrad==0.0.5
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
@@ -67,12 +67,7 @@
         x = self.l2(x)
         return x
         
 model = RobinNet()
 res = model(X_train[0].reshape((1,5)))
 draw_dot(res)
 ```
-
-## Todos
-
-* Implement the `optim` module.
-* Test for Linear layer.
```

### Comparing `robingrad-0.0.4/README.md` & `robingrad-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.4
+pip install robingrad==0.0.5
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
@@ -46,12 +46,7 @@
         x = self.l2(x)
         return x
         
 model = RobinNet()
 res = model(X_train[0].reshape((1,5)))
 draw_dot(res)
 ```
-
-## Todos
-
-* Implement the `optim` module.
-* Test for Linear layer.
```

### Comparing `robingrad-0.0.4/pyproject.toml` & `robingrad-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robingrad"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Something between Tinygrad and Micrograd"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `robingrad-0.0.4/robingrad/graph.py` & `robingrad-0.0.5/robingrad/graph.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.4/robingrad/lab.py` & `robingrad-0.0.5/robingrad/lab.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.4/robingrad/optim.py` & `robingrad-0.0.5/robingrad/optim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tinygrad.tensor import Tensor
+from robingrad.tensor import Tensor
 import numpy as np
 from typing import List
 
 class Optimizer:
     def __init__(self, params: List[Tensor]):
         self.params = params
```

### Comparing `robingrad-0.0.4/robingrad/state.py` & `robingrad-0.0.5/robingrad/state.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.4/robingrad/tensor.py` & `robingrad-0.0.5/robingrad/tensor.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.4/robingrad.egg-info/PKG-INFO` & `robingrad-0.0.5/robingrad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.4
+Version: 0.0.5
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.4
+pip install robingrad==0.0.5
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
@@ -67,12 +67,7 @@
         x = self.l2(x)
         return x
         
 model = RobinNet()
 res = model(X_train[0].reshape((1,5)))
 draw_dot(res)
 ```
-
-## Todos
-
-* Implement the `optim` module.
-* Test for Linear layer.
```

### Comparing `robingrad-0.0.4/tests/test_tensor.py` & `robingrad-0.0.5/tests/test_tensor.py`

 * *Files identical despite different names*

