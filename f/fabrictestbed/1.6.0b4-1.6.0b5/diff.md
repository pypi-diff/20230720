# Comparing `tmp/fabrictestbed-1.6.0b4.tar.gz` & `tmp/fabrictestbed-1.6.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.6.0b4.tar", last modified: Mon Jul 17 15:15:47 2023, max compression
+gzip compressed data, was "fabrictestbed-1.6.0b5.tar", last modified: Thu Jul 20 18:01:55 2023, max compression
```

## Comparing `fabrictestbed-1.6.0b4.tar` & `fabrictestbed-1.6.0b5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b4/.gitignore
--rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b4/LICENSE
--rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b4/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b4/README.md
--rw-r--r--   0        0        0       24 2023-07-17 15:05:37.299608 fabrictestbed-1.6.0b4/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b4/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    18169 2023-07-13 18:40:33.775336 fabrictestbed-1.6.0b4/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b4/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b4/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b4/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    20585 2023-07-17 15:14:15.587130 fabrictestbed-1.6.0b4/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b4/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.776762 fabrictestbed-1.6.0b4/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0     1071 2023-07-17 15:05:27.950690 fabrictestbed-1.6.0b4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b4/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b4/test/test_cli.py
--rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b5/.gitignore
+-rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b5/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b5/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b5/README.md
+-rw-r--r--   0        0        0       24 2023-07-20 17:44:51.409667 fabrictestbed-1.6.0b5/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b5/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    18169 2023-07-13 18:40:33.775336 fabrictestbed-1.6.0b5/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b5/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b5/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b5/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    20667 2023-07-20 17:44:05.832982 fabrictestbed-1.6.0b5/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b5/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.776762 fabrictestbed-1.6.0b5/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     1073 2023-07-20 17:44:05.838824 fabrictestbed-1.6.0b5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b5/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b5/test/test_cli.py
+-rw-r--r--   0        0        0     6536 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b5/PKG-INFO
```

### Comparing `fabrictestbed-1.6.0b4/.gitignore` & `fabrictestbed-1.6.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b4/LICENSE` & `fabrictestbed-1.6.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b4/README.md` & `fabrictestbed-1.6.0b5/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b4/fabrictestbed/cli/cli.py` & `fabrictestbed-1.6.0b5/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b4/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.6.0b5/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b4/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.6.0b5/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b4/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.6.0b5/fabrictestbed/slice_manager/slice_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,31 +360,32 @@
         if self.__should_renew():
             self.__load_tokens()
 
         return self.oc_proxy.renew(token=self.get_id_token(), slice_id=slice_object.slice_id,
                                    new_lease_end_time=new_lease_end_time)
 
     def poa(self, *, sliver_id: str, operation: str, vcpu_cpu_map: List[Dict[str, str]] = None,
-            node_set: List[str] = None) ->Tuple[Status, Union[Exception, List[PoaData]]]:
+            node_set: List[str] = None, keys: List[str] = None) ->Tuple[Status, Union[Exception, List[PoaData]]]:
         """
         Issue POA for a sliver
         @param sliver_id sliver Id for which to trigger POA
         @param operation operation
         @param vcpu_cpu_map list of mappings from virtual CPU to physical cpu
         @param node_set list of the numa nodes
+        @param keys list of keys to add/remove
         @return Tuple containing Status and POA information
        """
         if sliver_id is None or operation is None:
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - sliver_id or operation")
 
         if self.__should_renew():
             self.__load_tokens()
 
         return self.oc_proxy.poa(token=self.get_id_token(), sliver_id=sliver_id, operation=operation,
-                                 vcpu_cpu_map=vcpu_cpu_map, node_set=node_set)
+                                 vcpu_cpu_map=vcpu_cpu_map, node_set=node_set, keys=keys)
 
     def get_poas(self, sliver_id: str = None, poa_id: str = None, limit: int = 20,
                  offset: int = 0, ) -> Tuple[Status, Union[Exception, List[PoaData]]]:
         """
         Get POAs
         @param sliver_id sliver Id for which to trigger POA
         @param limit maximum number of slices to return
```

### Comparing `fabrictestbed-1.6.0b4/fabrictestbed/util/constants.py` & `fabrictestbed-1.6.0b5/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b4/pyproject.toml` & `fabrictestbed-1.6.0b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click",
     "fabric-credmgr-client==1.6.0b4",
-    "fabric-orchestrator-client==1.5.1",
+    "fabric-orchestrator-client==1.6.0b1",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.optional-dependencies]
 test = ["coverage>=4.0.3",
```

### Comparing `fabrictestbed-1.6.0b4/test/test_cli.py` & `fabrictestbed-1.6.0b5/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b4/PKG-INFO` & `fabrictestbed-1.6.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.6.0b4
+Version: 1.6.0b5
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
 Requires-Dist: fabric-credmgr-client==1.6.0b4
-Requires-Dist: fabric-orchestrator-client==1.5.1
+Requires-Dist: fabric-orchestrator-client==1.6.0b1
 Requires-Dist: paramiko
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
```

