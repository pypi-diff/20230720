# Comparing `tmp/agentaction-0.1.1.tar.gz` & `tmp/agentaction-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentaction-0.1.1.tar", last modified: Thu Jul 20 10:08:29 2023, max compression
+gzip compressed data, was "agentaction-0.1.2.tar", last modified: Thu Jul 20 11:09:44 2023, max compression
```

## Comparing `agentaction-0.1.1.tar` & `agentaction-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:29.891830 agentaction-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 10:08:16.000000 agentaction-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-20 10:08:29.891830 agentaction-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-20 10:08:16.000000 agentaction-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:29.891830 agentaction-0.1.1/agentaction/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-20 10:08:16.000000 agentaction-0.1.1/agentaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-07-20 10:08:16.000000 agentaction-0.1.1/agentaction/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:08:29.891830 agentaction-0.1.1/agentaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 10:08:29.000000 agentaction-0.1.1/agentaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:08:29.891830 agentaction-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 10:08:16.000000 agentaction-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:44.747807 agentaction-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 11:09:24.000000 agentaction-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-20 11:09:44.747807 agentaction-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-20 11:09:24.000000 agentaction-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:44.747807 agentaction-0.1.2/agentaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-20 11:09:24.000000 agentaction-0.1.2/agentaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-20 11:09:24.000000 agentaction-0.1.2/agentaction/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:44.747807 agentaction-0.1.2/agentaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:09:44.747807 agentaction-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 11:09:24.000000 agentaction-0.1.2/setup.py
```

### Comparing `agentaction-0.1.1/LICENSE` & `agentaction-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.1/PKG-INFO` & `agentaction-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.1
+Version: 0.1.2
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -132,14 +132,17 @@
 
 ### `get_last_action() -> str or None`
 Retrieves the last executed action from the action history.
 
 ### `get_available_actions(search_text: str) -> list`
 Retrieves the available actions based on relevance and last action.
 
+### `get_formatted_actions(search_text: str) -> list`
+Retrieve a dict containing the available actions in several formats
+
 ### `search_actions(search_text: str, n_results: int=5) -> list`
 Searches for actions based on a query text.
 
 ### `use_action(function_name: str, arguments: dict) -> dict`
 Executes a specific action by its function name.
 
 ### `add_action(name: str, action: dict)`
```

### Comparing `agentaction-0.1.1/README.md` & `agentaction-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -115,14 +115,17 @@
 
 ### `get_last_action() -> str or None`
 Retrieves the last executed action from the action history.
 
 ### `get_available_actions(search_text: str) -> list`
 Retrieves the available actions based on relevance and last action.
 
+### `get_formatted_actions(search_text: str) -> list`
+Retrieve a dict containing the available actions in several formats
+
 ### `search_actions(search_text: str, n_results: int=5) -> list`
 Searches for actions based on a query text.
 
 ### `use_action(function_name: str, arguments: dict) -> dict`
 Executes a specific action by its function name.
 
 ### `add_action(name: str, action: dict)`
```

### Comparing `agentaction-0.1.1/agentaction/__init__.py` & `agentaction-0.1.2/agentaction/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .main import (
     compose_action_prompt,
     get_actions,
     add_to_action_history,
     get_action_history,
     get_last_action,
     get_available_actions,
+    get_formatted_actions,
     search_actions,
     use_action,
     add_action,
     get_action,
     remove_action,
     import_actions,
     clear_actions
@@ -17,14 +18,15 @@
 __all__ = [
     "compose_action_prompt",
     "get_actions",
     "add_to_action_history",
     "get_action_history",
     "get_last_action",
     "get_available_actions",
+    "get_formatted_actions",
     "search_actions",
     "use_action",
     "add_action",
     "get_action",
     "remove_action",
     "import_actions",
     "clear_actions"
```

### Comparing `agentaction-0.1.1/agentaction/main.py` & `agentaction-0.1.2/agentaction/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -90,39 +90,43 @@
     history = get_action_history(n_results=1)
     if len(history) == 0:
         return None
     last = history[0]["document"]
     return last
 
 
-def get_available_actions(search_text, n_results=5, chain=True):
+def get_available_actions(search_text, n_results=5):
     available_actions = search_actions(search_text=search_text, n_results=n_results)
-
-    if chain is False:
-        return available_actions
-    
     recommended_actions = []
     ignored_actions = []
-    
+
     last_action = get_last_action()
     if last_action is not None:
         recommended_actions = actions[last_action]["suggestion_after_actions"]
+        # get actions from named list
+        recommended_action_objects = []
+        for action in recommended_actions:
+            recommended_action_objects.append(get_action_from_memory(action))
         ignored_actions = actions[last_action]["never_after_actions"]
+        ignored_action_objects = []
+        for action in ignored_actions:
+            ignored_action_objects.append(get_action_from_memory(action))
         # check if available_actions contains recommended actions, if not, add them
-        for action in recommended_actions:
+        for action in recommended_action_objects:
             if action not in available_actions:
-                action["metadata"]["recommended"] = True
+                print("action")
+                print(action)
+                action["recommended"] = True
                 available_actions.append(action)
-    merged_actions = []
-    for action in available_actions:
-        if action["id"] in ignored_actions:
-            continue
-        merged_actions.append(action)
+        # for each action in ignored, delete from available
+        for action in ignored_action_objects:
+            if action in available_actions:
+                available_actions.remove(action)
 
-    return merged_actions
+    return available_actions
 
 
 def search_actions(search_text, n_results=5):
     """
     Searches for actions based on a query text.
 
     Args:
@@ -249,7 +253,58 @@
 
     Returns:
     None
     """
     wipe_category("actions")
     global actions
     actions = {}
+
+
+def get_formatted_actions(search_text):
+    """
+    Retrieve a dict containing the available actions in several formats
+
+    Args:
+        search_text: Find most revelant actions whith are available.
+
+    Returns:
+        {
+        "available_actions": a list of available actions in memory format
+        "formatted_actions": a list of actions as a string
+        "short_actions": a list of actions names as a string, comma separated
+    }
+    """
+    # check if context['summary'] exists
+    header_text = "Available actions for me to choose from:"
+    available_actions = get_available_actions(search_text, n_results=5)
+
+    # sort available_actions so that recommended are first
+    # recommended are action["metadata"].get("recommended", None)
+    available_actions = sorted(
+        available_actions,
+        key=lambda x: x.get("recommended", None) is True,
+        reverse=True,
+    )
+
+    def create_formatted_actions(actions):
+        formatted_actions = []
+        for action in actions:
+            if action.get("recommended", None) is True:
+                formatted_actions.append(f"(recommended) {action['document']}")
+            else:
+                formatted_actions.append(action["document"])
+        # join the actions with a newline
+        return "\n".join(formatted_actions)
+
+    short_actions = "Available actions (name): " + ", ".join(
+        [k["metadata"]["name"] for k in available_actions]
+    )
+
+    formatted_actions = (
+        header_text + "\n" + create_formatted_actions(available_actions) + "\n"
+    )
+
+    return {
+        "available_actions": available_actions,
+        "formatted_actions": formatted_actions,
+        "short_actions": short_actions,
+    }
```

### Comparing `agentaction-0.1.1/agentaction.egg-info/PKG-INFO` & `agentaction-0.1.2/agentaction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.1
+Version: 0.1.2
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -132,14 +132,17 @@
 
 ### `get_last_action() -> str or None`
 Retrieves the last executed action from the action history.
 
 ### `get_available_actions(search_text: str) -> list`
 Retrieves the available actions based on relevance and last action.
 
+### `get_formatted_actions(search_text: str) -> list`
+Retrieve a dict containing the available actions in several formats
+
 ### `search_actions(search_text: str, n_results: int=5) -> list`
 Searches for actions based on a query text.
 
 ### `use_action(function_name: str, arguments: dict) -> dict`
 Executes a specific action by its function name.
 
 ### `add_action(name: str, action: dict)`
```

### Comparing `agentaction-0.1.1/setup.py` & `agentaction-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentaction",
-    version="0.1.1",
+    version="0.1.2",
     description="Action chaining and history for agents",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentaction",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

