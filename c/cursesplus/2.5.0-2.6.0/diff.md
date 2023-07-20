# Comparing `tmp/cursesplus-2.5.0.tar.gz` & `tmp/cursesplus-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.5.0.tar", last modified: Sat Jul 15 21:29:39 2023, max compression
+gzip compressed data, was "cursesplus-2.6.0.tar", last modified: Thu Jul 20 15:56:49 2023, max compression
```

## Comparing `cursesplus-2.5.0.tar` & `cursesplus-2.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 21:29:39.116721 cursesplus-2.5.0/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.5.0/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1176 2023-07-15 21:29:39.116721 cursesplus-2.5.0/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      573 2023-07-15 21:27:06.000000 cursesplus-2.5.0/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-07-15 21:26:24.000000 cursesplus-2.5.0/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-07-15 21:29:39.116721 cursesplus-2.5.0/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 21:29:39.106721 cursesplus-2.5.0/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      545 2023-07-15 21:14:23.000000 cursesplus-2.5.0/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 21:29:39.116721 cursesplus-2.5.0/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.5.0/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18822 2023-07-15 21:23:54.000000 cursesplus-2.5.0/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-07-15 20:49:42.000000 cursesplus-2.5.0/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     9323 2023-07-15 20:50:21.000000 cursesplus-2.5.0/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 21:29:39.116721 cursesplus-2.5.0/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1176 2023-07-15 21:29:39.000000 cursesplus-2.5.0/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-07-15 21:29:39.000000 cursesplus-2.5.0/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-07-15 21:29:39.000000 cursesplus-2.5.0/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-07-15 21:29:39.000000 cursesplus-2.5.0/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-20 15:56:49.009852 cursesplus-2.6.0/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.6.0/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1299 2023-07-20 15:56:49.009852 cursesplus-2.6.0/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      696 2023-07-20 15:56:29.000000 cursesplus-2.6.0/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-07-20 15:55:46.000000 cursesplus-2.6.0/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-07-20 15:56:49.009852 cursesplus-2.6.0/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-20 15:56:49.009852 cursesplus-2.6.0/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      450 2023-07-20 15:54:19.000000 cursesplus-2.6.0/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-20 15:56:49.009852 cursesplus-2.6.0/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.6.0/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    19567 2023-07-20 15:55:11.000000 cursesplus-2.6.0/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-07-15 20:49:42.000000 cursesplus-2.6.0/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     9323 2023-07-15 20:50:21.000000 cursesplus-2.6.0/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-20 15:56:49.009852 cursesplus-2.6.0/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1299 2023-07-20 15:56:48.000000 cursesplus-2.6.0/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-07-20 15:56:48.000000 cursesplus-2.6.0/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-07-20 15:56:48.000000 cursesplus-2.6.0/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-07-20 15:56:48.000000 cursesplus-2.6.0/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.5.0/LICENSE` & `cursesplus-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.5.0/PKG-INFO` & `cursesplus-2.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.5.0
+Version: 2.6.0
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,22 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
+### Version 2.6: Numericinput
+
+-Add numericinput() function
+
+-Configurable to allow negatives and decimals
+
+-Number input
+
 ### Version 2.5: Please Wait
 
 -Add PleaseWait() class
 
 -It plays an animated timer for long tasks
 
 ## Uses
```

### Comparing `cursesplus-2.5.0/pyproject.toml` & `cursesplus-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.5.0"
+version = "2.6.0"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.5.0/src/cursesplus/__init__.py` & `cursesplus-2.6.0/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.5.0/src/cursesplus/cp.py` & `cursesplus-2.6.0/src/cursesplus/cp.py`

 * *Files 3% similar despite different names*

```diff
@@ -357,14 +357,36 @@
     """Hide Cursor. Can only be called in an active curses window"""
     curses.curs_set(0)
 
 def showcursor():
     """Show cursor. Can only be called in an active curses window"""
     curses.curs_set(1)
 
+def numericinput(stdscr,message="Please input a number",allowdecimals=False,allownegatives=False) -> float:
+    while True:
+        strrepr = cursesinput(stdscr,message,maxlen=12)
+        if len(strrepr) == 0 or (allownegatives and strrepr[0] == "-" and len(strrepr) < 2):
+            curses.beep()
+            continue
+        if not allownegatives and strrepr[0] == "-":
+            curses.beep()
+            continue
+        if not allowdecimals:
+            try:
+                return int(strrepr)
+            except:
+                curses.beep()
+                continue
+        else:
+            try:
+                return float(strrepr)
+            except:
+                curses.beep()
+                continue
+
 class PleaseWaitScreen:
     def __init__(self,stdscr,message=["Please Wait"]):
         self.message = message + [""]
         self.screen = stdscr
         self.tick = 0
         self.stopped = False
     def _update(self):
```

### Comparing `cursesplus-2.5.0/src/cursesplus/filedialog.py` & `cursesplus-2.6.0/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.5.0/src/cursesplus/messagebox.py` & `cursesplus-2.6.0/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.5.0/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.6.0/src/cursesplus.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.5.0
+Version: 2.6.0
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,22 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
+### Version 2.6: Numericinput
+
+-Add numericinput() function
+
+-Configurable to allow negatives and decimals
+
+-Number input
+
 ### Version 2.5: Please Wait
 
 -Add PleaseWait() class
 
 -It plays an animated timer for long tasks
 
 ## Uses
```

