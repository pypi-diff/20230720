# Comparing `tmp/enzope-0.0.3.tar.gz` & `tmp/enzope-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enzope-0.0.3.tar", last modified: Thu May 18 19:09:47 2023, max compression
+gzip compressed data, was "enzope-0.0.4.tar", last modified: Thu Jul 20 15:14:54 2023, max compression
```

## Comparing `enzope-0.0.3.tar` & `enzope-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1072 2023-05-18 18:19:34.000000 enzope-0.0.3/LICENSE
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      635 2023-05-18 19:09:47.688875 enzope-0.0.3/PKG-INFO
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        4 2023-05-11 13:40:28.000000 enzope-0.0.3/README.md
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      720 2023-05-18 19:09:07.000000 enzope-0.0.3/pyproject.toml
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       38 2023-05-18 19:09:47.688875 enzope-0.0.3/setup.cfg
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       38 2023-05-18 19:07:01.000000 enzope-0.0.3/setup.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/src/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:36:25.000000 enzope-0.0.3/src/__init__.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/src/enzope.egg-info/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      635 2023-05-18 19:09:47.000000 enzope-0.0.3/src/enzope.egg-info/PKG-INFO
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      436 2023-05-18 19:09:47.000000 enzope-0.0.3/src/enzope.egg-info/SOURCES.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        1 2023-05-18 19:09:47.000000 enzope-0.0.3/src/enzope.egg-info/dependency_links.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       43 2023-05-18 19:09:47.000000 enzope-0.0.3/src/enzope.egg-info/top_level.txt
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/src/graphs/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-12 15:11:48.000000 enzope-0.0.3/src/graphs/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6766 2023-05-12 15:20:06.000000 enzope-0.0.3/src/graphs/custom_gtg.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     4532 2023-05-15 13:39:45.000000 enzope-0.0.3/src/graphs/graph_class.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/src/kernels/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-11 14:05:10.000000 enzope-0.0.3/src/kernels/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1368 2023-05-15 19:19:28.000000 enzope-0.0.3/src/kernels/k_ys.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      434 2023-05-13 20:26:31.000000 enzope-0.0.3/src/kernels/locks.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/src/model/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:36:37.000000 enzope-0.0.3/src/model/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6442 2023-05-15 16:53:38.000000 enzope-0.0.3/src/model/model_gpu.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/src/trades/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:17.000000 enzope-0.0.3/src/trades/__init__.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/src/utils/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:24.000000 enzope-0.0.3/src/utils/__init__.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 19:09:47.688875 enzope-0.0.3/tests/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       37 2023-05-15 13:42:25.000000 enzope-0.0.3/tests/test.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      593 2023-07-20 15:14:54.429321 enzope-0.0.4/PKG-INFO
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        4 2023-05-11 13:40:28.000000 enzope-0.0.4/README.md
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       78 2023-07-20 15:14:54.429321 enzope-0.0.4/setup.cfg
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1528 2023-07-20 15:14:35.000000 enzope-0.0.4/setup.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.425321 enzope-0.0.4/src/
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.425321 enzope-0.0.4/src/enzope/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      244 2023-07-17 16:53:44.000000 enzope-0.0.4/src/enzope/__init__.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/graphs/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-06-21 16:54:29.000000 enzope-0.0.4/src/enzope/graphs/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6768 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/graphs/custom_gtg.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     5185 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/graphs/graph_class.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/kernels/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-11 14:05:10.000000 enzope-0.0.4/src/enzope/kernels/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     2558 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/kernels/k_ys.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      430 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/kernels/locks.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/metrics/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:05.000000 enzope-0.0.4/src/enzope/metrics/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      465 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/metrics/gpu_measures.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      795 2023-07-20 15:13:09.000000 enzope-0.0.4/src/enzope/metrics/measures.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/models/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:02.000000 enzope-0.0.4/src/enzope/models/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)    10199 2023-07-20 15:13:10.000000 enzope-0.0.4/src/enzope/models/model.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/trades/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:17.000000 enzope-0.0.4/src/enzope/trades/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       63 2023-06-01 14:02:21.000000 enzope-0.0.4/src/enzope/trades/ys.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.425321 enzope-0.0.4/src/enzope.egg-info/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      593 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/PKG-INFO
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      609 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/SOURCES.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        1 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/dependency_links.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       40 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/requires.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        7 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/top_level.txt
```

### Comparing `enzope-0.0.3/src/graphs/custom_gtg.py` & `enzope-0.0.4/src/enzope/graphs/custom_gtg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import math
 from itertools import combinations
+
 import networkx as nx
-import math
 from networkx.utils import py_random_state
 
+
 # Generating function for additive and multiplicative threshold graphs, 
 # slightly modified version from the function provided in the networkx package.
 @py_random_state(7)
 def geographical_threshold_graph_custom(
     n,
     theta,
     dim=2,
```

### Comparing `enzope-0.0.3/src/graphs/graph_class.py` & `enzope-0.0.4/src/enzope/graphs/graph_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Any
-from custom_gtg import geographical_threshold_graph_custom
+import os
+
+import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
-import matplotlib.pyplot as plt
 from IPython.display import display
-import os
 
+from .custom_gtg import geographical_threshold_graph_custom
 
 # ---------------------- #
 #        Classes         #
 # ---------------------- #
 
 
 class BaseGraph:
@@ -22,14 +22,15 @@
         figpath=None,
         plotable=False,
     ):
         self.n_nodes = n_nodes
         self.upd_w = upd_w
         self.upd_graph = upd_graph
         self.upd_plot = upd_plot
+        self.G = None
 
         if plotable:
             self.fig, self.ax = plt.subplots(dpi=150)
             self.ax.set_xlim([-0.03, 1.03])
             self.ax.set_ylim([-0.03, 1.03])
             plt.close(self.fig)
 
@@ -44,15 +45,20 @@
         pass
 
     def update_graph(self, *args, **kwargs):
         pass
 
     def get_opponents_cpu(self, *args, **kwargs):
         pass
-
+    
+    def get_mean_connectivity(self):
+        pass
+    
+    def get_average_distance(self):
+        pass
 
 class GTG(BaseGraph):
     def __init__(
         self, n_nodes, theta, join="add", w0=None, posi=None, seed=None, **kwargs
     ):
         super().__init__(n_nodes, **kwargs)
         self.theta = theta
@@ -77,21 +83,24 @@
 
         self.w = dict(enumerate(self.G.nodes[i]["weight"] for i in range(self.n_nodes)))
 
     def __call__(self, *args, **kwds):
         return self.G
 
     # Modificar la funcion para que o bien guarde en temp o bien muestre en pantalla
-    def plot_snapshot(self, w_min, mcs=None, mode="save", *args, **kwargs):
+    def plot_snapshot(self, w_min=1e-17, new_w=None, mcs=None, mode="show", *args, **kwargs):
         # Esto se tiene que escribir mejor
+        if new_w is not None:
+            self.update_weights(new_w)
+
         a = np.array(list(self.w.values()))
 
         dead_nodes = [node for node, weight in self.w.items() if weight < w_min]
 
-        node_size = 25 * 200 * (a)
+        node_size = 25 * (a)
         node_colors = ["r" if n in dead_nodes else "royalblue" for n in self.G.nodes]
         edge_colors = [
             "r" if (e[0] in dead_nodes or e[1] in dead_nodes) else "black"
             for e in self.G.edges
         ]
 
         self.ax.clear()
@@ -137,20 +146,32 @@
             if neighbors := list(nx.all_neighbors(self.G, i)):
                 opponents[i] = np.random.choice(neighbors)
 
         return opponents
 
     # Function inspired by cuTradeNet's toLL() function in:
     # https://github.com/Qsanti/cuTradeNet/blob/e20f29e65bcac448d7fcd17fac45746f90e8538e/cuTradeNet/Models/Utils/GraphManager.py
-    def get_neigbhors_array_gpu(self, *args, **kwargs):
+    def get_neighbors_array_gpu(self, *args, **kwargs):
         """ """
         neighs = [(list(self.G.neighbors(i))) for i in range(self.n_nodes)]
-        cum_neighs = np.cumsum(np.array([len(x) for x in neighs], dtype=np.int32))
+        n_neighs = [0] + [len(x) for x in neighs]
+        n_neighs = np.array(n_neighs, dtype=np.int32)
+        # c_neighs has N+1 components, first is 0.
+        c_neighs = np.cumsum(n_neighs)
         neighs = np.hstack(neighs).astype(np.int32)
-        return cum_neighs, neighs
+        return c_neighs, neighs
+    
+    # Some networkx functions for comfort
+    def get_mean_connectivity(self):
+        return np.mean(list(dict(nx.degree(self.G)).values()))
+    
+    def get_average_distance(self):
+        Gcc = sorted(nx.connected_components(self.G), key=len, reverse=True)
+        G0 = self.G.subgraph(Gcc[0])
+        return nx.average_shortest_path_length(G0)
 
 
 # Acá iría la clase del multigraph
 
 
 # ---------------------- #
 #       Funciones        #
```

