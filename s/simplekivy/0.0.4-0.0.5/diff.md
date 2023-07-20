# Comparing `tmp/simplekivy-0.0.4.tar.gz` & `tmp/simplekivy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplekivy-0.0.4.tar", last modified: Sun Jul 16 12:32:23 2023, max compression
+gzip compressed data, was "simplekivy-0.0.5.tar", last modified: Thu Jul 20 16:19:01 2023, max compression
```

## Comparing `simplekivy-0.0.4.tar` & `simplekivy-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-16 12:32:23.277637 simplekivy-0.0.4/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1058 2023-07-13 13:38:06.000000 simplekivy-0.0.4/LICENSE
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4691 2023-07-16 12:32:23.277637 simplekivy-0.0.4/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4139 2023-07-16 12:25:53.000000 simplekivy-0.0.4/README.md
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-16 12:21:27.000000 simplekivy-0.0.4/pyproject.toml
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-16 12:32:23.277637 simplekivy-0.0.4/setup.cfg
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-16 12:32:23.277637 simplekivy-0.0.4/simplekivy/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.4/simplekivy/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      912 2023-07-16 11:59:18.000000 simplekivy-0.0.4/simplekivy/simplekivy.py
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-16 12:32:23.277637 simplekivy-0.0.4/simplekivy/widgets/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       37 2023-07-16 11:58:18.000000 simplekivy-0.0.4/simplekivy/widgets/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2849 2023-07-16 11:57:21.000000 simplekivy-0.0.4/simplekivy/widgets/app.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.4/simplekivy/widgets/main.kv
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-16 12:32:23.277637 simplekivy-0.0.4/simplekivy.egg-info/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4691 2023-07-16 12:32:23.000000 simplekivy-0.0.4/simplekivy.egg-info/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-16 12:32:23.000000 simplekivy-0.0.4/simplekivy.egg-info/SOURCES.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-16 12:32:23.000000 simplekivy-0.0.4/simplekivy.egg-info/dependency_links.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-16 12:32:23.000000 simplekivy-0.0.4/simplekivy.egg-info/top_level.txt
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-20 16:19:01.579148 simplekivy-0.0.5/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1058 2023-07-13 13:38:06.000000 simplekivy-0.0.5/LICENSE
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3383 2023-07-20 16:19:01.579148 simplekivy-0.0.5/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2830 2023-07-20 16:18:11.000000 simplekivy-0.0.5/README.md
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-20 16:10:44.000000 simplekivy-0.0.5/pyproject.toml
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-20 16:19:01.579148 simplekivy-0.0.5/setup.cfg
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-20 16:19:01.579148 simplekivy-0.0.5/simplekivy/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.5/simplekivy/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      912 2023-07-16 11:59:18.000000 simplekivy-0.0.5/simplekivy/simplekivy.py
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-20 16:19:01.579148 simplekivy-0.0.5/simplekivy/widgets/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       37 2023-07-16 11:58:18.000000 simplekivy-0.0.5/simplekivy/widgets/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3222 2023-07-20 16:06:46.000000 simplekivy-0.0.5/simplekivy/widgets/app.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.5/simplekivy/widgets/main.kv
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-20 16:19:01.579148 simplekivy-0.0.5/simplekivy.egg-info/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3383 2023-07-20 16:19:01.000000 simplekivy-0.0.5/simplekivy.egg-info/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-20 16:19:01.000000 simplekivy-0.0.5/simplekivy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-20 16:19:01.000000 simplekivy-0.0.5/simplekivy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-20 16:19:01.000000 simplekivy-0.0.5/simplekivy.egg-info/top_level.txt
```

### Comparing `simplekivy-0.0.4/LICENSE` & `simplekivy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.4/pyproject.toml` & `simplekivy-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "simplekivy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="yousuf", email="yosefmahmoud356@gmail.com" },
 ]
 description = "the idea is inspired by PySimpleGui , to quickly create simple kivy apps "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplekivy-0.0.4/simplekivy/simplekivy.py` & `simplekivy-0.0.5/simplekivy/simplekivy.py`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.4/simplekivy/widgets/app.py` & `simplekivy-0.0.5/simplekivy/widgets/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,35 +7,44 @@
 file_path = os.path.abspath(os.path.dirname(__file__))
 print(file_path)
 Builder.load_file(os.path.join(file_path, "main.kv"))
 
 
 class AppMethods:
     def freeze(self, wid, parent = None):
+        type_wid = type(wid)
+        
         #list for boxlayout
-        if type(wid) is list:
+        if type_wid is list:
             parent = F.BoxLayout(orientation="horizontal")
             self.row_widget_adder(wid, parent)
             return parent
         #tuple for floatlayout
-        elif type(wid) is tuple:
+        elif type_wid is tuple:
             parent = F.FloatLayout()
             self.row_widget_adder(wid, parent) 
             return parent
 
-        elif type(wid) is dict:
+        elif type_wid is dict:
             if parent:
                 self.row_widget_adder([wid], parent)
 
             else:
                 widgets = self.row_widget_adder([wid])
                 return widgets
             
-    
-        elif type(wid) is str:
+        elif type_wid is set:
+            
+            if not parent:
+                return wid
+            for i in wid:
+                if parent:
+                    self.row_widget_adder([i], parent)
+
+        elif type_wid is str:
             widget = Builder.load_string(wid)
             return widget
 
         else:
             return wid
             
         
@@ -49,16 +58,16 @@
         except TypeError:
             parent.add_widget(widget) 
 
     def row_widget_adder(self, widofmainlist, parent=None):
         if not parent:
             dict_keys = []
         for item in widofmainlist:
-        
-            if type(item) is dict:
+            item_type = type(item)
+            if item_type is dict:
                 items = item.copy().items()
                 for key, value in items:
                     if type(key) is not str :
                         try:keyI = key()  #keyI => keyInstance
                         except: keyI = key
                         wid = self.freeze(value, parent = keyI)
                         if wid:
@@ -70,27 +79,32 @@
                             dict_keys.append(keyI)
 
                         del item[key]
 
                 parent.__init__(**item)
                 if not parent:
                     return dict_keys
-            elif type(item) in (list, tuple, str):
+            elif item_type in (list, tuple, str):
                 wid = self.freeze(item)
                 self.add_to_widget(wid, parent)
+
+            elif item_type is set:
+                self.freeze(item, parent=parent)
+                    
+
             else:self.add_to_widget(item, parent)
 
 
 class MainApp(App, AppMethods):
     widgets = []
     def on_start(self):
         for widofmainlist in self.widgets:
             if type(widofmainlist) in (list, tuple,  str):
                 wid = self.freeze(widofmainlist)
                 self.add_to_root(wid)
 
-            elif type(widofmainlist) is dict:
+            elif type(widofmainlist) is dict or set:
                 self.freeze(widofmainlist, parent=self.root)
             else:
                 self.add_to_root(widofmainlist)
```

