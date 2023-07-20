# Comparing `tmp/pabutools-0.8.tar.gz` & `tmp/pabutools-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pabutools-0.8.tar", last modified: Tue Jan 17 12:03:28 2023, max compression
+gzip compressed data, was "pabutools-0.9.tar", last modified: Wed Mar  1 18:57:25 2023, max compression
```

## Comparing `pabutools-0.8.tar` & `pabutools-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-01-17 12:03:28.090744 pabutools-0.8/
--rw-r--r--   0 grzegorz   (501) staff       (20)     1078 2022-11-25 13:52:47.000000 pabutools-0.8/LICENSE.txt
--rw-r--r--   0 grzegorz   (501) staff       (20)     3425 2023-01-17 12:03:28.090411 pabutools-0.8/PKG-INFO
--rw-r--r--   0 grzegorz   (501) staff       (20)     3131 2023-01-17 12:01:00.000000 pabutools-0.8/README.md
-drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-01-17 12:03:28.087990 pabutools-0.8/pabutools/
--rw-r--r--   0 grzegorz   (501) staff       (20)        1 2022-11-25 13:42:45.000000 pabutools-0.8/pabutools/__init__.py
--rw-r--r--   0 grzegorz   (501) staff       (20)     4988 2023-01-03 08:14:24.000000 pabutools-0.8/pabutools/model.py
--rw-r--r--   0 grzegorz   (501) staff       (20)     6352 2023-01-17 11:59:18.000000 pabutools-0.8/pabutools/rules.py
-drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-01-17 12:03:28.089922 pabutools-0.8/pabutools.egg-info/
--rw-r--r--   0 grzegorz   (501) staff       (20)     3425 2023-01-17 12:03:28.000000 pabutools-0.8/pabutools.egg-info/PKG-INFO
--rw-r--r--   0 grzegorz   (501) staff       (20)      254 2023-01-17 12:03:28.000000 pabutools-0.8/pabutools.egg-info/SOURCES.txt
--rw-r--r--   0 grzegorz   (501) staff       (20)        1 2023-01-17 12:03:28.000000 pabutools-0.8/pabutools.egg-info/dependency_links.txt
--rw-r--r--   0 grzegorz   (501) staff       (20)        1 2023-01-17 12:03:28.000000 pabutools-0.8/pabutools.egg-info/not-zip-safe
--rw-r--r--   0 grzegorz   (501) staff       (20)       10 2023-01-17 12:03:28.000000 pabutools-0.8/pabutools.egg-info/top_level.txt
--rw-r--r--   0 grzegorz   (501) staff       (20)       38 2023-01-17 12:03:28.090876 pabutools-0.8/setup.cfg
--rw-rw-r--   0 grzegorz   (501) staff       (20)      479 2023-01-17 12:00:05.000000 pabutools-0.8/setup.py
+drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-03-01 18:57:25.053669 pabutools-0.9/
+-rw-r--r--   0 grzegorz   (501) staff       (20)     1078 2022-11-25 13:52:47.000000 pabutools-0.9/LICENSE.txt
+-rw-r--r--   0 grzegorz   (501) staff       (20)     3575 2023-03-01 18:57:25.053310 pabutools-0.9/PKG-INFO
+-rw-r--r--   0 grzegorz   (501) staff       (20)     3337 2023-03-01 18:56:58.000000 pabutools-0.9/README.md
+drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-03-01 18:57:25.050817 pabutools-0.9/pabutools/
+-rw-r--r--   0 grzegorz   (501) staff       (20)        1 2022-11-25 13:42:45.000000 pabutools-0.9/pabutools/__init__.py
+-rw-r--r--   0 grzegorz   (501) staff       (20)     5197 2023-03-01 18:53:29.000000 pabutools-0.9/pabutools/model.py
+-rw-r--r--   0 grzegorz   (501) staff       (20)     6352 2023-01-17 11:59:18.000000 pabutools-0.9/pabutools/rules.py
+drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-03-01 18:57:25.052844 pabutools-0.9/pabutools.egg-info/
+-rw-r--r--   0 grzegorz   (501) staff       (20)     3575 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/PKG-INFO
+-rw-r--r--   0 grzegorz   (501) staff       (20)      254 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/SOURCES.txt
+-rw-r--r--   0 grzegorz   (501) staff       (20)        1 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/dependency_links.txt
+-rw-r--r--   0 grzegorz   (501) staff       (20)        1 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/not-zip-safe
+-rw-r--r--   0 grzegorz   (501) staff       (20)       10 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/top_level.txt
+-rw-r--r--   0 grzegorz   (501) staff       (20)       38 2023-03-01 18:57:25.053787 pabutools-0.9/setup.cfg
+-rw-rw-r--   0 grzegorz   (501) staff       (20)      479 2023-03-01 18:55:41.000000 pabutools-0.9/setup.py
```

### Comparing `pabutools-0.8/LICENSE.txt` & `pabutools-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pabutools-0.8/PKG-INFO` & `pabutools-0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pabutools
-Version: 0.8
-Summary: Implementation of PB voting rules and tools for reading Pabulib datasets
-Home-page: UNKNOWN
-Author-email: g.pierczynski@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # pabutools---tools for participatory budgeting
 
 Pabutools provides two submodules: **model** and **rules**.
  ## model
  Provides the classes representing voters, candidates and election instances.
   - **Voter(id, sex=None, age=None, subunits=set())** with the following attributes:
 	- id: unique ID of the voter,
@@ -27,23 +16,24 @@
   - **Election(name=None, voters=None, profile=None, budget=0, subunits = None)** with the following attributes:
 	- voters: a set of Voter instances,
 	- profile: a dict where keys are Candidate instances and values are dicts in which keys are Voter instances and values are natural numbers (voters' utilities over candidates; if a voter has utility 0, she can be skipped),
 	- budget: a natural number,
 	- subunits: a set of strings (subunits within the instance).
 
 	and the following methods:
-	- read_from_file(pattern): takes as an input the pattern of the filepaths of Pabulib files and fills the data of the newly created Election instance with them (e.g. calling Election().read_from_files('pabulib/poland_warszawa_2021*') will create a PB election out of all Pabulib files under the provided path starting with 'poland_warszawa_2021'). If the pattern fits more than one file, they should all be from the same country, unit and year. By default, approval utilities are considered to be binary.
+	- read_from_files(pattern): takes as an input the pattern of the filepaths of Pabulib files and fills the data of the newly created Election instance with them (e.g. calling Election().read_from_files('pabulib/poland_warszawa_2021*') will create a PB election out of all Pabulib files under the provided path starting with 'poland_warszawa_2021'). If the pattern fits more than one file, they should all be from the same country, unit and year. By default, approval utilities are considered to be binary.
 	- cost_to_binary_utilities(): if the utilities are cost utilities, they are converted to binary
 	- binary_to_cost_utilities(): if the utilities are binary, they are converted to cost utilities
+    - cost_to_score_utilities(): if the utilities are cost utilities, they are converted to score utilities
+	- score_to_cost_utilities(): if the utilities are score utilities, they are converted to cost utilities
+
  ## rules
 Provides the implementation of a number of voting rules for PB. All the methods take as an argument an election instance and return a set of elected candidates.
  - **utilitarian_greedy(e : Election)**: the simple greedy algorithm,
  - **phragmen(e : Election)**: the Phragmen's Sequential Method,
  - **equal_shares(e : Election, completion=None)**: the method of equal shares. The 'completion' parameter can take the following values:
 	 - None: no completion (default option).
 	 - 'binsearch': initial endowments of the voters are set to maximize the exhaustiveness of the elected committee with the use of binary search.
 	 - 'add1': initial endowments of the voters are increased similarly as above so that the committee is as exhaustive as possible; instead of using binary search, we keep increasing voters' endowments by 1 unit until the outcome is exhaustive or we exceed the original budget.
-           - 'add1_utilitarian': similarly as in add1 completion, but if the outcome is still not exhaustive, it is completed by utilitarian greedy.
+	 - 'add1_utilitarian': similarly as in add1 completion, but if the outcome is still not exhaustive, it is completed by utilitarian greedy.
 	 - 'utilitarian_greedy': the completion with utilitarian_greedy.
 	 - 'phragmen': the completion with the Phragmen's Sequential Method.
-
-
```

### Comparing `pabutools-0.8/README.md` & `pabutools-0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: pabutools
+Version: 0.9
+Summary: Implementation of PB voting rules and tools for reading Pabulib datasets
+Author-email: g.pierczynski@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # pabutools---tools for participatory budgeting
 
 Pabutools provides two submodules: **model** and **rules**.
  ## model
  Provides the classes representing voters, candidates and election instances.
   - **Voter(id, sex=None, age=None, subunits=set())** with the following attributes:
 	- id: unique ID of the voter,
@@ -16,21 +24,24 @@
   - **Election(name=None, voters=None, profile=None, budget=0, subunits = None)** with the following attributes:
 	- voters: a set of Voter instances,
 	- profile: a dict where keys are Candidate instances and values are dicts in which keys are Voter instances and values are natural numbers (voters' utilities over candidates; if a voter has utility 0, she can be skipped),
 	- budget: a natural number,
 	- subunits: a set of strings (subunits within the instance).
 
 	and the following methods:
-	- read_from_file(pattern): takes as an input the pattern of the filepaths of Pabulib files and fills the data of the newly created Election instance with them (e.g. calling Election().read_from_files('pabulib/poland_warszawa_2021*') will create a PB election out of all Pabulib files under the provided path starting with 'poland_warszawa_2021'). If the pattern fits more than one file, they should all be from the same country, unit and year. By default, approval utilities are considered to be binary.
+	- read_from_files(pattern): takes as an input the pattern of the filepaths of Pabulib files and fills the data of the newly created Election instance with them (e.g. calling Election().read_from_files('pabulib/poland_warszawa_2021*') will create a PB election out of all Pabulib files under the provided path starting with 'poland_warszawa_2021'). If the pattern fits more than one file, they should all be from the same country, unit and year. By default, approval utilities are considered to be binary.
 	- cost_to_binary_utilities(): if the utilities are cost utilities, they are converted to binary
 	- binary_to_cost_utilities(): if the utilities are binary, they are converted to cost utilities
+    - cost_to_score_utilities(): if the utilities are cost utilities, they are converted to score utilities
+	- score_to_cost_utilities(): if the utilities are score utilities, they are converted to cost utilities
+
  ## rules
 Provides the implementation of a number of voting rules for PB. All the methods take as an argument an election instance and return a set of elected candidates.
  - **utilitarian_greedy(e : Election)**: the simple greedy algorithm,
  - **phragmen(e : Election)**: the Phragmen's Sequential Method,
  - **equal_shares(e : Election, completion=None)**: the method of equal shares. The 'completion' parameter can take the following values:
 	 - None: no completion (default option).
 	 - 'binsearch': initial endowments of the voters are set to maximize the exhaustiveness of the elected committee with the use of binary search.
 	 - 'add1': initial endowments of the voters are increased similarly as above so that the committee is as exhaustive as possible; instead of using binary search, we keep increasing voters' endowments by 1 unit until the outcome is exhaustive or we exceed the original budget.
-           - 'add1_utilitarian': similarly as in add1 completion, but if the outcome is still not exhaustive, it is completed by utilitarian greedy.
+	 - 'add1_utilitarian': similarly as in add1 completion, but if the outcome is still not exhaustive, it is completed by utilitarian greedy.
 	 - 'utilitarian_greedy': the completion with utilitarian_greedy.
 	 - 'phragmen': the completion with the Phragmen's Sequential Method.
```

### Comparing `pabutools-0.8/pabutools/model.py` & `pabutools-0.9/pabutools/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,24 +56,30 @@
         self.voters = voters if voters else set()
         self.profile = profile if profile else {} #dict: candidates -> voters -> score
         self.budget = budget
         self.subunits = subunits if subunits else set()
 
     def binary_to_cost_utilities(self) -> Election:
         assert all((self.profile[c][v] == 1) for c in self.profile for v in self.profile[c])
+        return self.score_to_cost_utilities()
+
+    def cost_to_binary_utilities(self) -> Election:
+        assert all((self.profile[c][v] == c.cost) for c in self.profile for v in self.profile[c])
+        return self.cost_to_score_utilities()
+
+    def score_to_cost_utilities(self) -> Election:
         for c in self.profile:
             for v in self.profile[c]:
-                self.profile[c][v] = c.cost
+                self.profile[c][v] *= c.cost
         return self
 
-    def cost_to_binary_utilities(self) -> Election:
-        assert all((self.profile[c][v] == c.cost) for c in self.profile for v in self.profile[c])
+    def cost_to_score_utilities(self) -> Election:
         for c in self.profile:
             for v in self.profile[c]:
-                self.profile[c][v] = 1
+                self.profile[c][v] /= c.cost * 1.0
         return self
 
     def read_from_files(self, pattern : str): #assumes Pabulib data format
         for filename in Path(".").glob(pattern):
             cand_id_to_obj = {}
             with open(filename, 'r', newline='', encoding="utf-8") as csvfile:
                 section = ""
```

### Comparing `pabutools-0.8/pabutools/rules.py` & `pabutools-0.9/pabutools/rules.py`

 * *Files identical despite different names*

### Comparing `pabutools-0.8/pabutools.egg-info/PKG-INFO` & `pabutools-0.9/pabutools.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: pabutools
-Version: 0.8
+Version: 0.9
 Summary: Implementation of PB voting rules and tools for reading Pabulib datasets
-Home-page: UNKNOWN
 Author-email: g.pierczynski@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pabutools---tools for participatory budgeting
 
 Pabutools provides two submodules: **model** and **rules**.
  ## model
@@ -27,23 +24,24 @@
   - **Election(name=None, voters=None, profile=None, budget=0, subunits = None)** with the following attributes:
 	- voters: a set of Voter instances,
 	- profile: a dict where keys are Candidate instances and values are dicts in which keys are Voter instances and values are natural numbers (voters' utilities over candidates; if a voter has utility 0, she can be skipped),
 	- budget: a natural number,
 	- subunits: a set of strings (subunits within the instance).
 
 	and the following methods:
-	- read_from_file(pattern): takes as an input the pattern of the filepaths of Pabulib files and fills the data of the newly created Election instance with them (e.g. calling Election().read_from_files('pabulib/poland_warszawa_2021*') will create a PB election out of all Pabulib files under the provided path starting with 'poland_warszawa_2021'). If the pattern fits more than one file, they should all be from the same country, unit and year. By default, approval utilities are considered to be binary.
+	- read_from_files(pattern): takes as an input the pattern of the filepaths of Pabulib files and fills the data of the newly created Election instance with them (e.g. calling Election().read_from_files('pabulib/poland_warszawa_2021*') will create a PB election out of all Pabulib files under the provided path starting with 'poland_warszawa_2021'). If the pattern fits more than one file, they should all be from the same country, unit and year. By default, approval utilities are considered to be binary.
 	- cost_to_binary_utilities(): if the utilities are cost utilities, they are converted to binary
 	- binary_to_cost_utilities(): if the utilities are binary, they are converted to cost utilities
+    - cost_to_score_utilities(): if the utilities are cost utilities, they are converted to score utilities
+	- score_to_cost_utilities(): if the utilities are score utilities, they are converted to cost utilities
+
  ## rules
 Provides the implementation of a number of voting rules for PB. All the methods take as an argument an election instance and return a set of elected candidates.
  - **utilitarian_greedy(e : Election)**: the simple greedy algorithm,
  - **phragmen(e : Election)**: the Phragmen's Sequential Method,
  - **equal_shares(e : Election, completion=None)**: the method of equal shares. The 'completion' parameter can take the following values:
 	 - None: no completion (default option).
 	 - 'binsearch': initial endowments of the voters are set to maximize the exhaustiveness of the elected committee with the use of binary search.
 	 - 'add1': initial endowments of the voters are increased similarly as above so that the committee is as exhaustive as possible; instead of using binary search, we keep increasing voters' endowments by 1 unit until the outcome is exhaustive or we exceed the original budget.
-           - 'add1_utilitarian': similarly as in add1 completion, but if the outcome is still not exhaustive, it is completed by utilitarian greedy.
+	 - 'add1_utilitarian': similarly as in add1 completion, but if the outcome is still not exhaustive, it is completed by utilitarian greedy.
 	 - 'utilitarian_greedy': the completion with utilitarian_greedy.
 	 - 'phragmen': the completion with the Phragmen's Sequential Method.
-
-
```

