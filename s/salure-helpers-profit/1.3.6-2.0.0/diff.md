# Comparing `tmp/salure_helpers_profit-1.3.6.tar.gz` & `tmp/salure_helpers_profit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-1.3.6.tar", last modified: Thu Jul 20 16:21:17 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-2.0.0.tar", last modified: Thu Jul 20 16:32:22 2023, max compression
```

## Comparing `salure_helpers_profit-1.3.6.tar` & `salure_helpers_profit-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   139049 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   139049 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/setup.py
```

### Comparing `salure_helpers_profit-1.3.6/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-2.0.0/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.6/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-2.0.0/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.6/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-2.0.0/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.6/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-2.0.0/salure_helpers/profit/profit_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -842,16 +842,16 @@
     def update_function(self, data: dict, overload_fields: dict = None, method="PUT") -> requests.Response:
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: Give the guid and value from a free field if wanted
         :param method: PUT or POST, depending on the case
         :return: status code for request and optional error message
         """
-        allowed_fields = ['formation', 'costcarrier']
-        required_fields = ['startdate', 'employee_id', 'organizational_unit', 'function', 'costcentre', 'employment_number']
+        allowed_fields = ['formation', 'costcarrier', 'employment_number']
+        required_fields = ['startdate', 'employee_id', 'organizational_unit', 'function', 'costcentre']
 
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'KnEmployee/AfasOrgunitFunction')
 
         base_body = {
             "AfasEmployee": {
```

### Comparing `salure_helpers_profit-1.3.6/setup.py` & `salure_helpers_profit-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='1.3.6',
+    version='2.0.0',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

