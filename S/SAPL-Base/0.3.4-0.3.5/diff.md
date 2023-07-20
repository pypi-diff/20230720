# Comparing `tmp/SAPL-Base-0.3.4.tar.gz` & `tmp/SAPL-Base-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPL-Base-0.3.4.tar", last modified: Thu Feb  2 16:17:28 2023, max compression
+gzip compressed data, was "SAPL-Base-0.3.5.tar", last modified: Thu Jul 20 21:53:32 2023, max compression
```

## Comparing `SAPL-Base-0.3.4.tar` & `SAPL-Base-0.3.5.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:28.782637 SAPL-Base-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-02-02 16:17:28.782637 SAPL-Base-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 16:17:28.782637 SAPL-Base-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:28.778637 SAPL-Base-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:28.778637 SAPL-Base-0.3.4/src/SAPL_Base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-02-02 16:17:28.000000 SAPL-Base-0.3.4/src/SAPL_Base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-02 16:17:28.000000 SAPL-Base-0.3.4/src/SAPL_Base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 16:17:28.000000 SAPL-Base-0.3.4/src/SAPL_Base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-02 16:17:28.000000 SAPL-Base-0.3.4/src/SAPL_Base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-02 16:17:28.000000 SAPL-Base-0.3.4/src/SAPL_Base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:28.778637 SAPL-Base-0.3.4/src/sapl_base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/authorization_subscription_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/authorization_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/base_authorization_subscription_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:28.778637 SAPL-Base-0.3.4/src/sapl_base/constraint_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/constraint_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/constraint_handling/constraint_handler_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/constraint_handling/constraint_handler_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/constraint_handling/constraint_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/decision.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17762 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/policy_decision_points.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 16:17:28.782637 SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/async_policy_enforcement_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/base_streaming_pep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/policy_enforcement_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/streaming_policy_enforcement_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/sync_policy_enforcement_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-02 16:17:17.000000 SAPL-Base-0.3.4/src/sapl_base/sapl_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:32.539214 SAPL-Base-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-20 21:53:32.539214 SAPL-Base-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:53:32.539214 SAPL-Base-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:32.531213 SAPL-Base-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:32.535214 SAPL-Base-0.3.5/src/SAPL_Base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-20 21:53:32.000000 SAPL-Base-0.3.5/src/SAPL_Base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-20 21:53:32.000000 SAPL-Base-0.3.5/src/SAPL_Base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:53:32.000000 SAPL-Base-0.3.5/src/SAPL_Base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 21:53:32.000000 SAPL-Base-0.3.5/src/SAPL_Base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 21:53:32.000000 SAPL-Base-0.3.5/src/SAPL_Base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:32.535214 SAPL-Base-0.3.5/src/sapl_base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/authorization_subscription_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/authorization_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/base_authorization_subscription_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:32.535214 SAPL-Base-0.3.5/src/sapl_base/constraint_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/constraint_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/constraint_handling/constraint_handler_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/constraint_handling/constraint_handler_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/constraint_handling/constraint_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/policy_decision_points.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:32.539214 SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/async_generator_policy_enforcement_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/async_policy_enforcement_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/policy_enforcement_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/streaming_policy_enforcement_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/sync_policy_enforcement_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/src/sapl_base/sapl_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:32.539214 SAPL-Base-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-20 21:53:18.000000 SAPL-Base-0.3.5/tests/test_policy_decision_points.py
```

### Comparing `SAPL-Base-0.3.4/LICENSE` & `SAPL-Base-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPL-Base-0.3.4/PKG-INFO` & `SAPL-Base-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPL-Base
-Version: 0.3.4
+Version: 0.3.5
 Summary: Base library to create SAPL Integrations for Python Frameworks
 Author-email: Dominic Heutelbeck <dominic@heutelbeck.com>
 License: Copyright 2017-2022 Dominic Heutelbeck
         
         Licensed under the Apache License, Version 2.0 (the "License"); you may not
         use this file except in compliance with the License. You may obtain a copy
         of the License at
```

### Comparing `SAPL-Base-0.3.4/pyproject.toml` & `SAPL-Base-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "SAPL-Base"
-version = "0.3.4"
+version = "0.3.5"
 description = "Base library to create SAPL Integrations for Python Frameworks"
 readme = "README.md"
 authors = [{ name = "Dominic Heutelbeck", email = "dominic@heutelbeck.com" }]
 license = { file = "LICENSE" }
 
 dependencies = [
     "backoff",
```

### Comparing `SAPL-Base-0.3.4/src/SAPL_Base.egg-info/PKG-INFO` & `SAPL-Base-0.3.5/src/SAPL_Base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPL-Base
-Version: 0.3.4
+Version: 0.3.5
 Summary: Base library to create SAPL Integrations for Python Frameworks
 Author-email: Dominic Heutelbeck <dominic@heutelbeck.com>
 License: Copyright 2017-2022 Dominic Heutelbeck
         
         Licensed under the Apache License, Version 2.0 (the "License"); you may not
         use this file except in compliance with the License. You may obtain a copy
         of the License at
```

### Comparing `SAPL-Base-0.3.4/src/SAPL_Base.egg-info/SOURCES.txt` & `SAPL-Base-0.3.5/src/SAPL_Base.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 src/sapl_base/policy_decision_points.py
 src/sapl_base/sapl_util.py
 src/sapl_base/constraint_handling/__init__.py
 src/sapl_base/constraint_handling/constraint_handler_bundle.py
 src/sapl_base/constraint_handling/constraint_handler_provider.py
 src/sapl_base/constraint_handling/constraint_handler_service.py
 src/sapl_base/policy_enforcement_points/__init__.py
+src/sapl_base/policy_enforcement_points/async_generator_policy_enforcement_point.py
 src/sapl_base/policy_enforcement_points/async_policy_enforcement_point.py
-src/sapl_base/policy_enforcement_points/base_streaming_pep.py
 src/sapl_base/policy_enforcement_points/policy_enforcement_point.py
 src/sapl_base/policy_enforcement_points/streaming_policy_enforcement_point.py
-src/sapl_base/policy_enforcement_points/sync_policy_enforcement_point.py
+src/sapl_base/policy_enforcement_points/sync_policy_enforcement_point.py
+tests/test_policy_decision_points.py
```

### Comparing `SAPL-Base-0.3.4/src/sapl_base/authorization_subscription_factory.py` & `SAPL-Base-0.3.5/src/sapl_base/authorization_subscription_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 import contextvars
+
 from abc import abstractmethod, ABC
-from typing import Dict
+from typing import Dict,Callable
 
 from .authorization_subscriptions import AuthorizationSubscription, MultiSubscription
 
 client_request = contextvars.ContextVar('request')
-authorization_subscription = contextvars.ContextVar('authorization_subscription')
 
 class AuthorizationSubscriptionFactory(ABC):
+    subject_function: Callable[[Dict],Dict]
+    action_function: Callable[[Dict],Dict]
+    resource_function: Callable[[Dict],Dict]
+
+    def __init__(self):
+        self.subject_function = self._default_subject_function
+        self.action_function = self._default_action_function
+        self.resource_function = self._default_resource_function
+
+    def register_default_subject_function(self,subject_function: Callable[[Dict],Dict]):
+        self.subject_function = subject_function
+
+    def register_default_action_function(self,action_function: Callable[[Dict],Dict]):
+        self.action_function = action_function
+
+    def register_default_resource_function(self,resource_function: Callable[[Dict],Dict]):
+        self.resource_function = resource_function
     """
     Baseclass of an AuthorizationSubscriptionFactory, which can be inherited to create a framework specific
     AuthorizationSubscriptionFactory.
     """
-
     def _create_subscription(self, values: Dict, subject=None, action=None, resource=None,
                              environment=None) -> AuthorizationSubscription:
         """
         Create an AuthorizationSubscription for the decorated function, with the arguments provided to the decorator
 
        :param values: Dictionary which contains data related to the decorated function
        :param subject: subject with which the function was decorated. None if not specified
@@ -25,27 +41,27 @@
        :param environment: environment with which the function was decorated. None if not specified
        :return: An authorization_subscription which can be sent to a pdp to get an authorization_decision
         """
 
         if subject is not None:
             _subject = self._argument_is_callable(subject, values)
         else:
-            _subject = self._default_subject_function(values)
+            _subject = self.subject_function(values)
         if not _subject:
             _subject = "anonymous"
 
         if action is not None:
             _action = self._argument_is_callable(action, values)
         else:
-            _action = self._default_action_function(values)
+            _action = self.action_function(values)
 
         if resource is not None:
             _resource = self._argument_is_callable(resource, values)
         else:
-            _resource = self._default_resource_function(values)
+            _resource = self.resource_function(values)
 
         if environment is not None:
             _environment = self._argument_is_callable(environment, values)
         else:
             _environment = {}
 
         return AuthorizationSubscription(self._remove_empty_dicts(_subject), self._remove_empty_dicts(_action),
@@ -97,15 +113,15 @@
         :param values: dictionary containing all values from which a resource can be created.
         :return: A dictionary which will be provided as resource, when an AuthorizationSubscription is created
         """
         pass
 
     @abstractmethod
     def create_authorization_subscription(self, values: Dict, subject, action, resource,
-                                          environment, scope, enforcement_type):
+                                          environment, scope, enforcement_type)-> AuthorizationSubscription:
         """
         Create an AuthorizationSubscription with the given dictionary and arguments
 
         The returned AuthorizationSubscription is dependent of the framework and the decorated function
 
         :param enforcement_type: the type of enforcement, with which the function is decorated
         :param scope: Argument which creates a AuthorizationSubscription according to the given scope instead of evaluating the scope based on other parameter
@@ -212,8 +228,8 @@
             raise Exception("already built")
         self._built = True
         return MultiSubscription(self._remove_empty_list(self.subject), self._remove_empty_list(self.action),
                                  self._remove_empty_list(self.resource), self._remove_empty_list(self.environment),
                                  self._remove_empty_list(self.authorization_subscription))
 
 
-auth_factory = None
+auth_factory : AuthorizationSubscriptionFactory
```

### Comparing `SAPL-Base-0.3.4/src/sapl_base/authorization_subscriptions.py` & `SAPL-Base-0.3.5/src/sapl_base/authorization_subscriptions.py`

 * *Files identical despite different names*

### Comparing `SAPL-Base-0.3.4/src/sapl_base/base_authorization_subscription_factory.py` & `SAPL-Base-0.3.5/src/sapl_base/base_authorization_subscription_factory.py`

 * *Files identical despite different names*

### Comparing `SAPL-Base-0.3.4/src/sapl_base/constraint_handling/constraint_handler_bundle.py` & `SAPL-Base-0.3.5/src/sapl_base/constraint_handling/constraint_handler_bundle.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,22 @@
     Exception is thrown.
     """
     _on_decision_handler: List[Callable[[Decision], None]]
     _error_handler: List[Callable[[Exception], Exception]]
     _result_handler: List[Callable[[Any], Any]]
     _function_arguments_mapper: List[Callable[[Dict], Dict]]
 
+    @classmethod
+    def empty_bundle(cls):
+        """
+        Create an empty ConstraintHandlerBundle
+        :return: ConstraintHandlerBundle with empty lists of ConstraintHandlerProvider
+        """
+        return ConstraintHandlerBundle(list(),list(),list())
+
     def __init__(self,
                  on_decision_handler: List[OnDecisionConstraintHandlerProvider],
                  error_handler: List[ErrorConstraintHandlerProvider],
                  result_handler: List[ResultConstraintHandlerProvider],
                  function_arguments_mapper: List[FunctionArgumentsConstraintHandlerProvider] = None):
         """
         :param on_decision_handler: sorted List of OnDecisionConstraintHandlerProvider, of which their handle()
```

### Comparing `SAPL-Base-0.3.4/src/sapl_base/constraint_handling/constraint_handler_provider.py` & `SAPL-Base-0.3.5/src/sapl_base/constraint_handling/constraint_handler_provider.py`

 * *Files identical despite different names*

### Comparing `SAPL-Base-0.3.4/src/sapl_base/constraint_handling/constraint_handler_service.py` & `SAPL-Base-0.3.5/src/sapl_base/constraint_handling/constraint_handler_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def __init__(self):
         self.on_decision_handler : List[OnDecisionConstraintHandlerProvider]= []
         self.error_handler : List[ErrorConstraintHandlerProvider]= []
         self.result_handler : List[ResultConstraintHandlerProvider]= []
         self.function_arguments_mapper : List[FunctionArgumentsConstraintHandlerProvider]= []
 
-    def register_decision_constraint_handler_provider(self, providers: Union[List[OnDecisionConstraintHandlerProvider], OnDecisionConstraintHandlerProvider]) -> None:
+    def register_on_decision_constraint_handler_provider(self, providers: Union[List[OnDecisionConstraintHandlerProvider], OnDecisionConstraintHandlerProvider]) -> None:
         try:
             for provider in providers:
                 self.on_decision_handler.append(provider)
         except TypeError:
             self.on_decision_handler.append(providers)
 
     def register_error_constraint_handler_provider(self, providers: Union[List[ErrorConstraintHandlerProvider] ,ErrorConstraintHandlerProvider]) -> None:
```

### Comparing `SAPL-Base-0.3.4/src/sapl_base/decision.py` & `SAPL-Base-0.3.5/src/sapl_base/decision.py`

 * *Files identical despite different names*

### Comparing `SAPL-Base-0.3.4/src/sapl_base/decorators.py` & `SAPL-Base-0.3.5/src/sapl_base/decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import asyncio
+import inspect
 from functools import wraps
+from typing import Callable
 
-from sapl_base.policy_enforcement_points.streaming_policy_enforcement_point import StreamingPolicyEnforcementPoint
+from sapl_base.policy_enforcement_points.async_generator_policy_enforcement_point import \
+    AsyncGeneratorPolicyEnforcementPoint
+import sapl_base.policy_enforcement_points.policy_enforcement_point as pep
 from sapl_base.policy_enforcement_points.async_policy_enforcement_point import AsyncPolicyEnforcementPoint
 from sapl_base.policy_enforcement_points.sync_policy_enforcement_point import SyncPolicyEnforcementPoint
 from sapl_base.sapl_util import double_wrap
 
 
 @double_wrap
 def pre_enforce(fn, subject: str = None, action: str = None, resource = None,
@@ -137,27 +141,38 @@
     :param subject: subject of an authorization_subscription or a function to create the subject
     :param action: action of an authorization_subscription or a function to create the action
     :param resource: resource of an authorization_subscription or a function to create the resource
     :param environment: environment of an authorization_subscription or a function to create the environment
     :param scope: Argument which creates a AuthorizationSubscription according to the given scope instead of evaluating the scope based on other parameter
     :return: The return_value of the decorated function with a generator which will enforce each value, which is sent with the stream
     """
-    if asyncio.iscoroutinefunction(fn):
+    if inspect.isclass(fn):
+        "Replace the original init method of the decorated class with an init method which inits the class and creates " \
+        "a Streaming PEP which enforces the decorated class with till_denied behaviour"
+        fn.original_init = fn.__init__
+
+        def new_init(self,*args,**kwargs):
+            fn.original_init(self,*args,**kwargs)
+            self.streaming_pep = pep.streaming_pep(fn,*args, instance=self,type_of_enforcement="enforce_till_denied",**kwargs)
+            self.streaming_pep.enforce_till_denied(subject, action, resource, environment, scope)
+
+        fn.__init__= new_init
+        return fn
+
+    if inspect.isasyncgenfunction(fn):
+
         @wraps(fn)
         async def async_wrap(*args, **kwargs):
-            enforcement_point = StreamingPolicyEnforcementPoint(fn, *args, **kwargs)
-            return await enforcement_point.enforce_till_denied(subject, action, resource, environment, scope)
+            enforcement_point = AsyncGeneratorPolicyEnforcementPoint(fn, *args,type_of_enforcement="enforce_till_denied", **kwargs)
+            async for value in enforcement_point.enforce_till_denied(subject,action,resource,environment,scope):
+                yield value
 
         return async_wrap
-    else:
-        @wraps(fn)
-        def wrap(*args, **kwargs):
-            raise Exception
 
-        return wrap
+    raise Exception
 
 
 @double_wrap
 def enforce_drop_while_denied(fn, subject: str = None, action: str = None, resource: str = None,
                               environment: str = None, scope: str = "automatic"):
     """
     Enforces a stream and drops values, when the current decision is not PERMIT
@@ -172,32 +187,46 @@
     :param subject: subject of an authorization_subscription or a function to create the subject
     :param action: action of an authorization_subscription or a function to create the action
     :param resource: resource of an authorization_subscription or a function to create the resource
     :param environment: environment of an authorization_subscription or a function to create the environment
     :param scope: Argument which creates a AuthorizationSubscription according to the given scope instead of evaluating the scope based on other parameter
     :return: The return_value of the decorated function with a generator which will enforce each value, which is sent with the stream
     """
-    if asyncio.iscoroutinefunction(fn):
+
+
+    if inspect.isclass(fn):
+        "Replace the original init method of the decorated class with an init method which inits the class and creates " \
+        "a Streaming PEP which enforces the decorated class with drop_while_denied behaviour"
+        fn.original_init = fn.__init__
+
+        def new_init(self,*args,**kwargs):
+            fn.original_init(self,*args,**kwargs)
+            self.streaming_pep = pep.streaming_pep(fn,*args, instance=self,type_of_enforcement="enforce_drop_while_denied",**kwargs)
+            self.streaming_pep.drop_while_denied(subject, action, resource, environment, scope)
+
+        fn.__init__= new_init
+        return fn
+
+
+    if inspect.isasyncgenfunction(fn):
+
         @wraps(fn)
         async def async_wrap(*args, **kwargs):
-            enforcement_point = StreamingPolicyEnforcementPoint(fn, *args, **kwargs)
-            return await enforcement_point.drop_while_denied(subject, action, resource, environment, scope)
+            enforcement_point = AsyncGeneratorPolicyEnforcementPoint(fn, *args,type_of_enforcement="enforce_drop_while_denied", **kwargs)
+            async for value in enforcement_point.drop_while_denied(subject,action,resource,environment,scope):
+                yield value
 
         return async_wrap
-    else:
-        @wraps(fn)
-        def wrap(*args, **kwargs):
-            raise Exception
 
-        return wrap
+    raise Exception
 
 
 @double_wrap
 def enforce_recoverable_if_denied(fn, subject: str = None, action: str = None, resource: str = None,
-                                  environment: str = None, scope: str = "automatic"):
+                                  environment: str = None, scope: str = "automatic", handle_recoverable_deny_function : Callable[[], None] = None):
     """
     Enforces a stream and drops values, when the current decision is not PERMIT and notify the client, that
     values are dropped, because they are not PERMITTED to receive them.
 
     SAPL Decorators must be used as first Decorator to gather needed information of the annotated Function.
 
     If the function doesn't return a stream, an exception will be thrown
@@ -209,20 +238,33 @@
     :param subject: subject of an authorization_subscription or a function to create the subject
     :param action: action of an authorization_subscription or a function to create the action
     :param resource: resource of an authorization_subscription or a function to create the resource
     :param environment: environment of an authorization_subscription or a function to create the environment
     :param scope: Argument which creates a AuthorizationSubscription according to the given scope instead of evaluating the scope based on other parameter
     :return: The return_value of the decorated function with a generator which will enforce each value, which is sent with the stream
     """
-    if asyncio.iscoroutinefunction(fn):
+    if inspect.isclass(fn):
+        "Replace the original init method of the decorated class with an init method which inits the class and creates " \
+        "a Streaming PEP which enforces the decorated class with recoverable_if_denied behaviour"
+        fn.original_init = fn.__init__
+
+        def new_init(self,*args,**kwargs):
+            fn.original_init(self,*args,**kwargs)
+            self.streaming_pep = pep.streaming_pep(fn,*args, instance=self,type_of_enforcement="enforce_recoverable_if_denied",**kwargs)
+            self.streaming_pep.recoverable_if_denied(subject, action, resource, environment, scope, handle_recoverable_deny_function)
+
+        fn.__init__= new_init
+        return fn
+
+    if inspect.isasyncgenfunction(fn):
+
         @wraps(fn)
         async def async_wrap(*args, **kwargs):
-            enforcement_point = StreamingPolicyEnforcementPoint(fn, *args, **kwargs)
-            return await enforcement_point.recoverable_if_denied(subject, action, resource, environment, scope)
+            enforcement_point = AsyncGeneratorPolicyEnforcementPoint(fn, *args, type_of_enforcement="enforce_recoverable_if_denied",**kwargs)
+            async for value in enforcement_point.recoverable_if_denied(subject,action,resource,environment,scope, handle_recoverable_deny_function):
+                yield value
 
         return async_wrap
-    else:
-        @wraps(fn)
-        def wrap(*args, **kwargs):
-            raise Exception
 
-        return wrap
+    raise Exception
+
+
```

### Comparing `SAPL-Base-0.3.4/src/sapl_base/policy_decision_points.py` & `SAPL-Base-0.3.5/src/sapl_base/policy_decision_points.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import types
 from abc import ABC, abstractmethod
 from base64 import b64encode
-from typing import Coroutine, Dict
+from typing import Coroutine, Dict, AsyncGenerator
 
 import aiohttp
 import backoff
 import requests
 from sseclient import SSEClient
 
 from sapl_base.authorization_subscriptions import AuthorizationSubscription
@@ -57,15 +57,15 @@
 
         :return: a DummyPolicyDecisionPoint, which always returns a 'PERMIT'
         """
         return DummyPolicyDecisionPoint()
 
     @abstractmethod
     async def async_decide(self, subscription: AuthorizationSubscription,
-                           pep_decision_stream: types.GeneratorType,
+                           pep_decision_stream: AsyncGenerator,
                            decision_events: str = "decide") -> (Decision, Coroutine):
         """
         Request Decisions based on the given AuthorizationSubscription and decision_event
         returns a tuple of the first received Decision and a Coroutine
         which will send received new Decisions to the generator of the calling StreamingPolicyEnforcementpoint
 
         :param pep_decision_stream: a generator function inside the calling StreamingPolicyEnforcementpoint, to which new Decisions are sent
@@ -107,30 +107,30 @@
         super(DummyPolicyDecisionPoint, self).__init__()
         self.logger.warning(
             "ATTENTION THE APPLICATION USES A DUMMY PDP. ALL AUTHORIZATION REQUEST WILL RESULT IN A SINGLE "
             "PERMIT DECISION. DO NOT USE THIS IN PRODUCTION! THIS IS A PDP FOR TESTING AND DEVELOPING "
             "PURPOSE ONLY!"
         )
 
-    async def async_decide(self, subscription: AuthorizationSubscription, pep_decision_stream: types.GeneratorType,
+    async def async_decide(self, subscription: AuthorizationSubscription, pep_decision_stream: AsyncGenerator,
                            decision_events: str = "decide") -> (Decision, Coroutine):
         """
         implementation of decide, which returns a tuple of a Decision with Permit and a Coroutine which will send a
         Permit to the provided Generator
         """
         return Decision.permit_decision(), self._yield_permit(pep_decision_stream)
 
     @staticmethod
-    async def _yield_permit(pep_decision_stream: types.GeneratorType):
+    async def _yield_permit(pep_decision_stream: AsyncGenerator):
         """
         Send a Permit to the given Generator
 
         :param pep_decision_stream:  Generator to which the Decision is sent
         """
-        pep_decision_stream.send(Decision.permit_decision())
+        await pep_decision_stream.asend(Decision.permit_decision())
 
     async def async_decide_once(
             self, subscription: AuthorizationSubscription = None, decision_events: str = None
     ) -> Decision:
         """
         Returns a single Decision with PERMIT
 
@@ -217,23 +217,23 @@
                 subscription.__str__(),
                 stream=True,
                 verify=self.verify,
                 headers=self.headers
         ) as stream_response:
             if stream_response.status_code != 200:
                 self.logger.debug("Responsecode != 200, was %s . Decision defaults to DENY",
-                                      stream_response.status_code)
+                                  stream_response.status_code)
                 return Decision.deny_decision()
             for event in SSEClient(stream_response).events():
                 decision = Decision(json.loads(event.data))
 
-                self.logger.debug("Decision : %s", json.dumps(decision.__dict__, indent=2, skipkeys=True, default=lambda o: str(o)))
+                self.logger.debug("Decision : %s",json.dumps(decision.__dict__, indent=2, skipkeys=True, default=lambda o: str(o)))
                 return decision
 
-    async def async_decide(self, subscription: AuthorizationSubscription, pep_decision_stream: types.GeneratorType,
+    async def async_decide(self, subscription: AuthorizationSubscription, pep_decision_stream: AsyncGenerator,
                            decision_events: str = "decide") -> (Decision, types.CoroutineType):
         """
         Establish a connection to the RemotePDP and receive new Decisions, which are send to the provided Generator.
         When the connection to the RemotePDP fails, an INDETERMINATE Decision is sent to the Generator and it is
         retried to establish a connection again. Retry works with an exponential backoff and a maximum.
 
         :param subscription: AuthorizationSubscription for which Decisions should be made
@@ -242,43 +242,43 @@
         :return: A tuple of the first received Decision and a Coroutine, which will send Decisions to the given pep_decision_stream
         """
         try:
             decision, decision_stream = await self._get_first_decision_and_stream(subscription=subscription,
                                                                                   decision_events=decision_events)
         except Exception as e:
             self.logger.debug("An Error occured while getting the first Decision. Decision defaults to INDETERMINATE")
-            decision = {"decision": "INDETERMINATE"}
+            decision = Decision({"decision": "INDETERMINATE"})
             decision_stream = None
         return decision, self._update_decision(subscription=subscription, decision_stream=decision_stream,
                                                pep_decision_stream=pep_decision_stream, decision_events=decision_events)
 
     @backoff.on_exception(backoff.expo, Exception, on_backoff=recreate_stream, max_value=set_expo_max_value)
-    async def _update_decision(self, subscription: AuthorizationSubscription, decision_stream: types.AsyncGeneratorType,
-                               pep_decision_stream: types.GeneratorType, decision_events: str = "decide") -> None:
+    async def _update_decision(self, subscription: AuthorizationSubscription, decision_stream: AsyncGenerator,
+                               pep_decision_stream: AsyncGenerator, decision_events: str = "decide") -> None:
         """
         Returns a Coroutine, which will send new Decisions to the provided Generator.
         When an Exception occurs this method sends a INDETERMINATE Decision to the Generator and trys to reestablish a
         connection to the RemotePDP with an exponential backoff
 
         :param subscription: AuthorizationSubscription for which Decision will be evaluated
         :param decision_stream: Generator, which receives new Decisions from the RemotePDP
         :param pep_decision_stream: Generator, to which new Decisions are sent
         :param decision_events: For what kind of AuthorizationSubscription should a Decision be returned
         """
         if decision_stream is None:
             self.logger.debug("Stream to PDP was cancelled. Retrying to connect to the PDP")
-            await pep_decision_stream.send({"decision": "INDETERMINATE"})
+            await pep_decision_stream.asend(Decision({"decision": "INDETERMINATE"}))
             decision_stream = self._get_decision_stream(subscription=subscription, decision_events=decision_events)
 
         async for decision in decision_stream:
-            await pep_decision_stream.send(decision)
+            await pep_decision_stream.asend(Decision(decision))
+
 
-    @backoff.on_exception(backoff.constant, Exception, max_time=set_const_max_time)
     async def _get_first_decision_and_stream(self, subscription: AuthorizationSubscription, decision_events: str) -> (
-            Decision, types.AsyncGeneratorType):
+            Decision, AsyncGenerator):
         """
         Establish a connection to the RemotePDP and return the first Decision together with the Generator,
         which receives new Decisions from the RemotePDP.
         When an Exception occurs this method trys again, until it gives up after 10 seconds.
 
         :param subscription: AuthorizationSubscription for which Decision will be evaluated
         :param decision_events: For what kind of AuthorizationSubscription should a Decision be returned
@@ -288,15 +288,15 @@
         decision = await decision_stream.__anext__()
         if decision == {"decision": "INDETERMINATE"}:
             self.logger.debug("First Decision was INDETERMINATE. Defaulting to DENY")
             return Decision.deny_decision(), decision_stream
         return Decision(decision), decision_stream
 
     async def _get_decision_stream(self, subscription: AuthorizationSubscription,
-                                   decision_events: str = "decide") -> types.AsyncGeneratorType:
+                                   decision_events: str = "decide") -> AsyncGenerator:
         """
         Establish a connection to the RemotePDP and yield new Decisions
 
         :param subscription: AuthorizationSubscription for which Decision will be evaluated
         :param decision_events: For what kind of AuthorizationSubscription should a Decision be returned
         :return: A Generator yielding new Decisions received from the RemotePDP
         """
@@ -317,16 +317,16 @@
                             line_set = lines.splitlines(False)
                             response = ''
                             for item in line_set:
                                 response += item.decode('utf-8')
                             data_begin = str.find(response, '{')
                             decision = json.loads(response[data_begin:])
                             try:
-                                self.logger.debug("Decision : %s",json.dumps(decision, indent=2, skipkeys=True,
-                                                             default=lambda o: str(o)))
+                                self.logger.debug("Decision : %s", json.dumps(decision, indent=2, skipkeys=True,
+                                                                              default=lambda o: str(o)))
                             except Exception:
                                 pass
                             yield decision
                             lines = b''
 
     @backoff.on_exception(backoff.constant, Exception, max_time=set_const_max_time, raise_on_giveup=False)
     async def async_decide_once(
```

### Comparing `SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/async_policy_enforcement_point.py` & `SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/async_policy_enforcement_point.py`

 * *Files identical despite different names*

### Comparing `SAPL-Base-0.3.4/src/sapl_base/policy_enforcement_points/sync_policy_enforcement_point.py` & `SAPL-Base-0.3.5/src/sapl_base/policy_enforcement_points/sync_policy_enforcement_point.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from sapl_base.constraint_handling.constraint_handler_service import constraint_handler_service
 from sapl_base.decision import Decision
 import sapl_base.policy_decision_points
-#from sapl_base.policy_decision_points import pdp
 from sapl_base.policy_enforcement_points.policy_enforcement_point import PolicyEnforcementPoint
 
 
 class SyncPolicyEnforcementPoint(PolicyEnforcementPoint):
 
     def post_enforce(self, subject, action, resource, environment, scope):
         """
```

