# Comparing `tmp/pynamicui-0.0.7.tar.gz` & `tmp/pynamicui-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamicui-0.0.7.tar", last modified: Wed Jul 19 05:30:43 2023, max compression
+gzip compressed data, was "pynamicui-0.0.8.tar", last modified: Thu Jul 20 19:11:31 2023, max compression
```

## Comparing `pynamicui-0.0.7.tar` & `pynamicui-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 05:30:43.749240 pynamicui-0.0.7/
--rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5792 2023-07-19 05:30:43.746238 pynamicui-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5309 2023-07-19 05:29:04.000000 pynamicui-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 05:30:43.681636 pynamicui-0.0.7/pynamicui/
--rw-rw-rw-   0        0        0      318 2023-07-19 05:29:37.000000 pynamicui-0.0.7/pynamicui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:30:43.730586 pynamicui-0.0.7/pynamicui/createDom/
--rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.7/pynamicui/createDom/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-07-19 05:26:39.000000 pynamicui-0.0.7/pynamicui/createDom/createDom.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:30:43.736099 pynamicui-0.0.7/pynamicui/createElement/
--rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.7/pynamicui/createElement/__init__.py
--rw-rw-rw-   0        0        0     5212 2023-07-19 05:12:51.000000 pynamicui-0.0.7/pynamicui/createElement/createElement.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:30:43.743162 pynamicui-0.0.7/pynamicui/createStylesheet/
--rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.7/pynamicui/createStylesheet/__init__.py
--rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.7/pynamicui/createStylesheet/createStylesheet.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:30:43.724546 pynamicui-0.0.7/pynamicui.egg-info/
--rw-rw-rw-   0        0        0     5792 2023-07-19 05:30:43.000000 pynamicui-0.0.7/pynamicui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-07-19 05:30:43.000000 pynamicui-0.0.7/pynamicui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 05:30:43.000000 pynamicui-0.0.7/pynamicui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-19 05:30:43.000000 pynamicui-0.0.7/pynamicui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-19 05:30:43.000000 pynamicui-0.0.7/pynamicui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-07-19 05:29:27.000000 pynamicui-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-19 05:30:43.749240 pynamicui-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-07-19 05:29:23.000000 pynamicui-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:11:31.914916 pynamicui-0.0.8/
+-rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     7598 2023-07-20 19:11:31.911915 pynamicui-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7115 2023-07-19 21:40:59.000000 pynamicui-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 19:11:31.793864 pynamicui-0.0.8/pynamicui/
+-rw-rw-rw-   0        0        0      318 2023-07-20 19:10:29.000000 pynamicui-0.0.8/pynamicui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:11:31.892397 pynamicui-0.0.8/pynamicui/createDom/
+-rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.8/pynamicui/createDom/__init__.py
+-rw-rw-rw-   0        0        0     2183 2023-07-19 05:26:39.000000 pynamicui-0.0.8/pynamicui/createDom/createDom.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:11:31.900905 pynamicui-0.0.8/pynamicui/createElement/
+-rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.8/pynamicui/createElement/__init__.py
+-rw-rw-rw-   0        0        0     6549 2023-07-20 18:44:32.000000 pynamicui-0.0.8/pynamicui/createElement/createElement.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:11:31.905915 pynamicui-0.0.8/pynamicui/createStylesheet/
+-rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.8/pynamicui/createStylesheet/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.8/pynamicui/createStylesheet/createStylesheet.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:11:31.871385 pynamicui-0.0.8/pynamicui.egg-info/
+-rw-rw-rw-   0        0        0     7598 2023-07-20 19:11:31.000000 pynamicui-0.0.8/pynamicui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-07-20 19:11:31.000000 pynamicui-0.0.8/pynamicui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:11:31.000000 pynamicui-0.0.8/pynamicui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-20 19:11:31.000000 pynamicui-0.0.8/pynamicui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-20 19:11:31.000000 pynamicui-0.0.8/pynamicui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-07-20 19:10:22.000000 pynamicui-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 19:11:31.915916 pynamicui-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-07-20 19:10:06.000000 pynamicui-0.0.8/setup.py
```

### Comparing `pynamicui-0.0.7/LICENSE` & `pynamicui-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.7/PKG-INFO` & `pynamicui-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pynamicui
-Version: 0.0.7
-Summary: dynamic web-like UIs using a declarative syntax
-Home-page: https://github.com/zacharie410/PynamicUI
-Author: zacharie410
-License: Apache Software License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PynamicUI
 
 PynamicUI is a lightweight Python library that provides a dynamic user interface (UI) framework for creating interactive and responsive applications. It simplifies the process of building user interfaces by abstracting away the complexities of working directly with a UI toolkit like Tkinter. With PynamicUI, you can create dynamic web-like UIs using a declarative syntax, making it easy to define and manage the UI components and their interactions.
 
 ## Features
 
 - **Declarative Syntax:** Define UI components using a declarative syntax similar to HTML, making it intuitive and easy to manage.
@@ -29,14 +15,42 @@
 
 PynamicUI requires the `CustomTkinter` library. To install PynamicUI and its dependencies, you can use `pip`:
 
 ```bash
 pip install pynamicui
 ```
 
+## Documentation
+
+For detailed documentation and usage examples, please refer to the [PynamicUI Wiki](https://github.com/zacharie410/PynamicUI/wiki).
+
+## Examples
+
+Check out the [examples](https://github.com/zacharie410/PynamicUI/blob/main/examples/) folder for practical examples building an application with PynamicUI.
+
+### [Example Calculator App](https://github.com/zacharie410/PynamicUI/wiki/Example-Calculator-App)
+![App](https://github.com/zacharie410/PynamicUI/blob/main/examples/screenshots/calculatorapp.png?raw=true)
+Explore a step-by-step tutorial on how to build a simple calculator app using PynamicUI.
+
+### [Example Counter App](https://github.com/zacharie410/PynamicUI/wiki/Example-Counter-App)
+![](https://github.com/zacharie410/PynamicUI/blob/main/examples/screenshots/counterapp.png?raw=true)
+See a practical example of creating a counter app to learn more about PynamicUI's state management and hooks.
+
+### [Example Dynamic List](https://github.com/zacharie410/PynamicUI/wiki/Example-Dynamic-List)
+![](https://github.com/zacharie410/PynamicUI/blob/main/examples/screenshots/dynamiclistapp.png?raw=true)
+Discover how to create a dynamic list using PynamicUI's powerful `place` method for flexible and responsive UI elements.
+
+### [Example NavBar App](https://github.com/zacharie410/PynamicUI/wiki/Example-NavBar-App)
+![](https://github.com/zacharie410/PynamicUI/blob/main/examples/screenshots/navbarapp.png?raw=true)
+Explore a tutorial on building a navigation bar with buttons to switch between different pages in your application.
+
+## An abstraction of CustomTkinter
+PynamicUI supports nearly all the same elements as [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter).
+![](https://github.com/TomSchimansky/CustomTkinter/blob/master/documentation_images/image_example_dark_Windows.png?raw=true)
+
 ## Getting Started
 
 ### Using PynamicUI in a New Project
 
 To start using PynamicUI in a new project, follow these steps:
 
 1. Import the required classes and functions from PynamicUI:
@@ -126,26 +140,23 @@
 6. Render the virtual DOM and launch your application:
 
 ```python
 if __name__ == "__main__":
     dom = createDom(root=existingCustomTkinterRoot)
 ```
 
-## Documentation
-
-For detailed documentation and usage examples, please refer to the [PynamicUI Wiki](https://github.com/zacharie410/PynamicUI/wiki).
-
-## Examples
-
-Check out the [examples](https://github.com/zacharie410/PynamicUI/blob/main/examples/) folder for practical examples building an application with PynamicUI.
-
 ## Contributions
 
 Contributions to PynamicUI are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on [GitHub](https://github.com/zacharie410/PynamicUI).
 
+## Issue Tracking
+
+This wiki page explains the proper procedures for submitting an issue related to PynamicUI
+[Issue Tracking with PynamicUI](https://github.com/zacharie410/PynamicUI/wiki/Issue-Tracking)
+
 ## License
 
 PynamicUI is licensed under the [Apache License](https://github.com/zacharie410/PynamicUI/blob/main/LICENSE). Feel free to use, modify, and distribute this library as permitted by the license.
 
 ## Acknowledgments
 
-PynamicUI is built upon the foundation of CustomTkinter. Special thanks to the developers of CustomTkinter for their valuable contributions.
+PynamicUI is built upon the foundation of [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) by Tom Schimansky. Special thanks to the developers of CustomTkinter for their valuable contributions.
```

### Comparing `pynamicui-0.0.7/pynamicui/createDom/createDom.py` & `pynamicui-0.0.8/pynamicui/createDom/createDom.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.7/pynamicui/createElement/createElement.py` & `pynamicui-0.0.8/pynamicui/createElement/createElement.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,24 +4,50 @@
     if hasattr(parent, "root"):
         return parent
     elif hasattr(parent, "parent"):
         return findDom(parent.parent)
     else:
         # If no "root" attribute is found and there is no "parent" attribute, return None or raise an exception
         return None
-        
+
+def applyPaddingToGeometry(geometry, padx, pady):
+    """
+    Adjust the geometry with padx and pady values relative to the scale of relwidth and relheight.
+
+    Parameters:
+        geometry (dict): A dictionary representing the geometry with keys 'relwidth', 'relheight', 'relx', and 'rely'.
+        padx (float): The padding value to be applied relative to the scale of relwidth.
+        pady (float): The padding value to be applied relative to the scale of relheight.
+
+    Returns:
+        dict: A new dictionary with adjusted geometry values after applying padding.
+    """
+    adjustedGeometry = {}
+
+    scale_width = geometry.get('relwidth', 1)
+    scale_height = geometry.get('relheight', 1)
+
+    adjustedGeometry['relwidth'] = scale_width - (scale_width * padx)
+    adjustedGeometry['relheight'] = scale_height - (scale_height * pady)
+
+    adjustedGeometry['relx'] = geometry.get('relx', 0) + (.5 * scale_width * padx)
+    adjustedGeometry['rely'] = geometry.get('rely', 0) + (.5 * scale_height * pady)
+
+    return adjustedGeometry
+
 class createElement:
-    def __init__(self, parent, tag, name=None, props=None, children=None, place=None, visible=True, hooks=None, style=None):
+    def __init__(self, parent, tag, name=None, props=None, children=None, place=None, visible=True, hooks=None, style=None, spacing=None):
         self.parent = parent
         self.name = name or "Pynamic" + tag + "Element"  # Name of the virtual element
         self.tag = "CTk" + tag  # Tag name for tkinter widget
         self.props = props or {}  # Dictionary to store widget properties
         self.children = children or []  # List of child elements
         self.widget = None  # Reference to the tkinter widget instance
         self.currentPlace = place or {}  # Placement options for the widget
+        self.spacing = spacing or {"padx": 0, "pady": 0} # padx and pady
         self.visible = visible  # Flag to indicate element visibility
         self.hooks = hooks or {}  # Dictionary to store hooks
         self.style = style or ""
         self.mounted = False
 
         if hasattr(self.parent, "root"):
             self.dom = self.parent
@@ -42,15 +68,15 @@
             
             self.updateStyle()
 
             for child in self.children:
                 if child.visible:
                     child.render()  # Render each child element
 
-            self.widget.place(**self.currentPlace)  # Place the widget in the parent
+            self.place(self.currentPlace)  # Place the widget in the parent
 
     def unmount(self):
         self.mounted = False
         for prop, hook in self.hooks.items():
             if hook[1] is not None:
                 hook[1](prop, self, self.props.get(prop))  # Invoke the unmount hook if present
         for child in self.children:
@@ -89,20 +115,23 @@
     def setStyle(self, style):
         self.style = style
         self.updateStyle()
 
     def place(self, geometry):
         self.currentPlace = geometry
         if self.widget:
-            self.widget.place(**self.currentPlace)
+            self.widget.place(**applyPaddingToGeometry(self.currentPlace, self.spacing.get("padx", 0), self.spacing.get("pady", 0)))
 
     def updateStyle(self):
         if self.style != "" and self.widget:
             for item, value in self.dom.stylesheet[self.style].items():
-                self.widget.configure(**{item: value})
+                if item in self.spacing:
+                    self.spacing[item] = value
+                else:
+                    self.widget.configure(**{item: value})
 
     def appendChild(self, child):
         if child in child.parent.children:
             index_to_remove = child.parent.children.index(child)
             child.parent.children.pop(index_to_remove)
         self.children.append(child)
         child.parent = self
```

### Comparing `pynamicui-0.0.7/pynamicui/createStylesheet/createStylesheet.py` & `pynamicui-0.0.8/pynamicui/createStylesheet/createStylesheet.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.7/pyproject.toml` & `pynamicui-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 github_url = "https://github.com/zacharie410/PynamicUI"
 
 [tool.tbump.version]
-current = "0.0.7"
+current = "0.0.8"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pynamicui-0.0.7/setup.py` & `pynamicui-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pynamicui',
-    version='0.0.7',
+    version='0.0.8',
     description='dynamic web-like UIs using a declarative syntax',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/zacharie410/PynamicUI',
     author='zacharie410',
     license='Apache Software License',
     classifiers=[
```

