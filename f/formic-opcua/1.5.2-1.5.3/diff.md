# Comparing `tmp/formic_opcua-1.5.2.tar.gz` & `tmp/formic_opcua-1.5.3.tar.gz`

## Comparing `formic_opcua-1.5.2.tar` & `formic_opcua-1.5.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    12239 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/core/parse.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.5.3/PKG-INFO
```

### Comparing `formic_opcua-1.5.2/.pre-commit-config.yaml` & `formic_opcua-1.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/examples/opcua_client.py` & `formic_opcua-1.5.3/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.5.3/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.5.3/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.5.3/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.5.3/formic_opcua/client/async_opcua_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,14 @@
             return self
 
     async def __aexit__(self, *args) -> None:
         await self._disconnect()
 
     async def _connect(self):
         try:
-            # if await self._test_server_connection():
-            #     logger.info('_connect called but there is a connection to the server.')
-            #     self._connection_status =
-            #     return
             if await self._disconnect():
                 self._client = Client(url=self._url, timeout=self.connect_timeout)
                 if self._username is not None and self._password is not None:
                     self._client.set_user(self._username)
                     self._client.set_password(self._password)
 
             logger.info('Connecting...')
@@ -124,35 +120,39 @@
         except Exception as e:
             logger.error(f'Unhandled exception while to disconnecting from server. {e} ')
             return False
 
     async def _dfs_mapper(self, node: Node, path: str) -> None:
         browse_path = await node.read_browse_name()
 
-        # if browse_path.NamespaceIndex != self._idx and browse_path.NamespaceIndex != 0:
-        #     return
-
         node_class = await node.read_node_class()
         path_to_node = path + '/' + browse_path.Name
 
         # if node_class == NodeClass.Variable and browse_path.NamespaceIndex == self._idx:
         if node_class == NodeClass.Variable:
             # Remove "/Objects/" since this client is intended for reading only custom nodes
             if path_to_node.startswith('/Objects/'):
                 path_to_node = path_to_node[9:]
             var_type = await node.read_data_type_as_variant_type()
             logger.info(f'Found OPCUA variable {path_to_node}, of variant type {var_type}')
             if not path_to_node.startswith('/'):
                 self._node_map['/' + path_to_node] = (node, var_type)
             else:
                 self._node_map[path_to_node] = (node, var_type)
-            # return
+            node_children = await node.get_properties()
+
+        elif node_class == NodeClass.Object:
+            node_children = await node.get_children()
+
+        else:
+            node_children = []
+            logger.warning(f"Path to node: {path_to_node}")
+            logger.warning(f"Expected NodeClass.Object or NodeClass.Variable but got {node_class}")
 
         child_node_list = []
-        node_children = await node.get_children()
 
         for child_node in node_children:
             child_node_list.append(self._dfs_mapper(child_node, path_to_node))
 
         await asyncio.gather(*child_node_list)
         return
```

### Comparing `formic_opcua-1.5.2/formic_opcua/client/opcua_client.py` & `formic_opcua-1.5.3/formic_opcua/client/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/formic_opcua/core/parse.py` & `formic_opcua-1.5.3/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/formic_opcua/core/type_conversions.py` & `formic_opcua-1.5.3/formic_opcua/core/type_conversions.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.5.3/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.5.3/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/formic_opcua/server/opcua_server.py` & `formic_opcua-1.5.3/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/hooks/add_issue_prefix.py` & `formic_opcua-1.5.3/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/tests/test_server_config.py` & `formic_opcua-1.5.3/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/.gitignore` & `formic_opcua-1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.5.2/pyproject.toml` & `formic_opcua-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.5.2"
+version = "1.5.3"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

