# Comparing `tmp/dys-connector-0.2.8.tar.gz` & `tmp/dys-connector-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dys-connector-0.2.8.tar", last modified: Mon Sep 12 07:34:52 2022, max compression
+gzip compressed data, was "dys-connector-0.2.9.tar", last modified: Fri Oct 14 12:22:40 2022, max compression
```

## Comparing `dys-connector-0.2.8.tar` & `dys-connector-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-09-12 07:34:52.668887 dys-connector-0.2.8/
--rw-rw-rw-   0        0        0    11558 2022-03-18 07:25:32.000000 dys-connector-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     1932 2022-09-12 07:34:52.669886 dys-connector-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1499 2022-03-18 07:25:32.000000 dys-connector-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2022-09-12 07:34:52.631886 dys-connector-0.2.8/dys_connector/
--rw-rw-rw-   0        0        0        0 2022-03-18 07:25:32.000000 dys-connector-0.2.8/dys_connector/__init__.py
--rw-rw-rw-   0        0        0      774 2022-05-27 08:20:53.000000 dys-connector-0.2.8/dys_connector/dto.py
--rw-rw-rw-   0        0        0    13088 2022-09-12 07:34:16.000000 dys-connector-0.2.8/dys_connector/dys_api_manager.py
--rw-rw-rw-   0        0        0     1726 2022-08-19 09:29:16.000000 dys-connector-0.2.8/dys_connector/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-09-12 07:34:52.664886 dys-connector-0.2.8/dys_connector.egg-info/
--rw-rw-rw-   0        0        0     1932 2022-09-12 07:34:52.000000 dys-connector-0.2.8/dys_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2022-09-12 07:34:52.000000 dys-connector-0.2.8/dys_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-12 07:34:52.000000 dys-connector-0.2.8/dys_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-09-12 07:34:52.000000 dys-connector-0.2.8/dys_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-09-12 07:34:52.000000 dys-connector-0.2.8/dys_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-09-12 07:34:52.678886 dys-connector-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      808 2022-09-12 07:34:16.000000 dys-connector-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-14 12:22:40.301993 dys-connector-0.2.9/
+-rw-rw-rw-   0        0        0    11558 2022-03-18 07:25:32.000000 dys-connector-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     1932 2022-10-14 12:22:40.302993 dys-connector-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1499 2022-03-18 07:25:32.000000 dys-connector-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-14 12:22:40.251991 dys-connector-0.2.9/dys_connector/
+-rw-rw-rw-   0        0        0        0 2022-03-18 07:25:32.000000 dys-connector-0.2.9/dys_connector/__init__.py
+-rw-rw-rw-   0        0        0      774 2022-05-27 08:20:53.000000 dys-connector-0.2.9/dys_connector/dto.py
+-rw-rw-rw-   0        0        0    13155 2022-10-14 12:16:49.000000 dys-connector-0.2.9/dys_connector/dys_api_manager.py
+-rw-rw-rw-   0        0        0     2045 2022-10-14 12:16:49.000000 dys-connector-0.2.9/dys_connector/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-10-14 12:22:40.296992 dys-connector-0.2.9/dys_connector.egg-info/
+-rw-rw-rw-   0        0        0     1932 2022-10-14 12:22:39.000000 dys-connector-0.2.9/dys_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2022-10-14 12:22:39.000000 dys-connector-0.2.9/dys_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-14 12:22:39.000000 dys-connector-0.2.9/dys_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-10-14 12:22:39.000000 dys-connector-0.2.9/dys_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-10-14 12:22:39.000000 dys-connector-0.2.9/dys_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-10-14 12:22:40.315992 dys-connector-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      808 2022-10-14 12:22:23.000000 dys-connector-0.2.9/setup.py
```

### Comparing `dys-connector-0.2.8/LICENSE` & `dys-connector-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dys-connector-0.2.8/PKG-INFO` & `dys-connector-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dys-connector
-Version: 0.2.8
+Version: 0.2.9
 Summary: Logo DYS Connector API Python Implementation
 Home-page: https://github.com/logo-group/dys-connector
 Author: Mustafa Talha Arslan, Furkan Arif Bozdag, Hilal Ozkan
 Author-email: mustafa.arslan@logo.com.tr, arif.bozdag@logo.com.tr, hilal.ozkan@logo.com.tr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dys-connector-0.2.8/README.md` & `dys-connector-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dys-connector-0.2.8/dys_connector/dto.py` & `dys-connector-0.2.9/dys_connector/dto.py`

 * *Files identical despite different names*

### Comparing `dys-connector-0.2.8/dys_connector/dys_api_manager.py` & `dys-connector-0.2.9/dys_connector/dys_api_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,16 @@
         logging.debug(response.text)
         if code == 400:
             raise DysBadRequestError()
         elif code == 401:
             raise DysUnauthorizedError()
         elif code == 500:
             raise DysInternalServerError()
+        elif code == 502:
+            raise DysBadGatewayError()
         elif int(code / 100) != 2:
             raise DysHttpException(status_code=code)
 
     def make_dys_request(self, method: str, url: str, headers=None, **kwargs):
         """
         General DYS requests with basic error handling
         :param method: Request method. Ex: "GET", "POST", "PUT"
```

### Comparing `dys-connector-0.2.8/dys_connector/exceptions.py` & `dys-connector-0.2.9/dys_connector/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,13 +32,22 @@
     """Raised when Dys Internal Server Error occurs with error code 500"""
     def __init__(self, message="Dys Internal Server Error!"):
         self.status_code = 500
         self.message = message
         super().__init__(status_code=self.status_code, message=message)
 
 
+class DysBadGatewayError(DysHttpException):
+    """Raised when Dys Bad Gateway Error occurs with error code 502"""
+    def __init__(self, message="Dys Bad Gateway Error!"):
+        self.status_code = 502
+        self.message = message
+        super().__init__(status_code=self.status_code, message=message)
+
+
 class DysClearDirectoryItemDeleteException(DysHttpException):
     """Raised when Dys Internal Server Error occurs with error code 500"""
     def __init__(self, message="Clear Directory Item Delete Exception"):
         self.status_code = 500
         self.message = message
         super().__init__(status_code=self.status_code, message=message)
+
```

### Comparing `dys-connector-0.2.8/dys_connector.egg-info/PKG-INFO` & `dys-connector-0.2.9/dys_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dys-connector
-Version: 0.2.8
+Version: 0.2.9
 Summary: Logo DYS Connector API Python Implementation
 Home-page: https://github.com/logo-group/dys-connector
 Author: Mustafa Talha Arslan, Furkan Arif Bozdag, Hilal Ozkan
 Author-email: mustafa.arslan@logo.com.tr, arif.bozdag@logo.com.tr, hilal.ozkan@logo.com.tr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dys-connector-0.2.8/setup.py` & `dys-connector-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import pathlib
 
-VERSION = '0.2.8'
+VERSION = '0.2.9'
 DESCRIPTION = 'Logo DYS Connector API Python Implementation'
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
```

