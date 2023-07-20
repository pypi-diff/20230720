# Comparing `tmp/toypandas-0.1.1.tar.gz` & `tmp/toypandas-0.2.0.tar.gz`

## Comparing `toypandas-0.1.1.tar` & `toypandas-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,20 @@
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 toypandas-0.1.1/Makefile
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 toypandas-0.1.1/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/Makefile
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/make.bat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/requirements.txt
--rw-r--r--   0        0        0  2504919 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/index.doctree
--rw-r--r--   0        0        0    18039 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/toypandas/index.doctree
--rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/toypandas/dataframe/index.doctree
--rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/toypandas/locating/index.doctree
--rw-r--r--   0        0        0    36717 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/doctrees/autoapi/toypandas/series/index.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/index.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/search.html
--rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/index.rst.txt
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/toypandas/index.rst.txt
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/toypandas/dataframe/index.rst.txt
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/toypandas/locating/index.rst.txt
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_sources/autoapi/toypandas/series/index.rst.txt
--rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/graphviz.css
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/index.html
--rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/toypandas/index.html
--rw-r--r--   0        0        0    17261 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/toypandas/dataframe/index.html
--rw-r--r--   0        0        0     6486 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/toypandas/locating/index.html
--rw-r--r--   0        0        0    16913 2020-02-02 00:00:00.000000 toypandas-0.1.1/docs/_build/html/autoapi/toypandas/series/index.html
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 toypandas-0.1.1/src/toypandas/__init__.py
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 toypandas-0.1.1/src/toypandas/dataframe.py
--rw-r--r--   0        0        0     5767 2020-02-02 00:00:00.000000 toypandas-0.1.1/src/toypandas/series.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toypandas-0.1.1/LICENSE
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 toypandas-0.1.1/README.md
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 toypandas-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 toypandas-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 toypandas-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 toypandas-0.2.0/Makefile
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 toypandas-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 toypandas-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 toypandas-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 toypandas-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 toypandas-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 toypandas-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 toypandas-0.2.0/src/toypandas/__init__.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 toypandas-0.2.0/src/toypandas/dataframe.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 toypandas-0.2.0/src/toypandas/series.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toypandas-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 toypandas-0.2.0/tests/data.csv
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 toypandas-0.2.0/tests/test_01_series.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 toypandas-0.2.0/tests/test_02_dataframe.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 toypandas-0.2.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toypandas-0.2.0/LICENSE
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 toypandas-0.2.0/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 toypandas-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 toypandas-0.2.0/PKG-INFO
```

### Comparing `toypandas-0.1.1/Makefile` & `toypandas-0.2.0/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,39 @@
+# Makefile by Davide Ponzini
+
 NAME=toypandas
 PY=python3
 
 
+prepare: test documentation
+	:
+
 install: uninstall build
-	sudo $(PY) -m pip install ./dist/*.whl
+	$(PY) -m pip install ./dist/*.whl
 
 build:
-	$(PY) -m pip install pipreqs
-	pipreqs --force
-	sudo $(PY) -m pip install --upgrade -r requirements.txt
 	sudo rm -rf dist/
-	$(PY) -m pip install build
 	$(PY) -m build
 
 uninstall:
-	sudo $(PY) -m pip uninstall -y $(NAME)
+	$(PY) -m pip uninstall -y $(NAME)
 
-### Documentation ###
 documentation:
-	$(PY) -m pip install autoapi
 	make html -C docs/
 
+test: install
+	pytest
+
+requirements.txt:
+	$(PY) -m pip install pipreqs
+	pipreqs --mode no-pin --force
+
+required-packages: requirements.txt
+	$(PY) -m pip install --upgrade build autoapi pytest -r requirements.txt
 
-### PyPi ###
-upload: build documentation
+upload: prepare
 	$(PY) -m pip install --upgrade twine
 	$(PY) -m twine upload --verbose dist/*
 
 download: uninstall
-	sudo $(PY) -m pip install $(NAME)
-
-
-### TestPyPi ###
-download-test: uninstall
-	$(PY) -m pip install --index-url https://test.pypi.org/simple/ --no-deps $(NAME)
-
-upload-test: build
-	$(PY) -m pip install --upgrade twine
-	$(PY) -m twine upload --repository testpypi dist/*
+	$(PY) -m pip install $(NAME)
```

### Comparing `toypandas-0.1.1/docs/Makefile` & `toypandas-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `toypandas-0.1.1/docs/conf.py` & `toypandas-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `toypandas-0.1.1/docs/make.bat` & `toypandas-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `toypandas-0.1.1/src/toypandas/dataframe.py` & `toypandas-0.2.0/src/toypandas/series.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,233 +1,204 @@
-'''Descrizione modulo'''
+'''Descizione modulo'''
 
 from __future__ import annotations
 
 import pandas as pd
 
-from .series import Series
-from . import concat_df
 
+class Series(pd.core.series.Series):
+    '''Represenation of a series of values (usually a column).'''
+    
+    def __init__(self, *args):
+        '''
+        Initialize a Series with the given values.
 
-class Dataframe(pd.core.frame.DataFrame):
-    '''Descrizione classe'''
+        :param args: Individual values or already existing Series.
+        '''
 
-    def __init__(self, *args):
+        if(len(args) == 0):
+            super().__init__()
+        elif (isinstance(args[0], pd.core.series.Series)): 
+            super().__init__(args[0])
+        else:
+            super().__init__(args)
+
+    def __add__(self, other) -> Series:
         '''
-        asdflkjs
+        Sums two series row by row.
         
-        :param args: asdfas
+        :param other: The other series to sum.
+        
+        :returns: A new series in which each value is the sum of the two rows.
         '''
 
-        super().__init__(*args)
+        return Series(super().__add__(other))
         
-    @property
-    def indexlocate(self) -> Locating:
+    def __getitem__(self, match: pd.core.series.Series) -> Series:
         '''
-        adshf
-
-        :returns: adskfh
+        Returns only the rows matching the argument.
+        
+        :param match: A Series of booleans (True/False). If an element is True, it will be returned.  
+        
+        :returns: A new Series with only the elements matching the argument.
         '''
 
-        return Locating(self)
+        result = super().__getitem__(match)
+        result.reset_index(drop=True, inplace=True)
+        return Series(result)
 
-    def show(self) -> Dataframe:
+    @property
+    def indexlocate(self) -> Locating_s:
         '''
-        alkjdfk - ma sta funzione fa qualcosa?
+        Locate an element by index.
 
-        :returns: sdlkfj
+        :returns: The element.
         '''
 
-        return self
- 
-    def __getitem__(self, *args) -> Series | Dataframe:
-        '''
-        adfag
-        
-        :param args:
+        return Locating_s(self)
 
-        :returns: asdfsaf
+    def apply(self, function) -> Series:
         '''
+        Apply a function of each value of the Series.
 
-        if ((type(args) == tuple) and (type(args[0]) == str)):
-            return Series(super().__getitem__(args[0]))
-        
-        elif ((type(args) == tuple) and (type(args[0]) == int)):
-            return Series(super().__getitem__(args[0]))
+        :param function: Function to apply to each element.
 
-        elif ((type(args) == tuple) and (type(args[0]) == float)):
-            return Series(super().__getitem__(args[0]))
-        
-        elif (type(args) == tuple and type(args[0]) == tuple):
-            d = Dataframe()
-            list_col = list()
-            for elem in args[0]:
-                s = Series(super().__getitem__(elem))
-                list_col.append(s)
-            tuple_col = tuple(list_col)
-            d = concat_df(tuple_col)
-            return d
-     
-        elif (isinstance(args[0], pd.core.series.Series)):
-            temp = super().__getitem__(args[0])
-            temp.reset_index(drop=True, inplace=True)
-            return Dataframe(temp)
-
-    # semplificazione: se aggiungo riga + lunga, perdo dati aggiuntivi, se + corta mette dei nan
-    # one row (series), more rows (dataframe: you can also use concat())
-    def append(self, obj):
-        '''
-        sadsdf
-
-        :param obj: sadfasf
-        '''
-
-        if(not(isinstance(obj, Series)) and not(isinstance(obj,Dataframe))):
-            raise TypeError("Can only add series or dataframe")
-
-        elif(isinstance(obj, Series)):
-            #obj.name = len(self.index)
-            #pd.concat([obj,self.loc[:]]).reset_index(drop=True)
-            #self.__init__(super().append(obj, ignore_index=True)) #append
-            s = Series()
-            for v, n in zip(obj.values, self.columns):
-                s.loc[n] = v
-            s.name = len(self.index)
-            self.__init__(super().append(s, ignore_index=True))
-            
-            #self.__init__(super().append(obj, ignore_index=False))
-            #return self
-            #temp.reset_index(drop=True, inplace=True)
-            #self.loc[len(self.index)] = obj
-        elif(isinstance(obj, Dataframe)):
-            for k,r in obj.iterrows():
-                self.loc[len(self.index)] = r
-            #return dataframe(self)
-        
-    def drop(self, item):
-        '''
-        sadfasfs
-        
-        :param item: dfasf
+        :returns: The resulting Series.
         '''
 
-        if(isinstance(item, int)):
-            super().drop(item, inplace=True)
-            self.reset_index(drop=True, inplace=True)
-        elif(isinstance(item, str)):
-            super().drop(item, inplace=True, axis=1)
+        aux = Series(super().apply(function))
+        return aux
 
-    def dropna(self, **kargs) -> Series | Dataframe:
+    def append(self, elem):
         '''
-        kjasdf
+        Appends a value at the end of the Series.
 
-        :param kwargs: asdfjkh
-
-        :returns: asdkfh
+        :param elem: The value to append.
         '''
 
-        if (len(kargs) > 1):
-            raise Exception("Error. Axis must be 0 or 1 (row or column).")    
-        elif ((kargs == {}) or (next(iter(kargs.keys())) == "axis" and next(iter(kargs.values())) == 0)):
-            temp = super().dropna()
-            if (len(temp.index) == 1):
-                return Series(temp)
-            else:
-                return Dataframe(temp)
-
-        elif (next(iter(kargs.keys())) == "axis" and next(iter(kargs.values())) == 1):
-            temp = super().dropna(axis=1)
-            if (len(temp.index) == 1):
-                return Series(temp)
-            else:
-                return Dataframe(temp)
-        else:
-            raise ValueError("The axis value must be 0 or 1 (row or column respectively)")     
+        if(len(self) <= 1):
+            self.astype(type(elem))
+        self.loc[len(self)] = elem
 
-    def drop_duplicates(self) -> Series | Dataframe:
+    def drop(self, index=None):
         '''
-        asfasbjkasd
-        
-        :returns: askfjsalj
+        Removes a given element from the Series.
+
+        :param elem: The index of the element to remove. If not specified, remove the last element.
         '''
 
-        #temp = super().drop_duplicates(inplace=True)
-        self = super().drop_duplicates()
-        if (len(self.index) == 1):
-            return Series(self)
-        else:
-            return Dataframe(self)
+        if (index is None):
+            size = self.size - 1
+            super().drop(size, inplace=True) 
+            self.reset_index(drop=True, inplace=True)
+            return
 
-    def isnull(self) -> Dataframe:
-        '''
-        asdlkfhasd
+        try:
+            super().drop(index, inplace=True)
+            self.reset_index(drop=True, inplace=True)
+        except KeyError:
+            print("Index might not exist")
 
-        :returns: asdfkjl
+    def astype(self, dtype) -> Series:
         '''
+        Cast a Series to type ``dtype``.
 
-        return Dataframe(super().isnull())
+        :param dtype: Data type
 
+        :returns: This Series, properly cast.
+        '''
+        self = Series(super().astype(dtype, copy=False))
+        return self
+        
+    def dropna(self) -> Series:
+        '''
+        Removes all NaN values.
 
-    def rename(self, *args):
+        :returns: This Series, without NaN values.
         '''
-        laskdhf
 
-        :param args: askjdfhk
+        self = pd.core.series.Series(self)
+        self = self.dropna()
+        self.reset_index(drop=True, inplace=True)
+        return Series(self) 
+        
+    def show(self):
+        '''
+        descr
         '''
         
-        if (len(args) == 2):
-            super().rename(columns={args[0]:args[1]}, inplace=True)
+        tipi = set()
+        if (len(self.index) == 0):
+            print("Empty series")
+        for elem in self.index:
+            if (pd.isnull(self.loc[elem])):
+                print(elem, "NaN")
+            else:
+                print(elem, self.loc[elem])
+            tipi.add(type(self.loc[elem]))
+        if (len(tipi) > 1):
+            print("name: ", self.name, " dtype: object")
         else:
-            raise ValueError("I expect two arguments: old column name, new column name")
-        #elif (len(args) == 1 and isinstance(args[0], series) and (len(args[0])==len(self.columns))):
-        #    old = list()
-        #    for c in self.columns:
-        #        old.append(c)
-        #    for i in args[0].index:
-        #        super().rename(columns={old[i]:args[1]}, inplace=True)
-
-
-     # for key,value in kargs.items():
-     #     super().rename(columns={key:value}, inplace=True)
+            tipi = str(tipi)
+            if(tipi == "{<class 'numpy.int64'>}" or tipi == "{<class 'int'>}"):
+                print("name: ", self.name, " dtype: int")
+            if(tipi == "{<class 'str'>}"):
+                print("name: ", self.name, " dtype: str")
+            if(tipi == "{<class 'numpy.float64'>}" or tipi == "{<class 'float'>}"):
+                print("name: ", self.name, " dtype: float")
+            if(tipi == "{<class 'numpy.bool_'>}" or tipi == "{<class 'bool'>}"):
+                print("name: ", self.name, " dtype: bool")
 
+    def fillna(self, value):
+        '''
+        Fill missing values with the given value.
+        
+        :param value: Value to use to fill holes.
+        '''
+        
+        Series(super().fillna(value, inplace=True))
 
-class Locating(pd.core.indexing._iLocIndexer):
-    '''descr classe'''
 
+class Locating_s(pd.core.indexing._iLocIndexer):
+    '''Index-based locator for Series'''
     def __init__(self, val):
         '''
-        defasdf
+        Initialize an index locator from a Series
         
-        :param val: dafaf
+        :param val: The Series
         '''
         
         super().__init__("iloc", val)
-        self.df = pd.core.frame.DataFrame(val)
-
-    def __getitem__(self, *args) -> Series | Dataframe:
+        self.s = pd.core.frame.Series(val)
+    
+    def __getitem__(self, *args):
         '''
-        dafdasf
+        Return the element(s) in the required position(s).
         
-        :param args: sdafsaf
+        :param args: Index of the row to return or condition to apply to whole Series.
 
-        :returns: sadfj
+        :returns: The element(s) in the required position(s).
         '''
 
-        if (isinstance(args[0], int)):
-            #print(series(super().__getitem__(args[0])))
+        if(isinstance(args[0],slice)):
             return Series(super().__getitem__(args[0]))
-        else:
-            return Dataframe(super().__getitem__(args[0]))
+        elif (self.s.empty or (len(self.s.index) <= args[0])):
+            raise IndexError("Series indexer is out-of-bounds")
+        else: 
+            return super().__getitem__(args[0]) # ho tolto casting a series()
     
-    def __setitem__(self, *args) -> Dataframe:
+    def __setitem__(self, *args) -> Series:
         '''
-        sadlkfjsldf
+        Set the given position to the given value.
 
-        :param args: asdfsf
+        :param args: Position and new value.
 
-        :returns: sadlfkjasl
+        :returns: The Series.
         '''
-        
-        if(len(self.df.index) > args[0]):
-            return Dataframe(super().__setitem__(args[0],args[1]))
+        if(len(self.s.index) > args[0]):
+            if(len(self.s.index) == 1):
+                #self.s.astype(type(args[1]))
+                return Series(super().__setitem__(args[0],args[1]))
+            else:
+                return Series(super().__setitem__(args[0],args[1]))
         else:
             raise IndexError("Series indexer is out-of-bounds")
```

### Comparing `toypandas-0.1.1/LICENSE` & `toypandas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toypandas-0.1.1/pyproject.toml` & `toypandas-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toypandas"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Daniele Traversaro", email="traversaro.daniele@gmail.com" },
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
 description = "A library for educational purposes to simplify the syntax and notional machine of Python Pandas."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "pandas",
+  "matplotlib",
 ]
 
 [project.urls]
 "Repository" = "https://github.com/researchDataset/Toypandas"
 "Documentation" = "https://toypandas.readthedocs.io/en/latest/index.html"
 "Bug Tracker" = "https://github.com/researchDataset/Toypandas/issues"
```

### Comparing `toypandas-0.1.1/PKG-INFO` & `toypandas-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: toypandas
-Version: 0.1.1
+Version: 0.2.0
 Summary: A library for educational purposes to simplify the syntax and notional machine of Python Pandas.
 Project-URL: Repository, https://github.com/researchDataset/Toypandas
 Project-URL: Documentation, https://toypandas.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/researchDataset/Toypandas/issues
 Author-email: Daniele Traversaro <traversaro.daniele@gmail.com>, Davide Ponzini <davide.ponzini95@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: matplotlib
 Requires-Dist: pandas
 Description-Content-Type: text/markdown
 
 # ToyPandas
 A library for educational purposes to simplify the syntax and notional machine of Python Pandas 
 
 ## Installation
```

