# Comparing `tmp/agentaction-0.1.2.tar.gz` & `tmp/agentaction-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentaction-0.1.2.tar", last modified: Thu Jul 20 11:09:44 2023, max compression
+gzip compressed data, was "agentaction-0.1.3.tar", last modified: Thu Jul 20 11:26:25 2023, max compression
```

## Comparing `agentaction-0.1.2.tar` & `agentaction-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:44.747807 agentaction-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 11:09:24.000000 agentaction-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-20 11:09:44.747807 agentaction-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-20 11:09:24.000000 agentaction-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:44.747807 agentaction-0.1.2/agentaction/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-20 11:09:24.000000 agentaction-0.1.2/agentaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-20 11:09:24.000000 agentaction-0.1.2/agentaction/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:44.747807 agentaction-0.1.2/agentaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 11:09:44.000000 agentaction-0.1.2/agentaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:09:44.747807 agentaction-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 11:09:24.000000 agentaction-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:26:25.853547 agentaction-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 11:26:05.000000 agentaction-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-20 11:26:25.853547 agentaction-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-20 11:26:05.000000 agentaction-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:26:25.853547 agentaction-0.1.3/agentaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-20 11:26:05.000000 agentaction-0.1.3/agentaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-20 11:26:05.000000 agentaction-0.1.3/agentaction/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:26:25.853547 agentaction-0.1.3/agentaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:26:25.853547 agentaction-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 11:26:05.000000 agentaction-0.1.3/setup.py
```

### Comparing `agentaction-0.1.2/LICENSE` & `agentaction-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.2/PKG-INFO` & `agentaction-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.2
+Version: 0.1.3
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentaction-0.1.2/README.md` & `agentaction-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.2/agentaction/__init__.py` & `agentaction-0.1.3/agentaction/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     compose_action_prompt,
     get_actions,
     add_to_action_history,
     get_action_history,
     get_last_action,
     get_available_actions,
     get_formatted_actions,
+    get_action_from_memory,
     search_actions,
     use_action,
     add_action,
     get_action,
     remove_action,
     import_actions,
     clear_actions
@@ -19,14 +20,15 @@
     "compose_action_prompt",
     "get_actions",
     "add_to_action_history",
     "get_action_history",
     "get_last_action",
     "get_available_actions",
     "get_formatted_actions",
+    "get_action_from_memory",
     "search_actions",
     "use_action",
     "add_action",
     "get_action",
     "remove_action",
     "import_actions",
     "clear_actions"
```

### Comparing `agentaction-0.1.2/agentaction/main.py` & `agentaction-0.1.3/agentaction/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,14 +120,29 @@
         # for each action in ignored, delete from available
         for action in ignored_action_objects:
             if action in available_actions:
                 available_actions.remove(action)
 
     return available_actions
 
+def get_action_from_memory(action_name):
+    """
+    Retrieve an action from memory based on the action's name.
+
+    Args:
+        action_name: The name of the action to retrieve.
+
+    Returns:
+        A dictionary representing the action.
+    """
+    action = get_memories("actions", filter_metadata={"name": action_name}, n_results=1)
+    if len(action) == 0:
+        return None
+    return action[0]
+
 
 def search_actions(search_text, n_results=5):
     """
     Searches for actions based on a query text.
 
     Args:
         search_text: Query text used to search for actions.
```

### Comparing `agentaction-0.1.2/agentaction.egg-info/PKG-INFO` & `agentaction-0.1.3/agentaction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.2
+Version: 0.1.3
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentaction-0.1.2/setup.py` & `agentaction-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentaction",
-    version="0.1.2",
+    version="0.1.3",
     description="Action chaining and history for agents",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentaction",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

