# Comparing `tmp/repleno-0.0.13.tar.gz` & `tmp/repleno-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repleno-0.0.13.tar", last modified: Thu Jul  6 16:22:58 2023, max compression
+gzip compressed data, was "repleno-0.0.14.tar", last modified: Thu Jul 20 16:46:48 2023, max compression
```

## Comparing `repleno-0.0.13.tar` & `repleno-0.0.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 16:22:58.465005 repleno-0.0.13/
--rw-rw-rw-   0        0        0     2608 2023-07-06 16:22:58.462998 repleno-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0     2017 2023-06-26 17:07:24.000000 repleno-0.0.13/README.md
--rw-rw-rw-   0        0        0     1009 2023-07-06 16:22:17.000000 repleno-0.0.13/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 16:22:58.465005 repleno-0.0.13/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 16:22:58.404663 repleno-0.0.13/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 16:22:58.440666 repleno-0.0.13/src/repleno/
--rw-rw-rw-   0        0        0    33949 2023-07-06 12:59:02.000000 repleno-0.0.13/src/repleno/SKU.py
--rw-rw-rw-   0        0        0      519 2023-06-25 14:02:32.000000 repleno-0.0.13/src/repleno/__init__.py
--rw-rw-rw-   0        0        0       96 2023-06-25 14:02:32.000000 repleno-0.0.13/src/repleno/__main__.py
--rw-rw-rw-   0        0        0    27226 2023-07-04 11:42:19.000000 repleno-0.0.13/src/repleno/factory.py
--rw-rw-rw-   0        0        0     2310 2023-06-26 18:04:48.000000 repleno-0.0.13/src/repleno/order.py
--rw-rw-rw-   0        0        0     9575 2023-07-06 16:17:59.000000 repleno-0.0.13/src/repleno/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:22:58.458989 repleno-0.0.13/src/repleno.egg-info/
--rw-rw-rw-   0        0        0     2608 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/top_level.txt
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-20 16:46:48.092092 repleno-0.0.14/
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-20 16:46:48.092092 repleno-0.0.14/PKG-INFO
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2017 2023-06-26 17:07:24.000000 repleno-0.0.14/README.md
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     1009 2023-07-20 16:44:34.000000 repleno-0.0.14/pyproject.toml
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       38 2023-07-20 16:46:48.092092 repleno-0.0.14/setup.cfg
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-20 16:46:48.092092 repleno-0.0.14/src/
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-20 16:46:48.092092 repleno-0.0.14/src/repleno/
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)    34310 2023-07-20 15:36:30.000000 repleno-0.0.14/src/repleno/SKU.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)      519 2023-06-25 14:02:32.000000 repleno-0.0.14/src/repleno/__init__.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)       96 2023-06-25 14:02:32.000000 repleno-0.0.14/src/repleno/__main__.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)    27547 2023-07-20 16:43:32.000000 repleno-0.0.14/src/repleno/factory.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2310 2023-06-26 18:04:48.000000 repleno-0.0.14/src/repleno/order.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     9575 2023-07-06 16:17:59.000000 repleno-0.0.14/src/repleno/utils.py
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-20 16:46:48.092092 repleno-0.0.14/src/repleno.egg-info/
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/PKG-INFO
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)      330 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/SOURCES.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        1 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/dependency_links.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       28 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/requires.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        8 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/top_level.txt
```

### Comparing `repleno-0.0.13/PKG-INFO` & `repleno-0.0.14/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-Metadata-Version: 2.1
-Name: repleno
-Version: 0.0.13
-Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
-Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
-Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Manufacturing
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-
-
-# repleno
-
-Repleno allows you to easily answer supply chain questions considering bill of
-materials (BOM) structure.
-
-- **PyPI**: https://pypi.org/project/repleno/ 
-- **Source code**: 
-- **Documentation**: 
-- **Bug reports**: 
-
-
-It answers the following questions:
-
-1. "Which finished/purchased goods are associated with this stock keeping unit (SKU)?"
-2. "Based on this master production schedule (MPS), which specific SKU quantities should be ordered from suppliers?"
-3. "Using the master requirements planning (MRP) results and current supplier orders, when will there be stock-out periods?"
-4. "If I discontinue SKU X, which other SKU's will also need to be discontinued?"
-
-By providing:
-
-- efficient queries about parent-child relationships for SKUs in the BOM
-- MRP simulations to analyze the impact of MPS changes on purchase orders to suppliers
-- inventory levels over a specific time periods
-- identification of collateral SKU's that need to be phased-out along with a specific SKU
-
-
-Installing:
-
-```bash
-python -m pip install requests
-```
-
-## Roadmap:
-
-1. Integrate phantom scenarios to `run_mrp` and `get_lineage` and `get_collaterals` methods;
-2. issue a warning when a parameter is not being loaded or a column has not been found;
-3. get_collaterals function should return a tree, so it can be used to fully deplete the inventory inside it;
-4. run special mrp for scenarios: produce all inventory left in the BOM (placing more order to deplete everything or with scrapage);
-5. method for propagating any general label from roots to child nodes (from fininshed goods to purchased goods, in supply chain terms);
-6. Method for quickly answering the question: if one component goes out of stock, what's the impact on the finished goods?
-7. per component, shows how much of its demand impact finished goods. If 1 component goes into only 1 FG, then 100%
-8. Add support to add lead times in different units (currently only support calendar days), like weeks or months
+Metadata-Version: 2.1
+Name: repleno
+Version: 0.0.14
+Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
+Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
+Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Manufacturing
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+
+
+# repleno
+
+Repleno allows you to easily answer supply chain questions considering bill of
+materials (BOM) structure.
+
+- **PyPI**: https://pypi.org/project/repleno/ 
+- **Source code**: 
+- **Documentation**: 
+- **Bug reports**: 
+
+
+It answers the following questions:
+
+1. "Which finished/purchased goods are associated with this stock keeping unit (SKU)?"
+2. "Based on this master production schedule (MPS), which specific SKU quantities should be ordered from suppliers?"
+3. "Using the master requirements planning (MRP) results and current supplier orders, when will there be stock-out periods?"
+4. "If I discontinue SKU X, which other SKU's will also need to be discontinued?"
+
+By providing:
+
+- efficient queries about parent-child relationships for SKUs in the BOM
+- MRP simulations to analyze the impact of MPS changes on purchase orders to suppliers
+- inventory levels over a specific time periods
+- identification of collateral SKU's that need to be phased-out along with a specific SKU
+
+
+Installing:
+
+```bash
+python -m pip install requests
+```
+
+## Roadmap:
+
+1. Integrate phantom scenarios to `run_mrp` and `get_lineage` and `get_collaterals` methods;
+2. issue a warning when a parameter is not being loaded or a column has not been found;
+3. get_collaterals function should return a tree, so it can be used to fully deplete the inventory inside it;
+4. run special mrp for scenarios: produce all inventory left in the BOM (placing more order to deplete everything or with scrapage);
+5. method for propagating any general label from roots to child nodes (from fininshed goods to purchased goods, in supply chain terms);
+6. Method for quickly answering the question: if one component goes out of stock, what's the impact on the finished goods?
+7. per component, shows how much of its demand impact finished goods. If 1 component goes into only 1 FG, then 100%
+8. Add support to add lead times in different units (currently only support calendar days), like weeks or months
```

### Comparing `repleno-0.0.13/README.md` & `repleno-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `repleno-0.0.13/pyproject.toml` & `repleno-0.0.14/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = 'repleno'
-version = '0.0.13'
+version = '0.0.14'
 authors = [
     {'name' = 'Afonso Schulz Albrecht', email = 'a.schulzalbrecht@gmail.com'},
 ]
 description = 'Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)'
 keywords = ['supply chain', 'bill of materials', 'material requirements planning', 'BOM', 'MRP']
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `repleno-0.0.13/src/repleno/SKU.py` & `repleno-0.0.14/src/repleno/SKU.py`

 * *Files 2% similar despite different names*

```diff
@@ -881,14 +881,15 @@
 
     def get_collaterals(
         self,
         include_obsoletes=False,
         skus_only=False,
         attributes=None,
         max_stack_size=None,
+        phaseout_skus=None,
     ):
         """
         # TODO: complete docstring
 
         It returns a list of dictionaries with the following keys:
 
         It generates a list of all items that meet the following criteria:
@@ -927,59 +928,67 @@
 
         # Breadth-first traversal (BFS) is used because it's easier to think
         # about the logic by levels
 
         if not include_obsoletes and self.obsolete:
             return []
 
-        output = _OutputFormatter(max_stack_size=max_stack_size)
+        output = _OutputFormatter(max_stack_size=max_stack_size) 
 
         output = self._scan_this_and_parents(
             collaterals=output,
             include_obsoletes=include_obsoletes,
+            phaseout_set=phaseout_skus
         )
         output = self._scan_children(
             collaterals=output,
             level=0,
             include_obsoletes=include_obsoletes,
+            phaseout_set=phaseout_skus
         )
 
         return output.get_output(skus_only, attributes, skus_only)
 
-    def _scan_this_and_parents(self, collaterals, include_obsoletes):
+    def _scan_this_and_parents(self, collaterals, include_obsoletes, phaseout_set):
         p_collaterals = collaterals
 
         child_skus = self.children if include_obsoletes else self.active_children  # just to record previous skus
         queue = [(child_skus, self, 0)]  # (previous_sku, current_sku, level)
         while queue:
             for _ in range(len(queue)):
                 sku_ancestor, sku, level = queue.pop(0)
 
-                # Scan the children and add the result to p_collaterals
-                if self != sku:
-                    p_collaterals = sku._scan_children(collaterals=p_collaterals, level=level, include_obsoletes=include_obsoletes)
-
                 # Filter out obsoletes if needed
                 selected_parents = sku.parents if include_obsoletes else sku.active_parents
 
-                # Add parent to collaterals
+                # Add sku to collaterals
                 p_collaterals.store(
                     sku=sku,
                     parent_skus=selected_parents,
                     child_skus=sku_ancestor,
                     level=level,
                     direction="parents",
                 )
 
+
+                # Scan the children and add the result to p_collaterals
+                if self != sku:
+                    p_collaterals = sku._scan_children(
+                        collaterals=p_collaterals, 
+                        level=level, 
+                        include_obsoletes=include_obsoletes,
+                        phaseout_set=phaseout_set
+                    )
+
                 for parent_node in selected_parents:
                     queue.append((sku, parent_node, level + 1))
 
         return p_collaterals
 
-    def _scan_children(self, collaterals, level, include_obsoletes):
+    def _scan_children(self, collaterals, level, include_obsoletes, phaseout_set):
         """
         Check if child items should be part of collaterals when self is being
         obsoleted
         """
 
         # Start from the children
         selected_children = self.children if include_obsoletes else self.active_children
@@ -989,17 +998,18 @@
         queue = [(self, sku, level - 1) for sku in selected_children]
         while queue:
             for _ in range(len(queue)):
                 sku_ancestor, sku, level = queue.pop(0)
 
                 # Logic to see if child should be added
                 unique_parent = len(sku.parents) <= 1
-                all_parents_in_collaterals = not bool(set(sku.parents) - collaterals._skus)
+                endoflife_items = set(collaterals._skus).union(phaseout_set)
+                all_parents_in_endoflife = not bool(set(sku.parents) - endoflife_items)
 
-                add_children = (unique_parent or all_parents_in_collaterals) and not sku.sellable
+                add_children = (unique_parent or all_parents_in_endoflife) and not sku.sellable
 
                 if add_children:
                     # Filter out obsoletes if needed
                     selected_children = sku.children if include_obsoletes else sku.active_children
                     selected_children = selected_children - collaterals._skus
 
                     # Add child to collaterals
```

### Comparing `repleno-0.0.13/src/repleno/__init__.py` & `repleno-0.0.14/src/repleno/__init__.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.13/src/repleno/factory.py` & `repleno-0.0.14/src/repleno/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -701,9 +701,20 @@
             qty = d["qty"]
 
             output.append([item, date_from, date_to, qty])
 
         return output
 
 
+    def get_collaterals(self, target, skus_only=False, phaseouts=None):
+        
+        sku = self.get_sku(target)
+
+        phaseout_skus = set()
+        for i in phaseouts:
+            phaseout_skus.add(self.get_sku(i))
+
+        return sku.get_collaterals(skus_only=skus_only, phaseout_skus=phaseout_skus)
+
+
 def run():
     pass
```

### Comparing `repleno-0.0.13/src/repleno/order.py` & `repleno-0.0.14/src/repleno/order.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.13/src/repleno/utils.py` & `repleno-0.0.14/src/repleno/utils.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.13/src/repleno.egg-info/PKG-INFO` & `repleno-0.0.14/src/repleno.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-Metadata-Version: 2.1
-Name: repleno
-Version: 0.0.13
-Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
-Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
-Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Manufacturing
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-
-
-# repleno
-
-Repleno allows you to easily answer supply chain questions considering bill of
-materials (BOM) structure.
-
-- **PyPI**: https://pypi.org/project/repleno/ 
-- **Source code**: 
-- **Documentation**: 
-- **Bug reports**: 
-
-
-It answers the following questions:
-
-1. "Which finished/purchased goods are associated with this stock keeping unit (SKU)?"
-2. "Based on this master production schedule (MPS), which specific SKU quantities should be ordered from suppliers?"
-3. "Using the master requirements planning (MRP) results and current supplier orders, when will there be stock-out periods?"
-4. "If I discontinue SKU X, which other SKU's will also need to be discontinued?"
-
-By providing:
-
-- efficient queries about parent-child relationships for SKUs in the BOM
-- MRP simulations to analyze the impact of MPS changes on purchase orders to suppliers
-- inventory levels over a specific time periods
-- identification of collateral SKU's that need to be phased-out along with a specific SKU
-
-
-Installing:
-
-```bash
-python -m pip install requests
-```
-
-## Roadmap:
-
-1. Integrate phantom scenarios to `run_mrp` and `get_lineage` and `get_collaterals` methods;
-2. issue a warning when a parameter is not being loaded or a column has not been found;
-3. get_collaterals function should return a tree, so it can be used to fully deplete the inventory inside it;
-4. run special mrp for scenarios: produce all inventory left in the BOM (placing more order to deplete everything or with scrapage);
-5. method for propagating any general label from roots to child nodes (from fininshed goods to purchased goods, in supply chain terms);
-6. Method for quickly answering the question: if one component goes out of stock, what's the impact on the finished goods?
-7. per component, shows how much of its demand impact finished goods. If 1 component goes into only 1 FG, then 100%
-8. Add support to add lead times in different units (currently only support calendar days), like weeks or months
+Metadata-Version: 2.1
+Name: repleno
+Version: 0.0.14
+Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
+Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
+Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Manufacturing
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+
+
+# repleno
+
+Repleno allows you to easily answer supply chain questions considering bill of
+materials (BOM) structure.
+
+- **PyPI**: https://pypi.org/project/repleno/ 
+- **Source code**: 
+- **Documentation**: 
+- **Bug reports**: 
+
+
+It answers the following questions:
+
+1. "Which finished/purchased goods are associated with this stock keeping unit (SKU)?"
+2. "Based on this master production schedule (MPS), which specific SKU quantities should be ordered from suppliers?"
+3. "Using the master requirements planning (MRP) results and current supplier orders, when will there be stock-out periods?"
+4. "If I discontinue SKU X, which other SKU's will also need to be discontinued?"
+
+By providing:
+
+- efficient queries about parent-child relationships for SKUs in the BOM
+- MRP simulations to analyze the impact of MPS changes on purchase orders to suppliers
+- inventory levels over a specific time periods
+- identification of collateral SKU's that need to be phased-out along with a specific SKU
+
+
+Installing:
+
+```bash
+python -m pip install requests
+```
+
+## Roadmap:
+
+1. Integrate phantom scenarios to `run_mrp` and `get_lineage` and `get_collaterals` methods;
+2. issue a warning when a parameter is not being loaded or a column has not been found;
+3. get_collaterals function should return a tree, so it can be used to fully deplete the inventory inside it;
+4. run special mrp for scenarios: produce all inventory left in the BOM (placing more order to deplete everything or with scrapage);
+5. method for propagating any general label from roots to child nodes (from fininshed goods to purchased goods, in supply chain terms);
+6. Method for quickly answering the question: if one component goes out of stock, what's the impact on the finished goods?
+7. per component, shows how much of its demand impact finished goods. If 1 component goes into only 1 FG, then 100%
+8. Add support to add lead times in different units (currently only support calendar days), like weeks or months
```

