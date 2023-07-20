# Comparing `tmp/polyp-1.1.1.tar.gz` & `tmp/polyp-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyp-1.1.1.tar", last modified: Mon Jun 27 15:35:38 2022, max compression
+gzip compressed data, was "polyp-1.1.2.tar", last modified: Thu Jul 20 16:41:33 2023, max compression
```

## Comparing `polyp-1.1.1.tar` & `polyp-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2022-06-27 15:35:38.568825 polyp-1.1.1/
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1067 2022-06-27 10:39:37.000000 polyp-1.1.1/LICENSE.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)    19575 2022-06-27 15:35:38.568825 polyp-1.1.1/PKG-INFO
--rw-r--r--   0 bredol    (1000) bredol    (1000)    19351 2022-06-27 10:39:37.000000 polyp-1.1.1/README.md
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2022-06-27 15:35:38.568825 polyp-1.1.1/polyp/
--rw-r--r--   0 bredol    (1000) bredol    (1000)      309 2022-06-27 10:39:37.000000 polyp-1.1.1/polyp/__init__.py
--rwxr-xr-x   0 bredol    (1000) bredol    (1000)     4144 2022-06-27 10:39:37.000000 polyp-1.1.1/polyp/__main__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    42606 2022-06-27 11:35:11.000000 polyp-1.1.1/polyp/calltree.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    27988 2022-06-27 10:39:37.000000 polyp-1.1.1/polyp/fonts.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    16224 2022-06-27 10:39:37.000000 polyp-1.1.1/polyp/geometry.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     2269 2022-06-27 10:39:37.000000 polyp-1.1.1/polyp/plotting.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    17681 2022-06-27 11:35:17.000000 polyp-1.1.1/polyp/plsscript.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     4649 2022-06-27 11:35:22.000000 polyp-1.1.1/polyp/utils.py
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2022-06-27 15:35:38.568825 polyp-1.1.1/polyp.egg-info/
--rw-r--r--   0 bredol    (1000) bredol    (1000)    19575 2022-06-27 15:35:37.000000 polyp-1.1.1/polyp.egg-info/PKG-INFO
--rw-r--r--   0 bredol    (1000) bredol    (1000)      345 2022-06-27 15:35:38.000000 polyp-1.1.1/polyp.egg-info/SOURCES.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)        1 2022-06-27 15:35:37.000000 polyp-1.1.1/polyp.egg-info/dependency_links.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       46 2022-06-27 15:35:38.000000 polyp-1.1.1/polyp.egg-info/entry_points.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       30 2022-06-27 15:35:38.000000 polyp-1.1.1/polyp.egg-info/requires.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)        6 2022-06-27 15:35:38.000000 polyp-1.1.1/polyp.egg-info/top_level.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       38 2022-06-27 15:35:38.582158 polyp-1.1.1/setup.cfg
--rwxr-xr-x   0 bredol    (1000) bredol    (1000)      753 2022-06-27 15:35:22.000000 polyp-1.1.1/setup.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 16:41:33.757659 polyp-1.1.2/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1067 2023-07-19 14:22:28.000000 polyp-1.1.2/LICENSE.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    20131 2023-07-20 16:41:33.757659 polyp-1.1.2/PKG-INFO
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    19907 2023-07-20 16:36:14.000000 polyp-1.1.2/README.md
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 16:41:33.757659 polyp-1.1.2/polyp/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      309 2022-06-27 10:39:37.000000 polyp-1.1.2/polyp/__init__.py
+-rwxr-xr-x   0 bredol    (1000) bredol    (1000)     4144 2023-07-19 14:22:28.000000 polyp-1.1.2/polyp/__main__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    43537 2023-07-20 16:04:18.000000 polyp-1.1.2/polyp/calltree.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    27988 2022-06-27 10:39:37.000000 polyp-1.1.2/polyp/fonts.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    17142 2023-07-20 16:30:33.000000 polyp-1.1.2/polyp/geometry.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     2269 2023-07-19 14:22:28.000000 polyp-1.1.2/polyp/plotting.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    17681 2023-07-19 14:22:28.000000 polyp-1.1.2/polyp/plsscript.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4666 2023-07-20 16:21:20.000000 polyp-1.1.2/polyp/utils.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 16:41:33.757659 polyp-1.1.2/polyp.egg-info/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    20131 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/PKG-INFO
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      345 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/SOURCES.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        1 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/dependency_links.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       46 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/entry_points.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       30 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/requires.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        6 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/top_level.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       38 2023-07-20 16:41:33.757659 polyp-1.1.2/setup.cfg
+-rwxr-xr-x   0 bredol    (1000) bredol    (1000)      753 2023-07-20 16:41:25.000000 polyp-1.1.2/setup.py
```

### Comparing `polyp-1.1.1/LICENSE.txt` & `polyp-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polyp-1.1.1/PKG-INFO` & `polyp-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: polyp
-Version: 1.1.1
+Version: 1.1.2
 Summary: A renderer that creates gdsII files from an all-ascii human-readble layout language 
 Author: zaphB
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Human-Readble-Ascii to gdsII Converter
 
-Polyp is a renderer that creates gdsII layout files from an all-ascii human-readble layout language. Geometric shapes are constructed from primitive shapes, e.g., squares, circles or text, that are translated, rotated, scaled or otherwise transformed and can be added, subtracted or intersected with each other.
+Polyp is a renderer that creates gdsII layout files from an all-ascii human-readable layout language. Geometric shapes are constructed from primitive shapes, e.g., squares, circles or text, that are translated, rotated, scaled or otherwise transformed and can be added, subtracted or intersected with each other.
 
 Polyp is definitely interesting for you if you
 * are not afraid of using the command line
 * have experience with drawing gdsII files
 * are a fan of mark-up languages
 
 Polyp is probably not for you if you
 * prefer manually drawing geometry
-* fell uncomfortable using the command line
+* feel uncomfortable using the command line
 
 A minimal example is shown in the following:
 
 ```
 SYMBOL main
   LAYER 0
     rect(10).rotate(45) - text("hello world", dy=3)
@@ -40,26 +40,26 @@
 
 Install polyp and its dependencies with
 
 ```
 pip install polyp
 ```
 
-Executing `polyp -h` on the shell should now show the polyp quick help, `polyp --ersion` should show the expected version number.
+Executing `polyp -h` on the shell should now show the polyp quick help, `polyp --version` should show the expected version number.
 
 
 # Basic usage
 
 To compile a .pls polyp layout script to a .gds file, run `polyp filename`, where `filename` has to be replaced with the path of the .pls file.
 
-Passing the `-v` option (`polyp -v filename`) compiles the layout script and opens a simple viewer afterwards.
+Passing the `-v` (`--view`) option (`polyp -v filename`) compiles the layout script and opens a simple viewer afterwards.
 
-Passing the `-w` option keeps checkign the .pls file for updates, recompiles it in case a change in the file is detected and keeps the compiled result open in a viewer.
+Passing the `-w` (`--watch`) option keeps checking the .pls file for updates, re-compiles in case a change in the file is detected and keeps the compiled result open in a viewer.
 
-If the `-p` option is passed to polyp, the layout script is compiled to .pdf instead of .gds. One pdf file is created for each gdsII symbol.
+If the `-p` (`--pdf`) option is passed to polyp, the layout script is compiled to .pdf instead of .gds. One pdf file is created for each gdsII symbol.
 
 
 # Examples
 
 This list of examples starts from a minimal .pls example and moves to more and more complex layout scripts step by step. A formal documentation of the polyp layout language is currently not available, feel free to contact me or open an issue in case this is needed.
 
 
@@ -143,15 +143,22 @@
 Translate supports the optional boolean arguement `copy`, which if set to true, causes the untranslated shape to be kept in the result, e.g. `rect(10).translate(0, 20, copy=True)`.
 
 
 ### Rotate
 
 To rotate a square by 30 degrees, use `rect(10).rotate(30)`. Optionally, the center of rotation can be specified as a second parameter: `rect(10).rotate(30, [0, 10])`. By default, the center of rotation is given by the center of mass of the rotated geometry.
 
-Rotate supports the optional boolean arguement `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
+Rotate supports the optional boolean argument `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
+
+
+### Scale
+
+To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `a1`.
+
+Scale supports the optional boolean argument `copy`, which if set to true, causes the unscaled shape to be kept in the result, e.g. `rect(10).scale(3, center=[0,0], copy=True)`.
 
 
 ### Mirror
 
 To mirror a geometry at a given point or line, use the `.mirror(...)`. The following example shows three different ways of calling the method:
 
 ```
@@ -196,19 +203,19 @@
 ```
 
 ### Calculating height, width, bounding box and center of mass
 
 The functions `height(...)` and `width(...)` return the height and width of the shape that is passed as an argument. For example `height(rect(10))` returns 10. The function `bb(...)` returns the bounding box of a shape. The function `center(...)` returns a shapes center of mass.
 
 
-### Mathematical functions
+### Math
 
 The trigonometric functions and there inverse functions are available as `cos`, `sin`, `tan`, `asin`, `acos`, `atan`. Angles are given in units of degrees. The function `atan2` is a variant of `atan` that uses two arguments and is able to handle the full circle. See the numpy documentation of `atan2` for further details.
 
-The function `abs(...)` returns the absolute value of the passed number. The functions `min`, `max` and `mean` return the minimum, maximum or arithmetical mean of the passed list of numbers.
+The function `abs(...)` returns the absolute value of the passed number, `sqrt(...)` returns the square root. The functions `min`, `max` and `mean` return the minimum, maximum or arithmetical mean of the passed list of numbers.
 
 
 ### Type conversions
 
 Use `int(...)` to convert a number to integer. Use `char(...)` to convert an integer number to the respective letter of the alphabet.
 
 
@@ -405,12 +412,12 @@
 SYMBOL main
   LAYER 0
     wire(*optsA)
   LAYER 1
     wire(*optsB)
 ```
 
-The unary `*` operator applied to objects unpacks the obect into a parameter list. This way it is not necessary to write down all argument names anymore, which is helpful in layouts with many free parameters.
+The unary `*` operator applied to objects unpacks the object into a parameter list. This way it is not necessary to write down all argument names anymore, which is helpful in layouts with many free parameters.
 
 ## QR codes
 
 The `qrcode` native creates a qr code geometry from a given string. The optional named parameters `dx` and `dy` specify the size of the resulting code in x and y directions. With the `robust` parameter (1...4, higher=more robust, default 2) the redundancy in the generated code can be adjusted. The `res` parameter controls the number of "pixels" used in the qrcode. By default, the `res` is automatically chosen according to the input string.
```

### Comparing `polyp-1.1.1/README.md` & `polyp-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Human-Readble-Ascii to gdsII Converter
 
-Polyp is a renderer that creates gdsII layout files from an all-ascii human-readble layout language. Geometric shapes are constructed from primitive shapes, e.g., squares, circles or text, that are translated, rotated, scaled or otherwise transformed and can be added, subtracted or intersected with each other.
+Polyp is a renderer that creates gdsII layout files from an all-ascii human-readable layout language. Geometric shapes are constructed from primitive shapes, e.g., squares, circles or text, that are translated, rotated, scaled or otherwise transformed and can be added, subtracted or intersected with each other.
 
 Polyp is definitely interesting for you if you
 * are not afraid of using the command line
 * have experience with drawing gdsII files
 * are a fan of mark-up languages
 
 Polyp is probably not for you if you
 * prefer manually drawing geometry
-* fell uncomfortable using the command line
+* feel uncomfortable using the command line
 
 A minimal example is shown in the following:
 
 ```
 SYMBOL main
   LAYER 0
     rect(10).rotate(45) - text("hello world", dy=3)
@@ -32,26 +32,26 @@
 
 Install polyp and its dependencies with
 
 ```
 pip install polyp
 ```
 
-Executing `polyp -h` on the shell should now show the polyp quick help, `polyp --ersion` should show the expected version number.
+Executing `polyp -h` on the shell should now show the polyp quick help, `polyp --version` should show the expected version number.
 
 
 # Basic usage
 
 To compile a .pls polyp layout script to a .gds file, run `polyp filename`, where `filename` has to be replaced with the path of the .pls file.
 
-Passing the `-v` option (`polyp -v filename`) compiles the layout script and opens a simple viewer afterwards.
+Passing the `-v` (`--view`) option (`polyp -v filename`) compiles the layout script and opens a simple viewer afterwards.
 
-Passing the `-w` option keeps checkign the .pls file for updates, recompiles it in case a change in the file is detected and keeps the compiled result open in a viewer.
+Passing the `-w` (`--watch`) option keeps checking the .pls file for updates, re-compiles in case a change in the file is detected and keeps the compiled result open in a viewer.
 
-If the `-p` option is passed to polyp, the layout script is compiled to .pdf instead of .gds. One pdf file is created for each gdsII symbol.
+If the `-p` (`--pdf`) option is passed to polyp, the layout script is compiled to .pdf instead of .gds. One pdf file is created for each gdsII symbol.
 
 
 # Examples
 
 This list of examples starts from a minimal .pls example and moves to more and more complex layout scripts step by step. A formal documentation of the polyp layout language is currently not available, feel free to contact me or open an issue in case this is needed.
 
 
@@ -135,15 +135,22 @@
 Translate supports the optional boolean arguement `copy`, which if set to true, causes the untranslated shape to be kept in the result, e.g. `rect(10).translate(0, 20, copy=True)`.
 
 
 ### Rotate
 
 To rotate a square by 30 degrees, use `rect(10).rotate(30)`. Optionally, the center of rotation can be specified as a second parameter: `rect(10).rotate(30, [0, 10])`. By default, the center of rotation is given by the center of mass of the rotated geometry.
 
-Rotate supports the optional boolean arguement `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
+Rotate supports the optional boolean argument `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
+
+
+### Scale
+
+To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `a1`.
+
+Scale supports the optional boolean argument `copy`, which if set to true, causes the unscaled shape to be kept in the result, e.g. `rect(10).scale(3, center=[0,0], copy=True)`.
 
 
 ### Mirror
 
 To mirror a geometry at a given point or line, use the `.mirror(...)`. The following example shows three different ways of calling the method:
 
 ```
@@ -188,19 +195,19 @@
 ```
 
 ### Calculating height, width, bounding box and center of mass
 
 The functions `height(...)` and `width(...)` return the height and width of the shape that is passed as an argument. For example `height(rect(10))` returns 10. The function `bb(...)` returns the bounding box of a shape. The function `center(...)` returns a shapes center of mass.
 
 
-### Mathematical functions
+### Math
 
 The trigonometric functions and there inverse functions are available as `cos`, `sin`, `tan`, `asin`, `acos`, `atan`. Angles are given in units of degrees. The function `atan2` is a variant of `atan` that uses two arguments and is able to handle the full circle. See the numpy documentation of `atan2` for further details.
 
-The function `abs(...)` returns the absolute value of the passed number. The functions `min`, `max` and `mean` return the minimum, maximum or arithmetical mean of the passed list of numbers.
+The function `abs(...)` returns the absolute value of the passed number, `sqrt(...)` returns the square root. The functions `min`, `max` and `mean` return the minimum, maximum or arithmetical mean of the passed list of numbers.
 
 
 ### Type conversions
 
 Use `int(...)` to convert a number to integer. Use `char(...)` to convert an integer number to the respective letter of the alphabet.
 
 
@@ -397,12 +404,12 @@
 SYMBOL main
   LAYER 0
     wire(*optsA)
   LAYER 1
     wire(*optsB)
 ```
 
-The unary `*` operator applied to objects unpacks the obect into a parameter list. This way it is not necessary to write down all argument names anymore, which is helpful in layouts with many free parameters.
+The unary `*` operator applied to objects unpacks the object into a parameter list. This way it is not necessary to write down all argument names anymore, which is helpful in layouts with many free parameters.
 
 ## QR codes
 
 The `qrcode` native creates a qr code geometry from a given string. The optional named parameters `dx` and `dy` specify the size of the resulting code in x and y directions. With the `robust` parameter (1...4, higher=more robust, default 2) the redundancy in the generated code can be adjusted. The `res` parameter controls the number of "pixels" used in the qrcode. By default, the `res` is automatically chosen according to the input string.
```

### Comparing `polyp-1.1.1/polyp/__main__.py` & `polyp-1.1.2/polyp/__main__.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.1/polyp/calltree.py` & `polyp-1.1.2/polyp/calltree.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,21 +68,30 @@
   def _addText(self, text):
     text = text.strip()
     if len(text) > 0:
       self._children.append(text.strip())
 
   def _py2lit(self, *vals):
     res = []
+    def isInt(x):
+      try: return _np.isclose(int(x), float(x))
+      except KeyboardInterrupt: raise
+      except: pass
+    def isFloat(x):
+      try: float(x); return True
+      except KeyboardInterrupt: raise
+      except: pass
+
     for val in vals:
       if type(val) is list and type(val[0]) is str:
         res.append(val)
-      elif type(val) is float:
-        res.append(['float', val])
-      elif type(val) is int:
-        res.append(['int', val])
+      elif isInt(val):
+        res.append(['int', int(val)])
+      elif isFloat(val):
+        res.append(['float', float(val)])
       elif type(val) is list and len(val) == 2:
         res.append(['point', val])
       elif type(val) is str:
         res.append(['string', val])
       elif isinstance(val, geometry.Shape):
         res.append(['shape', val])
       else:
@@ -252,14 +261,21 @@
       # translate function
       elif self._func == "translate":
         requireResolvedNamesOnly()
         self._literals = [['func', utils.TypeCheck(["shape", "point", "shaperef"])
                                   +geometry.Translator(*largs, **dargs)]]
 
       #=====================================================================
+      # scale function
+      elif self._func == "scale":
+        requireResolvedNamesOnly()
+        self._literals = [['func', utils.TypeCheck(["shape",])
+                                  +geometry.Scaler(*largs, **dargs)]]
+
+      #=====================================================================
       # rotate function
       elif self._func == "rotate":
         requireResolvedNamesOnly()
         self._literals = [['func', utils.TypeCheck(["shape", "point", "shaperef"])
                                   +geometry.Rotator(*largs, **dargs)]]
 
       #=====================================================================
@@ -302,15 +318,15 @@
       elif self._func == "int":
         requireResolvedNamesOnly()
         if len(dargs) > 0 or len(largs) != 1:
           raise ValueError("Invalid arguments to 'int' call.")
         self._literals = [['int', int(largs[0])]]
 
       #=====================================================================
-      # absolute
+      # absolute value
       elif self._func == "abs":
         requireResolvedNamesOnly()
         if len(dargs) > 0 or len(largs) != 1:
           raise ValueError("Invalid arguments to 'abs' call.")
         self._literals = [['float', abs(largs[0])]]
 
       #=====================================================================
@@ -334,26 +350,35 @@
           largs = [float(f) for f in largs]
         except:
           raise ValueError("Function '"+self._func+"' supports only numerical inputs.")
         fdict = {"min": min, "max": max, "mean": lambda l: sum(l)/len(l)}
         self._literals = [['float', fdict[self._func](largs)]]
 
       #=====================================================================
+      # square root
+      elif self._func == "sqrt":
+        requireResolvedNamesOnly()
+        if len(dargs) > 0 or len(largs) != 1 or largs[0]<0:
+          raise ValueError("Invalid arguments to 'sqrt' call.")
+        self._literals = [['float', _np.sqrt(largs[0])]]
+
+      #=====================================================================
       # trigonometric functions
       elif self._func in ["cos", "sin", "tan", "asin", "acos", "atan"]:
         requireResolvedNamesOnly()
         if len(largs) != 1 or any([a not in ['unit'] for a in dargs]):
           raise ValueError("Invalid arguments to 'cos' function.")
         u = dargs.get('unit', 'deg')
         if u == 'deg':
           largs[0] *= _np.pi/180
         elif u == 'rad':
           pass
         else:
-          raise ValueError("Invalid value for 'unit' argument in 'cos' function.")
+          raise ValueError(f"Invalid value for 'unit' argument in "
+                           f"'{self._func}' function.")
         if self._func == "sin":
           self._literals = [['float', _np.sin(largs[0])]]
         elif self._func == "cos":
           self._literals = [['float', _np.cos(largs[0])]]
         elif self._func == "tan":
           self._literals = [['float', _np.tan(largs[0])]]
         elif self._func == "asin":
```

### Comparing `polyp-1.1.1/polyp/fonts.py` & `polyp-1.1.2/polyp/fonts.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.1/polyp/geometry.py` & `polyp-1.1.2/polyp/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,20 +73,28 @@
         elif self._anchorType == 'c':
           self._shape.translate(-0.5*(bb[0][0]+bb[2][0]), -0.5*(bb[0][1]+bb[2][1]))
       self._shape.translate(dx, dy)
     return self
 
   def rotate(self, angle, center=None):
     if not self._shape is None:
-      if center != None:
+      if center is not None:
         self._shape.rotate(angle, center)
       else:
         self._shape.rotate(angle, self.center())
     return self
 
+  def scale(self, s1, s2, center=None):
+    if not self._shape is None:
+      if center is not None:
+        self._shape.scale(s1, s2, center)
+      else:
+        self._shape.scale(s1, s2, self.center())
+    return self
+
   def mirror(self, p1, p2, copy=False):
     self._shape.mirror(p1, p2)
     return self
 
   def grow(self, size):
     if not self._shape is None:
       self._shape = _gdspy.offset(self._shape, size)
@@ -339,14 +347,41 @@
       elif self._anchorType == 'w':
         self.translate(-min(bb[0][0], bb[2][0]), -0.5*(bb[0][1]+bb[2][1]))
     else:
       self.translate(-0.5*(bb[0][0]+bb[2][0]), -0.5*(bb[0][1]+bb[2][1]))
     self.translate(self.anchor[0], self.anchor[1])
 
 
+class Translator:
+  def __init__(self, *largs, **dargs):
+    self._largs = largs
+    self._dargs = dargs
+
+  def __call__(self, op):
+    if hasattr(op, 'translate'):
+      if self._dargs.get('copy', False):
+        return op.copy().union(op.translate(*self._largs, **self._dargs))
+      else:
+        return op.translate(*self._largs, **self._dargs)
+    elif len(self._largs) == 2 and len(self._dargs) == 0:
+      self._dx = self._largs[0]
+      self._dy = self._largs[1]
+    elif (len(self._largs) == 0
+          and len(self._dargs) == 2
+          and 'dx' in self._dargs
+          and 'dy' in self._dargs):
+      self._dx = self._dargs['dx']
+      self._dy = self._dargs['dy']
+    else:
+      raise ValueError("Invalid translator instanciation.")
+    if 'copy' in self._dargs:
+      raise ValueError('"copy" may only be specified when translating shapes.')
+    return (op[0]+self._dx, op[1]+self._dy)
+
+
 class Rotator:
   def __init__(self, angle, center=None, unit="deg", copy=False):
     self._copy = copy
     if unit not in ['deg', 'rad']:
       raise ValueError("Unsupported angle unit: '"+unit+"', use 'deg' or 'rad'.")
     if unit == 'rad':
       self._angle = angle
@@ -376,14 +411,36 @@
       if not hasattr(c, '__len__') or len(c) != 2:
         c = [0,0]
 
       return ((op[0]-c[0])*_np.cos(self._angle) - (op[1]-c[1])*_np.sin(self._angle) + c[0],
               (op[0]-c[0])*_np.sin(self._angle) + (op[1]-c[1])*_np.cos(self._angle) + c[1])
 
 
+class Scaler:
+  def __init__(self, s1=None, s2=None, center=None, copy=False):
+    self._copy = copy
+    self._center = center
+    if s1 is not None and s2 is None:
+      self._s1 = s1
+      self._s2 = s1
+    elif s1 is not None and s2 is not None:
+      self._s1 = s1
+      self._s2 = s2
+    else:
+      raise ValueError("Incomplete parameters to scale: specify at least "           
+                       "one scale factor. Parameters 'x', 'y' and 'copy' "
+                       "are optional")
+
+  def __call__(self, op):
+    if self._copy:
+      return op.copy().union(op.scale(self._s1, self._s2, self._center))
+    else:
+      return op.scale(self._s1, self._s2, self._center)
+
+
 class Mirrower:
   def __init__(self, p1=None, p2=None, x=None, y=None, copy=False):
     self._copy = copy
     if p1 is not None:
       self._p1 = p1
       self._p2 = p2
     elif x is not None and y is None:
@@ -408,48 +465,22 @@
         return op.copy().union(op.mirror(self._p1, self._p2))
     else:
       if self._p2 is None:
         return op.rotate(_np.pi, self._p1)
       else:
         return op.mirror(self._p1, self._p2)
 
-class Translator:
-  def __init__(self, *largs, **dargs):
-    self._largs = largs
-    self._dargs = dargs
-
-  def __call__(self, op):
-    if hasattr(op, 'translate'):
-      if self._dargs.get('copy', False):
-        return op.copy().union(op.translate(*self._largs, **self._dargs))
-      else:
-        return op.translate(*self._largs, **self._dargs)
-    elif len(self._largs) == 2 and len(self._dargs) == 0:
-      self._dx = self._largs[0]
-      self._dy = self._largs[1]
-    elif (len(self._largs) == 0
-          and len(self._dargs) == 2
-          and 'dx' in self._dargs
-          and 'dy' in self._dargs):
-      self._dx = self._dargs['dx']
-      self._dy = self._dargs['dy']
-    else:
-      raise ValueError("Invalid translator instanciation.")
-    if 'copy' in dargs:
-      raise ValueError('"copy" may only be specified when translating shapes.')
-    return (op[0]+self._dx, op[1]+self._dy)
 
 class Grower:
   def __init__(self, d):
     self._d = d
 
   def __call__(self, op):
     return op.grow(self._d)
 
-
 class Rounder:
   def __init__(self, r):
     self._r = r
 
   def __call__(self, op):
     return op.roundCorners(self._r)
```

### Comparing `polyp-1.1.1/polyp/plotting.py` & `polyp-1.1.2/polyp/plotting.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.1/polyp/plsscript.py` & `polyp-1.1.2/polyp/plsscript.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.1/polyp/utils.py` & `polyp-1.1.2/polyp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,16 @@
         currentArglist = [makeLiteral(dargs['start'])]
         while True:
           self._arglist.append(currentArglist)
           currentArglist = [[currentArglist[0][0], currentArglist[0][1] + dargs['step']]]
           if currentArglist[0][1] > dargs['stop']:
             break
 
-    elif len(largs) > 0 or len(dargs) > 0:
-      raise ValueError("Invalid arguments in parametric function call.")
+    elif len(dargs) > 0:
+      raise ValueError("Invalid arguments in parametric function call, expect 'start', 'step' and 'stop'.")
 
   def _isNum(self, v):
     return type(v) is float or type(v) is int
 
   def _toNum(self, v):
     if type(v) is str and len(v) == 1 and v.lower() in self._letters:
       return self._letters.index(v.lower())
```

### Comparing `polyp-1.1.1/polyp.egg-info/PKG-INFO` & `polyp-1.1.2/polyp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: polyp
-Version: 1.1.1
+Version: 1.1.2
 Summary: A renderer that creates gdsII files from an all-ascii human-readble layout language 
 Author: zaphB
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Human-Readble-Ascii to gdsII Converter
 
-Polyp is a renderer that creates gdsII layout files from an all-ascii human-readble layout language. Geometric shapes are constructed from primitive shapes, e.g., squares, circles or text, that are translated, rotated, scaled or otherwise transformed and can be added, subtracted or intersected with each other.
+Polyp is a renderer that creates gdsII layout files from an all-ascii human-readable layout language. Geometric shapes are constructed from primitive shapes, e.g., squares, circles or text, that are translated, rotated, scaled or otherwise transformed and can be added, subtracted or intersected with each other.
 
 Polyp is definitely interesting for you if you
 * are not afraid of using the command line
 * have experience with drawing gdsII files
 * are a fan of mark-up languages
 
 Polyp is probably not for you if you
 * prefer manually drawing geometry
-* fell uncomfortable using the command line
+* feel uncomfortable using the command line
 
 A minimal example is shown in the following:
 
 ```
 SYMBOL main
   LAYER 0
     rect(10).rotate(45) - text("hello world", dy=3)
@@ -40,26 +40,26 @@
 
 Install polyp and its dependencies with
 
 ```
 pip install polyp
 ```
 
-Executing `polyp -h` on the shell should now show the polyp quick help, `polyp --ersion` should show the expected version number.
+Executing `polyp -h` on the shell should now show the polyp quick help, `polyp --version` should show the expected version number.
 
 
 # Basic usage
 
 To compile a .pls polyp layout script to a .gds file, run `polyp filename`, where `filename` has to be replaced with the path of the .pls file.
 
-Passing the `-v` option (`polyp -v filename`) compiles the layout script and opens a simple viewer afterwards.
+Passing the `-v` (`--view`) option (`polyp -v filename`) compiles the layout script and opens a simple viewer afterwards.
 
-Passing the `-w` option keeps checkign the .pls file for updates, recompiles it in case a change in the file is detected and keeps the compiled result open in a viewer.
+Passing the `-w` (`--watch`) option keeps checking the .pls file for updates, re-compiles in case a change in the file is detected and keeps the compiled result open in a viewer.
 
-If the `-p` option is passed to polyp, the layout script is compiled to .pdf instead of .gds. One pdf file is created for each gdsII symbol.
+If the `-p` (`--pdf`) option is passed to polyp, the layout script is compiled to .pdf instead of .gds. One pdf file is created for each gdsII symbol.
 
 
 # Examples
 
 This list of examples starts from a minimal .pls example and moves to more and more complex layout scripts step by step. A formal documentation of the polyp layout language is currently not available, feel free to contact me or open an issue in case this is needed.
 
 
@@ -143,15 +143,22 @@
 Translate supports the optional boolean arguement `copy`, which if set to true, causes the untranslated shape to be kept in the result, e.g. `rect(10).translate(0, 20, copy=True)`.
 
 
 ### Rotate
 
 To rotate a square by 30 degrees, use `rect(10).rotate(30)`. Optionally, the center of rotation can be specified as a second parameter: `rect(10).rotate(30, [0, 10])`. By default, the center of rotation is given by the center of mass of the rotated geometry.
 
-Rotate supports the optional boolean arguement `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
+Rotate supports the optional boolean argument `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
+
+
+### Scale
+
+To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `a1`.
+
+Scale supports the optional boolean argument `copy`, which if set to true, causes the unscaled shape to be kept in the result, e.g. `rect(10).scale(3, center=[0,0], copy=True)`.
 
 
 ### Mirror
 
 To mirror a geometry at a given point or line, use the `.mirror(...)`. The following example shows three different ways of calling the method:
 
 ```
@@ -196,19 +203,19 @@
 ```
 
 ### Calculating height, width, bounding box and center of mass
 
 The functions `height(...)` and `width(...)` return the height and width of the shape that is passed as an argument. For example `height(rect(10))` returns 10. The function `bb(...)` returns the bounding box of a shape. The function `center(...)` returns a shapes center of mass.
 
 
-### Mathematical functions
+### Math
 
 The trigonometric functions and there inverse functions are available as `cos`, `sin`, `tan`, `asin`, `acos`, `atan`. Angles are given in units of degrees. The function `atan2` is a variant of `atan` that uses two arguments and is able to handle the full circle. See the numpy documentation of `atan2` for further details.
 
-The function `abs(...)` returns the absolute value of the passed number. The functions `min`, `max` and `mean` return the minimum, maximum or arithmetical mean of the passed list of numbers.
+The function `abs(...)` returns the absolute value of the passed number, `sqrt(...)` returns the square root. The functions `min`, `max` and `mean` return the minimum, maximum or arithmetical mean of the passed list of numbers.
 
 
 ### Type conversions
 
 Use `int(...)` to convert a number to integer. Use `char(...)` to convert an integer number to the respective letter of the alphabet.
 
 
@@ -405,12 +412,12 @@
 SYMBOL main
   LAYER 0
     wire(*optsA)
   LAYER 1
     wire(*optsB)
 ```
 
-The unary `*` operator applied to objects unpacks the obect into a parameter list. This way it is not necessary to write down all argument names anymore, which is helpful in layouts with many free parameters.
+The unary `*` operator applied to objects unpacks the object into a parameter list. This way it is not necessary to write down all argument names anymore, which is helpful in layouts with many free parameters.
 
 ## QR codes
 
 The `qrcode` native creates a qr code geometry from a given string. The optional named parameters `dx` and `dy` specify the size of the resulting code in x and y directions. With the `robust` parameter (1...4, higher=more robust, default 2) the redundancy in the generated code can be adjusted. The `res` parameter controls the number of "pixels" used in the qrcode. By default, the `res` is automatically chosen according to the input string.
```

