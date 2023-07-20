# Comparing `tmp/partition_networkx-0.0.1.tar.gz` & `tmp/partition_networkx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/partition_networkx-0.0.1.tar", last modified: Tue May 19 19:34:51 2020, max compression
+gzip compressed data, was "partition_networkx-0.0.2.tar", last modified: Thu Jul 20 13:01:26 2023, max compression
```

## Comparing `partition_networkx-0.0.1.tar` & `partition_networkx-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 francois   (507) staff       (20)        0 2020-05-19 19:34:51.000000 partition_networkx-0.0.1/
--rw-r--r--   0 francois   (507) staff       (20)     4403 2020-05-19 19:34:51.000000 partition_networkx-0.0.1/PKG-INFO
-drwxr-xr-x   0 francois   (507) staff       (20)        0 2020-05-19 19:34:51.000000 partition_networkx-0.0.1/partition_networkx.egg-info/
--rw-r--r--   0 francois   (507) staff       (20)     4403 2020-05-19 19:34:50.000000 partition_networkx-0.0.1/partition_networkx.egg-info/PKG-INFO
--rw-r--r--   0 francois   (507) staff       (20)      299 2020-05-19 19:34:50.000000 partition_networkx-0.0.1/partition_networkx.egg-info/SOURCES.txt
--rw-r--r--   0 francois   (507) staff       (20)       30 2020-05-19 19:34:50.000000 partition_networkx-0.0.1/partition_networkx.egg-info/requires.txt
--rw-r--r--   0 francois   (507) staff       (20)       19 2020-05-19 19:34:50.000000 partition_networkx-0.0.1/partition_networkx.egg-info/top_level.txt
--rw-r--r--   0 francois   (507) staff       (20)        1 2020-05-19 19:34:50.000000 partition_networkx-0.0.1/partition_networkx.egg-info/dependency_links.txt
-drwxr-xr-x   0 francois   (507) staff       (20)        0 2020-05-19 19:34:51.000000 partition_networkx-0.0.1/partition_networkx/
--rw-r--r--   0 francois   (507) staff       (20)      191 2020-05-19 19:17:10.000000 partition_networkx-0.0.1/partition_networkx/__init__.py
--rw-r--r--   0 francois   (507) staff       (20)     5766 2020-05-19 19:20:05.000000 partition_networkx-0.0.1/partition_networkx/partition_networkx.py
--rw-r--r--   0 francois   (507) staff       (20)     3016 2020-05-19 19:30:58.000000 partition_networkx-0.0.1/README.md
--rw-r--r--   0 francois   (507) staff       (20)     1161 2020-05-19 19:26:21.000000 partition_networkx-0.0.1/setup.py
--rw-r--r--   0 francois   (507) staff       (20)       38 2020-05-19 19:34:51.000000 partition_networkx-0.0.1/setup.cfg
+drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-07-20 13:01:26.291633 partition_networkx-0.0.2/
+-rwxrwxrwx   0 francois   (501) staff       (20)     1076 2020-05-19 19:09:01.000000 partition_networkx-0.0.2/LICENSE
+-rw-r--r--   0 francois   (501) staff       (20)     3762 2023-07-20 13:01:26.291466 partition_networkx-0.0.2/PKG-INFO
+-rwxrwxrwx   0 francois   (501) staff       (20)     3016 2020-05-19 19:30:58.000000 partition_networkx-0.0.2/README.md
+drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-07-20 13:01:26.290573 partition_networkx-0.0.2/partition_networkx/
+-rwxrwxrwx   0 francois   (501) staff       (20)      191 2023-07-20 13:00:24.000000 partition_networkx-0.0.2/partition_networkx/__init__.py
+-rw-r--r--   0 francois   (501) staff       (20)     6004 2023-07-20 13:01:08.000000 partition_networkx-0.0.2/partition_networkx/partition_networkx.py
+drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-07-20 13:01:26.291258 partition_networkx-0.0.2/partition_networkx.egg-info/
+-rwxrwxrwx   0 francois   (501) staff       (20)     3762 2023-07-20 13:01:26.000000 partition_networkx-0.0.2/partition_networkx.egg-info/PKG-INFO
+-rwxrwxrwx   0 francois   (501) staff       (20)      307 2023-07-20 13:01:26.000000 partition_networkx-0.0.2/partition_networkx.egg-info/SOURCES.txt
+-rwxrwxrwx   0 francois   (501) staff       (20)        1 2023-07-20 13:01:26.000000 partition_networkx-0.0.2/partition_networkx.egg-info/dependency_links.txt
+-rwxrwxrwx   0 francois   (501) staff       (20)       30 2023-07-20 13:01:26.000000 partition_networkx-0.0.2/partition_networkx.egg-info/requires.txt
+-rwxrwxrwx   0 francois   (501) staff       (20)       19 2023-07-20 13:01:26.000000 partition_networkx-0.0.2/partition_networkx.egg-info/top_level.txt
+-rw-r--r--   0 francois   (501) staff       (20)       38 2023-07-20 13:01:26.291673 partition_networkx-0.0.2/setup.cfg
+-rwxrwxrwx   0 francois   (501) staff       (20)     1161 2023-07-20 13:00:10.000000 partition_networkx-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `partition_networkx-0.0.1/partition_networkx/partition_networkx.py` & `partition_networkx-0.0.2/partition_networkx/partition_networkx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # coding=utf-8
 import numpy as np
 import networkx
-import community
-from networkx.algorithms.core import core_number
-from collections import namedtuple
 
 ## Graph-aware measures (igraph version)
 def gam(self, u, v, method="rand", adjusted=True):
     """
     Compute one of 11 graph-aware measures to compare graph partitions.
     
     Parameters
@@ -90,33 +87,41 @@
         if method=="max":
             return(suv/np.max([su,sv]))
         else:
             print('Wrong method!')
         
     return None
 
-def community_ecg(self, weight='weight', ens_size = 16, min_weight = 0.05):
+networkx.classes.graph.Graph.gam = gam
+
+from networkx.algorithms.core import core_number
+import community
+from collections import namedtuple
+
+def community_ecg(self, weight='weight', ens_size = 16, min_weight = 0.05, resolution=1.0):
     """
     Stable ensemble-based graph clustering;
     the ensemble consists of single-level randomized Louvain; 
     each member of the ensemble gets a "vote" to determine if the edges 
     are intra-community or not;
     the votes are aggregated into ECG edge-weights in range [0,1]; 
     a final (full depth) Louvain is run using those edge weights;
     
     Parameters
     ----------
     self: graph of type 'networkx.classes.graph.Graph'
       Graph to define the partition on.
     weight : str, optional
       the key in graph to use as weight. Default to 'weight'
-    ens_size: int 
+    ens_size: int, optional
       the size of the ensemble of single-level Louvain
-    min_weight: double in range [0,1] 
+    min_weight: float in range [0,1], optional
       the ECG edge weight for edges with zero votes from the ensemble
+    resolution: positive float, optional
+      resolution parameter; larger values favors smaller communities
 
     Returns
     -------
     an object of type 'partition_networkx.Partition' with:
     
     Partition.partition:
         The final partition as a dictionary on the vertices
@@ -159,14 +164,16 @@
         m = min(core[e[0]],core[e[1]])
         if m > 1:
             W[e] = min_weight + (1-min_weight)*W[e]/ens_size
         else:
             W[e] = min_weight
 
     networkx.set_edge_attributes(self, W, 'W')
-    part = community.best_partition(self, weight='W')
+    part = community.best_partition(self, weight='W', resolution=resolution)
     P = namedtuple('Partition', ['partition', 'W', 'CSI'])
     w = list(W.values())
     CSI = 1-2*np.sum([min(1-i,i) for i in w])/len(w)
     p = P(part,W,CSI)
     return p
 
+community.ecg = community_ecg
+
```

### Comparing `partition_networkx-0.0.1/README.md` & `partition_networkx-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `partition_networkx-0.0.1/setup.py` & `partition_networkx-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 setuptools.setup(
     author="Valérie Poulin and François Théberge",
     author_email="theberge@ieee.org",
     name='partition_networkx',
     license="MIT",
     description='Adds ensemble clustering (ecg) and graph-aware measures (gam) to networkx.',
-    version='v0.0.1',
+    version='v0.0.2',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/ftheberge/graph-partition-and-measures',
     packages=setuptools.find_packages(),
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     install_requires=['networkx','python-louvain','numpy'],
     classifiers=[
         # Trove classifiers
         # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
```

