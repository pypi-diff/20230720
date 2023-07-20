# Comparing `tmp/gladier-0.9.0b1.tar.gz` & `tmp/gladier-0.9.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gladier-0.9.0b1.tar", last modified: Mon Jul 10 16:20:44 2023, max compression
+gzip compressed data, was "gladier-0.9.0b2.tar", last modified: Thu Jul 20 17:38:20 2023, max compression
```

## Comparing `gladier-0.9.0b1.tar` & `gladier-0.9.0b2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.201231 gladier-0.9.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 16:20:33.000000 gladier-0.9.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 16:20:33.000000 gladier-0.9.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-10 16:20:44.201231 gladier-0.9.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-10 16:20:33.000000 gladier-0.9.0b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.197230 gladier-0.9.0b1/gladier/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22417 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.197230 gladier-0.9.0b1/gladier/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/compute_login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/compute_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/flows_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.197230 gladier-0.9.0b1/gladier/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/storage/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/storage/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.201231 gladier-0.9.0b1/gladier/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/automate.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/dynamic_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/flow_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/flow_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/flow_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/name_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/tool_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/tool_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.197230 gladier-0.9.0b1/gladier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 16:20:33.000000 gladier-0.9.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 16:20:44.201231 gladier-0.9.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-10 16:20:33.000000 gladier-0.9.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 17:38:09.000000 gladier-0.9.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 17:38:09.000000 gladier-0.9.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-20 17:38:20.448307 gladier-0.9.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-20 17:38:09.000000 gladier-0.9.0b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.444307 gladier-0.9.0b2/gladier/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22625 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/gladier/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/compute_login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/compute_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/flows_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/gladier/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/storage/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/storage/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/gladier/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/dynamic_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/flow_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/flow_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/flow_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/name_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/tool_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/tool_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/gladier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 17:38:09.000000 gladier-0.9.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-20 17:38:20.448307 gladier-0.9.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-20 17:38:09.000000 gladier-0.9.0b2/setup.py
```

### Comparing `gladier-0.9.0b1/LICENSE` & `gladier-0.9.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b1/PKG-INFO` & `gladier-0.9.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -39,18 +39,18 @@
 .. image:: https://img.shields.io/pypi/wheel/gladier.svg
     :target: https://pypi.python.org/pypi/gladier
 
 .. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
     :alt: License
     :target: https://opensource.org/licenses/Apache-2.0
 
-Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage 
+Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage
 systems and manage using Globus Flows.
 
-Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field, 
+Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field,
 Gladier can help you streamline your data management and analysis workflows, so you can focus on your scientific discoveries.
 Try Gladier today and see how it can enhance your research capabilities!
 
 You can install Gladier and Gladier Tools with the following:
 
 
 .. code-block:: bash
```

### Comparing `gladier-0.9.0b1/README.rst` & `gladier-0.9.0b2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 .. image:: https://img.shields.io/pypi/wheel/gladier.svg
     :target: https://pypi.python.org/pypi/gladier
 
 .. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
     :alt: License
     :target: https://opensource.org/licenses/Apache-2.0
 
-Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage 
+Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage
 systems and manage using Globus Flows.
 
-Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field, 
+Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field,
 Gladier can help you streamline your data management and analysis workflows, so you can focus on your scientific discoveries.
 Try Gladier today and see how it can enhance your research capabilities!
 
 You can install Gladier and Gladier Tools with the following:
 
 
 .. code-block:: bash
```

### Comparing `gladier-0.9.0b1/gladier/base.py` & `gladier-0.9.0b2/gladier/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     """Gladier Defaults defines a common method of tying together
     flows, compute-functions, and default inputs for starting a flow."""
 
     flow_definition = None
     flow_input = dict()
     flow_transition_states = []
     required_input = []
-    alias_exempt = ['compute_endpoint']
+    alias_exempt = ["compute_endpoint"]
     compute_endpoints = dict()
     compute_functions = []
 
     def __init__(self, alias: str = None, alias_class: ToolAlias = None):
         self.alias = alias
         alias_cls = alias_class
         if alias and not alias_class:
             raise ValueError(
                 f'{self.__class__.__name__} given alias "{alias}" but not "alias_class". '
-                'ex: alias_class=gladier.utils.tool_alias.StateSuffixVariablePrefix'
+                "ex: alias_class=gladier.utils.tool_alias.StateSuffixVariablePrefix"
             )
         if alias_class:
             self.alias_renamer = alias_cls(alias)
 
     def get_required_input(self) -> List[str]:
         if self.alias:
             required = []
@@ -50,37 +50,47 @@
                 flow_input[input_var] = val
         return flow_input
 
     def get_flow_transition_states(self) -> List[str]:
         return self.flow_transition_states
 
     def get_original_inputs(self) -> Mapping[str, Any]:
-        return [input_var for input_var in set(self.required_input) | set(self.flow_input.keys())
-                if input_var not in self.alias_exempt]
-
-    def rename_state(self, state_name: str, state_data: Mapping[str, Any]) -> Mapping[str, Any]:
+        return [
+            input_var
+            for input_var in set(self.required_input) | set(self.flow_input.keys())
+            if input_var not in self.alias_exempt
+        ]
+
+    def rename_state(
+        self, state_name: str, state_data: Mapping[str, Any]
+    ) -> Mapping[str, Any]:
         name = self.alias_renamer.rename_state(state_name, self)
-        data = self.alias_renamer.rename_input_variables(state_data,
-                                                         self.get_original_inputs(), self)
+        data = self.alias_renamer.rename_input_variables(
+            state_data, self.get_original_inputs(), self
+        )
         return name, data
 
     def get_flow_definition(self) -> Mapping[str, Any]:
-
         if not self.alias:
             return self.flow_definition
 
         new_states = {}
         for state_name, state_data in iter_flow(self.flow_definition):
             new_name, new_state = self.rename_state(state_name, state_data)
             new_states[new_name] = new_state
-            if new_state.get('Next'):
-                new_state['Next'] = self.alias_renamer.rename_state(new_state['Next'], self)
-            if new_state['Type'] == 'Choice':
-                for choice in new_state['Choices']:
-                    if choice.get('Next'):
-                        choice['Next'] = self.alias_renamer.rename_state(choice['Next'], self)
+            if new_state.get("Next"):
+                new_state["Next"] = self.alias_renamer.rename_state(
+                    new_state["Next"], self
+                )
+            if new_state["Type"] == "Choice":
+                for choice in new_state["Choices"]:
+                    if choice.get("Next"):
+                        choice["Next"] = self.alias_renamer.rename_state(
+                            choice["Next"], self
+                        )
 
         new_flow_def = copy.deepcopy(self.flow_definition)
-        new_flow_def['States'] = new_states
-        new_flow_def['StartAt'] = self.alias_renamer.rename_state(self.flow_definition['StartAt'],
-                                                                  self)
+        new_flow_def["States"] = new_states
+        new_flow_def["StartAt"] = self.alias_renamer.rename_state(
+            self.flow_definition["StartAt"], self
+        )
         return new_flow_def
```

### Comparing `gladier-0.9.0b1/gladier/client.py` & `gladier-0.9.0b2/gladier/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import pathlib
 import logging
 from collections.abc import Iterable
 
 from gladier.base import GladierBaseTool
 from gladier.managers.login_manager import (
-    BaseLoginManager, AutoLoginManager, ConfidentialClientLoginManager
+    BaseLoginManager,
+    AutoLoginManager,
+    ConfidentialClientLoginManager,
 )
 from globus_sdk import AccessTokenAuthorizer, RefreshTokenAuthorizer
 from gladier.managers import FlowsManager, ComputeManager
 
 from gladier.storage.tokens import GladierSecretsConfig
 import gladier
 import gladier.storage.config
@@ -17,14 +19,15 @@
 import gladier.utils.automate
 import gladier.utils.name_generation
 import gladier.storage.migrations
 import gladier.utils.tool_alias
 import gladier.managers.compute_login_manager
 import gladier.exc
 import gladier.version
+
 log = logging.getLogger(__name__)
 
 
 class GladierBaseClient(object):
     """
     The Gladier Client ties together commonly used compute functions
     and basic flows with auto-registration tools to make complex tasks
@@ -92,50 +95,54 @@
     :param login_manager: Class defining login behavior. Defaults to AutoLoginManager, and
                           will auto-login when additional scopes are needed.
     :param flows_manager: A flows manager class with customized behavior. Attrs like group
                           and login_manager will automatically be set if None
     :raises gladier.exc.AuthException: if authorizers given are insufficient
 
     """
+
     secret_config_filename: str = None
-    app_name: str = 'Gladier Client'
-    client_id: str = 'f1631610-d9e4-4db2-81ba-7f93ad4414e3'
+    app_name: str = "Gladier Client"
+    client_id: str = "f1631610-d9e4-4db2-81ba-7f93ad4414e3"
     globus_group: str = None
     subscription_id: str = None
     alias_class = gladier.utils.tool_alias.StateSuffixVariablePrefix
 
     def __init__(
         self,
         auto_registration: bool = True,
         login_manager: BaseLoginManager = None,
         flows_manager: FlowsManager = None,
-            ):
-
+    ):
         self._tools = None
         self.storage = self._determine_storage()
-        self.login_manager = login_manager or self._determine_login_manager(self.storage)
-
-        self.flows_manager = flows_manager or FlowsManager(auto_registration=auto_registration)
+        self.login_manager = login_manager or self._determine_login_manager(
+            self.storage
+        )
+
+        self.flows_manager = flows_manager or FlowsManager(
+            auto_registration=auto_registration
+        )
         if self.globus_group:
             self.flows_manager.globus_group = self.globus_group
         if self.subscription_id:
             self.flows_manager.subscription_id = self.subscription_id
         if not self.flows_manager.flow_title:
-            self.flows_manager.flow_title = f'{self.__class__.__name__} flow'
+            self.flows_manager.flow_title = f"{self.__class__.__name__} flow"
 
         self.compute_manager = ComputeManager(auto_registration=auto_registration)
         self.storage.update()
 
         for man in (self.flows_manager, self.compute_manager):
             man.set_storage(self.storage, replace=False)
             man.set_login_manager(self.login_manager, replace=False)
             man.register_scopes()
 
     def _get_confidential_client_credentials(self):
-        return os.getenv('GLADIER_CLIENT_ID'), os.getenv('GLADIER_CLIENT_SECRET')
+        return os.getenv("GLADIER_CLIENT_ID"), os.getenv("GLADIER_CLIENT_SECRET")
 
     def _determine_storage(self):
         """
         Determine the storage location for Gladier. This is typically in the ~/.gladier directory,
         but can be changed by setting the ``secret_config_filename`` on the class.
 
         Setting GLADIER_CLIENT_ID will change the filename to the client id, so that config
@@ -147,85 +154,94 @@
 
         if self.secret_config_filename:
             storage_filename = pathlib.Path(self.secret_config_filename)
         else:
             storage_filename = pathlib.Path(f"~/.gladier/{client_id}.cfg").expanduser()
             storage_filename.parent.mkdir(exist_ok=True)
 
-        storage_section = gladier.utils.name_generation.get_snake_case(self.__class__.__name__)
-        storage_tokens_section = f'tokens_{client_id}'
-
-        return GladierSecretsConfig(storage_filename, storage_section,
-                                    tokens_section=storage_tokens_section)
+        storage_section = gladier.utils.name_generation.get_snake_case(
+            self.__class__.__name__
+        )
+        storage_tokens_section = f"tokens_{client_id}"
+
+        return GladierSecretsConfig(
+            storage_filename, storage_section, tokens_section=storage_tokens_section
+        )
 
     def _determine_login_manager(self, storage):
         """
         Determine the login manager to use for Glaider. First searches for evnironment
         variables for a confidential client, then defaults to an AutoLoginManager using
         a native client id set as ``client_id`` on this class.
         """
         CLI_ID, CLI_SEC = self._get_confidential_client_credentials()
         if CLI_ID and CLI_SEC:
-            log.info('Client Credentials detected, using custom internal storage for '
-                     'storing tokens.')
+            log.info(
+                "Client Credentials detected, using custom internal storage for "
+                "storing tokens."
+            )
             return ConfidentialClientLoginManager(CLI_ID, CLI_SEC, storage=storage)
         else:
             return AutoLoginManager(self.client_id, storage, self.app_name)
 
     @staticmethod
     def get_gladier_defaults_cls(tool_ref, alias_class=None):
         """
         Load a Gladier default class (gladier.GladierBaseTool) by import string. For
         Example: get_gladier_defaults_cls('gladier.tools.hello_world.HelloWorld')
 
         :param tool_ref: A tool ref can be a dotted import string or an actual GladierBaseTool
                          class.
         :return: gladier.GladierBaseTool
         """
-        log.debug(f'Looking for Gladier tool: {tool_ref} ({type(tool_ref)})')
+        log.debug(f"Looking for Gladier tool: {tool_ref} ({type(tool_ref)})")
         if isinstance(tool_ref, str):
             default_cls = gladier.utils.dynamic_imports.import_string(tool_ref)
             _, alias = gladier.utils.dynamic_imports.parse_alias(tool_ref)
             default_inst = default_cls(alias, alias_class)
             if issubclass(type(default_inst), gladier.base.GladierBaseTool):
                 return default_inst
-            raise gladier.exc.ConfigException(f'{default_inst} is not of type '
-                                              f'{gladier.base.GladierBaseTool}')
+            raise gladier.exc.ConfigException(
+                f"{default_inst} is not of type " f"{gladier.base.GladierBaseTool}"
+            )
         elif isinstance(tool_ref, gladier.base.GladierBaseTool):
             return tool_ref
         else:
             cls_inst = tool_ref()
             if isinstance(cls_inst, gladier.base.GladierBaseTool):
                 return cls_inst
             raise gladier.exc.ConfigException(
                 f'"{tool_ref}" must be a {gladier.base.GladierBaseTool} or a dotted import '
-                'string ')
+                "string "
+            )
 
     @property
     def version(self):
         return gladier.version.__version__
 
     @property
     def tools(self):
         """
         Load the current list of tools configured on this class
 
         :return: a list of subclassed instances of gladier.GladierBaseTool
         """
-        if getattr(self, '_tools', None):
+        if getattr(self, "_tools", None):
             return self._tools
 
-        gtools = getattr(self, 'gladier_tools', [])
+        gtools = getattr(self, "gladier_tools", [])
         if not gtools or not isinstance(gtools, Iterable):
             if not self.get_flow_definition():
                 raise gladier.exc.ConfigException(
                     '"gladier_tools" must be a defined list of Gladier Tools. '
-                    'Ex: ["gladier.tools.hello_world.HelloWorld"]')
-        self._tools = [self.get_gladier_defaults_cls(gt, self.alias_class)
-                       for gt in gtools]
+                    'Ex: ["gladier.tools.hello_world.HelloWorld"]'
+                )
+        self._tools = [
+            self.get_gladier_defaults_cls(gt, self.alias_class) for gt in gtools
+        ]
         return self._tools
 
     @property
     def scopes(self):
         """
         The current list of scopes required by this class. This changes if there
         is a flow configured in the local Gladier config file, otherwise it will
@@ -269,31 +285,34 @@
     def get_flow_definition(self):
         """
         Get the flow definition attached to this class. If the flow definition is an import string,
         it will automatically load the import string and return the full flow.
 
         :return: A dict of the Automate Flow definition
         """
-        if not getattr(self, 'flow_definition', None):
-            raise gladier.exc.ConfigException(f'"flow_definition" was not set on '
-                                              f'{self.__class__.__name__}')
+        if not getattr(self, "flow_definition", None):
+            raise gladier.exc.ConfigException(
+                f'"flow_definition" was not set on ' f"{self.__class__.__name__}"
+            )
 
         if isinstance(self.flow_definition, dict):
             return self.flow_definition
         elif isinstance(self.flow_definition, str):
             return self.get_gladier_defaults_cls(self.flow_definition).flow_definition
-        raise gladier.exc.ConfigException('"flow_definition" must be a dict or an import string '
-                                          'to a sub-class of type '
-                                          '"gladier.GladierBaseTool"')
+        raise gladier.exc.ConfigException(
+            '"flow_definition" must be a dict or an import string '
+            "to a sub-class of type "
+            '"gladier.GladierBaseTool"'
+        )
 
     def get_flow_schema(self):
         """
         Get the flow schema attached to this class.
         """
-        return getattr(self, 'flow_schema', None)
+        return getattr(self, "flow_schema", None)
 
     def sync_flow(self):
         self.flows_manager.flow_definition = self.get_flow_definition()
         schema = self.get_flow_schema()
         if schema:
             self.flows_manager.flow_schema = schema
         self.flows_manager.sync_flow()
@@ -348,19 +367,20 @@
         :raises: gladier.exc.RegistrationException
         :raises: gladier.exc.FunctionObsolete
         :raises: gladier.exc.AuthException
         :raises: Any globus_sdk.exc.BaseException
         """
         combine_flow_input = self.get_input() if use_defaults else dict()
         if flow_input is not None:
-            if not flow_input.get('input') or len(flow_input.keys()) != 1:
+            if not flow_input.get("input") or len(flow_input.keys()) != 1:
                 raise gladier.exc.ConfigException(
                     f'Malformed input to flow, all input must be nested under "input", got '
-                    f'{flow_input.keys()}')
-            combine_flow_input['input'].update(flow_input['input'])
+                    f"{flow_input.keys()}"
+                )
+            combine_flow_input["input"].update(flow_input["input"])
         for tool in self.tools:
             self.check_input(tool, combine_flow_input)
 
         self.sync_flow()
         return self.flows_manager.run_flow(flow_input=combine_flow_input, **flow_kwargs)
 
     def get_compute_function_ids(self):
@@ -371,24 +391,25 @@
 
         :raises: gladier.exc.RegistrationException
         :raises: gladier.exc.FunctionObsolete
         :returns: a dict of function ids where keys are names and values are compute function ids.
         """
         compute_ids = dict()
         for tool in self.tools:
-            log.debug(f'Checking functions for {tool}')
-            compute_funcs = (
-                getattr(tool, 'compute_functions', []) + getattr(tool, 'funcx_functions', [])
+            log.debug(f"Checking functions for {tool}")
+            compute_funcs = getattr(tool, "compute_functions", []) + getattr(
+                tool, "funcx_functions", []
             )
             if not compute_funcs:
-                log.warning(f'Tool {tool} did not define any compute functions!')
+                log.warning(f"Tool {tool} did not define any compute functions!")
             if not compute_funcs and not isinstance(compute_funcs, Iterable):
                 raise gladier.exc.DeveloperException(
                     f'Attribute "compute_functions" on {tool} needs to be an iterable! Found '
-                    f'{type(compute_funcs)}')
+                    f"{type(compute_funcs)}"
+                )
 
             for func in compute_funcs:
                 name, val = self.compute_manager.validate_function(tool, func)
                 compute_ids[name] = val
         return compute_ids
 
     def get_flow_id(self) -> str:
@@ -418,35 +439,43 @@
             #             if set(flow_input.keys()).intersection(set(tool.flow_input)):
             #                 raise gladier.exc.ConfigException(
             #                   f'Conflict: Tools {tool} and {prev_tool} 'both define {r}')
             flow_input.update(tool.get_flow_input())
             # Iterate over both private and public input variables, and include any relevant ones
             # Note: Precedence starts and ends with: Public --> Private --> Default on Tool
             input_keys = set(tool.get_flow_input()) | set(tool.get_required_input())
-            log.debug(f'{tool}: Looking for overrides for the following input keys: {input_keys}')
-            override_values = {k: self.storage.get_value(k) for k in input_keys
-                               if self.storage.get_value(k) is not None}
+            log.debug(
+                f"{tool}: Looking for overrides for the following input keys: {input_keys}"
+            )
+            override_values = {
+                k: self.storage.get_value(k)
+                for k in input_keys
+                if self.storage.get_value(k) is not None
+            }
             if override_values:
-                log.info(f'Updates from {self.storage.filename}: {list(override_values.keys())}')
+                log.info(
+                    f"Updates from {self.storage.filename}: {list(override_values.keys())}"
+                )
                 flow_input.update(override_values)
-        return {'input': flow_input}
+        return {"input": flow_input}
 
     def check_input(self, tool: GladierBaseTool, flow_input: dict):
         """
         Do basic checking on included input against requirements set by a tool. Raises an
         exception if the check does not 'pass'
 
         :param tool: The gladier.GladierBaseTool tool set in self.tools
         :param flow_input: Flow input intended to be passed to run_flow()
         :raises: gladier.exc.ConfigException
         """
         for req_input in tool.get_required_input():
-            if req_input not in flow_input['input']:
+            if req_input not in flow_input["input"]:
                 raise gladier.exc.ConfigException(
-                    f'{tool} requires flow input value: "{req_input}"')
+                    f'{tool} requires flow input value: "{req_input}"'
+                )
 
     def get_status(self, action_id: str):
         """
         Get the current status of the automate flow. Attempts to do additional work on compute
         functions to deserialize any exception output.
 
         :param action_id: The globus action UUID used for this flow. The Automate flow id is
@@ -475,8 +504,10 @@
         definition. Note: This is usually only possible when a flow completes.
 
         :param action_id: The action_id for this flow. Flow id is automatically determined based
                           on the current tool being run.
         :param state_name: The state in the automate definition to fetch
         :returns: sub-dict of get_status() describing the :state_name:.
         """
-        return gladier.utils.automate.get_details(self.get_status(action_id), state_name)
+        return gladier.utils.automate.get_details(
+            self.get_status(action_id), state_name
+        )
```

### Comparing `gladier-0.9.0b1/gladier/decorators.py` & `gladier-0.9.0b2/gladier/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,19 @@
                 c.flow_definition = generate_tool_flow(c, modifiers)
                 return c
             elif issubclass(cls, GladierBaseClient):
                 c = cls(*args, **kwargs)
                 c.flow_definition = combine_tool_flows(c, modifiers)
                 return c
             else:
-                raise FlowGenException(f'Invalid class {cls}, flow generation '
-                                       f'only supported for '
-                                       f'{[GladierBaseTool, GladierBaseClient]}')
+                raise FlowGenException(
+                    f"Invalid class {cls}, flow generation "
+                    f"only supported for "
+                    f"{[GladierBaseTool, GladierBaseClient]}"
+                )
 
         return wrapper
 
     if _cls is None:
         return decorator_wrapper
     else:
         return decorator_wrapper(_cls)
```

### Comparing `gladier-0.9.0b1/gladier/exc.py` & `gladier-0.9.0b2/gladier/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,73 @@
-
-
 class GladierException(Exception):
     """Top level Gladier Exception"""
+
     pass
 
 
 class AuthException(GladierException):
     """There was a problem with Globus Auth"""
+
     def __init__(self, message, missing_scopes=tuple()):
         self.missing_scopes = missing_scopes
         super().__init__(message)
 
 
 class ConfigException(GladierException):
     """Something in Gladier wasn't configured properly"""
+
     pass
 
 
 class DevelopmentException(GladierException):
     """A developer messed up."""
+
     pass
 
 
 class RegistrationException(ConfigException):
     """Something needs to be registered"""
+
     def __init__(self, message, items=tuple()):
         self.items = items
         super().__init__(message)
 
 
 class NoFlowRegistered(RegistrationException):
     pass
 
 
 class ObsoleteException(RegistrationException):
     """A compute function or flow has local changes not reflected
     in the currently registered id"""
+
     pass
 
 
 class FlowObsolete(ObsoleteException):
     """The local flow definition has changed and needs to be updated"""
+
     pass
 
 
 class FunctionObsolete(ObsoleteException):
     """A local compute function definition has changed and needs to be updated"""
+
     pass
 
 
 class FlowGenException(GladierException):
     """Something went wrong when auto-generating a flow"""
+
     pass
 
 
 class StateNameConflict(FlowGenException):
     """Two or more flow states share the same name"""
+
     pass
 
 
 class FlowModifierException(FlowGenException):
     """An error happened when applying a modifier during flow generation"""
+
     pass
```

### Comparing `gladier-0.9.0b1/gladier/managers/compute_login_manager.py` & `gladier-0.9.0b2/gladier/managers/compute_login_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,25 @@
 
 class ComputeLoginManager:
     """
     Implements the globus_compute_sdk.sdk.login_manager.protocol.LoginManagerProtocol class.
 
     https://github.com/funcx-faas/funcX/blob/main/compute_sdk/globus_compute_sdk/sdk/login_manager/protocol.py  # noqa
     """
+
     SCOPES = [
         Client.FUNCX_SCOPE,
         AuthScopes.openid,
     ]
 
     def __init__(self, authorizers: dict[str, globus_sdk.RefreshTokenAuthorizer]):
         self.authorizers = authorizers
 
     def get_auth_client(self) -> globus_sdk.AuthClient:
-        return globus_sdk.AuthClient(
-            authorizer=self.authorizers[AuthScopes.openid]
-        )
+        return globus_sdk.AuthClient(authorizer=self.authorizers[AuthScopes.openid])
 
     def get_web_client(
         self, *, base_url: str | None = None, app_name: str | None = None
     ) -> WebClient:
         return WebClient(
             base_url=base_url,
             app_name=app_name,
```

### Comparing `gladier-0.9.0b1/gladier/managers/compute_manager.py` & `gladier-0.9.0b2/gladier/managers/compute_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,84 +7,97 @@
 
 import gladier.managers.compute_login_manager
 
 log = logging.getLogger(__name__)
 
 
 class ComputeManager(ServiceManager):
-
     def __init__(self, auto_registration: bool = True, **kwargs):
         super().__init__(**kwargs)
         self.auto_registration = auto_registration
 
     def get_scopes(self):
         return gladier.managers.compute_login_manager.ComputeLoginManager.SCOPES
 
     @property
     def compute_client(self):
         """
         :return: an authorized compute client
         """
-        if getattr(self, '__compute_client', None) is not None:
+        if getattr(self, "__compute_client", None) is not None:
             return self.__compute_client
 
-        compute_login_manager = gladier.managers.compute_login_manager.ComputeLoginManager(
-            authorizers=self.login_manager.get_manager_authorizers()
+        compute_login_manager = (
+            gladier.managers.compute_login_manager.ComputeLoginManager(
+                authorizers=self.login_manager.get_manager_authorizers()
+            )
         )
 
-        self.__compute_client = Client(login_manager=compute_login_manager)
+        self.__compute_client = Client(
+            code_serialization_strategy=serialize.DillCodeSource(),
+            login_manager=compute_login_manager
+    )
         return self.__compute_client
 
     @staticmethod
     def get_compute_function_name(compute_function):
         """
         Generate a function name given a compute function. These function namse are used to refer
         to compute functions within the config. There is no guarantee of uniqueness for function
         names.
 
         :return: human readable string identifier for a function (intended for a gladier.cfg file)
         """
-        return f'{compute_function.__name__}_function_id'
+        return f"{compute_function.__name__}_function_id"
 
     @staticmethod
     def get_compute_function_checksum(compute_function):
         """
         Get the SHA256 checksum of a compute function
         :return: sha256 hex string of a given compute function
         """
-        fxs = serialize.ComputeSerializer()
+        fxs = serialize.ComputeSerializer(strategy_code=serialize.DillCodeSource())
         serialized_func = fxs.serialize(compute_function).encode()
         return hashlib.sha256(serialized_func).hexdigest()
 
     def validate_function(self, tool: GladierBaseTool, function):
         fid_name = gladier.utils.name_generation.get_compute_function_name(function)
         fid = self.storage.get_value(fid_name)
         checksum = self.get_compute_function_checksum(function)
-        checksum_name = gladier.utils.name_generation.get_compute_function_checksum_name(function)
+        checksum_name = (
+            gladier.utils.name_generation.get_compute_function_checksum_name(function)
+        )
         try:
             if not fid_name:
                 raise gladier.exc.RegistrationException(
-                    f'Tool {tool.__class__.__name__} missing compute registration for {fid_name}')
+                    f"Tool {tool.__class__.__name__} missing compute registration for {fid_name}"
+                )
             if not self.storage.get_value(checksum_name):
                 raise gladier.exc.RegistrationException(
-                    f'Tool {tool.__class__.__name__} with function {fid_name} '
-                    f'has a function id but no checksum!')
+                    f"Tool {tool.__class__.__name__} with function {fid_name} "
+                    f"has a function id but no checksum!"
+                )
             if not self.storage.get_value(checksum_name) == checksum:
                 raise gladier.exc.FunctionObsolete(
-                    f'Tool {tool.__class__.__name__} with function {fid_name} '
-                    f'has changed and needs to be re-registered.')
+                    f"Tool {tool.__class__.__name__} with function {fid_name} "
+                    f"has changed and needs to be re-registered."
+                )
         except (gladier.exc.RegistrationException, gladier.exc.FunctionObsolete):
             if self.auto_registration is True:
-                log.info(f'{tool.__class__.__name__}: function {function.__name__} is out of date')
+                log.info(
+                    f"{tool.__class__.__name__}: function {function.__name__} is out of date"
+                )
                 fid = self.register_function(tool, function)
-                fx_name = gladier.utils.name_generation.get_compute_function_name(function)
+                fx_name = gladier.utils.name_generation.get_compute_function_name(
+                    function
+                )
                 self.storage.set_value(fx_name, fid)
                 self.storage.set_value(checksum_name, checksum)
             else:
                 raise
         finally:
             return fid_name, fid
 
     def register_function(self, tool: GladierBaseTool, function):
         """Register the functions with Globus Compute."""
-        log.info(f'{tool.__class__.__name__}: registering function {function.__name__}')
+        log.info(f"{tool.__class__.__name__}: registering function {function.__name__}")
         return self.compute_client.register_function(function)
```

### Comparing `gladier-0.9.0b1/gladier/managers/flows_manager.py` & `gladier-0.9.0b2/gladier/managers/flows_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,18 @@
     RUN_STATUS_SCOPE,
     RUN_MANAGE_SCOPE,
 )
 
 log = logging.getLogger(__name__)
 
 
-def ensure_flow_registered(flows_manager_instance, exc: gladier.exc.RegistrationException):
-    log.info(f'Deploying/Updating flow due to: {str(exc)}')
+def ensure_flow_registered(
+    flows_manager_instance, exc: gladier.exc.RegistrationException
+):
+    log.info(f"Deploying/Updating flow due to: {str(exc)}")
     flows_manager_instance.register_flow()
 
 
 class FlowsManager(ServiceManager):
     """
     The flows manager tracks an externally defined flow_definition and ensures it stays
     up-to-date with a deployment in the flows service. It can be run without a flow_id
@@ -81,39 +83,44 @@
         MANAGE_FLOWS_SCOPE,
         VIEW_FLOWS_SCOPE,
         RUN_FLOWS_SCOPE,
         RUN_STATUS_SCOPE,
         RUN_MANAGE_SCOPE,
     ]
 
-    def __init__(self,
-                 flow_id: str = None,
-                 flow_definition: dict = None,
-                 flow_schema: dict = None,
-                 flow_title: str = None,
-                 globus_group: str = None,
-                 subscription_id: str = None,
-                 on_change: Callable = ensure_flow_registered,
-                 redeploy_on_404: bool = True,
-                 **kwargs):
+    def __init__(
+        self,
+        flow_id: str = None,
+        flow_definition: dict = None,
+        flow_schema: dict = None,
+        flow_title: str = None,
+        globus_group: str = None,
+        subscription_id: str = None,
+        on_change: Callable = ensure_flow_registered,
+        redeploy_on_404: bool = True,
+        **kwargs,
+    ):
         self.flow_id = flow_id
         self.flow_definition = flow_definition
         self.flow_schema = flow_schema
         self.flow_title = flow_title
         self.globus_group = globus_group
         self.on_change = on_change or (lambda self, exc: None)
         self.redeploy_on_404 = redeploy_on_404
 
         if subscription_id:
-            warnings.warn(f'{self.flow_title}: subscription_id is no longer used and '
-                          'should not be set on flows.', category=DeprecationWarning)
+            warnings.warn(
+                f"{self.flow_title}: subscription_id is no longer used and "
+                "should not be set on flows.",
+                category=DeprecationWarning,
+            )
 
         if self.flow_id is not None:
             self.redeploy_on_404 = False
-            log.info('Custom Flow ID set, redeploy_on_404 disabled.')
+            log.info("Custom Flow ID set, redeploy_on_404 disabled.")
 
         super().__init__(**kwargs)
 
     def get_scopes(self):
         scopes = self.AVAILABLE_SCOPES.copy()
         flow_scope = self.flow_scope
         if flow_scope:
@@ -130,59 +137,61 @@
             # It's possible storage wasn't set yet, and get_flow_id() raises
             # an error here. Simply ignore it for the time being.
             flow_id = None
         if flow_id:
             # In the future, this should be gettable via
             # globus_sdk.SpecificFlowClient(flow_id).scopes.url_scope_string('flow_id'))
             scope_name = f'flow_{flow_id.replace("-", "_")}_user'
-            return f'https://auth.globus.org/scopes/{flow_id}/{scope_name}'
+            return f"https://auth.globus.org/scopes/{flow_id}/{scope_name}"
 
     @property
     def flow_definition(self) -> dict:
         return self._flow_definition
 
     @flow_definition.setter
     def flow_definition(self, value: dict):
         self._flow_definition = value
 
     @property
     def flow_schema(self) -> dict:
         return self._flow_schema or {
-            'input_schema': {
-                'additionalProperties': True,
-                'properties': {},
-                'type': 'object'
+            "input_schema": {
+                "additionalProperties": True,
+                "properties": {},
+                "type": "object",
             }
         }
 
     @flow_schema.setter
     def flow_schema(self, value: dict):
         self._flow_schema = value
 
     @property
     def flows_client(self):
         """
         :return: an authorized Gloubs Automate Client. If a flow has been deployed,
         the client returned will be authorized to run the flow. Stale clients pre-flow-deployment
         will need to call this again in order to run flows.
         """
-        if getattr(self, '_flows_client', None) is not None:
+        if getattr(self, "_flows_client", None) is not None:
             return self._flows_client
         authorizers = self.login_manager.get_manager_authorizers()
 
         automate_authorizer = authorizers[
             globus_automate_client.flows_client.MANAGE_FLOWS_SCOPE
         ]
         flow_authorizer = authorizers.get(self.flow_scope)
 
         def get_flow_authorizer(*args, **kwargs):
             return flow_authorizer
 
         self._flows_client = globus_automate_client.FlowsClient.new_client(
-            None, get_flow_authorizer, automate_authorizer,
+            None,
+            get_flow_authorizer,
+            automate_authorizer,
         )
         return self._flows_client
 
     def refresh_flows_client(self) -> globus_automate_client.FlowsClient:
         self._flows_client = None
         return self.flows_client
 
@@ -196,24 +205,25 @@
 
         flow_def = json.dumps(flow_definition, sort_keys=True)
         flow_schema = json.dumps(flow_schema, sort_keys=True)
         data = (flow_def + flow_schema).encode()
         return hashlib.sha256(data).hexdigest()
 
     @staticmethod
-    def get_globus_urn(uuid, id_type='group'):
+    def get_globus_urn(uuid, id_type="group"):
         """Convenience method for appending the correct Globus URN prefix on a uuid."""
         URN_PREFIXES = {
-            'group': 'urn:globus:groups:id:',
-            'identity': 'urn:globus:auth:identity:'
+            "group": "urn:globus:groups:id:",
+            "identity": "urn:globus:auth:identity:",
         }
         if id_type not in URN_PREFIXES:
-            raise gladier.exc.DevelopmentException('"id_type" must be one of '
-                                                   f'{URN_PREFIXES.keys()}. Got: {id_type}')
-        return f'{URN_PREFIXES[id_type]}{uuid}'
+            raise gladier.exc.DevelopmentException(
+                '"id_type" must be one of ' f"{URN_PREFIXES.keys()}. Got: {id_type}"
+            )
+        return f"{URN_PREFIXES[id_type]}{uuid}"
 
     def get_flow_permission(self, permission_type, identities=None):
         """
         This function is a generic shim that should work for most Gladier clients that
         want basic permissions that will work with a single Globus Group. This method can be
         overridden to change any of the automate defaults:
 
@@ -225,26 +235,31 @@
 
         By default, always returns either None for using automate defaults, or setting every
         permission_type above to use the set client `globus_group`.
         """
         if identities is None and self.globus_group:
             identities = [self.get_globus_urn(self.globus_group)]
         permission_types = {
-            'flow_viewers', 'flow_starters', 'flow_administrators', 'run_managers', 'run_monitors'
+            "flow_viewers",
+            "flow_starters",
+            "flow_administrators",
+            "run_managers",
+            "run_monitors",
         }
         if permission_type not in permission_types:
-            raise gladier.exc.DevelopmentException(f'permission_type must be one of '
-                                                   f'{permission_types}')
+            raise gladier.exc.DevelopmentException(
+                f"permission_type must be one of " f"{permission_types}"
+            )
         return identities
 
     def get_flow_id(self) -> str:
         """Return flow id. If an ID was set on this class in the constructor, that is
         used. Otherwise, a retrieve from storage is attempted with 'flow_id'.
         :returns: flow_id uuid for deployed flow, or None if it does not exist"""
-        return self.flow_id or self.storage.get_value('flow_id')
+        return self.flow_id or self.storage.get_value("flow_id")
 
     def flow_changed(self) -> bool:
         """
         Returns True if a flow id exists and the stored checksum matches the set
         flow_definition. False otherwise.
         :raises: Nothing
         """
@@ -259,21 +274,25 @@
         Check if the flow has changed by validating the current flow_definition agaist
         the stored checksum. Raises an exception if the checksums do not match.
 
         :raises: gladier.exc.NoFlowRegistered if no flow has been registered
         :raises: gladier.exc.FlowObsolete if the stored flow checksums do not match
         """
         flow_id = self.get_flow_id()
-        flow_checksum = self.storage.get_value('flow_checksum')
+        flow_checksum = self.storage.get_value("flow_checksum")
         if not flow_id:
             raise gladier.exc.NoFlowRegistered(
-                'No flow_id set on flow manager and no id tracked in storage.')
-        elif flow_checksum != self.get_flow_checksum(self.flow_definition, self.flow_schema):
+                "No flow_id set on flow manager and no id tracked in storage."
+            )
+        elif flow_checksum != self.get_flow_checksum(
+            self.flow_definition, self.flow_schema
+        ):
             raise gladier.exc.FlowObsolete(
-                f'"flow_definition" on {self} has changed and needs to be re-registered.')
+                f'"flow_definition" on {self} has changed and needs to be re-registered.'
+            )
 
     def sync_flow(self) -> str:
         """
         Get the current flow id for the current Gladier flow definition.
         If self.auto_register is True, it will automatically (re)register a flow if it
         has changed on disk, otherwise raising exceptions.
 
@@ -301,122 +320,137 @@
         a new login will be needed before the flow can be run.
         :raises: globus_sdk.exc.GlobusAPIError on error deploying flow
         :return: an automate flow UUID
         """
         flow_id = self.get_flow_id()
         flow_permissions = {
             p_type: self.get_flow_permission(p_type)
-            for p_type in ['flow_viewers', 'flow_starters', 'flow_administrators']
+            for p_type in ["flow_viewers", "flow_starters", "flow_administrators"]
             if self.get_flow_permission(p_type)
         }
         log.debug(f'Flow permissions set to: {flow_permissions or "Flows defaults"}')
         flow_kwargs = flow_permissions
         # Input schema is a required field and must be part of all flows.
-        flow_kwargs['input_schema'] = self.flow_schema
+        flow_kwargs["input_schema"] = self.flow_schema
         if flow_id:
             try:
-                log.info(f'Flow checksum failed, updating flow {flow_id}...')
-                self.flows_client.update_flow(flow_id, self.flow_definition, **flow_kwargs)
+                log.info(f"Flow checksum failed, updating flow {flow_id}...")
+                self.flows_client.update_flow(
+                    flow_id, self.flow_definition, **flow_kwargs
+                )
                 self.storage.set_value(
-                    'flow_checksum', self.get_flow_checksum(self.flow_definition, self.flow_schema)
+                    "flow_checksum",
+                    self.get_flow_checksum(self.flow_definition, self.flow_schema),
                 )
             except globus_sdk.exc.GlobusAPIError as gapie:
                 if gapie.http_status == 404 and self.redeploy_on_404:
                     flow_id = None
                 else:
                     raise
         if flow_id is None:
-            log.info('No flow detected, deploying new flow...')
-            flow = self.flows_client.deploy_flow(self.flow_definition, title=self.flow_title,
-                                                 **flow_kwargs).data
+            log.info("No flow detected, deploying new flow...")
+            flow = self.flows_client.deploy_flow(
+                self.flow_definition, title=self.flow_title, **flow_kwargs
+            ).data
             log.debug(f'Flow deployed with id {flow["id"]}')
-            self.storage.set_value('flow_id', flow['id'])
+            self.storage.set_value("flow_id", flow["id"])
             self.storage.set_value(
-                'flow_checksum', self.get_flow_checksum(self.flow_definition, self.flow_schema)
+                "flow_checksum",
+                self.get_flow_checksum(self.flow_definition, self.flow_schema),
             )
-            self.login_manager.add_requirements([flow['globus_auth_scope']])
+            self.login_manager.add_requirements([flow["globus_auth_scope"]])
             self.refresh_flows_client()
 
         return flow_id
 
     def purge_flow(self):
         """
         Remove the stored flow_id and flow_checksum.
         """
-        self.storage.del_value('flow_id')
-        self.storage.del_value('flow_checksum')
+        self.storage.del_value("flow_id")
+        self.storage.del_value("flow_checksum")
 
     def run_flow(self, **kwargs):
         flow_id = self.get_flow_id()
 
         permissions = {
             p_type: self.get_flow_permission(p_type)
-            for p_type in ['run_managers', 'run_monitors']
+            for p_type in ["run_managers", "run_monitors"]
             if self.get_flow_permission(p_type)
         }
         log.debug(f'Flow run permissions set to: {permissions or "Flows defaults"}')
         kwargs.update(permissions)
 
         # Ensure the label is not longer than 64 chars
-        if 'label' in kwargs:
-            label = kwargs['label']
-            kwargs['label'] = (label[:62] + '..') if len(label) > 64 else label
+        if "label" in kwargs:
+            label = kwargs["label"]
+            kwargs["label"] = (label[:62] + "..") if len(label) > 64 else label
 
         try:
             flow = self.flows_client.run_flow(flow_id, self.flow_scope, **kwargs).data
         except globus_sdk.exc.GlobusAPIError as gapie:
-            log.debug('Encountered error when running flow', exc_info=True)
+            log.debug("Encountered error when running flow", exc_info=True)
             automate_error_message = json.loads(gapie.message)
-            detail_message = automate_error_message['error']['detail']
-            if 'unable to get tokens for scopes' in detail_message:
+            detail_message = automate_error_message["error"]["detail"]
+            if "unable to get tokens for scopes" in detail_message:
                 self.login_manager.add_scope_change([self.flow_scope])
                 self.refresh_flows_client()
-                log.info('Initiating new login for dependent scope change')
-                flow = self.flows_client.run_flow(flow_id, self.flow_scope, **kwargs).data
+                log.info("Initiating new login for dependent scope change")
+                flow = self.flows_client.run_flow(
+                    flow_id, self.flow_scope, **kwargs
+                ).data
             elif gapie.http_status == 404 and self.redeploy_on_404:
-                log.warning(f'Flow {flow_id} returned 404 and is either deleted or unavailable. '
-                            f'Purging flow_id from config file...')
+                log.warning(
+                    f"Flow {flow_id} returned 404 and is either deleted or unavailable. "
+                    f"Purging flow_id from config file..."
+                )
                 # On a 404, Gladier can't do anything since it cannot access the old flow.
                 # Therefore, purge the old flow and deploy a new one.
                 self.purge_flow()
                 # Ensure the new flow is deployed
                 self.sync_flow()
                 # Fetch the new flow id
                 flow_id = self.get_flow_id()
-                flow = self.flows_client.run_flow(flow_id, self.flow_scope, **kwargs).data
+                flow = self.flows_client.run_flow(
+                    flow_id, self.flow_scope, **kwargs
+                ).data
             else:
                 raise
-        log.info(f'Started flow {kwargs.get("label")} flow id '
-                 f'"{flow_id}" with run "{flow["run_id"]}"')
+        log.info(
+            f'Started flow {kwargs.get("label")} flow id '
+            f'"{flow_id}" with run "{flow["run_id"]}"'
+        )
 
-        if flow['status'] == 'FAILED':
-            raise gladier.exc.ConfigException(f'Flow Failed: {flow["details"]["description"]}')
+        if flow["status"] == "FAILED":
+            raise gladier.exc.ConfigException(
+                f'Flow Failed: {flow["details"]["description"]}'
+            )
         return flow
 
     def get_status(self, run_id):
         """
         Get the current status of the automate flow. Attempts to do additional work on compute
         functions to deserialize any exception output.
 
         :param run_id: The globus action UUID used for this flow. The Automate flow id is
                           always the flow_id configured for this tool.
         :raises: Globus Automate exceptions from self.flows_client.flow_action_status
         :returns: a Globus Automate status object (with varying state structures)
         """
         status = self.flows_client.flow_action_status(
-                self.get_flow_id(), self.flow_scope, run_id
-            ).data
+            self.get_flow_id(), self.flow_scope, run_id
+        ).data
         try:
             return gladier.utils.automate.get_details(status)
         except (KeyError, AttributeError):
             return status
 
     @staticmethod
     def _default_progress_callback(response):
-        if response['status'] == 'ACTIVE':
+        if response["status"] == "ACTIVE":
             print(f'[{response["status"]}]: {response["details"]["description"]}')
 
     def progress(self, run_id, callback=None):
         """
         Continuously call self.get_status() until the flow completes. Each status response is
         used as a parameter to the provided callback, by default will use the builtin callback
         to print the current state to stdout.
@@ -424,15 +458,15 @@
         :param run_id: The action id for a running flow. The flow is automatically pulled
                           based on the current tool's flow_definition.
         :param callback: The function to call with the result from self.get_status. Must take
                          a single parameter: mycallback(self.get_status())
         """
         callback = callback or self._default_progress_callback
         status = self.get_status(run_id)
-        while status['status'] not in ['SUCCEEDED', 'FAILED']:
+        while status["status"] not in ["SUCCEEDED", "FAILED"]:
             status = self.get_status(run_id)
             callback(status)
 
     def get_details(self, run_id, state_name):
         """
         Attempt to extrapolate details from get_status() for a given state_name define in the flow
         definition. Note: This is usually only possible when a flow completes.
```

### Comparing `gladier-0.9.0b1/gladier/managers/login_manager.py` & `gladier-0.9.0b2/gladier/managers/login_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,92 +1,105 @@
 import logging
 import time
 from typing import Callable, List, Set, Iterable, Union, Any, Mapping
 import abc
 
 import fair_research_login
-from globus_sdk import AccessTokenAuthorizer, RefreshTokenAuthorizer, ConfidentialAppAuthClient
+from globus_sdk import (
+    AccessTokenAuthorizer,
+    RefreshTokenAuthorizer,
+    ConfidentialAppAuthClient,
+)
 from gladier.exc import AuthException
 from gladier.storage.tokens import GladierSecretsConfig
 
 log = logging.getLogger(__name__)
 
 
 class BaseLoginManager(abc.ABC):
-
     def __init__(self, *args, **kwargs):
         self.required_scopes = set()
         self.scope_changes = set()
 
     @property
     def missing_authorizers(self) -> Set[str]:
         return self.get_missing_authorizers(self.get_authorizers())
 
     def get_missing_authorizers(
         self,
-        authorizers: Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]
-            ) -> Set[str]:
+        authorizers: Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]],
+    ) -> Set[str]:
         # Disregard any scopes not in the 'required' list. This allows implementers to return
         # unrelated scopes.
         absent = self.required_scopes.difference(authorizers)
-        log.info(f'Scopes Absent: {absent or None}, Need Update: {self.scope_changes or None}')
+        log.info(
+            f"Scopes Absent: {absent or None}, Need Update: {self.scope_changes or None}"
+        )
         return absent | self.scope_changes
 
     def get_manager_authorizers(self):
         authorizers = self.get_authorizers()
         missing = self.get_missing_authorizers(authorizers)
 
         if missing:
-            log.info('Attempting login to fetch missing authorizers.')
+            log.info("Attempting login to fetch missing authorizers.")
             self.login(missing)
             authorizers = self.get_authorizers()
             missing = self.get_missing_authorizers(authorizers)
 
         if missing:
-            raise AuthException('Manager Failed to produce '
-                                f'authorizers for missing scopes: {missing}')
+            raise AuthException(
+                "Manager Failed to produce "
+                f"authorizers for missing scopes: {missing}"
+            )
         return authorizers
 
     @abc.abstractmethod
-    def get_authorizers(self) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
+    def get_authorizers(
+        self,
+    ) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
         """
         This method MUST be implemented by the implementing class.
 
         Load any existing authorizers and return them to the client. A login *should not* be
         attempted. The Login Manager will determine if the scopes provided are sufficient, and
         automatically call login() they are not.
         """
-        raise NotImplementedError(f'{self.__class__.__name__} must implement .get_authorizers()')
+        raise NotImplementedError(
+            f"{self.__class__.__name__} must implement .get_authorizers()"
+        )
 
     @abc.abstractmethod
     def login(self, scopes: List[str]):
         """
         This method MUST be implemented by the implementing class.
 
         If this method is called, get_authorizers() has insufficient scopes and requires more
         scopes to continue operations. ``scopes`` MAY reference scopes already saved, which can
         happen if dependent scopes have been added to the scope since last login. For this reason,
         previously saved scopes in this list should be disregarded.
         """
-        raise NotImplementedError(f'{self.__class__.__name__} must implement .ensure_logged_in()')
+        raise NotImplementedError(
+            f"{self.__class__.__name__} must implement .ensure_logged_in()"
+        )
 
     def is_logged_in(self) -> bool:
         return not bool(self.missing_authorizers)
 
     def add_requirements(self, scopes: Iterable[str]):
-        log.debug(f'Added required scopes {scopes}')
+        log.debug(f"Added required scopes {scopes}")
         self.required_scopes = self.required_scopes | set(scopes)
 
     def add_scope_change(self, scopes: Iterable[str]):
         """
         A scope change happens when the underlying scope gets updated with new dependent scopes,
         and the current token we now have is invalid and can no longer be used. The solution is
         a new login to get a new token.
         """
-        log.debug(f'Tracking scope change: {scopes}')
+        log.debug(f"Tracking scope change: {scopes}")
         self.scope_changes = self.scope_changes | set(scopes)
 
 
 class AutoLoginManager(BaseLoginManager):
     """
     Default Login Manager class in Gladier. Automatically initiates a login if any scope
     is missing or needs to be updated.
@@ -99,35 +112,39 @@
         self.storage = storage
         self.client_id = client_id
         self.app_name = app_name
         self.auto_login = auto_login
 
     @property
     def native_client(self):
-        if getattr(self, 'client_id', None) is None:
+        if getattr(self, "client_id", None) is None:
             raise AuthException(
-                'Gladier client must be instantiated with a '
+                "Gladier client must be instantiated with a "
                 '"client_id" to use "login()!'
             )
-        return fair_research_login.NativeClient(client_id=self.client_id,
-                                                app_name=self.app_name,
-                                                token_storage=self.storage)
+        return fair_research_login.NativeClient(
+            client_id=self.client_id, app_name=self.app_name, token_storage=self.storage
+        )
 
-    def get_authorizers(self) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
+    def get_authorizers(
+        self,
+    ) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
         try:
             return self.native_client.get_authorizers_by_scope()
         except fair_research_login.LoadError:
             return dict()
 
     def login(self, scopes):
         if self.auto_login is False:
-            raise AuthException(f'Automatic login is disabled. Missing scopes: {scopes}')
-        self.native_client.login(requested_scopes=scopes,
-                                 refresh_toknes=self.refresh_tokens,
-                                 force=True)
+            raise AuthException(
+                f"Automatic login is disabled. Missing scopes: {scopes}"
+            )
+        self.native_client.login(
+            requested_scopes=scopes, refresh_toknes=self.refresh_tokens, force=True
+        )
 
     def logout(self):
         self.native_client.logout()
 
 
 class CallbackLoginManager(BaseLoginManager):
     """
@@ -141,70 +158,80 @@
     :param callback: A Callable which will be invoked if additional scopes are needed.
 
     """
 
     def __init__(
         self,
         authorizers: Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]],
-        callback: Callable = None
+        callback: Callable = None,
     ):
         super().__init__()
         self.authorizers = authorizers
         self.callback = callback
 
-    def get_authorizers(self) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
+    def get_authorizers(
+        self,
+    ) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
         return self.authorizers
 
     def login(self, scopes):
         if not self.callback:
-            raise AuthException('New login required for scopes and no callback set on '
-                                f'login manager: {scopes}')
+            raise AuthException(
+                "New login required for scopes and no callback set on "
+                f"login manager: {scopes}"
+            )
         new_authorizers = self.callback(scopes)
         self.authorizers.update(new_authorizers)
-        log.info('New authorizers have been cached for re-use.')
+        log.info("New authorizers have been cached for re-use.")
 
 
 class ConfidentialClientLoginManager(BaseLoginManager):
     refresh_tokens = True
 
-    def __init__(self, client_id: str, client_secret: str, storage: GladierSecretsConfig):
+    def __init__(
+        self, client_id: str, client_secret: str, storage: GladierSecretsConfig
+    ):
         super().__init__()
         self.storage: GladierSecretsConfig = storage
         self.client_id = client_id
         self.app = ConfidentialAppAuthClient(client_id, client_secret)
 
     def login(self, scopes: List[str]) -> None:
-        log.info('Initiating client credentials grant using client_id and secret')
+        log.info("Initiating client credentials grant using client_id and secret")
         response = self.app.oauth2_client_credentials_tokens(requested_scopes=scopes)
         self.storage.write_tokens(response.by_resource_server)
 
     def by_scopes(self, tokens):
         # Get a flat list of scopes
-        scopes = [tset['scope'].split() for tset in tokens.values()]
+        scopes = [tset["scope"].split() for tset in tokens.values()]
         scopes = [item for sublist in scopes for item in sublist]
 
         token_group = {}
         for scope in scopes:
             for tgroup in tokens.values():
-                if scope in tgroup['scope'].split():
+                if scope in tgroup["scope"].split():
                     token_group[scope] = tgroup
         return token_group
 
-    def get_authorizers(self) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
+    def get_authorizers(
+        self,
+    ) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
         tokens = self.storage.read_tokens()
         if not tokens:
-            log.info('Tokens failed to load, no tokens in storage.')
+            log.info("Tokens failed to load, no tokens in storage.")
             return dict()
 
-        expired = any(t['expires_at_seconds'] < time.time() for t in tokens.values())
+        expired = any(t["expires_at_seconds"] < time.time() for t in tokens.values())
         if expired:
-            log.info('Tokens Expired, clearing cache')
+            log.info("Tokens Expired, clearing cache")
             self.storage.clear_tokens()
             return dict()
 
         return {
-            scope: RefreshTokenAuthorizer(refresh_token=tdata['refresh_token'],
-                                          auth_client=self.app,
-                                          access_token=tdata['access_token'],
-                                          expires_at=tdata['expires_at_seconds'])
+            scope: RefreshTokenAuthorizer(
+                refresh_token=tdata["refresh_token"],
+                auth_client=self.app,
+                access_token=tdata["access_token"],
+                expires_at=tdata["expires_at_seconds"],
+            )
             for scope, tdata in self.by_scopes(tokens).items()
         }
```

### Comparing `gladier-0.9.0b1/gladier/managers/service_manager.py` & `gladier-0.9.0b2/gladier/managers/service_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-
 import logging
 from typing import List
 import abc
 from gladier.managers.login_manager import BaseLoginManager
 from gladier.storage.config import GladierConfig
 
 
 log = logging.getLogger(__name__)
 
 
 class ServiceManager(abc.ABC):
-
     def __init__(self, **kwargs):
-        self._storage = kwargs.get('storage')
+        self._storage = kwargs.get("storage")
 
-        self.login_manager = kwargs.get('login_manager')
+        self.login_manager = kwargs.get("login_manager")
         self.register_scopes()
 
     @property
     def storage(self):
         if self._storage is None:
-            raise AttributeError(f'Storage has not been set for {self}')
+            raise AttributeError(f"Storage has not been set for {self}")
         return self._storage
 
     @storage.setter
     def storage(self, value):
         self.set_storage(value)
 
     def set_storage(self, storage: GladierConfig, replace: bool = True) -> None:
         if replace:
-            log.info(f'Replacing storage {self._storage} with {storage}')
+            log.info(f"Replacing storage {self._storage} with {storage}")
             self._storage = storage
         else:
             self._storage = self._storage or storage
-        log.debug(f'Storage for {self} set to {self._storage}')
+        log.debug(f"Storage for {self} set to {self._storage}")
 
-    def set_login_manager(self, login_manager: BaseLoginManager, replace: bool = True) -> None:
+    def set_login_manager(
+        self, login_manager: BaseLoginManager, replace: bool = True
+    ) -> None:
         if replace:
-            log.info(f'Replacing login manager {self.login_manager} with {login_manager}')
+            log.info(
+                f"Replacing login manager {self.login_manager} with {login_manager}"
+            )
             self.login_manager = login_manager
         else:
             self.login_manager = self.login_manager or login_manager
         self.login_manager.add_requirements(self.get_scopes())
-        log.debug(f'Login Manager for {self} set to {self.login_manager}')
+        log.debug(f"Login Manager for {self} set to {self.login_manager}")
 
     def register_scopes(self):
         """
         Register scopes returned by `get_scopes()` with the login manager"""
         if self.login_manager is not None:
             self.login_manager.add_requirements(self.get_scopes())
 
     def get_scopes() -> List[str]:
-        raise NotImplementedError('Service Managers must define their own scope needs')
+        raise NotImplementedError("Service Managers must define their own scope needs")
```

### Comparing `gladier-0.9.0b1/gladier/storage/config.py` & `gladier-0.9.0b2/gladier/storage/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,32 +2,31 @@
 import configparser
 from gladier.storage.migrations import needs_migration, migrate_gladier
 
 log = logging.getLogger(__name__)
 
 
 class GladierConfig(configparser.ConfigParser):
-
-    def __init__(self, filename, section='default'):
+    def __init__(self, filename, section="default"):
         super().__init__()
         self.section = section
         self.filename = filename
         self.load()
 
     def load(self):
         self.read(self.filename)
         if self.section not in self.sections():
-            log.debug(f'Section {self.section} missing, adding to config.')
+            log.debug(f"Section {self.section} missing, adding to config.")
             self[self.section] = {}
             self.save()
 
     def save(self):
-        with open(self.filename, 'w') as configfile:
+        with open(self.filename, "w") as configfile:
             self.write(configfile)
-            log.debug(f'Saved local gladier config to {configfile}')
+            log.debug(f"Saved local gladier config to {configfile}")
 
     def update(self):
         if needs_migration(self):
             self = migrate_gladier(self)
             self.save()
 
     def get_value(self, name: str) -> str:
```

### Comparing `gladier-0.9.0b1/gladier/storage/migrations.py` & `gladier-0.9.0b2/gladier/storage/migrations.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 import gladier.version
 import traceback
 
 log = logging.getLogger(__name__)
 
 
 class ConfigMigration(ABC):
-
     def __init__(self, config):
         self.config = config
 
-        if 'general' not in self.config.sections():
-            log.debug('No version in config, adding...')
-            self.config.add_section('general')
-        cfg_version = self.config['general'].get('version')
+        if "general" not in self.config.sections():
+            log.debug("No version in config, adding...")
+            self.config.add_section("general")
+        cfg_version = self.config["general"].get("version")
 
         self.config_version = version.parse(cfg_version) if cfg_version else None
         self.version = version.parse(gladier.version.__version__)
 
     @abstractmethod
     def is_applicable(self):
         pass
@@ -31,123 +30,148 @@
         pass
 
 
 class AddVersionToConfig(ConfigMigration):
     """
     Add a version if one does not exist in the config.
     """
+
     def is_applicable(self):
         return self.config_version is None
 
     def migrate(self):
         # Set the version
-        self.config['general']['version'] = str(self.version)
-        log.info(f'Setting Version {self.version}')
+        self.config["general"]["version"] = str(self.version)
+        log.info(f"Setting Version {self.version}")
 
 
 class UpdateConfigVersion(ConfigMigration):
     """Sets the config version to the current version of Gladier.
     Should be run LAST, after all other migrations have taken place"""
+
     def is_applicable(self):
         return self.config_version != self.version
 
     def migrate(self):
-        self.config['general']['version'] = str(self.version)
+        self.config["general"]["version"] = str(self.version)
 
 
 class MigrateOldConfigFile(ConfigMigration):
     old_cfg = pathlib.Path("~/.gladier-secrets.cfg").expanduser()
 
     def is_applicable(self):
         if not self.old_cfg.exists():
             return False
-        log.warning(f'Old config {self.old_cfg} exists and should be migrated or removed.')
+        log.warning(
+            f"Old config {self.old_cfg} exists and should be migrated or removed."
+        )
 
         # The new default section will have some stuff pre-populated, but it will be empty.
         # Check for empty stuff, and then we can go ahead with migration.
         fname = self.config.filename
         sections = self.config.sections()
 
         # Check for extra sections, abort if more sections than expected
         if len(sections) > 3:
-            log.warning(f'Existing config {fname} contains section data, skipping migration..')
+            log.warning(
+                f"Existing config {fname} contains section data, skipping migration.."
+            )
             return False
 
         # Of three sections, one will be generic, one will be tokens, and the third will have
         # client-related info. Find the third one and check it for content, and abort if it
         # contains any.
-        data_section = [x for x in sections if x != 'general' and not x.startswith('tokens_')]
-        if len(data_section) == 0 or len(list(self.config[data_section[0]].values())) > 0:
-            log.warning(f'Existing config {fname} contains values in {data_section} which may be '
-                        'important, skipping...')
+        data_section = [
+            x for x in sections if x != "general" and not x.startswith("tokens_")
+        ]
+        if (
+            len(data_section) == 0
+            or len(list(self.config[data_section[0]].values())) > 0
+        ):
+            log.warning(
+                f"Existing config {fname} contains values in {data_section} which may be "
+                "important, skipping..."
+            )
             return False
 
         return True
 
     def migrate(self):
         try:
             # Read the old config file and copy values into it
-            log.info(f'Migrating old config {self.old_cfg} to {self.config.filename}')
+            log.info(f"Migrating old config {self.old_cfg} to {self.config.filename}")
             old_cfg = configparser.ConfigParser()
             old_cfg.read(self.old_cfg)
             for section, section_values in old_cfg.items():
                 if section not in self.config.sections():
                     self.config[section] = {}
                 for k, v in section_values.items():
                     self.config.set(section, k, v)
-            log.info(f'Successfully migrated {self.old_cfg} to {self.config.filename}')
+            log.info(f"Successfully migrated {self.old_cfg} to {self.config.filename}")
             self.old_cfg.unlink()
-            log.info(f'Removed {self.old_cfg}')
+            log.info(f"Removed {self.old_cfg}")
         except Exception:
             traceback.print_exc()
-            print('Failed to migrate Gladier config. Please send us the error above!')
-            print(f'If you see this error again, you can try deleting ~/.gladier-secrets.cfg '
-                  'and config files under ~/.gladier/')
+            print("Failed to migrate Gladier config. Please send us the error above!")
+            print(
+                f"If you see this error again, you can try deleting ~/.gladier-secrets.cfg "
+                "and config files under ~/.gladier/"
+            )
 
 
 class UpdateFuncXFunctions(ConfigMigration):
     """Updates from old functions which were named: my_thing_funcx_id to
     the newer compute function names named my_thing_function_id"""
+
     def is_applicable(self):
         for section in self.config.sections():
             for key in self.config[section].keys():
-                if key.endswith('funcx_id') and not key.count('funcx_id') > 1:
+                if key.endswith("funcx_id") and not key.count("funcx_id") > 1:
                     return True
 
     def migrate(self):
         for section in self.config.sections():
             try:
                 todelete = []
                 for key, value in self.config[section].items():
-                    if key.endswith('funcx_id') and not key.count('funcx_id') > 1:
-                        oldkey_checksum = f'{key}_checksum'
-                        newkey = key.replace('funcx_id', 'function_id')
-                        newkey_checksum = f'{newkey}_checksum'
+                    if key.endswith("funcx_id") and not key.count("funcx_id") > 1:
+                        oldkey_checksum = f"{key}_checksum"
+                        newkey = key.replace("funcx_id", "function_id")
+                        newkey_checksum = f"{newkey}_checksum"
                         if not self.config[section].get(newkey):
-                            log.info(f'Migrating new function name {section}.{key} to '
-                                     f'{section}.{newkey}')
+                            log.info(
+                                f"Migrating new function name {section}.{key} to "
+                                f"{section}.{newkey}"
+                            )
                             self.config[section][newkey] = value
-                            log.info('Migrating new function checksum name '
-                                     f'{section}.{oldkey_checksum} to {section}.{newkey_checksum}')
-                            self.config[section][newkey_checksum] = \
-                                self.config[section][oldkey_checksum]
+                            log.info(
+                                "Migrating new function checksum name "
+                                f"{section}.{oldkey_checksum} to {section}.{newkey_checksum}"
+                            )
+                            self.config[section][newkey_checksum] = self.config[
+                                section
+                            ][oldkey_checksum]
                         todelete.append(key)
 
                 # Delete old keys
                 for oldkey in todelete:
-                    log.info(f'Deleting {section}.{oldkey}')
+                    log.info(f"Deleting {section}.{oldkey}")
                     self.config.remove_option(section, oldkey)
                     if self.config[section].get(oldkey_checksum):
-                        log.info(f'Deleting {section}.{oldkey_checksum}')
+                        log.info(f"Deleting {section}.{oldkey_checksum}")
                         self.config.remove_option(section, oldkey_checksum)
 
             except Exception:
                 traceback.print_exc()
-                print('Failed to migrate Gladier config. Please send us the error above!')
-                print('If you see this error again, you can try deleting ~/.gladier-secrets.cfg')
+                print(
+                    "Failed to migrate Gladier config. Please send us the error above!"
+                )
+                print(
+                    "If you see this error again, you can try deleting ~/.gladier-secrets.cfg"
+                )
 
 
 MIGRATIONS = [
     MigrateOldConfigFile,
     AddVersionToConfig,
     UpdateConfigVersion,
     UpdateFuncXFunctions,
@@ -158,15 +182,15 @@
     return any(m(config).is_applicable() for m in MIGRATIONS)
 
 
 def migrate_gladier(config):
     for migration in MIGRATIONS:
         m_instance = migration(config)
         if m_instance.is_applicable():
-            log.info(f'Applying migration: {m_instance.__class__.__name__}')
+            log.info(f"Applying migration: {m_instance.__class__.__name__}")
             m_instance.migrate()
     return config
 
 
 def panic_print(message):
     """Print a message to console for the user to see. The message must be URGENT."""
     print(message)
```

### Comparing `gladier-0.9.0b1/gladier/storage/tokens.py` & `gladier-0.9.0b2/gladier/storage/tokens.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from gladier.storage.config import GladierConfig
 
 
 log = logging.getLogger(__name__)
 
 
 class GladierSecretsConfig(GladierConfig):
-
     DEFAULT_PERMISSION = stat.S_IRUSR | stat.S_IWUSR
 
-    def __init__(self, *args, tokens_section='tokens', **kwargs):
+    def __init__(self, *args, tokens_section="tokens", **kwargs):
         self.tokens_section = tokens_section
         super().__init__(*args, **kwargs)
 
     def save(self):
         super().save()
         os.chmod(self.filename, self.DEFAULT_PERMISSION)
 
@@ -26,20 +25,20 @@
             self[self.tokens_section] = {}
             self.save()
 
     def write_tokens(self, tokens):
         self.load()
         for name, value in flat_pack(tokens).items():
             self.set(self.tokens_section, name, value)
-        log.debug(f'Wrote tokens to {self.filename}')
+        log.debug(f"Wrote tokens to {self.filename}")
         self.save()
 
     def read_tokens(self):
         self.load()
         return flat_unpack(dict(self.items(self.tokens_section)))
 
     def clear_tokens(self):
         self.load()
         self.remove_section(self.tokens_section)
         self.add_section(self.tokens_section)
-        log.debug(f'Tokens cleared from {self.filename}')
+        log.debug(f"Tokens cleared from {self.filename}")
         self.save()
```

### Comparing `gladier-0.9.0b1/gladier/utils/dynamic_imports.py` & `gladier-0.9.0b2/gladier/utils/dynamic_imports.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from importlib import import_module
 
 
 def parse_alias(dotted_string_path):
-    if ':' in dotted_string_path:
-        return dotted_string_path.rsplit(':', 1)
+    if ":" in dotted_string_path:
+        return dotted_string_path.rsplit(":", 1)
     return dotted_string_path, None
 
 
 def import_string(dotted_string_path):
     dotted_string_path, _ = parse_alias(dotted_string_path)
-    module_paths = dotted_string_path.rsplit('.', 1)
+    module_paths = dotted_string_path.rsplit(".", 1)
     if len(module_paths) != 2:
         raise ImportError(f'Path "{dotted_string_path} must be a dotted path')
     module_path, class_name = module_paths
     module = import_module(module_path)
 
     try:
         return getattr(module, class_name)
     except AttributeError as ae:
-        raise ImportError(f'Failed to import {class_name} from {module}.') from ae
+        raise ImportError(f"Failed to import {class_name} from {module}.") from ae
```

### Comparing `gladier-0.9.0b1/gladier/utils/flow_generation.py` & `gladier-0.9.0b2/gladier/utils/flow_generation.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 from gladier.base import GladierBaseTool
 from gladier.client import GladierBaseClient
 from gladier.exc import FlowGenException
 from gladier.utils.flow_modifiers import FlowModifiers
 from gladier.utils.name_generation import (
     get_compute_flow_state_name,
-    get_compute_function_name
+    get_compute_function_name,
 )
 from gladier.utils.tool_chain import ToolChain
 
 
 log = logging.getLogger(__name__)
 
 
@@ -29,59 +29,66 @@
 def _get_duplicate_functions(compute_functions: typing.List[callable]):
     tracked_set = set()
     func_names = [get_compute_flow_state_name(f) for f in compute_functions]
     return [f for f in func_names if f in tracked_set or tracked_set.add(f)]
 
 
 def _fix_old_tools(tool):
-    funcx_functions = getattr(tool, 'funcx_functions', None)
-    compute_functions = getattr(tool, 'compute_functions', None)
+    funcx_functions = getattr(tool, "funcx_functions", None)
+    compute_functions = getattr(tool, "compute_functions", None)
 
     if funcx_functions and not compute_functions:
-        log.warning(f'Tool {tool} defines attributue "funcx_functions" which has now been '
-                    'changed to "compute_functions". Automatically configuring compute_functions '
-                    f'for new tool. Please update the old tool {tool}')
-        setattr(tool, 'compute_functions', funcx_functions)
+        log.warning(
+            f'Tool {tool} defines attributue "funcx_functions" which has now been '
+            'changed to "compute_functions". Automatically configuring compute_functions '
+            f"for new tool. Please update the old tool {tool}"
+        )
+        setattr(tool, "compute_functions", funcx_functions)
 
 
 def generate_tool_flow(tool: GladierBaseTool, modifiers):
     """Generate a flow definition for a Gladier Tool based on the defined ``compute_functions``.
     Accepts modifiers for compute functions"""
     _fix_old_tools(tool)
 
     duplicate_functions = _get_duplicate_functions(tool.compute_functions)
     if duplicate_functions:
-        raise FlowGenException(f'Tool {tool} contains duplicate function names: '
-                               f'{duplicate_functions}')
+        raise FlowGenException(
+            f"Tool {tool} contains duplicate function names: " f"{duplicate_functions}"
+        )
 
     flow_moder = FlowModifiers([tool], modifiers, cls=tool)
 
     tools = ToolChain()
     for fx_func in tool.compute_functions:
         tools.chain_state(*generate_compute_flow_state(fx_func))
 
     flow = tools.flow_definition
-    if not flow['States']:
-        raise FlowGenException(f'Tool {tool} has no flow states. Add a list of python functions '
-                               f'as "{tool}.compute_functions = [myfunction]" or set a custom flow '
-                               f'definition instead using `{tool}.flow_definition = mydef`')
+    if not flow["States"]:
+        raise FlowGenException(
+            f"Tool {tool} has no flow states. Add a list of python functions "
+            f'as "{tool}.compute_functions = [myfunction]" or set a custom flow '
+            f"definition instead using `{tool}.flow_definition = mydef`"
+        )
     return flow_moder.apply_modifiers(flow)
 
 
 def generate_compute_flow_state(compute_function):
     state_name = get_compute_flow_state_name(compute_function)
 
     return state_name, {
-        'Comment': compute_function.__doc__,
-        'Type': 'Action',
-        'ActionUrl': 'https://compute.actions.globus.org',
-        'ExceptionOnActionFailure': False,
-        'Parameters': {
-            'tasks': [{
-                'endpoint.$': '$.input.compute_endpoint',
-                'function.$': f'$.input.{get_compute_function_name(compute_function)}',
-                'payload.$': '$.input',
-            }]
+        "Comment": compute_function.__doc__,
+        "Type": "Action",
+        "ActionUrl": "https://compute.actions.globus.org",
+        "ExceptionOnActionFailure": False,
+        "Parameters": {
+            "tasks": [
+                {
+                    "endpoint.$": "$.input.compute_endpoint",
+                    "function.$": f"$.input.{get_compute_function_name(compute_function)}",
+                    "payload.$": "$.input",
+                }
+            ]
         },
-        'ResultPath': f'$.{state_name}',
-        'WaitTime': 300,
+        "ResultPath": f"$.{state_name}",
+        "WaitTime": 300,
     }
```

### Comparing `gladier-0.9.0b1/gladier/utils/flow_modifiers.py` & `gladier-0.9.0b2/gladier/utils/flow_modifiers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 from gladier.exc import FlowModifierException
 from gladier.utils.name_generation import get_compute_flow_state_name
 
 log = logging.getLogger(__name__)
-compute_modifiers = {'endpoint', 'payload', 'tasks'}
+compute_modifiers = {"endpoint", "payload", "tasks"}
 # All top level states can be modified.
 # https://globus-automate-client.readthedocs.io/en/latest/authoring_flows.html#action-state-type
 state_modifiers = {
-    'Type',
-    'ActionUrl',
-    'WaitTime',
-    'ExceptionOnActionFailure',
-    'RunAs',
-    'InputPath',
-    'Parameters',
-    'ResultPath',
-    'Catch',
-    'ActionScope',
-    'Next',
-    'End',
+    "Type",
+    "ActionUrl",
+    "WaitTime",
+    "ExceptionOnActionFailure",
+    "RunAs",
+    "InputPath",
+    "Parameters",
+    "ResultPath",
+    "Catch",
+    "ActionScope",
+    "Next",
+    "End",
 }
 
 
 class FlowModifiers:
     supported_modifiers = state_modifiers.union(compute_modifiers)
     compute_modifiers = compute_modifiers
     state_modifiers = state_modifiers
@@ -43,87 +43,95 @@
             return function_identifier
 
     def get_flow_state_name(self, function_identifier):
         func = self.get_function(function_identifier)
         return get_compute_flow_state_name(func)
 
     def get_state_result_path(self, state_name):
-        return f'$.{state_name}.details.results'
+        return f"$.{state_name}.details.results"
 
     def check_modifiers(self):
-        log.debug(f'Checking modifiers: {self.modifiers}')
+        log.debug(f"Checking modifiers: {self.modifiers}")
         if not isinstance(self.modifiers, dict):
-            raise FlowModifierException(f'{self.cls}: Flow Modifiers must be a dict')
+            raise FlowModifierException(f"{self.cls}: Flow Modifiers must be a dict")
 
-        legacy_funcs = [func for tool in self.tools
-                        for func in getattr(tool, 'funcx_functions', [])]
+        legacy_funcs = [
+            func for tool in self.tools for func in getattr(tool, "funcx_functions", [])
+        ]
         legacy_func_names = [f.__name__ for f in legacy_funcs]
 
         # Check if modifiers were set correctly
         for name, mods in self.modifiers.items():
             if name in legacy_func_names:
                 raise FlowModifierException(
-                    f'Class {self.cls} is a Legacy Gladier tool pre-v0.9.0. Please use a modern '
-                    'version or follow the migration guide here to make it compatible: \n\n'
-                    '\thttps://gladier.readthedocs.io/en/latest/migration.html\n')
+                    f"Class {self.cls} is a Legacy Gladier tool pre-v0.9.0. Please use a modern "
+                    "version or follow the migration guide here to make it compatible: \n\n"
+                    "\thttps://gladier.readthedocs.io/en/latest/migration.html\n"
+                )
 
             if not self.get_function(name):
-                raise FlowModifierException(f'Class {self.cls} included modifier which does not '
-                                            f'exist: {name}. Allowed modifiers include '
-                                            f'{", ".join(self.function_names)}')
+                raise FlowModifierException(
+                    f"Class {self.cls} included modifier which does not "
+                    f"exist: {name}. Allowed modifiers include "
+                    f'{", ".join(self.function_names)}'
+                )
 
             for mod_name, mod_value in mods.items():
                 if mod_name not in self.supported_modifiers:
-                    raise FlowModifierException(f'Class {self.cls}: Unsupported modifier '
-                                                f'"{mod_name}". The only supported modifiers are: '
-                                                f'{self.supported_modifiers}')
+                    raise FlowModifierException(
+                        f"Class {self.cls}: Unsupported modifier "
+                        f'"{mod_name}". The only supported modifiers are: '
+                        f"{self.supported_modifiers}"
+                    )
 
     def apply_modifiers(self, flow):
         for name, mods in self.modifiers.items():
             state_name = self.get_flow_state_name(name)
-            flow['States'][state_name] = self.apply_modifier(flow['States'][state_name], mods)
+            flow["States"][state_name] = self.apply_modifier(
+                flow["States"][state_name], mods
+            )
         return flow
 
     def apply_modifier(self, flow_state, state_modifiers):
-
         for modifier_name, value in state_modifiers.items():
             log.debug(f'Applying modifier "{modifier_name}", value "{value}"')
             # If this is for a compute task
             if modifier_name in self.compute_modifiers:
-                if modifier_name == 'tasks':
-                    flow_state['Parameters'] = self.generic_set_modifier(
-                        flow_state['Parameters'], 'tasks', value)
+                if modifier_name == "tasks":
+                    flow_state["Parameters"] = self.generic_set_modifier(
+                        flow_state["Parameters"], "tasks", value
+                    )
                 else:
-                    flow_state['Parameters']['tasks'] = [
+                    flow_state["Parameters"]["tasks"] = [
                         self.generic_set_modifier(fx_task, modifier_name, value)
-                        for fx_task in flow_state['Parameters']['tasks']
+                        for fx_task in flow_state["Parameters"]["tasks"]
                     ]
             elif modifier_name in self.state_modifiers:
                 self.generic_set_modifier(flow_state, modifier_name, value)
         return flow_state
 
     def generic_set_modifier(self, item, mod_name, mod_value):
         if not isinstance(mod_value, str):
             if mod_value in self.functions:
                 sn = get_compute_flow_state_name(mod_value)
                 mod_value = self.get_state_result_path(sn)
-        elif isinstance(mod_value, str) and not mod_value.startswith('$.'):
+        elif isinstance(mod_value, str) and not mod_value.startswith("$."):
             if mod_value in self.function_names:
                 sn = self.state_names[self.function_names.index(mod_value)]
                 mod_value = self.get_state_result_path(sn)
             elif mod_value in self.state_names:
                 mod_value = self.get_state_result_path(mod_value)
             elif mod_name not in state_modifiers:
-                mod_value = f'$.input.{mod_value}'
+                mod_value = f"$.input.{mod_value}"
 
         # Remove duplicate keys
-        for duplicate_mod_key in (mod_name, f'{mod_name}.$'):
+        for duplicate_mod_key in (mod_name, f"{mod_name}.$"):
             if duplicate_mod_key in item.keys():
                 item.pop(duplicate_mod_key)
 
         # Note: Top level State types don't end with '.$', all others must end with
         # '.$' to indicate the value should be replaced. '.=' is not supported or possible yet
-        if isinstance(mod_value, str) and mod_value.startswith('$.'):
-            mod_name = f'{mod_name}.$'
+        if isinstance(mod_value, str) and mod_value.startswith("$."):
+            mod_name = f"{mod_name}.$"
         item[mod_name] = mod_value
-        log.debug(f'Set modifier {mod_name} to {mod_value}')
+        log.debug(f"Set modifier {mod_name} to {mod_value}")
         return item
```

### Comparing `gladier-0.9.0b1/gladier/utils/flow_traversal.py` & `gladier-0.9.0b2/gladier/utils/flow_traversal.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,37 +25,43 @@
     visited = previously_visited.copy() if previously_visited else list()
 
     if state is None or state in visited:
         return
     visited.append(state)
 
     if state not in flow_states:
-        raise FlowGenException(f'State {state} not in definition!')
+        raise FlowGenException(f"State {state} not in definition!")
 
     yield state, flow_states[state]
 
     transition_state = get_transition(flow_states[state])
     if transition_state:
         _, state_name = transition_state
         yield from iter_flow_states(flow_states, state_name, previously_visited=visited)
 
     state_info = flow_states[state]
-    if state_info['Type'] == 'Choice':
-        for choice in state_info.get('Choices', []):
-            if choice.get('Next'):
-                yield from iter_flow_states(flow_states, choice['Next'], previously_visited=visited)
+    if state_info["Type"] == "Choice":
+        for choice in state_info.get("Choices", []):
+            if choice.get("Next"):
+                yield from iter_flow_states(
+                    flow_states, choice["Next"], previously_visited=visited
+                )
     return
 
 
-def iter_flow(flow_definition: Mapping[str, Any]) -> Iterator[Tuple[str, Mapping[str, Any]]]:
+def iter_flow(
+    flow_definition: Mapping[str, Any]
+) -> Iterator[Tuple[str, Mapping[str, Any]]]:
     """
     Yields a tuple containing the state name and state info for each state in a flow definition.
 
     """
-    yield from iter_flow_states(flow_definition['States'], flow_definition['StartAt'])
+    yield from iter_flow_states(flow_definition["States"], flow_definition["StartAt"])
 
 
 def get_end_states(flow_definition: Mapping[str, Any]) -> Iterator[str]:
     """Get all states for a flow that will cause the flow to exit normally. This includes any
     state which contains "End": True. A termination state is assumed if there is no next
     state to transition."""
-    yield from {name for name, state in iter_flow(flow_definition) if not get_transition(state)}
+    yield from {
+        name for name, state in iter_flow(flow_definition) if not get_transition(state)
+    }
```

### Comparing `gladier-0.9.0b1/gladier/utils/name_generation.py` & `gladier-0.9.0b2/gladier/utils/name_generation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 
 
 def get_upper_camel_case(snake_case_name):
     """Make a snake_case_name into UpperCamelCase"""
-    return ''.join([nb.capitalize() for nb in snake_case_name.split('_')])
+    return "".join([nb.capitalize() for nb in snake_case_name.split("_")])
 
 
 def get_snake_case(upper_camel_case):
     # https://stackoverflow.com/questions/1175208/elegant-python-function-to-convert-camelcase-to-snake-case
-    snake_name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', upper_camel_case)
-    snake_name = re.sub('([a-z0-9])([A-Z])', r'\1_\2', snake_name).lower()
+    snake_name = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", upper_camel_case)
+    snake_name = re.sub("([a-z0-9])([A-Z])", r"\1_\2", snake_name).lower()
     return snake_name
 
 
 def get_compute_flow_state_name(compute_function):
     """State names in Automate are typically upper camel case. This function generates
     an upper case compute function name for flow states."""
     return get_upper_camel_case(compute_function.__name__)
@@ -23,19 +23,19 @@
     """
     Generate a function name given a compute function. These function names are used to refer
     to compute functions within the config. There is no guarantee of uniqueness for function
     names.
 
     :return: human readable string identifier for a function (intended for a gladier.cfg file)
     """
-    return f'{compute_function.__name__}_function_id'
+    return f"{compute_function.__name__}_function_id"
 
 
 def get_compute_function_checksum_name(compute_function):
     """
     Generate a name to refer to the checksum for a given compute function. Based off of the
     name generated for the function self.get_compute_function_name. Human readable, intended
     for config.
 
     :return:  human readable string identifier for a function checksum (for a gladier.cfg file)
     """
-    return f'{get_compute_function_name(compute_function)}_checksum'
+    return f"{get_compute_function_name(compute_function)}_checksum"
```

### Comparing `gladier-0.9.0b1/gladier/utils/tool_alias.py` & `gladier-0.9.0b2/gladier/utils/tool_alias.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,60 +3,60 @@
 import logging
 import gladier.utils.name_generation
 
 log = logging.getLogger(__name__)
 
 
 class ToolAlias(abc.ABC):
-
-    input_location = 'input'
+    input_location = "input"
 
     def __init__(self, alias):
         self.alias = alias
 
     @abc.abstractmethod
     def rename_state(self, state_name, tool):
         return state_name
 
     @abc.abstractmethod
     def rename_variable(self, variable_name, tool):
         return variable_name
 
     def get_input_variable(self, flow_input_variable, tool_inputs):
-        location = f'$.{self.input_location}.'
-        input_name = flow_input_variable.replace(location, '')
+        location = f"$.{self.input_location}."
+        input_name = flow_input_variable.replace(location, "")
         if input_name in tool_inputs:
             return input_name
 
     def rename_input_variables(self, state_data, tool_inputs, tool):
         sdata = copy.deepcopy(state_data)
         if not sdata:
             return
         for k in sdata.keys():
             if isinstance(sdata[k], str):
                 input_var = self.get_input_variable(sdata[k], tool_inputs)
                 if input_var:
-                    new_var = f'$.{self.input_location}.{self.rename_variable(input_var, tool)}'
+                    new_var = f"$.{self.input_location}.{self.rename_variable(input_var, tool)}"
                     sdata[k] = new_var
             elif isinstance(sdata[k], dict):
                 sdata[k] = self.rename_input_variables(sdata[k], tool_inputs, tool)
             elif isinstance(sdata[k], list):
-                sdata[k] = [self.rename_input_variables(subsdata, tool_inputs, tool)
-                            for subsdata in sdata[k]]
+                sdata[k] = [
+                    self.rename_input_variables(subsdata, tool_inputs, tool)
+                    for subsdata in sdata[k]
+                ]
         return sdata
 
 
 class NoAlias(ToolAlias):
     def rename_state(self, state_name, tool):
         return state_name
 
     def rename_variable(self, variable_name, tool):
         return variable_name
 
 
 class StateSuffixVariablePrefix(ToolAlias):
-
     def rename_state(self, state_name, tool):
-        return f'{state_name}{self.alias}'
+        return f"{state_name}{self.alias}"
 
     def rename_variable(self, variable_name, tool):
-        return f'{gladier.utils.name_generation.get_snake_case(self.alias)}_{variable_name}'
+        return f"{gladier.utils.name_generation.get_snake_case(self.alias)}_{variable_name}"
```

### Comparing `gladier-0.9.0b1/gladier/utils/tool_chain.py` & `gladier-0.9.0b2/gladier/utils/tool_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,110 +6,117 @@
 from gladier.exc import FlowGenException, StateNameConflict
 from gladier.utils.flow_traversal import get_end_states
 
 log = logging.getLogger(__name__)
 
 
 class ToolChain:
-
     def __init__(self, flow_comment=None):
         self._flow_definition = {
-            'States': dict(),
-            'Comment': flow_comment,
-            'StartAt': None,
+            "States": dict(),
+            "Comment": flow_comment,
+            "StartAt": None,
         }
         self.transition_states = list()
 
     @property
     def flow_definition(self):
         flow_def = copy.deepcopy(self._flow_definition)
-        if not self._flow_definition.get('Comment'):
+        if not self._flow_definition.get("Comment"):
             state_names = ", ".join(flow_def["States"].keys())
-            flow_def['Comment'] = f'Flow with states: {state_names}'
+            flow_def["Comment"] = f"Flow with states: {state_names}"
             return flow_def
         return flow_def
 
     def chain(self, tools: List[GladierBaseTool]):
         """
         Given a list of tools, chain each one to the existing flow definition
         stored on this class. If there is no current flow definition, the first
         flow in the first tool will be used as the starting point.
         :raises FlowGenException: if there was a problem chaining together flows
         :returns self: a reference to this class.
         """
         self.check_tools(tools)
         for tool in tools:
-            log.debug(f'Chaining tool {tool.__class__.__name__} to existing flow '
-                      f'({len(self._flow_definition["States"])} states)')
+            log.debug(
+                f"Chaining tool {tool.__class__.__name__} to existing flow "
+                f'({len(self._flow_definition["States"])} states)'
+            )
 
             flow_definition = tool.get_flow_definition()
             self._chain_flow(flow_definition, tool)
 
         return self
 
     def chain_state(self, name: str, definition: Mapping[str, Any]):
         """Chain a single flow state to the existing flow definition. If there
         is no existing flow definition, a new flow definition will be created."""
-        log.debug(f'Chaining state {name} with definition {definition.keys()}')
+        log.debug(f"Chaining state {name} with definition {definition.keys()}")
         temp_flow = {
-            'StartAt': name,
-            'States': {name: definition},
+            "StartAt": name,
+            "States": {name: definition},
         }
-        temp_flow['States'][name]['End'] = True
+        temp_flow["States"][name]["End"] = True
         self._chain_flow(temp_flow)
         return self
 
     def _chain_flow(self, new_flow: Mapping[str, dict], tool: GladierBaseTool = None):
         # Base case, if this is the first 'chain' and no states exist yet.
-        if not self._flow_definition['States']:
-            self._flow_definition['States'] = copy.deepcopy(new_flow['States'])
-            self._flow_definition['StartAt'] = new_flow['StartAt']
+        if not self._flow_definition["States"]:
+            self._flow_definition["States"] = copy.deepcopy(new_flow["States"])
+            self._flow_definition["StartAt"] = new_flow["StartAt"]
         else:
-            self._flow_definition['States'].update(copy.deepcopy(new_flow['States']))
+            self._flow_definition["States"].update(copy.deepcopy(new_flow["States"]))
             for t_state in self.transition_states:
-                self.add_transition(t_state, new_flow['StartAt'])
+                self.add_transition(t_state, new_flow["StartAt"])
 
         self._set_new_transition_states(new_flow, tool)
 
-    def _set_new_transition_states(self, new_flow: Mapping[str, dict],
-                                   tool: GladierBaseTool = None):
+    def _set_new_transition_states(
+        self, new_flow: Mapping[str, dict], tool: GladierBaseTool = None
+    ):
         # Use the tool-defined states if they are defined, otherwise there is only one
         # End state on the flow and therefore can be assumed.
         t_states = list(get_end_states(new_flow))
         if tool:
             tool_t_states = tool.get_flow_transition_states()
         else:
             tool_t_states = []
         entity = tool or f'Flow with states: {tuple(new_flow["States"].keys())}'
         if len(t_states) > 1 and not tool_t_states:
-            raise FlowGenException(f'{entity} has multiple branching end states and must '
-                                   'define which states a flow may continue by setting '
-                                   '"flow_transition_states" containing one or more of '
-                                   f'{", ".join(t_states)} ')
+            raise FlowGenException(
+                f"{entity} has multiple branching end states and must "
+                "define which states a flow may continue by setting "
+                '"flow_transition_states" containing one or more of '
+                f'{", ".join(t_states)} '
+            )
         elif not t_states:
-            raise FlowGenException(f'{tool}: Could not find any end states in flow.')
+            raise FlowGenException(f"{tool}: Could not find any end states in flow.")
 
         self.transition_states = tool_t_states if tool_t_states else t_states
 
     def add_transition(self, cur_flow_term: str, new_chain_start: str):
-        if self._flow_definition['States'][cur_flow_term].get('End'):
-            self._flow_definition['States'][cur_flow_term].pop('End')
-        log.debug(f'Chaining {cur_flow_term} --> {new_chain_start}')
-        self._flow_definition['States'][cur_flow_term]['Next'] = new_chain_start
+        if self._flow_definition["States"][cur_flow_term].get("End"):
+            self._flow_definition["States"][cur_flow_term].pop("End")
+        log.debug(f"Chaining {cur_flow_term} --> {new_chain_start}")
+        self._flow_definition["States"][cur_flow_term]["Next"] = new_chain_start
 
     def check_tools(self, tools: List[GladierBaseTool]):
-
         states = set()
         for tool in tools:
             flow_def = tool.get_flow_definition()
             if flow_def is None:
-                raise FlowGenException(f'Tool {tool} did not set .flow_definition attribute or set '
-                                       '@generate_flow_definition (comptue functions only).'
-                                       'Please set a flow definition for'
-                                       f'{tool.__class__.__name__}.')
+                raise FlowGenException(
+                    f"Tool {tool} did not set .flow_definition attribute or set "
+                    "@generate_flow_definition (comptue functions only)."
+                    "Please set a flow definition for"
+                    f"{tool.__class__.__name__}."
+                )
 
-            new_states = set(flow_def.get('States'))
+            new_states = set(flow_def.get("States"))
             conflicts = states & new_states
             if conflicts:
-                raise StateNameConflict(f'States in tool {tool} '
-                                        f'has been defined more than once: {conflicts}')
+                raise StateNameConflict(
+                    f"States in tool {tool} "
+                    f"has been defined more than once: {conflicts}"
+                )
             states = states | new_states
```

### Comparing `gladier-0.9.0b1/gladier.egg-info/PKG-INFO` & `gladier-0.9.0b2/gladier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -39,18 +39,18 @@
 .. image:: https://img.shields.io/pypi/wheel/gladier.svg
     :target: https://pypi.python.org/pypi/gladier
 
 .. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
     :alt: License
     :target: https://opensource.org/licenses/Apache-2.0
 
-Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage 
+Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage
 systems and manage using Globus Flows.
 
-Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field, 
+Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field,
 Gladier can help you streamline your data management and analysis workflows, so you can focus on your scientific discoveries.
 Try Gladier today and see how it can enhance your research capabilities!
 
 You can install Gladier and Gladier Tools with the following:
 
 
 .. code-block:: bash
```

### Comparing `gladier-0.9.0b1/gladier.egg-info/SOURCES.txt` & `gladier-0.9.0b2/gladier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b1/setup.py` & `gladier-0.9.0b2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import os
 from setuptools import find_packages, setup
 
 # Single source of truth for version
 version_ns = {}
 with open(os.path.join("gladier", "version.py")) as f:
     exec(f.read(), version_ns)
-version = version_ns['__version__']
+version = version_ns["__version__"]
 
-with open('README.rst') as f:
+with open("README.rst") as f:
     long_description = f.read()
 
 install_requires = []
-with open('requirements.txt') as reqs:
+with open("requirements.txt") as reqs:
     for line in reqs.readlines():
         req = line.strip()
-        if not req or req.startswith('#'):
+        if not req or req.startswith("#"):
             continue
         install_requires.append(req)
 
 setup(
     name="gladier",
     description="Tooling for rapid deployment of automation tooling.",
     long_description=long_description,
-    long_description_content_type='text/x-rst',
-    url='https://github.com/globus-gladier/gladier',
+    long_description_content_type="text/x-rst",
+    url="https://github.com/globus-gladier/gladier",
     version=version,
     packages=find_packages(),
     install_requires=install_requires,
     python_requires=">=3.6",
-    license='Apache 2.0',
-    maintainer='',
-    maintainer_email='',
+    license="Apache 2.0",
+    maintainer="",
+    maintainer_email="",
     classifiers=[
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: POSIX',
-        'Operating System :: MacOS :: MacOS X',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ]
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: POSIX",
+        "Operating System :: MacOS :: MacOS X",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
 )
```

