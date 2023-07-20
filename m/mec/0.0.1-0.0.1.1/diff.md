# Comparing `tmp/mec-0.0.1.tar.gz` & `tmp/mec-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mec-0.0.1.tar", last modified: Tue Jul 18 08:49:44 2023, max compression
+gzip compressed data, was "mec-0.0.1.1.tar", last modified: Thu Jul 20 20:48:39 2023, max compression
```

## Comparing `mec-0.0.1.tar` & `mec-0.0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:44.010549 mec-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 08:49:44.010549 mec-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:44.010549 mec-0.0.1/mec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:37.000000 mec-0.0.1/mec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-18 08:49:37.000000 mec-0.0.1/mec/lp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:44.010549 mec-0.0.1/mec/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:37.000000 mec-0.0.1/mec/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:44.010549 mec-0.0.1/mec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 08:49:43.000000 mec-0.0.1/mec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 08:49:44.000000 mec-0.0.1/mec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:49:43.000000 mec-0.0.1/mec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 08:49:43.000000 mec-0.0.1/mec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:49:44.010549 mec-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 08:49:37.000000 mec-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:48:39.889820 mec-0.0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-20 20:48:39.889820 mec-0.0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:48:39.889820 mec-0.0.1.1/mec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:48:31.000000 mec-0.0.1.1/mec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-20 20:48:31.000000 mec-0.0.1.1/mec/lp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-20 20:48:31.000000 mec-0.0.1.1/mec/ot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:48:39.889820 mec-0.0.1.1/mec/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:48:31.000000 mec-0.0.1.1/mec/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:48:39.889820 mec-0.0.1.1/mec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-20 20:48:39.000000 mec-0.0.1.1/mec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-20 20:48:39.000000 mec-0.0.1.1/mec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:48:39.000000 mec-0.0.1.1/mec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:48:39.000000 mec-0.0.1.1/mec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:48:39.889820 mec-0.0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 20:48:31.000000 mec-0.0.1.1/setup.py
```

### Comparing `mec-0.0.1/mec/lp.py` & `mec-0.0.1.1/mec/lp.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,29 +58,27 @@
         self.nonbasic = list(symbols(names_nonbasic))
         self.base = { Symbol('obj') : c_j @ self.nonbasic }
         self.base.update( { list(symbols(names_basic))[i]: b_i[i]  - (A_i_j @ self.nonbasic)[i] for i in range(len(b_i))} )
 
     def variables(self):
         return( list(self.base.keys())[1:] + self.nonbasic)
 
-    def evaluate(self,thevar):
-        if thevar in set(self.nonbasic):
-            return 0.0
-        else:
-            return float(self.base[thevar].evalf(subs = {variable:0.0 for variable in self.nonbasic} ))
-
     def display(self):
         for i in self.base:
             print(i,' = ' ,round_expr(self.base[i],2))
             
-    def print_solution(self,title=None):
-        if not (title is None):
-            print(title)
+    def solution(self, verbose=0):
+        solution = {}
         for var in self.base:
-            print(str(var)+'='+str(self.base[var].subs([ (variable,0) for variable in self.nonbasic])))
+            solution[var] = float(self.base[var].subs([(variable,0) for variable in self.nonbasic]))
+            if verbose > 0: print(str(var) + ' = ' + str(solution[var]))
+        for var in self.nonbasic:
+            solution[var] = 0.0
+            if verbose > 1: print(str(var) + ' = ' + str(solution[var]))
+        return solution
 
     def determine_entering(self):
         self.nonbasic.sort(key=str) # Bland's rule
         for entering_var in self.nonbasic:
             if diff(self.base[Symbol('obj')],entering_var)>0 :
                 return entering_var
         return None # If no entering variable found, None returned
@@ -123,40 +121,40 @@
                 print('Unbounded solution.')
             else:
                 expr_entering_var = dual_tableau.pivot(entering_var,departing_var, verbose= 1)
                 _ = primal_tableau.pivot(primals[departing_var],primals[entering_var])
                 return False # not finished
         return True # finished
 
-def plot_path_so_far(the_path):
-    if self.A_i_j.shape[1] != 2:
-        print('Can\'t plot the solution in 2D, the number primal variables differs from two.')
-        return()
-    x1, x2 = np.meshgrid(np.linspace(-0.2, 1.4, 400), np.linspace(-0.2, 1.4, 400))
-    feasible_region = (x1 >= 0) & (x2 >= 0)
-    for i in range(len(self.bi)):
-        feasible_region = feasible_region & ( self.A_i_j[i,0]*x1 + self.A_i_j[i,1]*x2 <= self.b_i[i]  )
-    fig, ax = plt.subplots(figsize=(5, 5))
-    plt.contourf(x1, x2, np.where(feasible_region, self.c_j[0]*x1+self.c_j[1]*x2, np.nan), 50, alpha = 0.5, cmap='gray_r', levels=30)
-    plt.text(0.4, 0.4, 'Feasible solutions', color = 'white', ha='center', va='center')
-    for i in range(len(self.bi)):
-        ax.plot(x1[0, :], self.b_i[i] / self.A_i_j[i,1] - (self.A_i_j[i,0]/self.A_i_j[i,1])*x1[0, :], label='s'+str(i)+ ' = 0')
-    ax.plot([a for (a,_) in the_path], [b for (_,b) in the_path], 'r--', label='Algorithm path')
-    ax.scatter([a for (a,_) in the_path], [b for (_,b) in the_path], color='red')
-    for i, bfs in enumerate(the_path):
-        plt.text(bfs[0], bfs[1], 'BFS'+str(i), color = 'red', ha='left', va='bottom')
-    ax.set_xlim(-0.2, 1.4), ax.set_ylim(-0.2, 1.4)
-    ax.set_xlabel('x1'), ax.set_ylabel('x2')
-    ax.spines['left'].set_position('zero')
-    ax.spines['bottom'].set_position('zero')
-    ax.spines['right'].set_color('none')
-    ax.spines['top'].set_color('none')
-    ax.legend()
-    plt.show()
-
+    def Tableau_plot_path_so_far(self, the_path, legend=True):
+        if self.A_i_j.shape[1] != 2:
+            print('Can\'t plot the solution in 2D, the number of primal variables differs from two.')
+            return()
+
+        x1max = min(x for x in self.b_i / self.A_i_j[:,0] if x >= 0)
+        x2max = min(x for x in self.b_i / self.A_i_j[:,1] if x >= 0)
+        x1, x2 = np.meshgrid(np.linspace(-.2*x1max, 1.4*x1max, 400), np.linspace(-.2*x2max, 1.4*x2max, 400))
+        feasible_region = (x1 >= 0) & (x2 >= 0)
+        for i in range(len(self.b_i)) :
+            feasible_region = feasible_region & (self.A_i_j[i,0] * x1 + self.A_i_j[i,1] * x2 <= self.b_i[i])
+        fig, ax = plt.subplots(figsize=(5, 5))
+        plt.contourf(x1, x2, np.where(feasible_region, self.c_j[0]*x1+self.c_j[1]*x2, np.nan), 50, alpha = 0.5, cmap='gray_r', levels=30)
+        for i in range(len(self.b_i)):
+            if not self.A_i_j[i,1] == 0:
+                ax.plot(x1[0, :], self.b_i[i]/self.A_i_j[i,1] - self.A_i_j[i,0]/self.A_i_j[i,1]*x1[0, :], label='z'+str(i+1)+' = 0')
+            else:
+                ax.axvline(self.b_i[i]/self.A_i_j[i,0], label='z'+str(i+1)+' = 0')
+        ax.plot([a for (a,_) in the_path], [b for (_,b) in the_path], 'r--', label='Algorithm path')
+        ax.scatter([a for (a,_) in the_path], [b for (_,b) in the_path], color='red')
+        ax.set_xlim(-.2*x1max, 1.4*x1max), ax.set_ylim(-.2*x2max, 1.4*x2max)
+        ax.set_xlabel('x1'), ax.set_ylabel('x2')
+        ax.spines[ 'left' ].set_position('zero'), ax.spines['bottom'].set_position('zero')
+        ax.spines['right'].set_color('none'), ax.spines['top'].set_color('none')
+        if legend: ax.legend(loc='upper right')
+        plt.show()
         
 #########################
 # LP3: Interior Point Methods #
 #########################
 
 class InteriorPoint():
     def __init__(self,A,b,c,current_point=None):
```

