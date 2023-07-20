# Comparing `tmp/var_print-0.0.5.tar.gz` & `tmp/var_print-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "var_print-0.0.5.tar", last modified: Sun Jun 18 17:44:48 2023, max compression
+gzip compressed data, was "var_print-0.0.6.tar", last modified: Thu Jul 20 17:16:48 2023, max compression
```

## Comparing `var_print-0.0.5.tar` & `var_print-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 17:44:47.999219 var_print-0.0.5/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 var_print-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      159 2023-01-07 18:55:43.000000 var_print-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5750 2023-06-18 17:44:47.997969 var_print-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2023-01-07 18:59:14.000000 var_print-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-18 17:44:47.999219 var_print-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1803 2023-06-18 17:43:36.000000 var_print-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:44:47.986747 var_print-0.0.5/var_print/
--rw-rw-rw-   0        0        0       63 2023-06-18 17:43:37.000000 var_print-0.0.5/var_print/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:44:47.995683 var_print-0.0.5/var_print/data/
--rw-rw-rw-   0        0        0     6221 2023-01-07 18:45:09.000000 var_print-0.0.5/var_print/data/color_schemes.pickle
--rw-rw-rw-   0        0        0    35982 2023-06-18 17:42:21.000000 var_print-0.0.5/var_print/varPrint.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:44:47.993496 var_print-0.0.5/var_print.egg-info/
--rw-rw-rw-   0        0        0     5750 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 17:16:48.473708 var_print-0.0.6/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 var_print-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      159 2023-01-07 18:55:43.000000 var_print-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5750 2023-07-20 17:16:48.472709 var_print-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2023-01-07 18:59:14.000000 var_print-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 17:16:48.473708 var_print-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1803 2023-07-20 17:12:18.000000 var_print-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:16:48.463940 var_print-0.0.6/var_print/
+-rw-rw-rw-   0        0        0       78 2023-07-20 17:12:11.000000 var_print-0.0.6/var_print/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:16:48.471708 var_print-0.0.6/var_print/data/
+-rw-rw-rw-   0        0        0     6221 2023-01-07 18:45:09.000000 var_print-0.0.6/var_print/data/color_schemes.pickle
+-rw-rw-rw-   0        0        0    36696 2023-07-20 17:11:32.000000 var_print-0.0.6/var_print/varPrint.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:16:48.469709 var_print-0.0.6/var_print.egg-info/
+-rw-rw-rw-   0        0        0     5750 2023-07-20 17:16:48.000000 var_print-0.0.6/var_print.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-20 17:16:48.000000 var_print-0.0.6/var_print.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 17:16:48.000000 var_print-0.0.6/var_print.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-20 17:16:48.000000 var_print-0.0.6/var_print.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-20 17:16:48.000000 var_print-0.0.6/var_print.egg-info/top_level.txt
```

### Comparing `var_print-0.0.5/LICENSE` & `var_print-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `var_print-0.0.5/PKG-INFO` & `var_print-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: var_print
-Version: 0.0.5
+Version: 0.0.6
 Summary: Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. 
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `var_print-0.0.5/README.md` & `var_print-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `var_print-0.0.5/setup.py` & `var_print-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. "
 
 # Setting up
 setup(
     name="var_print",
     version=VERSION,
     author="André Herber",
```

### Comparing `var_print-0.0.5/var_print/data/color_schemes.pickle` & `var_print-0.0.6/var_print/data/color_schemes.pickle`

 * *Files identical despite different names*

### Comparing `var_print-0.0.5/var_print/varPrint.py` & `var_print-0.0.6/var_print/varPrint.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,32 @@
 
 def pickle_unpack(path):
     with open(path, "rb") as f:
         data = pickle.load(f)
     return data
 
 
+def get_var_names(*args):
+    frame = 1
+    if frame == 1:
+        callFrame = inspect.currentframe().f_back
+    elif frame == 2:
+        callFrame = inspect.currentframe().f_back.f_back
+    elif frame == 3:
+        callFrame = inspect.currentframe().f_back.f_back.f_back
+    else:
+        raise ValueError("frame geht nur bis 3")
+    callNode = Source.executing(callFrame).node
+    if callNode is None:
+        raise NoSourceAvailableError()
+    source = Source.for_frame(callFrame)
+    sanitizedArgStrs = [source.get_text_with_indentation(arg) for arg in callNode.args]
+    return sanitizedArgStrs
+
+
 class VarPrintColors:
     CYAN_YELLOW = {
         "name": "CYAN_YELLOW",
         "varname_rgb": (0, 255, 255),
         "value_rgb": (255, 255, 0),
         "name_value_sep_rgb": (200, 200, 200),
         "comma_rgb": (200, 200, 200),
@@ -290,15 +308,14 @@
         self.deactivated = False
 
     def deactivate(self):
         self.deactivated = True
 
     def __call__(self, *vars) -> None:
         if not self.deactivated:
-
             try:
                 var_names = self.get_var_names()
             except:
                 var_names = [f"{type(v)}" for v in vars]
 
             kwargs = {k: vars[i] for (i, k) in enumerate(var_names)}
 
@@ -311,31 +328,29 @@
             for i, line in enumerate(out.split("\n")):
                 if i < l:
                     print(line)
                 else:
                     colored_print(line)
 
     def get_var_names(self, frame=2):
-        match frame:
-            case 1:
-                callFrame = inspect.currentframe().f_back
-            case 2:
-                callFrame = inspect.currentframe().f_back.f_back
-            case 3:
-                callFrame = inspect.currentframe().f_back.f_back.f_back
-            case _:
-                raise ValueError("frame geht nur bis 3")
+        if frame == 1:
+            callFrame = inspect.currentframe().f_back
+        elif frame == 2:
+            callFrame = inspect.currentframe().f_back.f_back
+        elif frame == 3:
+            callFrame = inspect.currentframe().f_back.f_back.f_back
+        else:
+            raise ValueError("frame geht nur bis 3")
         callNode = Source.executing(callFrame).node
         if callNode is None:
             raise NoSourceAvailableError()
         source = Source.for_frame(callFrame)
         sanitizedArgStrs = [
             source.get_text_with_indentation(arg) for arg in callNode.args
         ]
-
         return sanitizedArgStrs
 
     def format_value(self, value, indent, recursion_level: int = -1):
         def iters_new_line_if_needed(index, total, ide, iipl, k_auf, v_type=str):
             k_auf_space = " " * len(k_auf)
             if (index + 1) % iipl == 0 and index != total - 1:
                 return f"\n{ide}{k_auf_space}"
@@ -481,14 +496,16 @@
             pref = ""
             iipl = self.iter_items_per_line
 
             if type(liste) == list:
                 k_auf, k_zu = "[", "]"
             elif type(liste) == tuple:
                 k_auf, k_zu = "(", ")"
+                if len(liste) == 1:
+                    k_zu = ",)"
             elif type(liste) == set:
                 k_auf, k_zu = "{", "}"
             elif type(liste) == frozenset:
                 pref = "frozenset"
                 k_auf, k_zu = "({", "})"
             elif type(liste) == GeneratorType:
                 pref = "generator"
@@ -1015,8 +1032,11 @@
 
 varp = VariableNameAndValuePrinter()
 
 if __name__ == "__main__":
     # varp.show_formating_of_different_types()
 
     test = "test"
+    test = ("test")
+    varp(test)
+    test = ("test",)
     varp(test)
```

### Comparing `var_print-0.0.5/var_print.egg-info/PKG-INFO` & `var_print-0.0.6/var_print.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: var-print
-Version: 0.0.5
+Version: 0.0.6
 Summary: Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. 
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

