# Comparing `tmp/order-2.1.2.tar.gz` & `tmp/order-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "order-2.1.2.tar", last modified: Tue Jul  4 11:14:11 2023, max compression
+gzip compressed data, was "order-2.1.3.tar", last modified: Thu Jul 20 08:21:59 2023, max compression
```

## Comparing `order-2.1.2.tar` & `order-2.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:14:11.534315 order-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-04 11:14:01.000000 order-2.1.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-04 11:14:01.000000 order-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 11:14:01.000000 order-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-04 11:14:11.534315 order-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-04 11:14:01.000000 order-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:14:11.530315 order-2.1.2/order/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-04 11:14:01.000000 order-2.1.2/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 11:14:01.000000 order-2.1.2/order/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-04 11:14:01.000000 order-2.1.2/order/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-04 11:14:01.000000 order-2.1.2/order/category.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-04 11:14:01.000000 order-2.1.2/order/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-07-04 11:14:01.000000 order-2.1.2/order/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    43464 2023-07-04 11:14:01.000000 order-2.1.2/order/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-04 11:14:01.000000 order-2.1.2/order/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-04 11:14:01.000000 order-2.1.2/order/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    50236 2023-07-04 11:14:01.000000 order-2.1.2/order/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-04 11:14:01.000000 order-2.1.2/order/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-07-04 11:14:01.000000 order-2.1.2/order/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:14:11.534315 order-2.1.2/order.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 11:14:01.000000 order-2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:14:11.534315 order-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-04 11:14:01.000000 order-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:59.298473 order-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-20 08:21:47.000000 order-2.1.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-20 08:21:47.000000 order-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-20 08:21:47.000000 order-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-20 08:21:59.298473 order-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-20 08:21:47.000000 order-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:59.298473 order-2.1.3/order/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-20 08:21:48.000000 order-2.1.3/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-20 08:21:48.000000 order-2.1.3/order/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-20 08:21:48.000000 order-2.1.3/order/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-20 08:21:48.000000 order-2.1.3/order/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-20 08:21:48.000000 order-2.1.3/order/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-20 08:21:48.000000 order-2.1.3/order/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43464 2023-07-20 08:21:48.000000 order-2.1.3/order/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-20 08:21:48.000000 order-2.1.3/order/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-20 08:21:48.000000 order-2.1.3/order/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50840 2023-07-20 08:21:48.000000 order-2.1.3/order/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-20 08:21:48.000000 order-2.1.3/order/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-07-20 08:21:48.000000 order-2.1.3/order/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:59.298473 order-2.1.3/order.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-20 08:21:59.000000 order-2.1.3/order.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-20 08:21:59.000000 order-2.1.3/order.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:21:59.000000 order-2.1.3/order.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:21:59.000000 order-2.1.3/order.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 08:21:59.000000 order-2.1.3/order.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 08:21:59.000000 order-2.1.3/order.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 08:21:48.000000 order-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:21:59.298473 order-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 08:21:48.000000 order-2.1.3/setup.py
```

### Comparing `order-2.1.2/LICENSE` & `order-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `order-2.1.2/PKG-INFO` & `order-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: order
-Version: 2.1.2
+Version: 2.1.3
 Summary: Pythonic class collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order
 Author: Marcel Rieger
 Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: order Version: 2.1.2 Summary: Pythonic class
+Metadata-Version: 2.1 Name: order Version: 2.1.3 Summary: Pythonic class
 collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order Author: Marcel Rieger Author-email:
 github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2 Classifier: Programming Language :: Python
 :: 2.7 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `order-2.1.2/README.md` & `order-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order/__init__.py` & `order-2.1.3/order/__init__.py`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order/analysis.py` & `order-2.1.3/order/analysis.py`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order/category.py` & `order-2.1.3/order/category.py`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order/config.py` & `order-2.1.3/order/config.py`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order/dataset.py` & `order-2.1.3/order/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,27 +265,27 @@
                     except:
                         raise TypeError("invalid info value type: {}".format(obj))
                 obj = DatasetInfo(**obj)
             _info[str(name)] = obj
 
         return _info
 
-    def set_info(self, shift_name, info):
+    def set_info(self, name, info):
         """
-        Sets an :py:class:`DatasetInfo` object *info* for a given *shift_name*. Returns the object.
+        Sets an :py:class:`DatasetInfo` object *info* for a given *name*. Returns the object.
         """
-        shift_name, info = list(self.__class__.info.fparse(self, {shift_name: info}).items())[0]
-        self.info[shift_name] = info
+        name, info = list(self.__class__.info.fparse(self, {name: info}).items())[0]
+        self.info[name] = info
         return info
 
-    def get_info(self, shift_name):
+    def get_info(self, name):
         """
-        Returns the :py:class:`DatasetInfo` object for a given *shift_name*.
+        Returns the :py:class:`DatasetInfo` object for a given *name*.
         """
-        return self.info[shift_name]
+        return self.info[name]
 
     @property
     def keys(self):
         # keys getter, nominal info object
         return self.info[Shift.NOMINAL].keys
 
     @property
```

### Comparing `order-2.1.2/order/mixins.py` & `order-2.1.3/order/mixins.py`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order/process.py` & `order-2.1.3/order/process.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,16 +29,17 @@
     ColorMixin,
 ):
     r"""
     Definition of a phyiscs process.
 
     **Arguments**
 
-    *xsecs* should be a mapping of center-of-mass energies to cross sections values (automatically
-    converted to `scinum.Number <https://scinum.readthedocs.io/en/latest/#number>`__ instances).
+    *xsecs* should be a mapping of (e.g.) center-of-mass energies to cross sections values
+    (automatically converted to `scinum.Number <https://scinum.readthedocs.io/en/latest/#number>`__
+    instances).
 
     *color*, *color1*, *color2* and *color3* are forwarded to the
     :py:class:`~order.mixins.ColorMixin`, *label* and *label_short* to the
     :py:class:`~order.mixins.LabelMixin`, *is_data* to the
     :py:class:`~order.mixins.DataSourceMixin`, *tags* to the :py:class:`~order.mixins.TagMixin`,
     *aux* to the :py:class:`~order.mixins.AuxDataMixin`, and *name* and *id* to the
     :py:class:`~order.unique.UniqueObject` constructor.
@@ -177,72 +178,78 @@
         try:
             xsecs = dict(xsecs)
         except:
             raise TypeError("invalid xsecs type: {}".format(xsecs))
 
         # parse particular values
         _xsecs = {}
-        for ecm, xsec in xsecs.items():
-            if not isinstance(ecm, (int, float)):
-                raise TypeError("invalid xsec energy type: {}".format(ecm))
+        for key, xsec in xsecs.items():
+            # when key is a number, make sure it's a float
+            if isinstance(key, (int, Number)):
+                key = float(key)
+            # value check
             if not isinstance(xsec, Number):
                 try:
                     xsec = Number(xsec)
                 except:
                     raise TypeError("invalid xsec value type: {}".format(xsec))
-            _xsecs[float(ecm)] = xsec
+            _xsecs[key] = xsec
 
         return _xsecs
 
-    def get_xsec(self, ecm):
+    def get_xsec(self, key):
         """
         Returns the cross section (a
-        `scinum.Number <https://scinum.readthedocs.io/en/latest/#number>`__ instance) for a
-        center-of-mass energy *ecm*.
+        `scinum.Number <https://scinum.readthedocs.io/en/latest/#number>`__ instance) for a *key*
+        (e.g. a center-of-mass energy). When *key* is an integer or a number instance, it is
+        converted to float first.
         """
-        return self.xsecs[ecm]
+        if isinstance(key, (int, Number)):
+            key = float(key)
+        return self.xsecs[key]
 
-    def set_xsec(self, ecm, xsec):
+    def set_xsec(self, key, xsec):
         """
-        Sets the cross section for a center-of-mass energy *ecm* to *xsec*. When *xsec* is not a
+        Sets the cross section for a *key* (e.g. a center-of-mass energy) to *xsec*. When *key* is
+        an integer or a number instance, it is converted to float first. When *xsec* is not a
         `scinum.Number <https://scinum.readthedocs.io/en/latest/#number>`__ instance, it is
         converted to one. The (probably converted) value is returned.
         """
-        ecm, xsec = list(self.__class__.xsecs.fparse(self, {ecm: xsec}).items())[0]
-        self.xsecs[ecm] = xsec
+        key, xsec = list(self.__class__.xsecs.fparse(self, {key: xsec}).items())[0]
+        self.xsecs[key] = xsec
         return xsec
 
-    def pretty_print(self, ecm=None, offset=40, max_depth=-1, stream=None, _depth=0, **kwargs):
-        """ pretty_print(ecm=None, offset=40, max_depth=-1, stream=None, **kwargs)
+    def pretty_print(self, xsec_key=None, offset=40, max_depth=-1, stream=None, _depth=0, **kwargs):
+        """ pretty_print(xsec_key=None, offset=40, max_depth=-1, stream=None, **kwargs)
         Prints this process and potentially its subprocesses down to a maximum depth *max_depth* in
-        a structured fashion. When *ecm* is set, process cross section values are shown as well
+        a structured fashion. When *xsec_key* is set, process cross section values are shown as well
         with a maximum horizontal distance of *offset*. *stream* can be a file object and defaults
         to *sys.stdout*. All *kwargs* are forwarded to the :py:meth:`Number.str` methods of the
         cross section numbers.
         """
         if not stream:
             stream = sys.stdout
 
         # start the entry to print
         entry = "| " * _depth + "> {} ({})".format(self.name, self.id)
 
-        # add cross-section values following an offset when ecm is set
-        if ecm is not None:
+        # add cross-section values following an offset when xsec_key is set
+        if xsec_key is not None:
             entry += " " * (offset - len(entry))
-            xsec = self.xsecs.get(ecm)
+            xsec = self.xsecs.get(xsec_key)
             entry += "  " * _depth + (xsec.str(**kwargs) if xsec else "no cross-section")
 
-        stream.write(six.b(entry + "\n"))
+        stream.write(six.b(entry + "\n") if six.PY3 else (entry + "\n"))
 
         # stop here when max_depth is reached
         if 0 <= max_depth <= _depth:
             return
 
         for proc in self.processes:
             proc.pretty_print(
-                ecm=ecm,
+                xsec_key=xsec_key,
                 offset=offset,
                 max_depth=max_depth,
                 stream=stream,
                 _depth=_depth + 1,
                 **kwargs  # noqa: C815
             )
```

### Comparing `order-2.1.2/order/shift.py` & `order-2.1.3/order/shift.py`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order/unique.py` & `order-2.1.3/order/unique.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,15 @@
                 break
 
         # add to the index
         self._index.append(obj)
 
         return obj
 
-    def extend(self, objs, overwrite=True):
+    def extend(self, objs, overwrite=False):
         """
         Adds multiple new objects to the index. All elements of the sequence *objs*, as well as
         *overwrite*, are forwarded to :py:meth:`add` and the added objects are returned in a list.
         When an object is a dictionary or a tuple, it is expanded for the invocation of
         :py:meth:`add`.
         """
         results = []
@@ -763,16 +763,18 @@
                 warnings.warn(
                     "the 'depth_first' attribute is deprecated; use 'algo=\"dfs\"' instead'",
                     DeprecationWarning,
                 )
                 algo = "dfs"
 
             # check the algo
-            if algo == "dfs":
+            if algo == "dfs" or algo == "dfs_pre":
                 algo = "dfs_preorder"
+            elif algo == "dfs_post":
+                algo = "dfs_postorder"
             known_algos = ["bfs", "dfs_preorder", "dfs_postorder"]
             if algo not in known_algos:
                 _known_algos = ", ".join(map("'{}'".format, known_algos))
                 raise ValueError(
                     "unknown traversel order '{}', should be one of {}".format(algo, _known_algos),
                 )
 
@@ -850,30 +852,31 @@
         else:  # deep_children
 
             # has child method
             @patch("has_" + singular)
             def has(self, obj, deep=True):
                 """
                 Checks if the :py:attr:`{plural}` index contains an *obj* which might be a *name*,
-                *id*, or an instance. If *deep* is *True*, the lookup is recursive.
+                *id*, or an instance. If *deep* is *True*, the lookup is recursive through
+                potentially nested child {plural}.
                 """
                 return getattr(self, "get_" + singular)(
                     obj,
                     default=_not_found,
                     deep=deep,
                 ) != _not_found
 
             # get child method
             @patch("get_" + singular)
             def get(self, obj, deep=True, default=_no_default):
                 """ get_{singular}(obj, deep=True, default=no_default)
                 Returns a child {singular} given by *obj*, which might be a *name*, *id*, or an
                 instance from the :py:attr:`{plural}` index. If *deep* is *True*, the lookup is
-                recursive. When no {singular} is found, *default* is returned when set. Otherwise,
-                an error is raised.
+                recursive through potentially nested child {plural}. When no {singular} is found,
+                *default* is returned when set. Otherwise, an error is raised.
                 """
                 indexes = [getattr(self, plural)]
                 while len(indexes) > 0:
                     index = indexes.pop(0)
                     _obj = index.get(obj, default=_not_found)
                     if _obj != _not_found:
                         return _obj
@@ -894,17 +897,19 @@
                 {singular}, its depth relative to *this* {singular}, and its child {plural} in a
                 list that can be modified to alter the walking.
 
                 The traversal order is defined by *algo* which allows different values (more
                 `info <https://en.wikipedia.org/wiki/Tree_traversal>`__):
 
                     - ``"bfs"``: Breadth-first search.
-                    - ``"dfs"``: Alias for ``"dfs_preorder"``.
                     - ``"dfs_preorder"``: Pre-order depth-first search.
                     - ``"dfs_postorder"``: Post-order depth-first search.
+                    - ``"dfs"``: Alias for ``"dfs_preorder"``.
+                    - ``"dfs_pre"``: Alias for ``"dfs_preorder"``.
+                    - ``"dfs_post"``: Alias for ``"dfs_postorder"``.
 
                 When *include_self* is *True*, this {singular} instance is yielded as well with a
                 depth of 0.
                 """
                 return _walk(
                     self,
                     (lambda obj: getattr(obj, plural).values()),
@@ -1127,30 +1132,32 @@
             else:  # deep_parents
 
                 # has child method
                 @patch("has_parent_" + singular)
                 def has(self, obj, deep=True):
                     """
                     Checks if the :py:attr:`parent_{plural}` index contains an *obj*, which might be
-                    a *name*, *id*, or an instance. If *deep* is *True*, the lookup is recursive.
+                    a *name*, *id*, or an instance. If *deep* is *True*, the lookup is recursive
+                    through potentially nested parent {plural}.
                     """
                     return getattr(self, "get_parent_" + singular)(
                         obj,
                         default=_not_found,
                         deep=deep,
                     ) != _not_found
 
                 # get parent method
                 @patch("get_parent_" + singular)
                 def get(self, obj, deep=True, default=_no_default):
                     """ get_parent_{singular}(obj, deep=True, default=no_default)
                     Returns a parent {singular} given by *obj*, which might be a *name*, *id*, or an
                     instance from the :py:attr:`parent_{plural}` index. If *deep* is *True*, the
-                    lookup is recursive. When no {singular} is found, *default* is returned when
-                    set. Otherwise, an error is raised.
+                    lookup is recursive through potentially nested parent {plural}. When no
+                    {singular} is found, *default* is returned when set. Otherwise, an error is
+                    raised.
                     """
                     indexes = [getattr(self, "parent_" + plural)]
                     while len(indexes) > 0:
                         index = indexes.pop(0)
                         _obj = index.get(obj, default=_not_found)
                         if _obj != _not_found:
                             return _obj
@@ -1171,17 +1178,19 @@
                     parent {singular}, its depth relative to *this* {singular}, and its parent
                     {plural} in a list that can be modified to alter the walking.
 
                     The traversal order is defined by *algo* which allows different values (more
                     `info <https://en.wikipedia.org/wiki/Tree_traversal>`__):
 
                         - ``"bfs"``: Breadth-first search.
-                        - ``"dfs"``: Alias for ``"dfs_preorder"``.
                         - ``"dfs_preorder"``: Pre-order depth-first search.
                         - ``"dfs_postorder"``: Post-order depth-first search.
+                        - ``"dfs"``: Alias for ``"dfs_preorder"``.
+                        - ``"dfs_pre"``: Alias for ``"dfs_preorder"``.
+                        - ``"dfs_post"``: Alias for ``"dfs_postorder"``.
 
                     When *include_self* is *True*, this {singular} instance is yielded as well with
                     a depth of 0.
                     """
                     return _walk(
                         self,
                         (lambda obj: getattr(obj, "parent_" + plural).values()),
```

### Comparing `order-2.1.2/order/util.py` & `order-2.1.3/order/util.py`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order/variable.py` & `order-2.1.3/order/variable.py`

 * *Files identical despite different names*

### Comparing `order-2.1.2/order.egg-info/PKG-INFO` & `order-2.1.3/order.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: order
-Version: 2.1.2
+Version: 2.1.3
 Summary: Pythonic class collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order
 Author: Marcel Rieger
 Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: order Version: 2.1.2 Summary: Pythonic class
+Metadata-Version: 2.1 Name: order Version: 2.1.3 Summary: Pythonic class
 collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order Author: Marcel Rieger Author-email:
 github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2 Classifier: Programming Language :: Python
 :: 2.7 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `order-2.1.2/setup.py` & `order-2.1.3/setup.py`

 * *Files identical despite different names*

