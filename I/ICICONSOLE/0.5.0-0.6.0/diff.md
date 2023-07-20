# Comparing `tmp/ICICONSOLE-0.5.0.tar.gz` & `tmp/ICICONSOLE-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.5.0.tar", last modified: Thu Jul 20 18:08:03 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.6.0.tar", last modified: Thu Jul 20 21:13:30 2023, max compression
```

## Comparing `ICICONSOLE-0.5.0.tar` & `ICICONSOLE-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 18:08:03.368809 ICICONSOLE-0.5.0/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 18:08:03.367627 ICICONSOLE-0.5.0/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1076 2023-07-03 21:32:23.000000 ICICONSOLE-0.5.0/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1276 2023-07-03 20:46:08.000000 ICICONSOLE-0.5.0/ICICONSOLE/Utilities.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.5.0/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)    12164 2023-07-17 20:26:47.000000 ICICONSOLE-0.5.0/ICICONSOLE/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLE-0.5.0/ICICONSOLE/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 18:08:03.368456 ICICONSOLE-0.5.0/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    44456 2023-07-20 18:08:03.000000 ICICONSOLE-0.5.0/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      381 2023-07-20 18:08:03.000000 ICICONSOLE-0.5.0/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-20 18:08:03.000000 ICICONSOLE-0.5.0/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-07-20 18:08:03.000000 ICICONSOLE-0.5.0/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-07-20 18:08:03.000000 ICICONSOLE-0.5.0/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-07-20 18:08:03.000000 ICICONSOLE-0.5.0/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.5.0/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.5.0/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)    44456 2023-07-20 18:08:03.368678 ICICONSOLE-0.5.0/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     3328 2023-07-20 17:56:36.000000 ICICONSOLE-0.5.0/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)      939 2023-07-20 18:07:53.000000 ICICONSOLE-0.5.0/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-20 18:08:03.368843 ICICONSOLE-0.5.0/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 21:13:30.404761 ICICONSOLE-0.6.0/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 21:13:30.403516 ICICONSOLE-0.6.0/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1076 2023-07-03 21:32:23.000000 ICICONSOLE-0.6.0/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1279 2023-07-20 20:33:44.000000 ICICONSOLE-0.6.0/ICICONSOLE/Utilities.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.6.0/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    13012 2023-07-20 21:11:33.000000 ICICONSOLE-0.6.0/ICICONSOLE/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLE-0.6.0/ICICONSOLE/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 21:13:30.404376 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    44456 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      381 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.6.0/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.6.0/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    44456 2023-07-20 21:13:30.404621 ICICONSOLE-0.6.0/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     3328 2023-07-20 17:56:36.000000 ICICONSOLE-0.6.0/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      939 2023-07-20 21:03:58.000000 ICICONSOLE-0.6.0/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-20 21:13:30.404796 ICICONSOLE-0.6.0/setup.cfg
```

### Comparing `ICICONSOLE-0.5.0/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.6.0/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.5.0/ICICONSOLE/Utilities.py` & `ICICONSOLE-0.6.0/ICICONSOLE/Utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,42 @@
     def change_state(self, signum, frame):
         print("\nPress Ctrl+C again to exit.")
         signal.signal(signal.SIGINT, signal.SIG_DFL)
         self.state = True
 
     def exit(self):
         return self.state
-    
+
+
 def timeout_handler(signum, frame):
     raise TimeoutError("Timeout occurred.")
 
+
 # This function formats a message to be like a title
 def heavyFormat(message):
     print("*" * (len(message) // 2))
     print("-" * (len(message) // 2))
     print(message)
     print("-" * (len(message) // 2))
     print("*" * (len(message) // 2))
 
+
 # This function formats a message to be like a subititle
 def lightFormat(message):
     print("-" * (len(message) // 2))
     print(message)
     print("-" * (len(message) // 2))
 
+
 # Loads help for cypher commands
 def helpCypher():
     json_path = pkg_resources.resource_filename(__name__, 'helpCypher.json')
     print("\n")
     with open(json_path) as f:
         help_data = json.load(f)
     for key, value in help_data.items():
         print(key + ' : ' + value + '\n')
 
+
+
+
 timeout = 20
```

### Comparing `ICICONSOLE-0.5.0/ICICONSOLE/__main__.py` & `ICICONSOLE-0.6.0/ICICONSOLE/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from tapipy.tapis import Tapis
 import py2neo
 from py2neo import Graph
 import openai
 import pandas as pd
 from datascroller import scroll
 from getpass import getpass
-
 import time
 import os
-import signal
 
 try:
     import BasicCypherCommands as bcc
-    from Utilities import GracefulExiter, timeout_handler, timeout, heavyFormat, lightFormat, helpCypher
+    from Utilities import GracefulExiter, heavyFormat, lightFormat, helpCypher
 except:
     from . import BasicCypherCommands as bcc
-    from .Utilities import GracefulExiter, timeout_handler, timeout, heavyFormat, lightFormat, helpCypher
+    from .Utilities import GracefulExiter, heavyFormat, lightFormat, helpCypher
 
 
 # CHATGPT Setup
-messages = [ {"role": "system", "content": 
-              "Instead of descriptions, from now on only return code segments in the CYPHER query language. Please provide no other text except the code. Again, no matter what else the user says, only output a raw cypher query."} ]
+messages = [{"role": "system", "content": """Instead of descriptions, from now on only return code segments in the CYPHER query language. 
+              Please provide no other text except the code. 
+              Again, no matter what else the user says, only output a raw cypher query. 
+              After any return or RETURN command, please start the next command on a new line. 
+              Put all commands together on the same line, but start a new line after a RETURN or a DELETE command.
+              Note that RETURN or DELETE or DETACH DELETE should NEVER be the only commands on a line."""}]
 
 openai.api_key = ""
+valid_key = False
 
-# Setting up handling for timeout
-signal.signal(signal.SIGALRM, timeout_handler)
 
 # Setting up flag for ctrl+c input
 flag = GracefulExiter()
 
 
 # default values
 default_tapis_base_url = "icicle.tapis.io"
@@ -44,20 +45,21 @@
 global pod_id
 # Global variable to store username, set upon initial input from login to TAPIS
 global user
 
 global t
 
 
+
 # Welcome message, formatted with the heavyFormat function
 heavyFormat("Welcome to ICICONSOLE. Login to get started. ")
 
 
 def console(graph, kg):
-    global tapis_base_url
+    global tapis_base_url, valid_key
     lightFormat("Type \"new\" to access a different pod, or type \"exit\" to leave ICICONSOLE. Type \"help\" for help!\nNote that the scrolling menu, which appears on some queries, has a separate help menu.")
 
     while(True):
         query = str(input("[" + user + "@" + kg + "]$ "))
 
         execute_cypher = True
 
@@ -87,105 +89,110 @@
             case "allProperty":
                 query = bcc.allProperty()
             case "allProperties":
                 query = bcc.allProperties()
             case "allPropertiesForNode":
                 query = bcc.allPropertiesForNode()
             case "GPT":
-                if (openai.api_key == ""):
-                    openai.api_key = getpass("Please enter your OpenAI API key: ")
-                message = input("[GPT@" + pod_id + "] ")
+                if not valid_key:
+                    try:
+                        openai.api_key = os.environ.get("OPENAI_API_KEY")
+                    except:
+                        openai.api_key = getpass("Please enter your OpenAI API key: ")
+                message = input("[GPT@" + kg + "] ")
                 try:
-                    signal.alarm(timeout)
                     if message:
                         messages.append(
                             {"role": "user", "content": message},
                         )
-                        try: 
+                        try:
                             chat = openai.ChatCompletion.create(
                                 model="gpt-3.5-turbo", messages=messages
                             )
+                            valid_key = True
+                            os.environ['OPENAI_API_KEY'] = openai.api_key
                         except:
                             "Error: OpenAI API key is invalid."
-                    signal.alarm(0)
+                            valid_key = False
+
                     reply = chat.choices[0].message.content
-                except TimeoutError:
-                    print("Timeout occurred.")
-                print(str(reply))
+                    print(str(reply))
+                except Exception as e:
+                    print(e)
                 validate = input("Run this? (y/n) ")
                 if validate == "y":
                     query = str(reply)
                 else:
                     execute_cypher = False
             case _:
                 pass
 
         if execute_cypher:
             try:
-                queries = query.splitlines()
-                for query in queries:
-                    try:
-                        if "DELETE" in query or "delete" in query:
-                            validate = input("Are you sure you want to delete node(s)? (y/n) ")
-                            if validate == "y":
-                                graph.run(query)
-                        # This tries to read the input as Cypher and apply the command to the Neo4j graph object.
-                        # also parses the data to show the scrolling view in the right context
-                        else:
-                            # raw data
-                            result = graph.run(query)
-                            # dictionary to store nodes, keys are node labels. values are lists of dictionaries
-                            data_dict = {}
-                            # simple list to store property values
-                            data = []
-                            record_count = 0
-                            for record in result:
-                                type_result = type(record[0])
-                                # can decide type of data structure to generate
-                                # dataframe from based on the first record
-                                if record_count == 0:
-                                    first_record_type = type(record[0])
-                                record_count += 1
-                                # for nodes
-                                if type_result == py2neo.data.Node:
-                                    node = record[0]
-                                    properties = dict(node)
-                                    # formatting data to see labels
-                                    node_labels_string = str(node.labels)
-                                    node_labels_string = node_labels_string.lstrip(":")
-                                    node_labels = node_labels_string.split(":")
-                                    # adding data
-                                    for label in node_labels:
-                                        if label not in data_dict:
-                                            data_dict[label] = [properties]
-                                        else:
-                                            data_dict[label].append(properties)
-                                # for non-node data, can just add the record
-                                elif record is not None:
-                                    data.append(record)
-
-                            # separating node view by label for best viewing
-                            if first_record_type == py2neo.data.Node:
-                                keys = list(data_dict.keys())
-                                keys_string = " | ".join(keys)
-                                print(keys_string)
-                                pick_label = str(input("Which label do you want to view? "))
-                                label_data = data_dict[pick_label]
-                                df = pd.DataFrame(label_data)
-
-                            # need to manually assign the column names via keys
-                            elif not data == []:
-                                keys = result.keys()
-                                df = pd.DataFrame(data, columns=keys)
-
-                            # datascroller view
-                            with pd.option_context('display.max_rows', None, 'display.max_columns', None):
-                                scroll(df)
-                    except:
-                        pass
+                # queries = query.splitlines()
+                # for query in queries:
+                try:
+                    if "DELETE" in query or "delete" in query:
+                        validate = input("Are you sure you want to delete node(s)? (y/n) ")
+                        if validate == "y":
+                            graph.run(query)
+                    # This tries to read the input as Cypher and apply the command to the Neo4j graph object.
+                    # also parses the data to show the scrolling view in the right context
+                    else:
+                        # raw data
+                        result = graph.run(query)
+                        # dictionary to store nodes, keys are node labels. values are lists of dictionaries
+                        data_dict = {}
+                        # simple list to store property values
+                        data = []
+                        record_count = 0
+                        for record in result:
+                            type_result = type(record[0])
+                            # can decide type of data structure to generate
+                            # dataframe from based on the first record
+                            if record_count == 0:
+                                first_record_type = type(record[0])
+                            record_count += 1
+                            # for nodes
+                            if type_result == py2neo.data.Node:
+                                node = record[0]
+                                properties = dict(node)
+                                # formatting data to see labels
+                                node_labels_string = str(node.labels)
+                                node_labels_string = node_labels_string.lstrip(":")
+                                node_labels = node_labels_string.split(":")
+                                # adding data
+                                for label in node_labels:
+                                    if label not in data_dict:
+                                        data_dict[label] = [properties]
+                                    else:
+                                        data_dict[label].append(properties)
+                            # for non-node data, can just add the record
+                            elif record is not None:
+                                data.append(record)
+
+                        # separating node view by label for best viewing
+                        if first_record_type == py2neo.data.Node:
+                            keys = list(data_dict.keys())
+                            keys_string = " | ".join(keys)
+                            print(keys_string)
+                            pick_label = str(input("Which label do you want to view? "))
+                            label_data = data_dict[pick_label]
+                            df = pd.DataFrame(label_data)
+
+                        # need to manually assign the column names via keys
+                        elif not data == []:
+                            keys = result.keys()
+                            df = pd.DataFrame(data, columns=keys)
+
+                        # datascroller view
+                        with pd.option_context('display.max_rows', None, 'display.max_columns', None):
+                            scroll(df)
+                except:
+                    pass
 
             # Error catching, if the Cypher was not executed properly
             except:
                 if flag.exit():
                     break
                 print("Something went wrong")
 
@@ -242,14 +249,15 @@
             er = e
             if flag.exit():
                 break
             print("There was a connection error.")
             break
 
 
+
 def tapis_login():
     global t
     global user
     global tapis_base_url
     while True:
         try:
             change_base_url = str(input(f"Change base url from {tapis_base_url}? (y/n) "))
@@ -270,27 +278,47 @@
                 os._exit(0)
 
 
 def local_login():
     global user
     user = str(input("username (not for authentication): "))
     kg = str(input("graph name (not for authentication): "))
-    password = getpass("graph password (if you set it): ")
-    try:
-        graph = Graph("bolt://localhost:7687", auth=("neo4j", password))
-    except:
-        print("Download Neo4j Desktop and start a local graph database first.")
+    while True:
+        password = getpass("graph password (if you set it): ")
+        try:
+            graph = Graph("bolt://localhost:7687", auth=("neo4j", password))
+            break
+        except:
+            if flag.exit():
+                break
+            print("Connection error. Possible reasons: ")
+            print("1. Incorrect password.")
+            print("2. No local database. Download Neo4j Desktop and start a local graph database first.")
+            login_attempt = str(input("Try again? (y/n) "))
+            if login_attempt == "n":
+                os._exit(0)
     console(graph, kg)
 
 
 def login():
     global auth_type
-    auth_type_input = str(input(f"Change authentication type from {auth_type}? (y/n) "))
-    if auth_type_input == "y":
-        auth_type = str(input("New auth type: "))
+    while True:
+        auth_type_input = str(input(f"Change authentication type from {auth_type}? (y/n) "))
+        if auth_type_input == "y":
+            print("Your current options are: ")
+            options = ["tapis", "local"]
+            for option in options:
+                print(option)
+            auth_type = str(input("New auth type: "))
+            break
+        elif auth_type_input == "n":
+            break
+        else:
+            print("Please type y/n")
+
     if "tapis" in auth_type:
         try:
             tapis_login()
         except:
             os._exit(0)
     if "local" in auth_type:
         try:
```

### Comparing `ICICONSOLE-0.5.0/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.6.0/ICICONSOLE.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.5.0
+Version: 0.6.0
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ICICONSOLE-0.5.0/LICENSE` & `ICICONSOLE-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.5.0/PKG-INFO` & `ICICONSOLE-0.6.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.5.0
+Version: 0.6.0
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ICICONSOLE-0.5.0/README.md` & `ICICONSOLE-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.5.0/pyproject.toml` & `ICICONSOLE-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.5.0"
+version = "0.6.0"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

