# Comparing `tmp/descarteslabs_dynamic_compute-0.6.1.tar.gz` & `tmp/descarteslabs_dynamic_compute-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descarteslabs_dynamic_compute-0.6.1.tar", max compression
+gzip compressed data, was "descarteslabs_dynamic_compute-0.6.2.tar", max compression
```

## Comparing `descarteslabs_dynamic_compute-0.6.1.tar` & `descarteslabs_dynamic_compute-0.6.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      561 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/LICENSE
--rw-r--r--   0        0        0     1786 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/README.md
--rw-r--r--   0        0        0      786 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/__init__.py
--rw-r--r--   0        0        0      308 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/catalog/__init__.py
--rw-r--r--   0        0        0     9728 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/catalog/blob.py
--rw-r--r--   0        0        0    22390 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/compute_map.py
--rw-r--r--   0        0        0     1467 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/datetime_utils.py
--rw-r--r--   0        0        0      648 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/dl_utils.py
--rw-r--r--   0        0        0     2394 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/dot.py
--rw-r--r--   0        0        0     1007 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/dynamic_compute.py
--rw-r--r--   0        0        0        0 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/__init__.py
--rw-r--r--   0        0        0      463 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/client/__init__.py
--rw-r--r--   0        0        0    22792 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/client/client.py
--rw-r--r--   0        0        0      160 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/interpreter/__init__.py
--rw-r--r--   0        0        0      223 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/interpreter/exceptions.py
--rw-r--r--   0        0        0     5705 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py
--rw-r--r--   0        0        0      848 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py
--rw-r--r--   0        0        0     5217 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/spec.md
--rw-r--r--   0        0        0      465 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/syntax/__init__.py
--rw-r--r--   0        0        0     3620 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/syntax/syntax.py
--rw-r--r--   0        0        0     9025 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/groupby.py
--rw-r--r--   0        0        0    18751 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/image_stack.py
--rw-r--r--   0        0        0       41 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/__init__.py
--rw-r--r--   0        0        0     1573 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/clearable.py
--rw-r--r--   0        0        0     1179 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/colormaps.py
--rw-r--r--   0        0        0    12531 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/inspector.py
--rw-r--r--   0        0        0    22374 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/layer.py
--rw-r--r--   0        0        0     3752 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/layer_controller.py
--rw-r--r--   0        0        0    17054 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/layer_controller_row.py
--rw-r--r--   0        0        0     1333 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/lonlat.py
--rw-r--r--   0        0        0    18499 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/map_.py
--rw-r--r--   0        0        0    23843 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/parameters.py
--rw-r--r--   0        0        0     3572 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/tile_url.py
--rw-r--r--   0        0        0     1543 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/utils.py
--rw-r--r--   0        0        0    18023 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/mosaic.py
--rw-r--r--   0        0        0    28360 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/operations.py
--rw-r--r--   0        0        0     3133 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/pyversions.py
--rw-r--r--   0        0        0     3148 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/reductions.py
--rw-r--r--   0        0        0      801 2023-07-19 22:37:39.446406 descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/serialization.py
--rw-r--r--   0        0        0      531 2023-07-19 22:37:39.450406 descarteslabs_dynamic_compute-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 descarteslabs_dynamic_compute-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      561 2023-07-20 21:48:32.355856 descarteslabs_dynamic_compute-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1786 2023-07-20 21:48:32.355856 descarteslabs_dynamic_compute-0.6.2/README.md
+-rw-r--r--   0        0        0      786 2023-07-20 21:48:32.355856 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/__init__.py
+-rw-r--r--   0        0        0      308 2023-07-20 21:48:32.355856 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/catalog/__init__.py
+-rw-r--r--   0        0        0     9728 2023-07-20 21:48:32.355856 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/catalog/blob.py
+-rw-r--r--   0        0        0    22390 2023-07-20 21:48:32.355856 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/compute_map.py
+-rw-r--r--   0        0        0     1467 2023-07-20 21:48:32.355856 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/datetime_utils.py
+-rw-r--r--   0        0        0      648 2023-07-20 21:48:32.355856 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/dl_utils.py
+-rw-r--r--   0        0        0     2394 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/dot.py
+-rw-r--r--   0        0        0     1007 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/dynamic_compute.py
+-rw-r--r--   0        0        0        0 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/__init__.py
+-rw-r--r--   0        0        0      463 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/client/__init__.py
+-rw-r--r--   0        0        0    22792 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/client/client.py
+-rw-r--r--   0        0        0      160 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/interpreter/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/interpreter/exceptions.py
+-rw-r--r--   0        0        0     5705 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py
+-rw-r--r--   0        0        0      848 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py
+-rw-r--r--   0        0        0     5217 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/spec.md
+-rw-r--r--   0        0        0      465 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/syntax/__init__.py
+-rw-r--r--   0        0        0     3620 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/syntax/syntax.py
+-rw-r--r--   0        0        0     9025 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/groupby.py
+-rw-r--r--   0        0        0    18751 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/image_stack.py
+-rw-r--r--   0        0        0       41 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/__init__.py
+-rw-r--r--   0        0        0     1573 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/clearable.py
+-rw-r--r--   0        0        0     1179 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/colormaps.py
+-rw-r--r--   0        0        0    12531 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/inspector.py
+-rw-r--r--   0        0        0    22374 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/layer.py
+-rw-r--r--   0        0        0     3752 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/layer_controller.py
+-rw-r--r--   0        0        0    17054 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/layer_controller_row.py
+-rw-r--r--   0        0        0     1333 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/lonlat.py
+-rw-r--r--   0        0        0    18499 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/map_.py
+-rw-r--r--   0        0        0    23843 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/parameters.py
+-rw-r--r--   0        0        0     3572 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/tile_url.py
+-rw-r--r--   0        0        0     1543 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/utils.py
+-rw-r--r--   0        0        0    18023 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/mosaic.py
+-rw-r--r--   0        0        0    28478 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/operations.py
+-rw-r--r--   0        0        0     3133 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/pyversions.py
+-rw-r--r--   0        0        0     3148 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/reductions.py
+-rw-r--r--   0        0        0      801 2023-07-20 21:48:32.359857 descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/serialization.py
+-rw-r--r--   0        0        0      531 2023-07-20 21:48:32.363857 descarteslabs_dynamic_compute-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 descarteslabs_dynamic_compute-0.6.2/PKG-INFO
```

### Comparing `descarteslabs_dynamic_compute-0.6.1/LICENSE` & `descarteslabs_dynamic_compute-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/README.md` & `descarteslabs_dynamic_compute-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/__init__.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/catalog/blob.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/catalog/blob.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/compute_map.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/compute_map.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/datetime_utils.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/dl_utils.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/dl_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/dot.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/dot.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/dynamic_compute.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/dynamic_compute.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/client/client.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/client/client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/spec.md` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/spec.md`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/graft/syntax/syntax.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/graft/syntax/syntax.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/groupby.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/groupby.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/image_stack.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/image_stack.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/clearable.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/clearable.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/colormaps.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/colormaps.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/inspector.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/inspector.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/layer.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/layer.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/layer_controller.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/layer_controller.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/layer_controller_row.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/layer_controller_row.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/lonlat.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/lonlat.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/map_.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/map_.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/parameters.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/parameters.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/tile_url.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/tile_url.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/interactive/utils.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/mosaic.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/mosaic.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/operations.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -810,23 +810,26 @@
         layer id to reuse if supplied
 
     Returns
     -------
         list of numbers
     """
 
+    def _get_most_common_value(array) -> int:
+        arr, counts = np.unique(array, return_counts=True)
+        return int(arr[counts == counts.max()][0])
+
     aoi = _geocontext_from_latlon(lat, lon)
     value_array, _ = compute_aoi(graft, aoi, layer_id)
     if len(value_array.shape) > 1:
         if np.issubdtype(value_array.dtype.type, np.bool_):
             # if we're dealing with booleans, return the most common value
-            arr, counts = np.unique(value_array, return_counts=True)
-            return [int(arr[counts == counts.max()][0])]
-        # otherwise, return the mean value
-        return [value_array.mean()]
+            return list(map(_get_most_common_value, value_array))
+        # otherwise, return each mean value per band
+        return list(map(np.mean, value_array))
     return list(value_array)
 
 
 def _geocontext_from_latlon(lat: float, lon: float) -> dl.geo.AOI:
     """
     Creates a tiny AOI from a lat/lon location. Private helper method for value_at, should only be called internally.
```

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/pyversions.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/pyversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/reductions.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/reductions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/descarteslabs/dynamic_compute/serialization.py` & `descarteslabs_dynamic_compute-0.6.2/descarteslabs/dynamic_compute/serialization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-0.6.1/pyproject.toml` & `descarteslabs_dynamic_compute-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descarteslabs-dynamic-compute"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 license = "Apache-2.0"
 authors = ["Descartes Labs"]
 readme = "README.md"
 packages = [
     { include = "descarteslabs" },
 ]
```

### Comparing `descarteslabs_dynamic_compute-0.6.1/PKG-INFO` & `descarteslabs_dynamic_compute-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descarteslabs-dynamic-compute
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 License: Apache-2.0
 Author: Descartes Labs
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

