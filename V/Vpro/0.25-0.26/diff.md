# Comparing `tmp/Vpro-0.25.tar.gz` & `tmp/Vpro-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vpro-0.25.tar", last modified: Thu Jul 20 09:18:07 2023, max compression
+gzip compressed data, was "Vpro-0.26.tar", last modified: Thu Jul 20 11:56:02 2023, max compression
```

## Comparing `Vpro-0.25.tar` & `Vpro-0.26.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 09:18:07.314864 Vpro-0.25/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-20 09:18:07.314609 Vpro-0.25/PKG-INFO
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 09:18:07.313566 Vpro-0.25/Vpro/
--rw-r--r--   0 Agastyaa   (502) staff       (20)     7735 2023-07-20 09:17:39.000000 Vpro-0.25/Vpro/__init__.py
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 09:18:07.314417 Vpro-0.25/Vpro.egg-info/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/PKG-INFO
--rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/SOURCES.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/dependency_links.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/requires.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/top_level.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-20 09:18:07.314906 Vpro-0.25/setup.cfg
--rw-r--r--   0 Agastyaa   (502) staff       (20)      547 2023-07-20 09:18:05.000000 Vpro-0.25/setup.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 11:56:02.018065 Vpro-0.26/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-20 11:56:02.017924 Vpro-0.26/PKG-INFO
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 11:56:02.016923 Vpro-0.26/Vpro/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)     7743 2023-07-20 11:55:51.000000 Vpro-0.26/Vpro/__init__.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 11:56:02.017698 Vpro-0.26/Vpro.egg-info/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-20 11:56:01.000000 Vpro-0.26/Vpro.egg-info/PKG-INFO
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-20 11:56:01.000000 Vpro-0.26/Vpro.egg-info/SOURCES.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-20 11:56:01.000000 Vpro-0.26/Vpro.egg-info/dependency_links.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-20 11:56:01.000000 Vpro-0.26/Vpro.egg-info/requires.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-20 11:56:01.000000 Vpro-0.26/Vpro.egg-info/top_level.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-20 11:56:02.018127 Vpro-0.26/setup.cfg
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      547 2023-07-20 11:55:56.000000 Vpro-0.26/setup.py
```

### Comparing `Vpro-0.25/Vpro/__init__.py` & `Vpro-0.26/Vpro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,40 +98,40 @@
 
     for i in range (U):
         b.append(np.zeros(D))
     b.append(np.zeros(O))
 
     return [w, b]
 
-def uniform_innitialise(I, U, D, O, a, b):
+def uniform_innitialise(I, U, D, O, a1, a2):
     w=[]
     b=[]
     w1=[]
     for i in range(I):
         wx=[]
         for j in range(D):
-            wx.append(random.uniform(a, b))
+            wx.append(random.uniform(a1, a2))
         w1.append(wx)
     w.append(np.array(w1))
 
     for k in range(U-1):
         wx=[]
         for i in range(D):
             wy=[]
             for j in range(D):
-                wy.append(random.uniform(a, b))
+                wy.append(random.uniform(a1, a2))
             wx.append(wy)
         w.append(np.array(wx))
     
     wf=[]
 
     for i in range(D):
         wx=[]
         for j in range(O):
-            wx.append(random.uniform(a,b))
+            wx.append(random.uniform(a1,a2))
         wf.append(wx)
     
     w.append(np.array(wf))
 
     for i in range (U):
         b.append(np.zeros(D))
     b.append(np.zeros(O))
```

### Comparing `Vpro-0.25/setup.py` & `Vpro-0.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 from setuptools import setup
 
 setup(name= "Vpro",
-      version= 0.25,
+      version= 0.26,
       description="This is a Machine Learning Module that grants one access to a Multilayer percepton with an adjustable number of hidden layers and neurons per each layer. It also includes functionality to train the network based on a database, and has adjustable innitialisation types, activation functions, and learning hyperparamters.", 
       author="Agastyaa Vishvanath",
       packages=["Vpro"],
       install_requires= ["numpy", "tqdm"])
```

