# Comparing `tmp/polyp-1.1.2.tar.gz` & `tmp/polyp-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyp-1.1.2.tar", last modified: Thu Jul 20 16:41:33 2023, max compression
+gzip compressed data, was "polyp-1.1.4.tar", last modified: Thu Jul 20 19:06:28 2023, max compression
```

## Comparing `polyp-1.1.2.tar` & `polyp-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 16:41:33.757659 polyp-1.1.2/
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1067 2023-07-19 14:22:28.000000 polyp-1.1.2/LICENSE.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)    20131 2023-07-20 16:41:33.757659 polyp-1.1.2/PKG-INFO
--rw-r--r--   0 bredol    (1000) bredol    (1000)    19907 2023-07-20 16:36:14.000000 polyp-1.1.2/README.md
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 16:41:33.757659 polyp-1.1.2/polyp/
--rw-r--r--   0 bredol    (1000) bredol    (1000)      309 2022-06-27 10:39:37.000000 polyp-1.1.2/polyp/__init__.py
--rwxr-xr-x   0 bredol    (1000) bredol    (1000)     4144 2023-07-19 14:22:28.000000 polyp-1.1.2/polyp/__main__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    43537 2023-07-20 16:04:18.000000 polyp-1.1.2/polyp/calltree.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    27988 2022-06-27 10:39:37.000000 polyp-1.1.2/polyp/fonts.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    17142 2023-07-20 16:30:33.000000 polyp-1.1.2/polyp/geometry.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     2269 2023-07-19 14:22:28.000000 polyp-1.1.2/polyp/plotting.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    17681 2023-07-19 14:22:28.000000 polyp-1.1.2/polyp/plsscript.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     4666 2023-07-20 16:21:20.000000 polyp-1.1.2/polyp/utils.py
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 16:41:33.757659 polyp-1.1.2/polyp.egg-info/
--rw-r--r--   0 bredol    (1000) bredol    (1000)    20131 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/PKG-INFO
--rw-r--r--   0 bredol    (1000) bredol    (1000)      345 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/SOURCES.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)        1 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/dependency_links.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       46 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/entry_points.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       30 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/requires.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)        6 2023-07-20 16:41:33.000000 polyp-1.1.2/polyp.egg-info/top_level.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       38 2023-07-20 16:41:33.757659 polyp-1.1.2/setup.cfg
--rwxr-xr-x   0 bredol    (1000) bredol    (1000)      753 2023-07-20 16:41:25.000000 polyp-1.1.2/setup.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 19:06:28.063978 polyp-1.1.4/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1067 2023-07-19 14:22:28.000000 polyp-1.1.4/LICENSE.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    20131 2023-07-20 19:06:28.063978 polyp-1.1.4/PKG-INFO
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    19907 2023-07-20 16:44:30.000000 polyp-1.1.4/README.md
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 19:06:28.063978 polyp-1.1.4/polyp/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      309 2022-06-27 10:39:37.000000 polyp-1.1.4/polyp/__init__.py
+-rwxr-xr-x   0 bredol    (1000) bredol    (1000)     4137 2023-07-20 18:14:14.000000 polyp-1.1.4/polyp/__main__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    43537 2023-07-20 16:04:18.000000 polyp-1.1.4/polyp/calltree.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    27988 2022-06-27 10:39:37.000000 polyp-1.1.4/polyp/fonts.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    17142 2023-07-20 16:30:33.000000 polyp-1.1.4/polyp/geometry.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     2269 2023-07-19 14:22:28.000000 polyp-1.1.4/polyp/plotting.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    17657 2023-07-20 18:23:56.000000 polyp-1.1.4/polyp/plsscript.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4666 2023-07-20 16:21:20.000000 polyp-1.1.4/polyp/utils.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2023-07-20 19:06:28.063978 polyp-1.1.4/polyp.egg-info/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    20131 2023-07-20 19:06:28.000000 polyp-1.1.4/polyp.egg-info/PKG-INFO
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      345 2023-07-20 19:06:28.000000 polyp-1.1.4/polyp.egg-info/SOURCES.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        1 2023-07-20 19:06:28.000000 polyp-1.1.4/polyp.egg-info/dependency_links.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       46 2023-07-20 19:06:28.000000 polyp-1.1.4/polyp.egg-info/entry_points.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       30 2023-07-20 19:06:28.000000 polyp-1.1.4/polyp.egg-info/requires.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        6 2023-07-20 19:06:28.000000 polyp-1.1.4/polyp.egg-info/top_level.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       38 2023-07-20 19:06:28.063978 polyp-1.1.4/setup.cfg
+-rwxr-xr-x   0 bredol    (1000) bredol    (1000)      753 2023-07-20 19:06:21.000000 polyp-1.1.4/setup.py
```

### Comparing `polyp-1.1.2/LICENSE.txt` & `polyp-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polyp-1.1.2/PKG-INFO` & `polyp-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyp
-Version: 1.1.2
+Version: 1.1.4
 Summary: A renderer that creates gdsII files from an all-ascii human-readble layout language 
 Author: zaphB
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Human-Readble-Ascii to gdsII Converter
 
@@ -148,15 +148,15 @@
 To rotate a square by 30 degrees, use `rect(10).rotate(30)`. Optionally, the center of rotation can be specified as a second parameter: `rect(10).rotate(30, [0, 10])`. By default, the center of rotation is given by the center of mass of the rotated geometry.
 
 Rotate supports the optional boolean argument `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
 
 
 ### Scale
 
-To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `a1`.
+To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `s1`.
 
 Scale supports the optional boolean argument `copy`, which if set to true, causes the unscaled shape to be kept in the result, e.g. `rect(10).scale(3, center=[0,0], copy=True)`.
 
 
 ### Mirror
 
 To mirror a geometry at a given point or line, use the `.mirror(...)`. The following example shows three different ways of calling the method:
```

### Comparing `polyp-1.1.2/README.md` & `polyp-1.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 To rotate a square by 30 degrees, use `rect(10).rotate(30)`. Optionally, the center of rotation can be specified as a second parameter: `rect(10).rotate(30, [0, 10])`. By default, the center of rotation is given by the center of mass of the rotated geometry.
 
 Rotate supports the optional boolean argument `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
 
 
 ### Scale
 
-To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `a1`.
+To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `s1`.
 
 Scale supports the optional boolean argument `copy`, which if set to true, causes the unscaled shape to be kept in the result, e.g. `rect(10).scale(3, center=[0,0], copy=True)`.
 
 
 ### Mirror
 
 To mirror a geometry at a given point or line, use the `.mirror(...)`. The following example shows three different ways of calling the method:
```

### Comparing `polyp-1.1.2/polyp/__main__.py` & `polyp-1.1.4/polyp/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import gdspy
 import threading
 import signal
 import os
 import time
 import traceback
-import re
 import polyp
 import sys
 
 
 def main():
   if '--version' in sys.argv:
     print(f'polyp version {polyp.__version__}')
@@ -59,15 +58,15 @@
 
             if lasthash != script.hash:
               currentLibMtl[0] = gdspy.current_library
               time.sleep(2)
               lasthash = script.hash
 
               if not args.no_output:
-                script.writeResults(re.sub('\.[^\.]*$', '', args.layout.name)+'.'+suffix)
+                script.writeResults('.'.join(args.layout.name.split('.')[:-1])+'.'+suffix)
 
               if not thr or not thr.is_alive():
                 thr = threading.Thread(target=script.openViewer, args=(currentLibMtl,))
                 thr.start()
 
               print(' > Successful.')
               parseTime = time.time() - started
@@ -97,15 +96,15 @@
       currentLibMtl[1] = True
       if thr and thr.is_alive():
         thr.join()
 
     else:
       script = polyp.plsscript.PlsScript(args.layout, args.force_rerender)
       if not args.no_output:
-        script.writeResults(re.sub('\.[^\.]*$', '', args.layout.name)+"."+suffix)
+        script.writeResults('.'.join(args.layout.name.split('.')[:-1])+'.'+suffix)
       if args.view:
         script.openViewer()
 
   except Exception as e:
     if args.watch:
       print("Warning: watching not supported for .gds files.")
 
@@ -113,15 +112,15 @@
       gds = gdspy.GdsLibrary()
       path = args.layout.name
       args.layout.close()
       gds.read_gds(path)
       script = polyp.plsscript.PlsScript()
       script.gdsLib = gds
       if not args.no_output and suffix != 'gds':
-        script.writeResults(re.sub('\.[^\.]*$', '', args.layout.name)+"."+suffix)
+        script.writeResults('.'.join(args.layout.name.split('.')[:-1])+'.'+suffix)
       if args.view:
         script.openViewer()
     except:
       raise e
 
 if __name__ == "__main__":
   main()
```

### Comparing `polyp-1.1.2/polyp/calltree.py` & `polyp-1.1.4/polyp/calltree.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.2/polyp/fonts.py` & `polyp-1.1.4/polyp/fonts.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.2/polyp/geometry.py` & `polyp-1.1.4/polyp/geometry.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.2/polyp/plotting.py` & `polyp-1.1.4/polyp/plotting.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.2/polyp/plsscript.py` & `polyp-1.1.4/polyp/plsscript.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         if not _re.match("\s*#", line):
           _text += line + "\n"
       text = _text
 
     def getCachedPath(path):
       if not path:
         return ''
-      filename = '.'.join(self.path.split('/')[-1].split('.')[:-1])
-      basedir = '/'.join(self.path.split('/')[:-1])
-      return basedir+'/.'+filename+'.plb'
+      base, fname = _os.path.split(path)
+      fname = '.'.join(fname.split('.')[:-1])
+      return _os.path.join(base, '.'+fname+'.plb')
 
     def isPathCached(path, newerThan=0):
       if forceRerender:
         return False
       cachedPath = getCachedPath(path)
       return (_os.path.exists(cachedPath)
           and _os.path.getmtime(path) < _os.path.getmtime(cachedPath)
```

### Comparing `polyp-1.1.2/polyp/utils.py` & `polyp-1.1.4/polyp/utils.py`

 * *Files identical despite different names*

### Comparing `polyp-1.1.2/polyp.egg-info/PKG-INFO` & `polyp-1.1.4/polyp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyp
-Version: 1.1.2
+Version: 1.1.4
 Summary: A renderer that creates gdsII files from an all-ascii human-readble layout language 
 Author: zaphB
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Human-Readble-Ascii to gdsII Converter
 
@@ -148,15 +148,15 @@
 To rotate a square by 30 degrees, use `rect(10).rotate(30)`. Optionally, the center of rotation can be specified as a second parameter: `rect(10).rotate(30, [0, 10])`. By default, the center of rotation is given by the center of mass of the rotated geometry.
 
 Rotate supports the optional boolean argument `copy`, which if set to true, causes the unrotated shape to be kept in the result, e.g. `rect(10).rotate(120, copy=True)`.
 
 
 ### Scale
 
-To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `a1`.
+To scale a shape, use `.scale(s1, s2, center)`, where `s1` is the scale factor in x-direction, `s2` is the scale factor in y-direction and `center` is the reference point of the scaling. If `center` is omitted, the center of mass of the shape is used. If `s2` is omitted, both directions will be scaled by `s1`.
 
 Scale supports the optional boolean argument `copy`, which if set to true, causes the unscaled shape to be kept in the result, e.g. `rect(10).scale(3, center=[0,0], copy=True)`.
 
 
 ### Mirror
 
 To mirror a geometry at a given point or line, use the `.mirror(...)`. The following example shows three different ways of calling the method:
```

### Comparing `polyp-1.1.2/setup.py` & `polyp-1.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 setup(name='polyp',
       description='A renderer that creates gdsII files from an '
                   'all-ascii human-readble layout language ',
       long_description=description,
       long_description_content_type='text/markdown',
       author='zaphB',
-      version='1.1.2',
+      version='1.1.4',
       packages=['polyp'],
       entry_points={
         'console_scripts': [
           'polyp = polyp.__main__:main'
         ],
         'gui_scripts': []
       },
```

