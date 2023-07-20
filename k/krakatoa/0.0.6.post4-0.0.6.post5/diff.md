# Comparing `tmp/krakatoa-0.0.6.post4.tar.gz` & `tmp/krakatoa-0.0.6.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakatoa-0.0.6.post4.tar", last modified: Mon Jul 17 19:55:56 2023, max compression
+gzip compressed data, was "krakatoa-0.0.6.post5.tar", last modified: Thu Jul 20 14:33:39 2023, max compression
```

## Comparing `krakatoa-0.0.6.post4.tar` & `krakatoa-0.0.6.post5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:56.295020 krakatoa-0.0.6.post4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-17 19:55:56.295020 krakatoa-0.0.6.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:56.291019 krakatoa-0.0.6.post4/krakatoa/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:56.291019 krakatoa-0.0.6.post4/krakatoa/future/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/future/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/future/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/future/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/future/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/future/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:56.295020 krakatoa-0.0.6.post4/krakatoa/models/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/models/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/models/_getmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/models/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/models/autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/krakatoa/models/quick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:56.291019 krakatoa-0.0.6.post4/krakatoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-17 19:55:56.000000 krakatoa-0.0.6.post4/krakatoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-17 19:55:56.000000 krakatoa-0.0.6.post4/krakatoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:55:56.000000 krakatoa-0.0.6.post4/krakatoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 19:55:56.000000 krakatoa-0.0.6.post4/krakatoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 19:55:56.000000 krakatoa-0.0.6.post4/krakatoa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 19:55:56.295020 krakatoa-0.0.6.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-17 19:55:42.000000 krakatoa-0.0.6.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.480266 krakatoa-0.0.6.post5/krakatoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/krakatoa/future/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/krakatoa/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/_getmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/autotune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/quick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.480266 krakatoa-0.0.6.post5/krakatoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/setup.py
```

### Comparing `krakatoa-0.0.6.post4/LICENSE` & `krakatoa-0.0.6.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/PKG-INFO` & `krakatoa-0.0.6.post5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6.post4
+Version: 0.0.6.post5
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post4.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post5.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6.post4/krakatoa/future/analysis.py` & `krakatoa-0.0.6.post5/krakatoa/future/analysis.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/krakatoa/future/evaluate.py` & `krakatoa-0.0.6.post5/krakatoa/future/evaluate.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/krakatoa/future/experiment.py` & `krakatoa-0.0.6.post5/krakatoa/future/experiment.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/krakatoa/future/preprocess.py` & `krakatoa-0.0.6.post5/krakatoa/future/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder, LabelEncoder
 
 #============================================================
 def changeColType(df, columns, newType):
     
     for col in columns:
         df[col] = df[col].astype(newType)
-        
+    
+
     return df
 
 def splitDataset(x, y, test_size=0.3, random_state=0):
     x_train, x_test, y_train, y_test = train_test_split(x, 
                                                         y, 
                                                         test_size=test_size, 
                                                         random_state=random_state)
@@ -194,21 +195,24 @@
         self.catUniquePerc = catUniquePerc
         self.uniqueCount = uniqueCount
         self.uniquePerc = uniquePerc
 
     def dropColumns(self, columns):
 
         self.dataset.drop(columns=columns, inplace=True)
+        self.getColType()
         return self.dataset
     
     def dropNaColumns(self, threshold=50):
         
         percNull = self._nullPercFeatures()
 
         self.dataset.drop(columns=list(percNull[percNull > threshold].keys()), inplace=True)
+        self.getColType()
+
         return self.dataset
     
     def fillNa(self, strategy='mean'): #mean / most frequent | drop 
         # preencher com media | mais frequente (caso categorico)
         self.getColType()
         dataset = self.dataset.copy()
         if strategy == "mean":
@@ -237,51 +241,50 @@
         # Dont drop target column for any reason | Dont drop numeric columns
         col_drop = [x for x in col_drop if x != self.target and x not in (self.numeric_cols)] 
 
         dataset.drop(columns=col_drop, inplace=True)
 
         self.dataset = dataset
 
-
         # refresh column data in self
         self.getColType()
 
         return self.dataset
 
     def encodeColumns(self, columns: list, encoder='one_hot_encoder'):
         
         for col in columns:
 
             res_encoder = encode(self.dataset, column=col, encoder=encoder)
 
         self.dataset = res_encoder["dataset"]
         self.encoder = res_encoder["encoder"]
 
-        return self.dataset
-    
+        return self.dataset   
 
-    def getDummies(self):
+    def getDummies(self, columns = None):
 
         # self.dataset = pd.get_dummies(self.dataset)
         # return self.dataset
         self.dataset.reset_index(inplace=True, drop=True)
 
-        cat_cols = self.category_cols
-
         # Instancia e fit one hot encoder
         hot = OneHotEncoder(handle_unknown='ignore', sparse=False)
-        hot.fit(self.dataset[cat_cols])
 
-        hot_ds = hot.transform(self.dataset[cat_cols])
+        if columns is None:
+            columns = self.category_cols        
+
+        hot.fit(self.dataset[columns])
+        hot_ds = hot.transform(self.dataset[columns])
 
         # Cria dataframe transformada
-        hot_df = pd.DataFrame(hot_ds, columns = hot.get_feature_names_out(input_features=cat_cols))
+        hot_df = pd.DataFrame(hot_ds, columns = hot.get_feature_names_out(input_features=columns))
 
         # Concatena o dataframe do one hot com o original
-        concat_df = pd.concat([self.dataset, hot_df], axis=1).drop(columns=cat_cols, axis=1)
+        concat_df = pd.concat([self.dataset, hot_df], axis=1).drop(columns=columns, axis=1)
         self.oneHotEncoding = hot
         self.dataset = concat_df
 
         return self.dataset
 
     def scaleColumns(self, columns: list, scaler: str='min_max', **kwargs):
```

### Comparing `krakatoa-0.0.6.post4/krakatoa/models/_config.py` & `krakatoa-0.0.6.post5/krakatoa/models/_config.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/krakatoa/models/_getmodels.py` & `krakatoa-0.0.6.post5/krakatoa/models/_getmodels.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/krakatoa/models/_metrics.py` & `krakatoa-0.0.6.post5/krakatoa/models/_metrics.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/krakatoa/models/autotune.py` & `krakatoa-0.0.6.post5/krakatoa/models/autotune.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/krakatoa/models/quick.py` & `krakatoa-0.0.6.post5/krakatoa/models/quick.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/krakatoa.egg-info/PKG-INFO` & `krakatoa-0.0.6.post5/krakatoa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6.post4
+Version: 0.0.6.post5
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post4.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post5.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6.post4/krakatoa.egg-info/SOURCES.txt` & `krakatoa-0.0.6.post5/krakatoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post4/setup.py` & `krakatoa-0.0.6.post5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
   name = 'krakatoa',       
   packages = ['krakatoa', 'krakatoa/models', 'krakatoa/future'],  
-  version = '0.0.6post4',      
+  version = '0.0.6post5',      
   license='MIT',        
   description = 'Machine Learning high level package.',  
   long_description='Machine Learning high level package.',  
   author = 'Matheus de Prá Andrade',              
   author_email = 'mpandrade@ucs.br',    
   url = 'https://github.com/aitec-mp/krakatoa',  
-  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post4.tar.gz',    
+  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post5.tar.gz',    
   keywords = ['krakatoa', 'machine learning'],  
   install_requires=[    
           'scikit-learn',
           'numpy',
           'pandas',
           'xgboost',
           'seaborn'
```

