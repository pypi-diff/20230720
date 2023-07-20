# Comparing `tmp/cellmap-1.0.1.dev202307201017-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202307201018-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 21518 bytes, number of entries: 5
+Zip file size: 21526 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   130559 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1948 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307201017.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307201017.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202307201017.dist-info/RECORD
-5 files, 133052 bytes uncompressed, 20764 bytes compressed:  84.4%
+-rw-r--r--  2.0 unx   130423 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1948 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307201018.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307201018.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202307201018.dist-info/RECORD
+5 files, 132916 bytes uncompressed, 20772 bytes compressed:  84.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307201017.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202307201018.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307201017.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202307201018.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307201017.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202307201018.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -673,16 +673,16 @@
         kwargs_arg["exp_key"],
         kwargs_arg["vkey"],
         kwargs_arg["basis"],
     )
 
     exp_2d_key_ = "X_%s" % basis
     vel_2d_key_ = "%s_%s" % (vkey, basis)
-    pot_vkey_ = "%s_%s" % (potential_vkey, basis)
-    rot_vkey_ = "%s_%s" % (rotation_vkey, basis)
+    pot_vkey_ = "%s_%s_%s" % (potential_key, vkey, basis)
+    rot_vkey_ = "%s_%s_%s" % (rotation_key, vkey, basis)
 
     if exp_key == None:
         if scipy.sparse.issparse(adata.X):
             exp_HD = adata.X.toarray()
         else:
             exp_HD = adata.X
     elif exp_key in adata.obsm.keys():
@@ -993,28 +993,30 @@
                 texts.append(txt)
 
 
 def view_stream(
     adata,
     basis="umap",
     vkey="velocity",
-    potential_vkey="potential_velocity",
-    rotation_vkey="rotation_velocity",
+    potential_key="potential",
+    rotation_key="rotation",
     cluster_key="clusters",
     figsize=(24, 6),
     density=2,
     alpha=0.3,
     fontsize=18,
     legend_fontsize=18,
     **kwargs,
 ):
     kwargs_arg = _check_arguments(adata, basis=basis)
     basis = kwargs_arg["basis"]
     basis_key = "X_%s" % basis
     data_pos = adata.obsm[basis_key]
+    pot_vkey_ = "%s_%s" % (potential_key, vkey)
+    rot_vkey_ = "%s_%s" % (rotation_key, vkey)
 
     fig, ax = plt.subplots(1, 3, figsize=figsize, tight_layout=True,facecolor="w")
     scv.pl.velocity_embedding_stream(
         adata,
         basis=basis,
         vkey=vkey,
         title="RNA velocity",
@@ -1029,15 +1031,15 @@
         arrow_size=2,
         linewidth=2,
         **kwargs,
     )
     scv.pl.velocity_embedding_stream(
         adata,
         basis=basis,
-        vkey=potential_vkey,
+        vkey=pot_vkey_,
         title="Potential flow",
         ax=ax[1],
         color=cluster_key,
         show=False,
         density=density,
         alpha=alpha,
         fontsize=fontsize,
@@ -1046,15 +1048,15 @@
         arrow_size=2,
         linewidth=2,
         **kwargs,
     )
     scv.pl.velocity_embedding_stream(
         adata,
         basis=basis,
-        vkey=rotation_vkey,
+        vkey=rot_vkey_,
         title="Rotational flow",
         ax=ax[2],
         color=cluster_key,
         show=False,
         density=density,
         alpha=alpha,
         fontsize=fontsize,
@@ -2217,21 +2219,14 @@
     target_clusters,
     path_key="path",
     exp_key=None,
     gene_dynamics_key="gene_dynamics",
     n_div=100,
     degree=10,
 ):
-    # if exp_key == None:
-    #     if scipy.sparse.issparse(adata.X):
-    #         data_exp = adata.X.toarray()
-    #     else:
-    #         data_exp = adata.X
-    # else:
-    #     data_exp = adata.layers[exp_key]
     data_exp = _set_expression_data(adata, exp_key)
     
     path = adata.uns[path_key]
 
     gene_dynamics_ = {}
     for i in range(len(path)):
         name_ = source_cluster + "_" + target_clusters[i]
```

## Comparing `cellmap-1.0.1.dev202307201017.dist-info/METADATA` & `cellmap-1.0.1.dev202307201018.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202307201017
+Version: 1.0.1.dev202307201018
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

