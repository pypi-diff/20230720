# Comparing `tmp/Vpro-0.2.tar.gz` & `tmp/Vpro-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vpro-0.2.tar", last modified: Tue Jul 18 16:40:21 2023, max compression
+gzip compressed data, was "Vpro-0.25.tar", last modified: Thu Jul 20 09:18:07 2023, max compression
```

## Comparing `Vpro-0.2.tar` & `Vpro-0.25.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-18 16:40:21.903145 Vpro-0.2/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      403 2023-07-18 16:40:21.903015 Vpro-0.2/PKG-INFO
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-18 16:40:21.902139 Vpro-0.2/Vpro/
--rw-r--r--   0 Agastyaa   (502) staff       (20)     7721 2023-07-18 16:40:10.000000 Vpro-0.2/Vpro/__init__.py
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-18 16:40:21.902834 Vpro-0.2/Vpro.egg-info/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      403 2023-07-18 16:40:21.000000 Vpro-0.2/Vpro.egg-info/PKG-INFO
--rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-18 16:40:21.000000 Vpro-0.2/Vpro.egg-info/SOURCES.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-18 16:40:21.000000 Vpro-0.2/Vpro.egg-info/dependency_links.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-18 16:40:21.000000 Vpro-0.2/Vpro.egg-info/requires.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-18 16:40:21.000000 Vpro-0.2/Vpro.egg-info/top_level.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-18 16:40:21.903182 Vpro-0.2/setup.cfg
--rw-r--r--   0 Agastyaa   (502) staff       (20)      546 2023-07-18 16:40:08.000000 Vpro-0.2/setup.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 09:18:07.314864 Vpro-0.25/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-20 09:18:07.314609 Vpro-0.25/PKG-INFO
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 09:18:07.313566 Vpro-0.25/Vpro/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)     7735 2023-07-20 09:17:39.000000 Vpro-0.25/Vpro/__init__.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-20 09:18:07.314417 Vpro-0.25/Vpro.egg-info/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/PKG-INFO
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/SOURCES.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/dependency_links.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/requires.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-20 09:18:07.000000 Vpro-0.25/Vpro.egg-info/top_level.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-20 09:18:07.314906 Vpro-0.25/setup.cfg
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      547 2023-07-20 09:18:05.000000 Vpro-0.25/setup.py
```

### Comparing `Vpro-0.2/Vpro/__init__.py` & `Vpro-0.25/Vpro/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -322,33 +322,33 @@
 def train(I, w, b, A, Ns, h, T, activ):
 
     for i in tqdm(range(T)):
         
         
 
         L=[]
-        for i in range(Ns):
+        for i1 in range(Ns):
             L.append(random.randint(0, len(I)-1))
         Is=[]
-        for i in range(Ns):
-            Is.append(I[L[i]])
+        for i2 in range(Ns):
+            Is.append(I[L[i2]])
         Is=np.array(Is)
 
         ACs=[]
 
         for l in range(Ns):
             ACs.append(A[L[l]])
         ACs= np.array(ACs)
 
         X=grad(Is, w, b, ACs, activ)
 
-        for i in range(len(w)):
-            for j in range (len(w[i])):
-                for k in range(len(w[i][0])):
-                    w[i][j][k]=w[i][j][k]-h*X[0][i][j][k]
+        for i3 in range(len(w)):
+            for j in range (len(w[i3])):
+                for k in range(len(w[i3][0])):
+                    w[i3][j][k]=w[i3][j][k]-h*X[0][i3][j][k]
         
 
-        for i in range(len(b)):
-            for j in range(len(b[i])):
-                b[i][j]=b[i][j]-h*X[1][i][j]
+        for i4 in range(len(b)):
+            for j in range(len(b[i4])):
+                b[i4][j]=b[i4][j]-h*X[1][i4][j]
 
     return [w, b]
```

### Comparing `Vpro-0.2/setup.py` & `Vpro-0.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 from setuptools import setup
 
 setup(name= "Vpro",
-      version= 0.2,
+      version= 0.25,
       description="This is a Machine Learning Module that grants one access to a Multilayer percepton with an adjustable number of hidden layers and neurons per each layer. It also includes functionality to train the network based on a database, and has adjustable innitialisation types, activation functions, and learning hyperparamters.", 
       author="Agastyaa Vishvanath",
       packages=["Vpro"],
       install_requires= ["numpy", "tqdm"])
```

