# Comparing `tmp/djgraphql-0.0.5.tar.gz` & `tmp/djgraphql-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djgraphql-0.0.5.tar", last modified: Sat Aug 20 18:36:49 2022, max compression
+gzip compressed data, was "djgraphql-1.0.1.tar", last modified: Thu Jul 20 14:16:16 2023, max compression
```

## Comparing `djgraphql-0.0.5.tar` & `djgraphql-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 18:36:49.477944 djgraphql-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-20 18:36:28.000000 djgraphql-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-20 18:36:28.000000 djgraphql-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-20 18:36:49.477944 djgraphql-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-08-20 18:36:28.000000 djgraphql-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 18:36:49.477944 djgraphql-0.0.5/djgraphql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 18:36:49.477944 djgraphql-0.0.5/djgraphql/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/test/test_api_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-08-20 18:36:28.000000 djgraphql-0.0.5/djgraphql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 18:36:49.477944 djgraphql-0.0.5/djgraphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-20 18:36:49.000000 djgraphql-0.0.5/djgraphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-08-20 18:36:49.000000 djgraphql-0.0.5/djgraphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-20 18:36:49.000000 djgraphql-0.0.5/djgraphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-20 18:36:49.000000 djgraphql-0.0.5/djgraphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-20 18:36:49.000000 djgraphql-0.0.5/djgraphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-08-20 18:36:28.000000 djgraphql-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-20 18:36:49.477944 djgraphql-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-08-20 18:36:28.000000 djgraphql-0.0.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-20 18:36:28.000000 djgraphql-0.0.5/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 14:15:51.000000 djgraphql-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 14:15:51.000000 djgraphql-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-20 14:16:16.387680 djgraphql-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-20 14:15:51.000000 djgraphql-1.0.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-20 14:15:51.000000 djgraphql-1.0.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-20 14:15:51.000000 djgraphql-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/djgraphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/djgraphql/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/djgraphql/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/utils/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/utils/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/djgraphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 14:15:51.000000 djgraphql-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:16:16.387680 djgraphql-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-20 14:15:51.000000 djgraphql-1.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 14:15:51.000000 djgraphql-1.0.1/version
```

### Comparing `djgraphql-0.0.5/LICENSE.txt` & `djgraphql-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-0.0.5/PKG-INFO` & `djgraphql-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 0.0.5
+Version: 1.0.1
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-0.0.5/README.md` & `djgraphql-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `djgraphql-0.0.5/djgraphql/settings.py` & `djgraphql-1.0.1/djgraphql/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,27 @@
 from django.conf import settings
 from django.test.signals import setting_changed
-from django.utils.module_loading import import_string
 
-from .defaults import get_defaults
-
-
-def perform_import(val, setting_name):
-    """
-    If the given setting is a string import notation,
-    then perform the necessary import or imports.
-    """
-    if val is None:
-        return None
-    elif isinstance(val, str):
-        return import_from_string(val, setting_name)
-    elif isinstance(val, (list, tuple)):
-        return [import_from_string(item, setting_name) for item in val]
-    return val
-
-
-def import_from_string(val, setting_name):
-    """
-    Attempt to import a class from a string representation.
-    """
-    try:
-        return import_string(val)
-    except ImportError as e:
-        msg = "Could not import '%s' for API setting '%s'. %s: %s." % (val, setting_name, e.__class__.__name__, e)
-        raise ImportError(msg)
+from djgraphql.defaults import Defaults
 
 
 class ImportSettings:
-    def defaults(self):
-        params = get_defaults()
+    @staticmethod
+    def defaults():
+        params = {key:value for key, value in Defaults.__dict__.items() if not key.startswith('__') and not callable(key)}
         new_defaults = {}
         for key, value in params.items():
             try:
                 new_defaults[key] = getattr(settings, key, value)
             except Exception as e:  # noqa
                 new_defaults[key] = value
-
         return new_defaults
 
 
-_settings = ImportSettings()
-DEFAULTS = _settings.defaults()
+DEFAULTS = ImportSettings.defaults()
 
 
 class APISettings:
     """
     A settings object that allows REST Framework settings to be accessed as
     properties. For example:
         from common.settings import api_settings
```

### Comparing `djgraphql-0.0.5/djgraphql.egg-info/PKG-INFO` & `djgraphql-1.0.1/djgraphql.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 0.0.5
+Version: 1.0.1
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-0.0.5/setup.py` & `djgraphql-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,11 +34,11 @@
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     ],
     include_package_data=True,
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=[
-        'django==3',
+        'django',
         'graphene-django',
     ],
 )
```

