# Comparing `tmp/SAPL-Django-0.3.4.tar.gz` & `tmp/SAPL-Django-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPL-Django-0.3.4.tar", last modified: Mon Feb  6 11:49:50 2023, max compression
+gzip compressed data, was "SAPL-Django-0.3.5.tar", last modified: Thu Jul 20 21:53:35 2023, max compression
```

## Comparing `SAPL-Django-0.3.4.tar` & `SAPL-Django-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 11:49:50.721005 SAPL-Django-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-06 11:49:50.721005 SAPL-Django-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 11:49:50.721005 SAPL-Django-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 11:49:50.717005 SAPL-Django-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 11:49:50.717005 SAPL-Django-0.3.4/src/SAPL_Django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-06 11:49:50.000000 SAPL-Django-0.3.4/src/SAPL_Django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-06 11:49:50.000000 SAPL-Django-0.3.4/src/SAPL_Django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 11:49:50.000000 SAPL-Django-0.3.4/src/SAPL_Django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-06 11:49:50.000000 SAPL-Django-0.3.4/src/SAPL_Django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-06 11:49:50.000000 SAPL-Django-0.3.4/src/SAPL_Django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 11:49:50.721005 SAPL-Django-0.3.4/src/sapl_django/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/src/sapl_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/src/sapl_django/django_authorization_subscription_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/src/sapl_django/django_streaming_policy_enforcement_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-06 11:49:31.000000 SAPL-Django-0.3.4/src/sapl_django/sapl_request_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:35.135176 SAPL-Django-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20600 2023-07-20 21:53:35.135176 SAPL-Django-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:53:35.135176 SAPL-Django-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:35.131176 SAPL-Django-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:35.131176 SAPL-Django-0.3.5/src/SAPL_Django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20600 2023-07-20 21:53:35.000000 SAPL-Django-0.3.5/src/SAPL_Django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-20 21:53:35.000000 SAPL-Django-0.3.5/src/SAPL_Django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:53:35.000000 SAPL-Django-0.3.5/src/SAPL_Django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 21:53:35.000000 SAPL-Django-0.3.5/src/SAPL_Django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 21:53:35.000000 SAPL-Django-0.3.5/src/SAPL_Django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:35.135176 SAPL-Django-0.3.5/src/sapl_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/src/sapl_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/src/sapl_django/django_authorization_subscription_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/src/sapl_django/django_streaming_policy_enforcement_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/src/sapl_django/sapl_request_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:35.135176 SAPL-Django-0.3.5/src/sapl_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/src/sapl_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/src/sapl_django/templatetags/sapl_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:53:35.135176 SAPL-Django-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-20 21:53:18.000000 SAPL-Django-0.3.5/tests/test_authorization_subscription_factory.py
```

### Comparing `SAPL-Django-0.3.4/LICENSE` & `SAPL-Django-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPL-Django-0.3.4/pyproject.toml` & `SAPL-Django-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "SAPL-Django"
-version = "0.3.4"
+version = "0.3.5"
 description = "initial upload to register the name for future development"
 readme = "README.md"
 authors = [{ name = "Dominic Heutelbeck", email = "dominic@heutelbeck.com"}]
 license = { file = "LICENSE" }
 dependencies = [
     'django',
     'channels',
```

### Comparing `SAPL-Django-0.3.4/src/sapl_django/__init__.py` & `SAPL-Django-0.3.5/src/sapl_django/__init__.py`

 * *Files identical despite different names*

### Comparing `SAPL-Django-0.3.4/src/sapl_django/django_authorization_subscription_factory.py` & `SAPL-Django-0.3.5/src/sapl_django/django_authorization_subscription_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,124 @@
+import contextvars
 from typing import Dict
 
 from channels.consumer import AsyncConsumer
 from django.db.models import QuerySet, Manager, Model
 from django.forms import model_to_dict
 from django.urls import ResolverMatch
 from django.views import View
 
-from sapl_base.authorization_subscription_factory import AuthorizationSubscriptionFactory, client_request, authorization_subscription
+from sapl_base.authorization_subscription_factory import AuthorizationSubscriptionFactory, client_request
+from sapl_base.authorization_subscriptions import AuthorizationSubscription
+
+
+def identify_type(values: Dict) -> str:
+    """
+    Identifies the type of the decorated function
+
+    :param values: dict containing all values needed to create the AuthorizationSubscription
+    :return: The name of the type of the decorated function
+    """
+    if 'self' in values:
+        try:
+            classes_names = values['self']
+            if isinstance(classes_names, View):
+                return 'View'
+            if isinstance(classes_names, QuerySet):
+                return 'Queryset'
+            if isinstance(classes_names, Manager):
+                return 'Manager'
+            if isinstance(classes_names, AsyncConsumer):
+                return 'Consumer'
+        except Exception:
+            pass
+    return 'View'
+
+
+def get_authorization(request):
+    if request.headers.get("Authorization") is not None:
+        authorization = request.headers.get("Authorization")
+        if authorization.find('Bearer ') == 0:
+            return authorization[7:]
+        else:
+            return None
 
 
 class DjangoAuthorizationSubscriptionFactory(AuthorizationSubscriptionFactory):
     """
     AuthorizationSubscriptionFactory for Django projects
     Creates AuthorizationSubscription, when SAPL is used in a Django project.
     """
 
-    STREAMING_ENFORCEMENTS = ('enforce_till_denied', 'enforce_while_denied', 'drop_while_denied')
+    STREAMING_ENFORCEMENTS = ('enforce_till_denied', 'enforce_drop_while_denied','enforce_recoverable_if_denied')
     POST_ENFORCE_CLASSES = ('Manager', 'Queryset')
 
     def _default_action_function(self, values: Dict) -> Dict:
         """
         Create a dict which is used as action to create an AuthorizationSubscription
         :param values: dict containing all values needed to create an AuthorizationSubscription
         :param fn_type: Type of the decorated function
         :return: A dictionary which will be provided as action, when an AuthorizationSubscription is created
         """
         action = {}
-        request = values['request']
-        resolver: ResolverMatch = request.resolver_match
         function_para = {}
 
         if 'self' in values:
             function_para.update({'class': values['self'].__class__.__name__})
-        function_para.update({'function_name': values['function'].__name__})
+        try:
+            function_para.update({'function_name': values['function'].__name__})
+        except Exception:
+            pass
         function_para.update({'type': values['type']})
         request_para = {}
-        request_para.update({'path': request.path})
-        request_para.update({'method': request.method})
-        request_para.update({'view_name': resolver.view_name})
-        request_para.update({'route': resolver.route})
-        request_para.update({'url_name': resolver.url_name})
+        if values.get('request') is not None:
+            request = values['request']
+            resolver: ResolverMatch = request.resolver_match
+            request_para.update({'path': request.path})
+            request_para.update({'method': request.method})
+            request_para.update({'view_name': resolver.view_name})
+            request_para.update({'route': resolver.route})
+            request_para.update({'url_name': resolver.url_name})
+        elif values.get('scope') is not None:
+            request = values['scope']
+            request_para.update({'path': request["path"]})
+            request_para.update({'type': request["type"]})
+
 
         action.update({'request': request_para})
         action.update({'function': function_para})
         return action
 
     def _default_resource_function(self, values: Dict) -> Dict:
         """
         Create a dict which is used as resource to create an AuthorizationSubscription
         :param values: dict containing all values needed to create an AuthorizationSubscription
         :return: A dictionary which will be provided as resource, when an AuthorizationSubscription is created
         """
         resource = {}
-        request = values['request']
-        resolver: ResolverMatch = request.resolver_match
-        request_method = request.method
         request_resources = {}
         function_resources = {}
-        if request_method == 'GET':
-            request_resources.update({'GET': request.GET.dict()})
-        if request_method == 'POST':
-            request_resources.update({'POST': request.POST.dict()})
 
-        function_resources.update({'url_kwargs': resolver.kwargs})
+        if values.get('request') is not None:
+            request = values['request']
+            resolver: ResolverMatch = request.resolver_match
+            request_method = request.method
+            if request_method == 'GET':
+                request_resources.update({'GET': request.GET.dict()})
+            if request_method == 'POST':
+                request_resources.update({'POST': request.POST.dict()})
+            function_resources.update({'url_kwargs': resolver.kwargs})
+
+        elif values.get('scope') is not None:
+            request = values['scope']
+            function_resources.update({'url_kwargs': request["url_route"]["kwargs"]})
+            function_resources.update({'cookies': request["cookies"]})
+            function_resources.update({'asgi': request["asgi"]})
+
+
         args_copy: dict = values.get('args').copy()
         if 'self' in args_copy:
             args_copy.pop('self')
         function_resources.update({'kwargs': self._map_model_to_dict(args_copy)})
         if 'return_value' in values:
             return_value = values['return_value']
             if isinstance(return_value, Model):
@@ -94,53 +146,45 @@
 
     def _default_subject_function(self, values: Dict):
         """
         Create a dict which is used as subject to create an AuthorizationSubscription
         :param values: dict containing all values needed to create an AuthorizationSubscription
         :return: A dictionary which will be provided as subject, when an AuthorizationSubscription is created
         """
-        request = values['request']
+
+        request = values.get('request') if values.get('request') is not None else values.get('scope')
 
         try:
             user = request.user
             if user.is_anonymous:
                 if request.headers.get("Authorization") is not None:
-                    return self._get_authorization(request)
+                    return {"authorization": get_authorization(request)}
                 return 'anonymous'
         except Exception:
-            return 'anonymous'   
+            return 'anonymous'
         subj = {}
         subj.update({'user_id': user.id,
                      'username': user.username,
                      'first_name': user.first_name,
                      'last_name': user.last_name,
                      'is_active': user.is_active,
                      'is_superuser': user.is_superuser,
                      'permissions': list(user.get_all_permissions()),
                      'groups': [group.name for group in list(user.groups.all())],
                      'last_login': user.last_login,
                      'is_authenticated': user.is_authenticated,
                      })
         try:
-            subj.update({'authorization':self._get_authorization(request)})
+            subj.update({'authorization': get_authorization(request)})
         except Exception:
             pass
         return subj
 
-
-    def _get_authorization(self,request):
-        if request.headers.get("Authorization") is not None:
-            authorization = request.headers.get("Authorization")
-            if authorization.find('Bearer ') == 0:
-                return authorization[7:]
-            else:
-                return None
-
     def create_authorization_subscription(self, values: Dict, subject, action, resource,
-                                          environment, scope, enforcement_type):
+                                          environment, scope, enforcement_type)-> AuthorizationSubscription:
         """
         Create an AuthorizationSubscription with the given dictionary and arguments
 
         The returned AuthorizationSubscription is dependent of the framework and the decorated function
 
         :param enforcement_type: the type of enforcement, with which the function is decorated
         :param scope: Argument which creates a AuthorizationSubscription according to the given scope instead of evaluating the scope based on other parameter
@@ -150,23 +194,22 @@
         :param resource: resource with which the function was decorated. None if not specified
         :param environment: environment with which the function was decorated. None if not specified
         :return: An authorization_subscription which can be sent to a pdp to get an authorization_decision
         """
         fn_type: str
         self._add_contextvar_to_values(values)
         if scope == "automatic":
-            fn_type = self._identify_type(values)
+            fn_type = identify_type(values)
         else:
             fn_type = scope
 
         self._valid_combination(fn_type, enforcement_type)
         values.update({'type': fn_type})
 
         authz = self._create_subscription(values, subject, action, resource, environment)
-        authorization_subscription.set(authz)
         return authz
 
     def _valid_combination(self, fn_type: str, enforcement_type: str) -> None:
         """
         Checks if the combination of the type of the decorated function and the type of enforcement is valid
 
         :param fn_type: Type of decorated function
@@ -174,38 +217,24 @@
         """
         if fn_type == 'View' and enforcement_type == 'pre_enforce':
             return
         if fn_type == 'Consumer' and enforcement_type in self.STREAMING_ENFORCEMENTS:
             return
         if fn_type in self.POST_ENFORCE_CLASSES and enforcement_type in ('post_enforce', 'pre_enforce'):
             return
+        if fn_type == 'Template' and enforcement_type == 'pre_enforce':
+            return
         raise
 
-    def _identify_type(self, values: Dict) -> str:
-        """
-        Identifies the type of the decorated function
-
-        :param values: dict containing all values needed to create the AuthorizationSubscription
-        :return: The name of the type of the decorated function
-        """
-        if 'self' in values:
-            try:
-                classes_names = values['self']
-                if isinstance(classes_names, View):
-                    return 'View'
-                if isinstance(classes_names, QuerySet):
-                    return 'Queryset'
-                if isinstance(classes_names, Manager):
-                    return 'Manager'
-                if isinstance(classes_names, AsyncConsumer):
-                    return 'Consumer'
-            except Exception:
-                pass
-        return 'View'
-
     def _add_contextvar_to_values(self, values: Dict) -> None:
         """
         Adds the request made to the dict which is used to create the AuthorizationSubscription
         :param values: A dict object containing all values needed to create an AuthorizationSubscription
         """
-        request = client_request.get('request')
-        values.update({'request': request})
+        if client_request.get('request') != 'request':
+            values.update({'request': client_request.get('request')})
+        if consumer_scope.get('scope') != 'scope':
+            values.update({'scope': consumer_scope.get()})
+
+
+
+consumer_scope = contextvars.ContextVar('scope')
```

### Comparing `SAPL-Django-0.3.4/src/sapl_django/sapl_request_middleware.py` & `SAPL-Django-0.3.5/src/sapl_django/sapl_request_middleware.py`

 * *Files identical despite different names*

