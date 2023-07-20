# Comparing `tmp/kuplift-0.0.3.tar.gz` & `tmp/kuplift-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuplift-0.0.3.tar", last modified: Tue Jul 18 13:29:33 2023, max compression
+gzip compressed data, was "kuplift-0.0.4.tar", last modified: Thu Jul 20 14:03:30 2023, max compression
```

## Comparing `kuplift-0.0.3.tar` & `kuplift-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:29:33.791177 kuplift-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 13:29:13.000000 kuplift-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 13:29:33.791177 kuplift-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-18 13:29:13.000000 kuplift-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:29:33.787177 kuplift-0.0.3/kuplift/
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/BayesianDecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/BayesianRandomForest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/BinaryDiscretizationFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/FeatureSelection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/HelperFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/Tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    30719 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/UMODL_SearchAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/UnivariateEncoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:29:33.791177 kuplift-0.0.3/kuplift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 13:29:33.791177 kuplift-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-18 13:29:13.000000 kuplift-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:29:33.791177 kuplift-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test.py
--rw-r--r--   0 runner    (1001) docker     (123)   149105 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test_BayesianDecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)   146337 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test_BayesianRandomForest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test_FeatureSelection.py
--rw-r--r--   0 runner    (1001) docker     (123)   246158 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test_UnvariateEncoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:03:30.885376 kuplift-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-20 14:03:18.000000 kuplift-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 14:03:30.885376 kuplift-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-20 14:03:18.000000 kuplift-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:03:30.885376 kuplift-0.0.4/kuplift/
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/BayesianDecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/BayesianRandomForest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/BinaryDiscretizationFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/FeatureSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/HelperFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30684 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/UMODL_SearchAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/UnivariateEncoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-20 14:03:18.000000 kuplift-0.0.4/kuplift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:03:30.885376 kuplift-0.0.4/kuplift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 14:03:30.000000 kuplift-0.0.4/kuplift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 14:03:30.000000 kuplift-0.0.4/kuplift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:03:30.000000 kuplift-0.0.4/kuplift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 14:03:30.000000 kuplift-0.0.4/kuplift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 14:03:30.000000 kuplift-0.0.4/kuplift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 14:03:30.885376 kuplift-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-20 14:03:18.000000 kuplift-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:03:30.885376 kuplift-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)   149105 2023-07-20 14:03:18.000000 kuplift-0.0.4/test/test_BayesianDecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146337 2023-07-20 14:03:18.000000 kuplift-0.0.4/test/test_BayesianRandomForest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-20 14:03:18.000000 kuplift-0.0.4/test/test_FeatureSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246158 2023-07-20 14:03:18.000000 kuplift-0.0.4/test/test_UnvariateEncoding.py
```

### Comparing `kuplift-0.0.3/LICENSE` & `kuplift-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kuplift-0.0.3/PKG-INFO` & `kuplift-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: kuplift
-Version: 0.0.3
-Summary: A User Parameter-free Bayesian Framework for Uplift Modeling
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 ## kuplift package
 
 <p  align="center">
   <img src="https://raw.githubusercontent.com/UData-Orange/kuplift/main/docs/source/logo.png" width="310" />
 </p>
 
@@ -47,21 +40,31 @@
 
 # Uplift Bayesian Decision Tree
 tree = kp.BayesianDecisionTree(df, "treatment", "outcome")
 tree.fit()
 preds = tree.predict(df[column_names])
 
 # Uplift Bayesian Random Forest
-forest = kp.BayesianRandomForest(df, "treatment", "outcome", nb_trees)
+forest = kp.BayesianRandomForest(df, "treatment", "outcome")
 forest.fit()
 preds = forest.predict(df[features])
 ```
 
 **Documentation**:
 
 Refer to the documentation at https://udata-orange.github.io/kuplift/
 
+**Credits**:
+kuplift has been developed at Orange Labs.
+
+Current contributors:
+
+Mina Rafla
+
+Nicolas Voisine
+
+
 **References**:
 
 Rafla, M., Voisine, N., Crémilleux, B., & Boullé, M. (2023, March). A non-parametric bayesian approach for uplift discretization and feature selection. **_ECML PKDD 2022_**
 
 Rafla, M., Voisine, N., & Crémilleux, B. (2023, May). Parameter-free Bayesian decision trees for uplift modeling. **_PAKDD 2023_**
```

### Comparing `kuplift-0.0.3/README.md` & `kuplift-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: kuplift
+Version: 0.0.4
+Summary: A User Parameter-free Bayesian Framework for Uplift Modeling
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 ## kuplift package
 
 <p  align="center">
   <img src="https://raw.githubusercontent.com/UData-Orange/kuplift/main/docs/source/logo.png" width="310" />
 </p>
 
@@ -40,21 +47,31 @@
 
 # Uplift Bayesian Decision Tree
 tree = kp.BayesianDecisionTree(df, "treatment", "outcome")
 tree.fit()
 preds = tree.predict(df[column_names])
 
 # Uplift Bayesian Random Forest
-forest = kp.BayesianRandomForest(df, "treatment", "outcome", nb_trees)
+forest = kp.BayesianRandomForest(df, "treatment", "outcome")
 forest.fit()
 preds = forest.predict(df[features])
 ```
 
 **Documentation**:
 
 Refer to the documentation at https://udata-orange.github.io/kuplift/
 
+**Credits**:
+kuplift has been developed at Orange Labs.
+
+Current contributors:
+
+Mina Rafla
+
+Nicolas Voisine
+
+
 **References**:
 
 Rafla, M., Voisine, N., Crémilleux, B., & Boullé, M. (2023, March). A non-parametric bayesian approach for uplift discretization and feature selection. **_ECML PKDD 2022_**
 
 Rafla, M., Voisine, N., & Crémilleux, B. (2023, May). Parameter-free Bayesian decision trees for uplift modeling. **_PAKDD 2023_**
```

### Comparing `kuplift-0.0.3/kuplift/BayesianDecisionTree.py` & `kuplift-0.0.4/kuplift/BayesianDecisionTree.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,25 +31,15 @@
         Outcome column.
     """
 
     def __init__(self, data, treatment_col, y_col):
         super().__init__(data, treatment_col, y_col)
 
     def fit(self):
-        """Fit an uplift decision tree model using UB-DT
-
-        Parameters
-        ----------
-        X_train : pd.Dataframe
-            Dataframe containing feature variables.
-        treatment_col : pd.Series
-            Treatment column.
-        y_col : pd.Series
-            Outcome column.
-        """
+        """Fit an uplift decision tree model using UB-DT."""
         # In case if we have a new attribute for splitting
         prob_kt_plus_one = (
             universal_code_natural_numbers(self.k_t + 1)
             - log_fact(self.k_t + 1)
             + (self.k_t + 1) * log(self.k)
         )
         prob_of_attribute_selection_among_subset_attributes_plus_one = log(
@@ -73,20 +63,21 @@
             + encoding_of_being_a_leaf_node_and_containing_te_plus_two
         )
 
         i = 0
         while True:
             node_vs_best_attribute_corresponding_to_the_best_cost = {}
             node_vs_best_cost = {}
-            node_vs_candidate_splits_costs = (
-                {}
-            )  # Dictionary containing Nodes as key and their values are another dictionary each with attribute:CostSplit
+            # Dictionary containing Nodes as key and their values are another
+            # dictionary each with attribute:CostSplit
+            node_vs_candidate_splits_costs = {}
 
             for terminal_node in self.terminal_nodes:
-                # This if condition is here to not to repeat calculations of candidate splits
+                # This if condition is here to not to repeat calculations of
+                # candidate splits
                 if terminal_node.candidate_splits_vs_criterion is None:
                     node_vs_candidate_splits_costs[
                         terminal_node
                     ] = (
                         terminal_node.discretize_vars_and_get_attributes_splits_costs()
                     )
                 else:
@@ -164,14 +155,7 @@
                 self.terminal_nodes.append(new_right_leaf)
                 self.internal_nodes.append(optimal_node)
                 self.terminal_nodes.remove(optimal_node)
 
                 self.calc_criterion()
             else:
                 break
-        print("Learning Finished")
-        for node in self.terminal_nodes:
-            print("Node id ", node.id)
-            print("Node outcome_prob_in_trt ", node.outcome_prob_in_trt)
-            print("Node outcome_prob_in_ctrl ", node.outcome_prob_in_ctrl)
-            print("self ntj ", node.ntj)
-        print("===============")
```

### Comparing `kuplift-0.0.3/kuplift/BayesianRandomForest.py` & `kuplift-0.0.4/kuplift/BayesianRandomForest.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,82 +61,96 @@
             + encoding_of_being_a_leaf_node_and_containing_te_plus_two
         )
 
         i = 0
         while True:
             node_vs_best_attribute_corresponding_to_the_best_cost = {}
             node_vs_best_cost = {}
-            node_vs_candidate_splits_costs = (
-                {}
-            )  # Dictionary containing Nodes as key and their values are another dictionary each with attribute:CostSplit
-
+            # Dictionary containing Nodes as key and their values are another
+            # dictionary each with attribute:CostSplit
+            node_vs_candidate_splits_costs = {}
             for terminal_node in self.terminal_nodes:
-                # This if condition is here to not to repeat calculations of candidate splits
+                # This if condition is here to not to repeat calculations of
+                # candidate splits
                 if terminal_node.candidate_splits_vs_criterion is None:
                     node_vs_candidate_splits_costs[
                         terminal_node
-                    ] = terminal_node.discretize_vars_and_get_attributes_splits_costs()
+                    ] = (
+                        terminal_node.discretize_vars_and_get_attributes_splits_costs()
+                    )
                 else:
                     node_vs_candidate_splits_costs[
                         terminal_node
                     ] = terminal_node.candidate_splits_vs_criterion.copy()
 
                 if len(node_vs_candidate_splits_costs[terminal_node]) == 0:
                     continue
 
                 # Update Costs
                 list_of_attribute_splits_improving_tree_criterion = []
                 for attribute in node_vs_candidate_splits_costs[terminal_node]:
                     if attribute in self.feature_subset:
-                        node_vs_candidate_splits_costs[terminal_node][attribute] += (
+                        node_vs_candidate_splits_costs[terminal_node][
+                            attribute
+                        ] += (
                             self.prob_kt
                             + self.prob_attribute_selection
                             + encoding_of_internal_and_leaves_and_w_with_extra_nodes
                             + self.leaf_prior
                             + self.tree_likelihood
                             + self.prior_of_internal_nodes
                         )
                     else:
-                        node_vs_candidate_splits_costs[terminal_node][attribute] += (
+                        node_vs_candidate_splits_costs[terminal_node][
+                            attribute
+                        ] += (
                             prob_kt_plus_one
                             + encoding_of_internal_and_leaves_and_w_with_extra_nodes
                             + prob_of_attribute_selection_among_subset_attributes_plus_one
                             + self.leaf_prior
                             + self.tree_likelihood
                             + self.prior_of_internal_nodes
                         )
 
                     if (
-                        node_vs_candidate_splits_costs[terminal_node][attribute]
+                        node_vs_candidate_splits_costs[terminal_node][
+                            attribute
+                        ]
                         < self.tree_criterion
                     ):
                         list_of_attribute_splits_improving_tree_criterion.append(
                             attribute
                         )
                 if len(list_of_attribute_splits_improving_tree_criterion) == 0:
                     continue
                 key_of_the_minimal_val = random.choice(
                     list_of_attribute_splits_improving_tree_criterion
                 )  # key_of_the_minimal_val is the attribute name
 
                 node_vs_best_attribute_corresponding_to_the_best_cost[
                     terminal_node
                 ] = key_of_the_minimal_val
-                node_vs_best_cost[terminal_node] = node_vs_candidate_splits_costs[
+                node_vs_best_cost[
                     terminal_node
-                ][key_of_the_minimal_val]
+                ] = node_vs_candidate_splits_costs[terminal_node][
+                    key_of_the_minimal_val
+                ]
 
             if len(list(node_vs_best_cost)) == 0:
                 break
-            optimal_node_attribute_to_split_up = random.choice(list(node_vs_best_cost))
+            optimal_node_attribute_to_split_up = random.choice(
+                list(node_vs_best_cost)
+            )
             optimal_val = node_vs_best_cost[optimal_node_attribute_to_split_up]
             optimal_node = optimal_node_attribute_to_split_up
-            optimal_attribute = node_vs_best_attribute_corresponding_to_the_best_cost[
-                optimal_node_attribute_to_split_up
-            ]
+            optimal_attribute = (
+                node_vs_best_attribute_corresponding_to_the_best_cost[
+                    optimal_node_attribute_to_split_up
+                ]
+            )
 
             if optimal_val < self.tree_criterion:
                 self.tree_criterion = optimal_val
                 if optimal_attribute not in self.feature_subset:
                     self.feature_subset.append(optimal_attribute)
                     self.k_t += 1
                 new_left_leaf, new_right_leaf = optimal_node.perform_split(
@@ -145,15 +159,14 @@
                 self.terminal_nodes.append(new_left_leaf)
                 self.terminal_nodes.append(new_right_leaf)
                 self.internal_nodes.append(optimal_node)
                 self.terminal_nodes.remove(optimal_node)
 
                 self.calc_criterion()
             else:
-                print("WILL NEVER ENTER HERE")
                 break
 
         self.tree_criterion = (
             self.prob_kt
             + self.encoding_of_being_an_internal_node
             + self.prob_attribute_selection
             + self.prior_of_internal_nodes
@@ -173,70 +186,70 @@
     ----------
     data : pd.Dataframe
         Dataframe containing data.
     treatment_col : pd.Series
         Treatment column.
     outcome_col : pd.Series
         Outcome column.
-    n_trees : int
+    n_trees : int, default 10
         Number of trees in a forest.
-    vars_subset : boolean
-        Use a random subset of the variables for each tree in the forest
+    vars_subset : bool, default False
+        Use a random subset of the variables for each tree in the forest.
+    random_state : int, default 10
+        Seed used by the random number generator.
     """
 
     def __init__(
         self,
         data,
         treatment_col,
         y_col,
-        n_trees,
+        n_trees=10,
         vars_subset=False,
         random_state=10,
     ):
         self.list_of_trees = []
         self.data = data
         random.seed(random_state)
-        
+
         # Randomly select columns for the data
         if vars_subset:
             cols = list(self.data.columns)
             cols.remove(treatment_col)
             cols.remove(y_col)
-            print("cols before are ", cols)
             cols = random.sample(cols, int(np.sqrt(len(cols))))
-            print("cols after are ", cols)
             self.data = self.data[cols + [treatment_col, y_col]]
         for i in range(n_trees):
-            Tree = _UpliftTreeClassifier(self.data.copy(), treatment_col, y_col)
+            Tree = _UpliftTreeClassifier(
+                self.data.copy(), treatment_col, y_col
+            )
             self.list_of_trees.append(Tree)
 
     def fit(self):
-        """
-        Fit a decision tree algorithm
-        """
+        """Fit a decision tree algorithm."""
         for tree in self.list_of_trees:
             tree.grow_tree()
 
     def predict(self, X_test, weighted_average=False):
         """
-        Predict the uplift value for each example in X_test
+        Predict the uplift value for each example in X_test.
 
         Parameters
         ----------
         X_test : pd.Dataframe
             Dataframe containing test data.
-        weighted_average : boolean
-            Give a weight for the predictions of each tree according to its cost (default = False)
+        weighted_average : bool, default False
+            Give a weight for the predictions of each tree according to its cost.
 
         Returns
         -------
-        y_pred_list(ndarray, shape=(num_samples, 1))
+        y_pred_list : (ndarray, shape=(num_samples, 1))
             An array containing the predicted uplift for each sample.
         """
-        if weighted_average == False:
+        if not weighted_average:
             list_of_preds = []
 
             for tree in self.list_of_trees:
                 list_of_preds.append(np.array(tree.predict(X_test)))
             return np.mean(list_of_preds, axis=0)
         else:
             list_of_criterion = []
@@ -249,9 +262,8 @@
             for i in range(len(list_of_criterion)):
                 list_of_criterion[i] = sum_of_criterions / list_of_criterion[i]
             sum_of_weights = sum(list_of_criterion)
 
             list_of_weights = []
             for i in range(len(list_of_criterion)):
                 list_of_weights.append(list_of_criterion[i] / sum_of_weights)
-            print("list of weights is ", list_of_weights)
             return np.average(list_of_preds, axis=0, weights=list_of_weights)
```

### Comparing `kuplift-0.0.3/kuplift/BinaryDiscretizationFunctions.py` & `kuplift-0.0.4/kuplift/BinaryDiscretizationFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,16 @@
         data_nitj[int((interval_list[1] * 2) + interval_list[2])] += 1
 
     N = len(data)
     including_left_border = True
     left_bound = data[0][0]  # The smallest value
     right_bound = data[-1][0]  # The biggest value
 
-    # Get all the unique values in the data i.e All unique values between left and right bounds
+    # Get all the unique values in the data i.e All unique values between left
+    # and right bounds
     unique_values_in_both_intervals = list(
         data.irange_key(left_bound, right_bound, (including_left_border, True))
     )
     unique_values_in_both_intervals = list(
         map(itemgetter(0), unique_values_in_both_intervals)
     )
     unique_values_in_both_intervals = list(
@@ -176,17 +177,16 @@
     prior_rissanen = log(2) + log_binomial_coefficient(N + 1, 1) + 2 * log(2)
 
     for val in unique_values_in_both_intervals:
         if (len(unique_values_in_both_intervals) <= 1) or (val == right_bound):
             break
 
         if prev_val is None:  # Enters here only for the first unique value
-            left_split = list(
-                data.irange_key(left_bound, val, (True, True))
-            )  # Get a list of all data between left_bound and current unique value
+            # Get a list of data between left_bound and current unique value
+            left_split = list(data.irange_key(left_bound, val, (True, True)))
             left_interval = [0, 0, 0, 0]
             for interval_list in left_split:
                 left_interval[
                     int((interval_list[1] * 2) + interval_list[2])
                 ] += 1
         else:
             left_split = list(data.irange_key(prev_val, val, (False, True)))
@@ -226,21 +226,14 @@
         split_criterion_val_left_and_right = (
             prior_rissanen + criterion_one + criterion_two
         )
         stop_counter(24)
         # If the MODL value is smaller than the null model value add it
         # to the splits dictionary
         if split_criterion_val_left_and_right < null_model_value:
-            if sum(right_interval) == 0:
-                print("strange case")
-                print("null_model_value ", null_model_value)
-                print(
-                    "split_criterion_val_left_and_right ",
-                    split_criterion_val_left_and_right,
-                )
             splits[val] = split_criterion_val_left_and_right
     best_split = None
 
     # If dictionary splits contain value, get the minimal one
     if splits:
         best_split = min(splits, key=splits.get)  # To be optimized maybe
         left_split = list(
```

### Comparing `kuplift-0.0.3/kuplift/FeatureSelection.py` & `kuplift-0.0.4/kuplift/FeatureSelection.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         features = list(data.columns)
         features.remove(treatment_col)
         features.remove(y_col)
 
         var_vs_importance = {}
         var_vs_disc = {}
         for feature in features:
-            print("feature is ", feature)
             (
                 var_vs_importance[feature],
                 var_vs_disc[feature],
             ) = execute_greedy_search_and_post_opt(
                 data[[feature, treatment_col, y_col]]
             )
         # sort the dictionary by values in ascending order
@@ -65,15 +64,15 @@
             for k, v in sorted(
                 var_vs_importance.items(), key=lambda item: item[1]
             )
         }
         return var_vs_importance
 
     @staticmethod
-    def get_the_best_var_parallel(args):
+    def __get_the_best_var_parallel(args):
         """
         Parameters
         ----------
         data : pd.Dataframe
             Dataframe containing data.
         treatment_col : pd.Series
             Treatment column.
@@ -92,15 +91,14 @@
         """
         data, treatment_col, y_col = args[0], args[1], args[2]
 
         features = list(data.columns)
         feature = features[0]
         features.remove(treatment_col)
         features.remove(y_col)
-        print("feature is ", feature)
         var_vs_importance = {}
         var_vs_disc = {}
         (
             var_vs_importance[feature],
             var_vs_disc[feature],
         ) = execute_greedy_search_and_post_opt(
             data[[feature, treatment_col, y_col]]
@@ -118,41 +116,41 @@
         ----------
         data : pd.Dataframe
             Dataframe containing feature variables.
         treatment_col : pd.Series
             Treatment column.
         y_col : pd.Series
             Outcome column.
-        parallelized : Boolean
-            Whether to run the code on several processes (default = 5)
-        num_processes : int
-            number of processes to use in parallel (default = 5)
+        parallelized : bool, default False
+            Whether to run the code on several processes.
+        num_processes : int, default 5
+            Number of processes to use in parallel.
 
         Returns
         -------
         Python Dictionary
             Variables names and their corresponding importance value (Sorted).
         """
         cols = list(data.columns)
 
         cols.remove(treatment_col)
         cols.remove(y_col)
         data = data[cols + [treatment_col, y_col]]
         data = preprocess_data(data, treatment_col, y_col)
 
-        if parallelized == True:
+        if parallelized:
             pool = mp.Pool(processes=num_processes)
 
             arguments_to_pass_in_parallel = []
             for col in cols:
                 arguments_to_pass_in_parallel.append(
                     [data[[col, treatment_col, y_col]], treatment_col, y_col]
                 )
             list_of_tuples_feature_vs_importance = pool.map(
-                FeatureSelection.get_the_best_var_parallel,
+                FeatureSelection.__get_the_best_var_parallel,
                 arguments_to_pass_in_parallel,
             )
             pool.close()
 
             # transform tuple to dict
             list_of_tuples_feature_vs_importance = dict(
                 list_of_tuples_feature_vs_importance
```

### Comparing `kuplift-0.0.3/kuplift/HelperFunctions.py` & `kuplift-0.0.4/kuplift/HelperFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,38 +105,39 @@
     k : int
 
     Returns
     -------
     float
         Value of the result.
     """
-    dC0 = 2.86511  # First value computed following the given estimation formula, as e(3)=65536 + d_log2^5 / (1-d_log2)
+    dC0 = 2.86511  # First value computed following the given estimation
+    # formula, as e(3)=65536 + d_log2^5 / (1-d_log2)
     d_log2 = log(2.0)
 
     if k < 1:
         raise ValueError(
             "Universal code is defined for natural numbers over 1"
         )
     else:
         d_cost = log(dC0) / d_log2  # Initialize code length cost to log_2(dC0)
         d_cost += log_2_star(k)  # Add log_2*(k)
         d_cost *= d_log2  # Go back to the natural log
         return d_cost
 
 
 def preprocess_data(data, treatment_col="segment", y_col="visit"):
-    """Description?
+    """preprocess data
 
     Parameters
     ----------
     data : pd.Dataframe
         Dataframe containing feature variables.
-    treatment_col : pd.Series, optional
+    treatment_col : pd.Series, default "segment"
         Treatment column.
-    y_col : pd.Series, optional
+    y_col : pd.Series, default "visit"
         Outcome column.
 
     Returns
     -------
     pd.Dataframe
         Pandas Dataframe that contains encoded data.
     """
```

### Comparing `kuplift-0.0.3/kuplift/Node.py` & `kuplift-0.0.4/kuplift/Node.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     ----------
     data : pd.Dataframe
         Dataframe containing feature variables.
     treatment_col : pd.Series
         Treatment column.
     y_col : pd.Series
         Outcome column.
-    ID : ?, optional
-        ?
+    ID : int, default None
+        Tree node ID.
     """
 
     def __init__(self, data, treatment_col, y_col, ID=None):
         # Initialize attributes
         self.id = ID
         self.treatment = treatment_col
         self.output = y_col
@@ -177,17 +177,17 @@
         self.candidate_splits_vs_criterion = (
             candidate_splits_vs_criterion.copy()
         )
         return candidate_splits_vs_criterion.copy()
 
     def __get_attributes_splits_costs(self, dict_of_each_att_vs_effectifs):
         # Prior of Internal node is only the combinatorial calculations
-        criterion_to_be_internal = (
-            self.__calc_prior_of_internal_node()
-        )  # In case we split this node, it will be no more a leaf but an internal node
+        # In case we split this node, it will be no more a leaf but an internal
+        # node
+        criterion_to_be_internal = self.__calc_prior_of_internal_node()
         new_prior_vals = (
             criterion_to_be_internal - self.prior_leaf - self.likelihood_leaf
         )
 
         candidate_splits_vs_criterion = {}
         for key in dict_of_each_att_vs_effectifs:
             leaves_val = self.__update_tree_criterion(
```

### Comparing `kuplift-0.0.3/kuplift/Tree.py` & `kuplift-0.0.4/kuplift/Tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,58 +193,52 @@
 
         row = (
             self.summary_df[self.summary_df["NodeId"] == IdValue]
             .iloc[:1]
             .reset_index(drop=True)
             .squeeze()
         )
-        #     print("row is ",type(row))
-        #     print("row is ",row)
-        if row["isLeaf"] == False:
-            #         print(" id ",str(IdValue)," not leaf")
+        if not row["isLeaf"]:
             text_desc = createTabs(text_desc, numTabs)
             text_desc = (
                 text_desc
                 + "|--- "
                 + " "
                 + str(row["SplittedAttribute"])
                 + " <= "
                 + str(row["SplitThreshold"])
                 + "\n"
             )
-            #         print(text_desc)
             text_desc = self.export_tree(IdValue * 2, numTabs + 1, text_desc)
-
             text_desc = createTabs(text_desc, numTabs)
             text_desc = (
                 text_desc
                 + "|--- "
                 + " "
                 + str(row["SplittedAttribute"])
                 + " >= "
                 + str(row["SplitThreshold"])
                 + "\n"
             )
             text_desc = self.export_tree(
                 IdValue * 2 + 1, numTabs + 1, text_desc
             )
         else:
-            #         print(" id ",str(IdValue),"is leaf")
             text_desc = createTabs(text_desc, numTabs)
             text_desc += "|--- Leaf \n"
             text_desc = createTabs(text_desc, numTabs + 1)
             try:
                 text_desc = (
                     text_desc
                     + "|--- "
                     + " Outcome Distribution in Treatment "
                     + str(row["T1Y1"] / (row["T1Y1"] + row["T1Y0"]))
                     + "\n"
                 )
-            except:
+            except Exception:
                 text_desc = (
                     text_desc
                     + "|--- "
                     + " Outcome Distribution in Treatment "
                     + str(row["T1Y1"] / 0.0001)
                     + "(No treatment)\n"
                 )
@@ -254,15 +248,15 @@
                 text_desc = (
                     text_desc
                     + "|--- "
                     + " Outcome Distribution in Control "
                     + str(row["T0Y1"] / (row["T0Y1"] + row["T0Y0"]))
                     + "\n"
                 )
-            except:
+            except Exception:
                 text_desc = (
                     text_desc
                     + "|--- "
                     + " Outcome Distribution in Control "
                     + str(row["T0Y1"] / 0.001)
                     + " (No control)\n"
                 )
```

### Comparing `kuplift-0.0.3/kuplift/UMODL_SearchAlgorithm.py` & `kuplift-0.0.4/kuplift/UMODL_SearchAlgorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,23 +336,27 @@
 
         return [self.modl_value, self.count, interval_bounds, list_of_ws]
 
 
 def create_elementary_discretization(dll, data):
     """
     params
-    data : list of lists, each internal list contains [data value, treatment value, y value]
+    data : list of lists, each internal list contains
+    [data value, treatment value, y value]
 
     returns
-    1- a list of lists. Each internal list represents an interval and contains Effectifs of T0J0, T0J1, T1J0, T1J1 respectively.
+    1- a list of lists. Each internal list represents an interval and contains
+        Effectifs of T0J0, T0J1, T1J0, T1J1 respectively.
     2- frontier value per interval
-    3- w : list containing the Wi value for each interval, the initial discretization has Wi = 0 for all i
+    3- w : list containing the Wi value for each interval, the initial
+        discretization has Wi = 0 for all i
     """
     start_counter(0)
-    # This is a list of lists, each internal list represents an interval and contains Effectifs of T0J0, T0J1, T1J0, T1J1 respectively
+    # This is a list of lists, each internal list represents an interval and
+    # contains Effectifs of T0J0, T0J1, T1J0, T1J1 respectively
     prev = None
     i = -1
     for interval_list in data:
         if interval_list[0] != prev:
             if i != -1:
                 dll.tail.calculate_priors_and_likelihoods()
             dll.append([[0, 0, 0, 0], interval_list[0], 0])
@@ -441,17 +445,21 @@
             old_left_interval_node_criterion = (
                 interval_to_be_merged.sum_of_priors_and_likelihoods
             )
             old_right_interval_node_criterion = (
                 interval_right_of_the_merge.sum_of_priors_and_likelihoods
             )
 
-            left_interval_node_criterion = interval_to_be_merged.calculate_priors_and_likelihoods(
-                mode="MergeAndUpdate"
-            )  # it will update w, Priors, lkelihoods and sum_of_priors_and_likelihoods
+            # it will update w, priors, likelihoods and
+            # sum_of_priors_and_likelihoods
+            left_interval_node_criterion = (
+                interval_to_be_merged.calculate_priors_and_likelihoods(
+                    mode="MergeAndUpdate"
+                )
+            )
             intervals.modl_value = (
                 intervals.modl_value
                 - old_right_interval_node_criterion
                 - old_left_interval_node_criterion
                 - log_binomial_coefficient(
                     intervals.n + intervals.i - 1, intervals.i - 1
                 )
@@ -548,18 +556,19 @@
             -1
         ].sum_of_priors_and_likelihoods
 
     interval.nitj = merged_intervals
     interval.included_right_frontier = neighbours_to_merge[
         -1
     ].included_right_frontier
-    # NOW WE HAVE TO SEARCH for the old values of the sum of prior and likelihoods !!!!
+    # for the old values of the sum of prior and likelihoods
+    # it will update w, priors, likelihoods and sum_of_priors_and_likelihoods
     left_interval_node_criterion = interval.calculate_priors_and_likelihoods(
         mode="MergeAndUpdate"
-    )  # it will update w, Priors, lkelihoods and sum_of_priors_and_likelihoods
+    )
     intervals.modl_value = (
         intervals.modl_value
         - sum_of_old_priors_and_likelihoods
         - log_binomial_coefficient(
             intervals.n + intervals.i - 1, intervals.i - 1
         )
         - ((intervals.i) * log(2))
@@ -567,17 +576,17 @@
             intervals.n + intervals.i - number_of_merges - 1,
             intervals.i - number_of_merges - 1,
         )
         + ((intervals.i - number_of_merges) * log(2))
         + left_interval_node_criterion
     )
 
-    for i in range(
-        1, len(neighbours_to_merge)
-    ):  # Note the first element is the current interval that we are merging, no need to remove it!
+    # Note the first element is the current interval that we are merging,
+    # no need to remove it!
+    for i in range(1, len(neighbours_to_merge)):
         intervals.remove_interval(neighbours_to_merge[i])
 
 
 def split_interval(
     interval, intervals, data, i
 ):  # i is interval index in intervalsList
     if interval == intervals.head:
@@ -673,20 +682,18 @@
             i + 1,
         )
         Right_interval = intervals.get_nth(i + 1)
 
         Left_interval.nitj = left_interval
         Left_interval.included_right_frontier = best_split
 
-        Left_interval.calculate_priors_and_likelihoods(
-            mode="MergeAndUpdate"
-        )  # it will update w, Priors, lkelihoods and sum_of_priors_and_likelihoods
-        Right_interval.calculate_priors_and_likelihoods(
-            mode="MergeAndUpdate"
-        )  # it will update w, Priors, lkelihoods and sum_of_priors_and_likelihoods
+        # it will update w, priors, likelihoods and
+        # sum_of_priors_and_likelihoods
+        Left_interval.calculate_priors_and_likelihoods(mode="MergeAndUpdate")
+        Right_interval.calculate_priors_and_likelihoods(mode="MergeAndUpdate")
 
         intervals.modl_value = splits[best_split]
         split_done = True
     return split_done, best_split, intervals
 
 
 def post_optimization_to_be_repeated(intervals, data, i=0):
@@ -845,33 +852,34 @@
     return absolute_sum
 
 
 def execute_greedy_search_and_post_opt(df):
     treatment_col_name = df.columns[1]
     y_name = df.columns[2]
 
-    df = df.astype({treatment_col_name:'int'})
-    df = df.astype({y_name:'int'})
+    df = df.astype({treatment_col_name: "int"})
+    df = df.astype({y_name: "int"})
 
     df = df.values.tolist()
     df = sorted(df, key=itemgetter(0))
     intervals = _DLL()
     intervals.n = len(df)
 
     intervals, intervals.modl_value, w = create_elementary_discretization(
         intervals, df
     )  # Elementary discretization
 
     compute_criterion_delta_for_all_possible_merges(
         intervals
     )  # Compute the cost of all possible merges of two adjacent intervals
 
+    # All the costs of 'all possible merges of two adjacent intervals' sorted
     best_merges = intervals.get_sorted_list_of_address_and_right_merge_value(
         intervals.head
-    )  # Get all the costs of 'all possible merges of two adjacent intervals' sorted
+    )
     best_merges = SortedKeyList(best_merges, key=itemgetter(0))
 
     # Start greedy search
     greedy_search(best_merges, intervals, intervals.n)
 
     # Post Optimization steps
     (
```

### Comparing `kuplift-0.0.3/kuplift/UnivariateEncoding.py` & `kuplift-0.0.4/kuplift/UnivariateEncoding.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,82 +11,88 @@
 import multiprocessing as mp
 from .HelperFunctions import preprocess_data
 from .UMODL_SearchAlgorithm import execute_greedy_search_and_post_opt
 
 
 class UnivariateEncoding:
     """
-    The UnivariateEncoding class implements the UMODL algorithm for uplift data encoding described in:
+    The UnivariateEncoding class implements the UMODL algorithm for uplift data
+    encoding described in:
     Rafla, M., Voisine, N., Crémilleux, B., & Boullé, M.
     (2023, March). A non-parametric bayesian approach for uplift
-    discretization and feature selection. ECML PKDD
+    discretization and feature selection. ECML PKDD.
     """
 
     def __init__(self):
         self.var_vs_disc = {}
         self.treatment_col = ""
         self.y_col = ""
 
     def fit_transform(
         self, data, treatment_col, y_col, parallelized=False, num_processes=5
     ):
         """
-        fit_transform() learns a discretisation model using UMODL and transforms the data.
+        fit_transform() learns a discretisation model using UMODL and
+        transforms the data.
 
         Parameters
         ----------
         data : pd.Dataframe
             Dataframe containing feature variables.
         treatment_col : pd.Series
             Treatment column.
         y_col : pd.Series
             Outcome column.
+        parallelized : bool, default False
+            Whether to run the code on several processes.
+        num_processes : int, default 5
+            Number of processes to use in parallel.
 
         Returns
         -------
         pd.Dataframe
             Pandas Dataframe that contains encoded data.
         """
         self.fit(data, treatment_col, y_col, parallelized, num_processes)
         data = self.transform(data)
         return data
 
     def fit(
         self, data, treatment_col, y_col, parallelized=False, num_processes=5
     ):
         """
-         fit() learns a discretisation model using the UMODL approach
+        fit() learns a discretisation model using the UMODL approach.
 
         Parameters
         ----------
         data : pd.Dataframe
             Dataframe containing feature variables.
         treatment_col : pd.Series
             Treatment column.
         y_col : pd.Series
             Outcome column.
-        parallelized : Boolean
-            Whether to run the code on several processes (default = 5)
-        num_processes : int
-            number of processes to use in parallel (default = 5)
+        parallelized : bool, default False
+            Whether to run the code on several processes.
+        num_processes : int, default 5
+            Number of processes to use in parallel.
         """
         self.treatment_col = treatment_col
         self.y_col = y_col
 
         cols = list(data.columns)
         cols.remove(treatment_col)
         cols.remove(y_col)
 
         data = data[cols + [treatment_col, y_col]]
         data = preprocess_data(data, treatment_col, y_col)
 
         var_vs_importance = {}
         self.var_vs_disc = {}
 
-        if parallelized == True:
+        if parallelized:
             pool = mp.Pool(processes=num_processes)
 
             arguments_to_pass_in_parallel = []
             for col in cols:
                 arguments_to_pass_in_parallel.append(
                     [data[[col, treatment_col, y_col]]]
                 )
@@ -115,15 +121,16 @@
                     self.var_vs_disc[col] = None
                 else:
                     self.var_vs_disc[col] = self.var_vs_disc[col][:-1]
         return self.var_vs_disc
 
     def transform(self, data):
         """
-        transform() applies the discretisation model learned by the fit() method
+        transform() applies the discretisation model learned by the
+        fit() method.
 
         Parameters
         ----------
         data : pd.Dataframe
             Dataframe containing feature variables.
 
         Returns
```

### Comparing `kuplift-0.0.3/kuplift/__init__.py` & `kuplift-0.0.4/kuplift/__init__.py`

 * *Files identical despite different names*

### Comparing `kuplift-0.0.3/kuplift.egg-info/PKG-INFO` & `kuplift-0.0.4/kuplift.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuplift
-Version: 0.0.3
+Version: 0.0.4
 Summary: A User Parameter-free Bayesian Framework for Uplift Modeling
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## kuplift package
 
@@ -47,21 +47,31 @@
 
 # Uplift Bayesian Decision Tree
 tree = kp.BayesianDecisionTree(df, "treatment", "outcome")
 tree.fit()
 preds = tree.predict(df[column_names])
 
 # Uplift Bayesian Random Forest
-forest = kp.BayesianRandomForest(df, "treatment", "outcome", nb_trees)
+forest = kp.BayesianRandomForest(df, "treatment", "outcome")
 forest.fit()
 preds = forest.predict(df[features])
 ```
 
 **Documentation**:
 
 Refer to the documentation at https://udata-orange.github.io/kuplift/
 
+**Credits**:
+kuplift has been developed at Orange Labs.
+
+Current contributors:
+
+Mina Rafla
+
+Nicolas Voisine
+
+
 **References**:
 
 Rafla, M., Voisine, N., Crémilleux, B., & Boullé, M. (2023, March). A non-parametric bayesian approach for uplift discretization and feature selection. **_ECML PKDD 2022_**
 
 Rafla, M., Voisine, N., & Crémilleux, B. (2023, May). Parameter-free Bayesian decision trees for uplift modeling. **_PAKDD 2023_**
```

### Comparing `kuplift-0.0.3/kuplift.egg-info/SOURCES.txt` & `kuplift-0.0.4/kuplift.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,11 @@
 kuplift/UnivariateEncoding.py
 kuplift/__init__.py
 kuplift.egg-info/PKG-INFO
 kuplift.egg-info/SOURCES.txt
 kuplift.egg-info/dependency_links.txt
 kuplift.egg-info/requires.txt
 kuplift.egg-info/top_level.txt
-test/test.py
 test/test_BayesianDecisionTree.py
 test/test_BayesianRandomForest.py
 test/test_FeatureSelection.py
 test/test_UnvariateEncoding.py
```

### Comparing `kuplift-0.0.3/setup.py` & `kuplift-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
 setup(
     name="kuplift",
-    version="0.0.3",
+    version="0.0.4",
     packages=["kuplift"],
     description="A User Parameter-free Bayesian Framework for Uplift Modeling",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "numpy",
         "pandas",
```

### Comparing `kuplift-0.0.3/test/test_BayesianDecisionTree.py` & `kuplift-0.0.4/test/test_BayesianDecisionTree.py`

 * *Files identical despite different names*

### Comparing `kuplift-0.0.3/test/test_BayesianRandomForest.py` & `kuplift-0.0.4/test/test_BayesianRandomForest.py`

 * *Files identical despite different names*

### Comparing `kuplift-0.0.3/test/test_FeatureSelection.py` & `kuplift-0.0.4/test/test_FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `kuplift-0.0.3/test/test_UnvariateEncoding.py` & `kuplift-0.0.4/test/test_UnvariateEncoding.py`

 * *Files identical despite different names*

