# Comparing `tmp/agentaction-0.1.0.tar.gz` & `tmp/agentaction-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentaction-0.1.0.tar", last modified: Sun Jul 16 06:48:37 2023, max compression
+gzip compressed data, was "agentaction-0.1.1.tar", last modified: Thu Jul 20 10:08:29 2023, max compression
```

## Comparing `agentaction-0.1.0.tar` & `agentaction-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:48:37.742992 agentaction-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-16 06:48:27.000000 agentaction-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-16 06:48:37.742992 agentaction-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-16 06:48:27.000000 agentaction-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:48:37.742992 agentaction-0.1.0/agentaction/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-16 06:48:27.000000 agentaction-0.1.0/agentaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-16 06:48:27.000000 agentaction-0.1.0/agentaction/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:48:37.742992 agentaction-0.1.0/agentaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-16 06:48:37.000000 agentaction-0.1.0/agentaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-16 06:48:37.000000 agentaction-0.1.0/agentaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 06:48:37.000000 agentaction-0.1.0/agentaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 06:48:37.000000 agentaction-0.1.0/agentaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 06:48:37.000000 agentaction-0.1.0/agentaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 06:48:37.742992 agentaction-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-16 06:48:27.000000 agentaction-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:29.891830 agentaction-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 10:08:16.000000 agentaction-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-20 10:08:29.891830 agentaction-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-20 10:08:16.000000 agentaction-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:29.891830 agentaction-0.1.1/agentaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-20 10:08:16.000000 agentaction-0.1.1/agentaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-07-20 10:08:16.000000 agentaction-0.1.1/agentaction/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:29.891830 agentaction-0.1.1/agentaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:08:29.891830 agentaction-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 10:08:16.000000 agentaction-0.1.1/setup.py
```

### Comparing `agentaction-0.1.0/LICENSE` & `agentaction-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.0/PKG-INFO` & `agentaction-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.0
+Version: 0.1.1
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -47,15 +47,15 @@
     # Your function logic here
     return "Hello, " + args["name"]
 
 def get_actions():
     return [
         {
             "prompt": "Say hello",
-            "composer": None,
+            "builder": None,
             "handler": sample_function,
             "suggestion_after_actions": [],
             "never_after_actions": [],
             "function": {
                 "name": "sample_function",
                 "description": "Says hello to a person",
                 "args": ["name"]
@@ -84,16 +84,16 @@
 
 ### Action Creation and Addition
 ```python
 from actions_manager import add_action
 
 action = {
     "prompt": "Action Prompt",
-    "composer": None,
-    "handler": your_function_name,
+    "builder": None, # the function that is called to build the action prompt
+    "handler": your_function_name, # the function that is called when the action is executed
     "suggestion_after_actions": ["other_action_name1", "other_action_name2"],
     "never_after_actions": ["action_name3", "action_name4"],
     "function": {
         "name": "your_function_name",
         "description": "Your function description",
         "args": ["arg1", "arg2"]
     }
```

### Comparing `agentaction-0.1.0/README.md` & `agentaction-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # Your function logic here
     return "Hello, " + args["name"]
 
 def get_actions():
     return [
         {
             "prompt": "Say hello",
-            "composer": None,
+            "builder": None,
             "handler": sample_function,
             "suggestion_after_actions": [],
             "never_after_actions": [],
             "function": {
                 "name": "sample_function",
                 "description": "Says hello to a person",
                 "args": ["name"]
@@ -67,16 +67,16 @@
 
 ### Action Creation and Addition
 ```python
 from actions_manager import add_action
 
 action = {
     "prompt": "Action Prompt",
-    "composer": None,
-    "handler": your_function_name,
+    "builder": None, # the function that is called to build the action prompt
+    "handler": your_function_name, # the function that is called when the action is executed
     "suggestion_after_actions": ["other_action_name1", "other_action_name2"],
     "never_after_actions": ["action_name3", "action_name4"],
     "function": {
         "name": "your_function_name",
         "description": "Your function description",
         "args": ["arg1", "arg2"]
     }
```

### Comparing `agentaction-0.1.0/agentaction/__init__.py` & `agentaction-0.1.1/agentaction/__init__.py`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.0/agentaction/main.py` & `agentaction-0.1.1/agentaction/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import importlib
 import json
+import sys
 
 from agentmemory import (
     create_memory,
     delete_memory,
     get_memories,
     search_memory,
     wipe_category,
@@ -89,40 +90,37 @@
     history = get_action_history(n_results=1)
     if len(history) == 0:
         return None
     last = history[0]["document"]
     return last
 
 
-def get_available_actions(search_text):
-    """
-    Retrieves the available actions based on relevance and last action.
-
-    Args:
-        search_text: Text to search for most relevant actions by.
+def get_available_actions(search_text, n_results=5, chain=True):
+    available_actions = search_actions(search_text=search_text, n_results=n_results)
 
-    Returns:
-        A list of strings representing the available actions.
-    """
-    available_actions = search_actions(search_text=search_text, n_results=10)
+    if chain is False:
+        return available_actions
+    
     recommended_actions = []
     ignored_actions = []
-
+    
     last_action = get_last_action()
     if last_action is not None:
         recommended_actions = actions[last_action]["suggestion_after_actions"]
         ignored_actions = actions[last_action]["never_after_actions"]
+        # check if available_actions contains recommended actions, if not, add them
+        for action in recommended_actions:
+            if action not in available_actions:
+                action["metadata"]["recommended"] = True
+                available_actions.append(action)
     merged_actions = []
     for action in available_actions:
-        if action["id"] in recommended_actions:
-            merged_actions.append(f"(recommended) {action['document']}")
-        elif action["id"] in ignored_actions:
+        if action["id"] in ignored_actions:
             continue
-        else:
-            merged_actions.append(action["document"])
+        merged_actions.append(action)
 
     return merged_actions
 
 
 def search_actions(search_text, n_results=5):
     """
     Searches for actions based on a query text.
@@ -223,27 +221,30 @@
     The actions returned are then added to the 'actions' dictionary.
 
     Returns:
     None
     """
 
     actions_dir = os.path.abspath(actions_dir)
-    # get the name of the directory
-    dir_name = os.path.basename(actions_dir)
+    print("actiond_dir", actions_dir)
+    sys.path.insert(0, actions_dir)
 
     for filename in os.listdir(actions_dir):
         if filename.endswith(".py"):
-            module = importlib.import_module(f"{dir_name}.{filename[:-3]}")
+            module_name = filename[:-3]  # filename without .py
+            module = importlib.import_module(module_name)
 
             if hasattr(module, "get_actions"):
                 action_funcs = module.get_actions()
 
                 for i in range(len(action_funcs)):
                     name = action_funcs[i]["function"]["name"]
                     add_action(name, action_funcs[i])
+    # Remove the added path after done with imports
+    sys.path.remove(actions_dir)
 
 
 def clear_actions():
     """
     Wipe the 'actions' collection in memory and reset the 'actions' dictionary.
 
     Returns:
```

### Comparing `agentaction-0.1.0/agentaction.egg-info/PKG-INFO` & `agentaction-0.1.1/agentaction.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.0
+Version: 0.1.1
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -47,15 +47,15 @@
     # Your function logic here
     return "Hello, " + args["name"]
 
 def get_actions():
     return [
         {
             "prompt": "Say hello",
-            "composer": None,
+            "builder": None,
             "handler": sample_function,
             "suggestion_after_actions": [],
             "never_after_actions": [],
             "function": {
                 "name": "sample_function",
                 "description": "Says hello to a person",
                 "args": ["name"]
@@ -84,16 +84,16 @@
 
 ### Action Creation and Addition
 ```python
 from actions_manager import add_action
 
 action = {
     "prompt": "Action Prompt",
-    "composer": None,
-    "handler": your_function_name,
+    "builder": None, # the function that is called to build the action prompt
+    "handler": your_function_name, # the function that is called when the action is executed
     "suggestion_after_actions": ["other_action_name1", "other_action_name2"],
     "never_after_actions": ["action_name3", "action_name4"],
     "function": {
         "name": "your_function_name",
         "description": "Your function description",
         "args": ["arg1", "arg2"]
     }
```

### Comparing `agentaction-0.1.0/setup.py` & `agentaction-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentaction",
-    version="0.1.0",
+    version="0.1.1",
     description="Action chaining and history for agents",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentaction",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

