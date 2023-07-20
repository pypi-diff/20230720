# Comparing `tmp/im-squonk2-client-2.2.0.tar.gz` & `tmp/im-squonk2-client-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im-squonk2-client-2.2.0.tar", last modified: Tue May 23 14:49:51 2023, max compression
+gzip compressed data, was "im-squonk2-client-2.2.1.tar", last modified: Tue May 23 17:43:24 2023, max compression
```

## Comparing `im-squonk2-client-2.2.0.tar` & `im-squonk2-client-2.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:51.820092 im-squonk2-client-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-23 14:49:51.820092 im-squonk2-client-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:49:51.820092 im-squonk2-client-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:51.812091 im-squonk2-client-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:51.816091 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:51.820092 im-squonk2-client-2.2.0/src/squonk2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19931 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/as_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    46803 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/dm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/ui_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:24.618975 im-squonk2-client-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-23 17:43:24.618975 im-squonk2-client-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:43:24.618975 im-squonk2-client-2.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:24.614975 im-squonk2-client-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:24.614975 im-squonk2-client-2.2.1/src/im_squonk2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-23 17:43:24.000000 im-squonk2-client-2.2.1/src/im_squonk2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-23 17:43:24.000000 im-squonk2-client-2.2.1/src/im_squonk2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:43:24.000000 im-squonk2-client-2.2.1/src/im_squonk2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:43:24.000000 im-squonk2-client-2.2.1/src/im_squonk2_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 17:43:24.000000 im-squonk2-client-2.2.1/src/im_squonk2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 17:43:24.000000 im-squonk2-client-2.2.1/src/im_squonk2_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:24.618975 im-squonk2-client-2.2.1/src/squonk2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/src/squonk2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19931 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/src/squonk2/as_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/src/squonk2/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46803 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/src/squonk2/dm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/src/squonk2/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-23 17:43:13.000000 im-squonk2-client-2.2.1/src/squonk2/ui_api.py
```

### Comparing `im-squonk2-client-2.2.0/LICENSE` & `im-squonk2-client-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.2.0/PKG-INFO` & `im-squonk2-client-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-squonk2-client
-Version: 2.2.0
+Version: 2.2.1
 Summary: Squonk2 Python Client
 Home-page: https://github.com/informaticsmatters/squonk2-python-client
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: api
 Platform: any
```

### Comparing `im-squonk2-client-2.2.0/README.rst` & `im-squonk2-client-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.2.0/setup.py` & `im-squonk2-client-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/PKG-INFO` & `im-squonk2-client-2.2.1/src/im_squonk2_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-squonk2-client
-Version: 2.2.0
+Version: 2.2.1
 Summary: Squonk2 Python Client
 Home-page: https://github.com/informaticsmatters/squonk2-python-client
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: api
 Platform: any
```

### Comparing `im-squonk2-client-2.2.0/src/squonk2/as_api.py` & `im-squonk2-client-2.2.1/src/squonk2/as_api.py`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.2.0/src/squonk2/auth.py` & `im-squonk2-client-2.2.1/src/squonk2/auth.py`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.2.0/src/squonk2/dm_api.py` & `im-squonk2-client-2.2.1/src/squonk2/dm_api.py`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.2.0/src/squonk2/environment.py` & `im-squonk2-client-2.2.1/src/squonk2/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,16 +266,16 @@
         value found in the environment.
         """
         return self.__ui_hostname
 
     @property
     def ui_api(self) -> Optional[str]:
         """Return the web/UI API. This is the UI hostname
-        with a 'http' prefix and '/api' postfix.
+        with a 'http' prefix and '/data-manager-ui/api' postfix.
         """
         if not self.__ui_hostname:
             return None
         if not self.__ui_hostname.startswith("http"):
-            ret_val: str = f"https://{self.__ui_hostname}/api"
+            ret_val: str = f"https://{self.__ui_hostname}/data-manager-ui/api"
         else:
             ret_val = self.__ui_hostname
         return ret_val
```

### Comparing `im-squonk2-client-2.2.0/src/squonk2/ui_api.py` & `im-squonk2-client-2.2.1/src/squonk2/ui_api.py`

 * *Files identical despite different names*

