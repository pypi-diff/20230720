# Comparing `tmp/partition_igraph-0.0.6.tar.gz` & `tmp/partition_igraph-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/partition_igraph-0.0.6.tar", last modified: Thu Jan 19 17:33:19 2023, max compression
+gzip compressed data, was "partition_igraph-0.0.7.tar", last modified: Thu Jul 20 12:39:32 2023, max compression
```

## Comparing `partition_igraph-0.0.6.tar` & `partition_igraph-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/
--rwxrwxrwx   0 francois   (501) staff       (20)     1076 2020-05-19 14:45:42.000000 partition_igraph-0.0.6/LICENSE
--rw-r--r--   0 francois   (501) staff       (20)     3057 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/PKG-INFO
--rwxrwxrwx   0 francois   (501) staff       (20)     2315 2020-05-19 14:46:01.000000 partition_igraph-0.0.6/README.md
-drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/partition_igraph/
--rwxrwxrwx   0 francois   (501) staff       (20)      163 2023-01-19 17:33:00.000000 partition_igraph-0.0.6/partition_igraph/__init__.py
--rwxrwxrwx   0 francois   (501) staff       (20)     5789 2022-05-13 16:57:29.000000 partition_igraph-0.0.6/partition_igraph/partition_igraph.py
-drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/partition_igraph.egg-info/
--rwxrwxrwx   0 francois   (501) staff       (20)     3057 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/partition_igraph.egg-info/PKG-INFO
--rwxrwxrwx   0 francois   (501) staff       (20)      291 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/partition_igraph.egg-info/SOURCES.txt
--rwxrwxrwx   0 francois   (501) staff       (20)        1 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/partition_igraph.egg-info/dependency_links.txt
--rwxrwxrwx   0 francois   (501) staff       (20)       21 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/partition_igraph.egg-info/requires.txt
--rwxrwxrwx   0 francois   (501) staff       (20)       17 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/partition_igraph.egg-info/top_level.txt
--rw-r--r--   0 francois   (501) staff       (20)       38 2023-01-19 17:33:19.000000 partition_igraph-0.0.6/setup.cfg
--rwxrwxrwx   0 francois   (501) staff       (20)     1144 2023-01-19 17:32:46.000000 partition_igraph-0.0.6/setup.py
+drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-07-20 12:39:32.650959 partition_igraph-0.0.7/
+-rwxrwxrwx   0 francois   (501) staff       (20)     1076 2020-05-19 14:45:42.000000 partition_igraph-0.0.7/LICENSE
+-rw-r--r--   0 francois   (501) staff       (20)     3057 2023-07-20 12:39:32.650782 partition_igraph-0.0.7/PKG-INFO
+-rwxrwxrwx   0 francois   (501) staff       (20)     2315 2020-05-19 14:46:01.000000 partition_igraph-0.0.7/README.md
+drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-07-20 12:39:32.649908 partition_igraph-0.0.7/partition_igraph/
+-rwxrwxrwx   0 francois   (501) staff       (20)      163 2023-07-20 12:33:35.000000 partition_igraph-0.0.7/partition_igraph/__init__.py
+-rw-r--r--   0 francois   (501) staff       (20)     6985 2023-07-20 12:31:38.000000 partition_igraph-0.0.7/partition_igraph/partition_igraph.py
+drwxr-xr-x   0 francois   (501) staff       (20)        0 2023-07-20 12:39:32.650596 partition_igraph-0.0.7/partition_igraph.egg-info/
+-rwxrwxrwx   0 francois   (501) staff       (20)     3057 2023-07-20 12:39:32.000000 partition_igraph-0.0.7/partition_igraph.egg-info/PKG-INFO
+-rwxrwxrwx   0 francois   (501) staff       (20)      291 2023-07-20 12:39:32.000000 partition_igraph-0.0.7/partition_igraph.egg-info/SOURCES.txt
+-rwxrwxrwx   0 francois   (501) staff       (20)        1 2023-07-20 12:39:32.000000 partition_igraph-0.0.7/partition_igraph.egg-info/dependency_links.txt
+-rwxrwxrwx   0 francois   (501) staff       (20)       21 2023-07-20 12:39:32.000000 partition_igraph-0.0.7/partition_igraph.egg-info/requires.txt
+-rwxrwxrwx   0 francois   (501) staff       (20)       17 2023-07-20 12:39:32.000000 partition_igraph-0.0.7/partition_igraph.egg-info/top_level.txt
+-rw-r--r--   0 francois   (501) staff       (20)       38 2023-07-20 12:39:32.651005 partition_igraph-0.0.7/setup.cfg
+-rwxrwxrwx   0 francois   (501) staff       (20)     1144 2023-07-20 12:32:52.000000 partition_igraph-0.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `partition_igraph-0.0.6/LICENSE` & `partition_igraph-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `partition_igraph-0.0.6/PKG-INFO` & `partition_igraph-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: partition_igraph
-Version: 0.0.6
+Version: 0.0.7
 Summary: Adds ensemble clustering (ecg) and graph-aware measures (gam) to igraph.
 Home-page: https://github.com/ftheberge/graph-partition-and-measures
 Author: Valérie Poulin and François Théberge
 Author-email: theberge@ieee.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Graph Partition and Measures
 
 Python3 code implementing 11 graph-aware measures (gam) for comparing graph partitions as well as a stable ensemble-based graph partition algorithm (ecg). This verion works with the igraph package. A version for networkx is also available: partition-networkx.
```

### Comparing `partition_igraph-0.0.6/README.md` & `partition_igraph-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `partition_igraph-0.0.6/partition_igraph/partition_igraph.py` & `partition_igraph-0.0.7/partition_igraph/partition_igraph.py`

 * *Files 21% similar despite different names*

```diff
@@ -87,35 +87,38 @@
     return None
 
 igraph.Graph.gam = gam
 
 import igraph
 import numpy as np
 
-def community_ecg(self, weights=None, ens_size = 16, min_weight = 0.05, final='louvain'):
+def community_ecg(self, weights=None, ens_size = 16, min_weight = 0.05, 
+                  final='louvain', resolution=1.0, refuse_score=False):
     """
     Stable ensemble-based graph clustering;
     the ensemble consists of single-level randomized Louvain; 
     each member of the ensemble gets a "vote" to determine if the edges 
     are intra-community or not;
     the votes are aggregated into ECG edge-weights in range [0,1]; 
     a final (full depth) Louvain is run using those edge weights;
     
     Parameters
     ----------
     self: graph of type 'igraph.Graph'
       Graph to define the partition on.
     weights: list of double, optional 
       the edge weights
-    ens_size: int 
+    ens_size: int, optional
       the size of the ensemble of single-level Louvain
-    min_weight: double in range [0,1] 
+    min_weight: double in range [0,1], optional
       the ECG edge weight for edges with zero votes from the ensemble
-    final: 'louvain' or 'leiden'
+    final: 'louvain' (default) or 'leiden'
       the algorithm to run on the final re-weighted graph
+    resolution: positive float, optional
+      resolution parameter; larger values favors smaller communities
       
     Returns
     -------
     partition
       The final partition, of type 'igraph.clustering.VertexClustering'
     partition.W
       The ECG edge weights
@@ -153,17 +156,45 @@
         W = [W[i]+b[i] for i in range(len(W))]
     W = [min_weight + (1-min_weight)*W[i]/ens_size for i in range(len(W))]
     ## Force min_weight outside 2-core
     core = self.shell_index()
     ecore = [min(core[x.tuple[0]],core[x.tuple[1]]) for x in self.es]
     w = [W[i] if ecore[i]>1 else min_weight for i in range(len(ecore))]
     if final=='leiden':
-        part = self.community_leiden(weights=w, objective_function='modularity')
+        part = self.community_leiden(weights=w, objective_function='modularity', resolution=resolution)
     else:
-        part = self.community_multilevel(weights=w)
+        part = self.community_multilevel(weights=w, resolution=resolution)
     part.W = w
     part.CSI = 1-2*np.sum([min(1-i,i) for i in w])/len(w)
     part._modularity_params['weights'] = weights
     part.recalculate_modularity()
+    
+    ## experimental - "refuse to cluster" scores
+    if refuse_score:
+        self.vs['_deg'] = self.degree()
+        self.es['_W'] = part.W
+        self.vs['_ecg'] = part.membership
+        for v in self.vs:
+            scr = 0
+            my_comm = v['_ecg']
+            good = 0
+            bad = 0
+            for e in v.incident():
+                scr += e['_W']
+                if self.vs[e.source]['_ecg'] == self.vs[e.target]['_ecg']:
+                    good += e['_W']
+                else:
+                    bad += e['_W']
+            v['_overall'] = ((v['_deg']-scr)/v['_deg'])
+            v['_community'] = (bad/(bad+good))        
+        part.refuse_overall = self.vs['_overall']
+        part.refuse_community = self.vs['_community']
+        del(self.vs['_deg'])
+        del(self.es['_W'])
+        del(self.vs['_ecg'])
+        del(self.vs['_overall'])
+        del(self.vs['_community'])            
+    ## end experimental scores
+    
     return part
 
 igraph.Graph.community_ecg = community_ecg
```

### Comparing `partition_igraph-0.0.6/partition_igraph.egg-info/PKG-INFO` & `partition_igraph-0.0.7/partition_igraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: partition-igraph
-Version: 0.0.6
+Version: 0.0.7
 Summary: Adds ensemble clustering (ecg) and graph-aware measures (gam) to igraph.
 Home-page: https://github.com/ftheberge/graph-partition-and-measures
 Author: Valérie Poulin and François Théberge
 Author-email: theberge@ieee.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Graph Partition and Measures
 
 Python3 code implementing 11 graph-aware measures (gam) for comparing graph partitions as well as a stable ensemble-based graph partition algorithm (ecg). This verion works with the igraph package. A version for networkx is also available: partition-networkx.
```

### Comparing `partition_igraph-0.0.6/setup.py` & `partition_igraph-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 setuptools.setup(
     author="Valérie Poulin and François Théberge",
     author_email="theberge@ieee.org",
     name='partition_igraph',
     license="MIT",
     description='Adds ensemble clustering (ecg) and graph-aware measures (gam) to igraph.',
-    version='v0.0.6',
+    version='v0.0.7',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/ftheberge/graph-partition-and-measures',
     packages=setuptools.find_packages(),
-    python_requires=">=3.6",
-    install_requires=['igraph>=0.9.11','numpy'],
+    python_requires=">=3.9",
+    install_requires=['igraph>=0.10.1','numpy'],
     classifiers=[
         # Trove classifiers
         # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

