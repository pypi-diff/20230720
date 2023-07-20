# Comparing `tmp/splunk-sdk-1.7.3.tar.gz` & `tmp/splunk-sdk-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splunk-sdk-1.7.3.tar", last modified: Mon Feb 13 06:03:56 2023, max compression
+gzip compressed data, was "dist/splunk-sdk-1.7.4.tar", last modified: Thu Jul 20 09:11:05 2023, max compression
```

## Comparing `splunk-sdk-1.7.3.tar` & `splunk-sdk-1.7.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4401 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/splunk_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/splunk_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/splunk_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/splunk_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/splunk_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/splunklib/
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60209 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)   150652 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/splunklib/modularinput/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/event_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/input_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/modularinput/validation_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:56.000000 splunk-sdk-1.7.3/splunklib/searchcommands/
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/eventing_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/external_search_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/generating_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    28820 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/internals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/reporting_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    40702 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/search_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/streaming_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/searchcommands/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    34536 2023-02-13 06:03:48.000000 splunk-sdk-1.7.3/splunklib/six.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:11:05.000000 splunk-sdk-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-20 09:11:05.000000 splunk-sdk-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14647 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 09:11:05.000000 splunk-sdk-1.7.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4401 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:11:05.000000 splunk-sdk-1.7.4/splunk_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-20 09:11:04.000000 splunk-sdk-1.7.4/splunk_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-20 09:11:05.000000 splunk-sdk-1.7.4/splunk_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:11:04.000000 splunk-sdk-1.7.4/splunk_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 09:11:04.000000 splunk-sdk-1.7.4/splunk_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:11:05.000000 splunk-sdk-1.7.4/splunklib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60887 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150652 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:11:05.000000 splunk-sdk-1.7.4/splunklib/modularinput/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/event_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/input_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/modularinput/validation_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:11:05.000000 splunk-sdk-1.7.4/splunklib/searchcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/eventing_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/external_search_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/generating_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28820 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/reporting_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40720 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/search_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/streaming_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/searchcommands/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34536 2023-07-20 09:10:55.000000 splunk-sdk-1.7.4/splunklib/six.py
```

### Comparing `splunk-sdk-1.7.3/PKG-INFO` & `splunk-sdk-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: splunk-sdk
-Version: 1.7.3
+Version: 1.7.4
 Summary: The Splunk Software Development Kit for Python.
 Home-page: http://github.com/splunk/splunk-sdk-python
 Author: Splunk, Inc.
 Author-email: devinfo@splunk.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `splunk-sdk-1.7.3/README.md` & `splunk-sdk-1.7.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-[![Build Status](https://travis-ci.org/splunk/splunk-sdk-python.svg?branch=master)](https://travis-ci.org/splunk/splunk-sdk-python)
-[![Documentation Status](https://readthedocs.org/projects/splunk-python-sdk/badge/?version=latest)](https://splunk-python-sdk.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://github.com/splunk/splunk-sdk-python/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/splunk/splunk-sdk-python/actions/workflows/test.yml)
+
+[Reference Docs](https://dev.splunk.com/enterprise/reference)
 
 # The Splunk Enterprise Software Development Kit for Python
 
-#### Version 1.7.3
+#### Version 1.7.4
 
 The Splunk Enterprise Software Development Kit (SDK) for Python contains library code designed to enable developers to build applications using the Splunk platform.
 
 The Splunk platform is a search engine and analytic environment that uses a distributed map-reduce architecture to efficiently index, search, and process large time-varying data sets.
 
 The Splunk platform is popular with system administrators for aggregation and monitoring of IT machine data, security, compliance, and a wide variety of other scenarios that share a requirement to efficiently index, search, analyze, and generate real-time notifications from large volumes of time-series data.
 
@@ -123,15 +124,15 @@
 
 The Splunk Enterprise SDK for Python contains a collection of unit tests. To run them, open a command prompt in the **/splunk-sdk-python** directory and enter:
 
     make
 
 You can also run individual test files, which are located in **/splunk-sdk-python/tests**. To run a specific test, enter:
 
-    make specific_test_name
+    make test_specific
 
 The test suite uses Python's standard library, the built-in `unittest` library, `pytest`, and `tox`.
 
 >**Notes:**
 >*  The test run fails unless the [SDK App Collection](https://github.com/splunk/sdk-app-collection) app is installed.
 >*  To exclude app-specific tests, use the `make test_no_app` command.
 >*  To learn about our testing framework, see [Splunk Test Suite](https://github.com/splunk/splunk-sdk-python/tree/master/tests) on GitHub.
```

### Comparing `splunk-sdk-1.7.3/setup.py` & `splunk-sdk-1.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunk_sdk.egg-info/PKG-INFO` & `splunk-sdk-1.7.4/splunk_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: splunk-sdk
-Version: 1.7.3
+Version: 1.7.4
 Summary: The Splunk Software Development Kit for Python.
 Home-page: http://github.com/splunk/splunk-sdk-python
 Author: Splunk, Inc.
 Author-email: devinfo@splunk.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `splunk-sdk-1.7.3/splunk_sdk.egg-info/SOURCES.txt` & `splunk-sdk-1.7.4/splunk_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/__init__.py` & `splunk-sdk-1.7.4/splunklib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 # ex. To enable debug logs, call this method with parameter 'logging.DEBUG'
 # default logging level is set to 'WARNING'
 def setup_logging(level, log_format=DEFAULT_LOG_FORMAT, date_format=DEFAULT_DATE_FORMAT):
     logging.basicConfig(level=level,
                         format=log_format,
                         datefmt=date_format)
 
-__version_info__ = (1, 7, 3)
+__version_info__ = (1, 7, 4)
 __version__ = ".".join(map(str, __version_info__))
```

### Comparing `splunk-sdk-1.7.3/splunklib/binding.py` & `splunk-sdk-1.7.4/splunklib/binding.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 If you want a friendlier interface to the Splunk REST API, use the
 :mod:`splunklib.client` module.
 """
 
 from __future__ import absolute_import
 
 import io
+import json
 import logging
 import socket
 import ssl
 import sys
 import time
 from base64 import b64encode
 from contextlib import contextmanager
@@ -56,31 +57,58 @@
     "AuthenticationError",
     "connect",
     "Context",
     "handler",
     "HTTPError"
 ]
 
+SENSITIVE_KEYS = ['Authorization', 'Cookie', 'action.email.auth_password', 'auth', 'auth_password', 'clear_password', 'clientId',
+                  'crc-salt', 'encr_password', 'oldpassword', 'passAuth', 'password', 'session', 'suppressionKey',
+                  'token']
+
 # If you change these, update the docstring
 # on _authority as well.
 DEFAULT_HOST = "localhost"
 DEFAULT_PORT = "8089"
 DEFAULT_SCHEME = "https"
 
+
 def _log_duration(f):
     @wraps(f)
     def new_f(*args, **kwargs):
         start_time = datetime.now()
         val = f(*args, **kwargs)
         end_time = datetime.now()
         logger.debug("Operation took %s", end_time-start_time)
         return val
     return new_f
 
 
+def mask_sensitive_data(data):
+    '''
+    Masked sensitive fields data for logging purpose
+    '''
+    if not isinstance(data, dict):
+        try:
+            data = json.loads(data)
+        except Exception as ex:
+            return data
+
+    # json.loads will return "123"(str) as 123(int), so return the data if it's not 'dict' type
+    if not isinstance(data, dict):
+        return data
+    mdata = {}
+    for k, v in data.items():
+        if k in SENSITIVE_KEYS:
+            mdata[k] = "******"
+        else:
+            mdata[k] = mask_sensitive_data(v)
+    return mdata
+
+
 def _parse_cookies(cookie_str, dictionary):
     """Tries to parse any key-value pairs of cookies in a string,
     then updates the the dictionary with any key-value pairs found.
 
     **Example**::
 
         dictionary = {}
@@ -627,15 +655,15 @@
                  'status': 200}
             c.delete('nonexistant/path') # raises HTTPError
             c.logout()
             c.delete('apps/local') # raises AuthenticationError
         """
         path = self.authority + self._abspath(path_segment, owner=owner,
                                               app=app, sharing=sharing)
-        logger.debug("DELETE request to %s (body: %s)", path, repr(query))
+        logger.debug("DELETE request to %s (body: %s)", path, mask_sensitive_data(query))
         response = self.http.delete(path, self._auth_headers, **query)
         return response
 
     @_authentication
     @_log_duration
     def get(self, path_segment, owner=None, app=None, headers=None, sharing=None, **query):
         """Performs a GET operation from the REST path segment with the given
@@ -690,15 +718,15 @@
             c.get('apps/local') # raises AuthenticationError
         """
         if headers is None:
             headers = []
 
         path = self.authority + self._abspath(path_segment, owner=owner,
                                               app=app, sharing=sharing)
-        logger.debug("GET request to %s (body: %s)", path, repr(query))
+        logger.debug("GET request to %s (body: %s)", path, mask_sensitive_data(query))
         all_headers = headers + self.additional_headers + self._auth_headers
         response = self.http.get(path, all_headers, **query)
         return response
 
     @_authentication
     @_log_duration
     def post(self, path_segment, owner=None, app=None, sharing=None, headers=None, **query):
@@ -769,20 +797,15 @@
                    search='search * earliest=-1m | head 1')
         """
         if headers is None:
             headers = []
 
         path = self.authority + self._abspath(path_segment, owner=owner, app=app, sharing=sharing)
 
-        # To avoid writing sensitive data in debug logs
-        endpoint_having_sensitive_data = ["/storage/passwords"]
-        if any(endpoint in path for endpoint in endpoint_having_sensitive_data):
-            logger.debug("POST request to %s ", path)
-        else:
-            logger.debug("POST request to %s (body: %s)", path, repr(query))
+        logger.debug("POST request to %s (body: %s)", path, mask_sensitive_data(query))
         all_headers = headers + self.additional_headers + self._auth_headers
         response = self.http.post(path, all_headers, **query)
         return response
 
     @_authentication
     @_log_duration
     def request(self, path_segment, method="GET", headers=None, body={},
@@ -841,16 +864,15 @@
 
         path = self.authority \
             + self._abspath(path_segment, owner=owner,
                             app=app, sharing=sharing)
 
         all_headers = headers + self.additional_headers + self._auth_headers
         logger.debug("%s request to %s (headers: %s, body: %s)",
-                      method, path, str(all_headers), repr(body))
-
+                     method, path, str(mask_sensitive_data(dict(all_headers))), mask_sensitive_data(body))
         if body:
             body = _encode(**body)
 
             if method == "GET":
                 path = path + UrlEncoded('?' + body, skip_encode=True)
                 message = {'method': method,
                            'headers': all_headers}
```

### Comparing `splunk-sdk-1.7.3/splunklib/client.py` & `splunk-sdk-1.7.4/splunklib/client.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/data.py` & `splunk-sdk-1.7.4/splunklib/data.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/modularinput/argument.py` & `splunk-sdk-1.7.4/splunklib/modularinput/argument.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/modularinput/event.py` & `splunk-sdk-1.7.4/splunklib/modularinput/event.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/modularinput/event_writer.py` & `splunk-sdk-1.7.4/splunklib/modularinput/event_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def write_xml_document(self, document):
         """Writes a string representation of an
         ``ElementTree`` object to the output stream.
 
         :param document: An ``ElementTree`` object.
         """
-        self._out.write(ensure_str(ET.tostring(document)))
+        self._out.write(ensure_str(ET.tostring(document), errors="replace"))
         self._out.flush()
 
     def close(self):
         """Write the closing </stream> tag to make this XML well formed."""
         if self.header_written:
           self._out.write("</stream>")
         self._out.flush()
```

### Comparing `splunk-sdk-1.7.3/splunklib/modularinput/input_definition.py` & `splunk-sdk-1.7.4/splunklib/modularinput/input_definition.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/modularinput/scheme.py` & `splunk-sdk-1.7.4/splunklib/modularinput/scheme.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/modularinput/script.py` & `splunk-sdk-1.7.4/splunklib/modularinput/script.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/modularinput/utils.py` & `splunk-sdk-1.7.4/splunklib/modularinput/utils.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/modularinput/validation_definition.py` & `splunk-sdk-1.7.4/splunklib/modularinput/validation_definition.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/results.py` & `splunk-sdk-1.7.4/splunklib/results.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/__init__.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/decorators.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/decorators.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/environment.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/environment.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/eventing_command.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/eventing_command.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/external_search_command.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/external_search_command.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/generating_command.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/generating_command.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/internals.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/internals.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/reporting_command.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/reporting_command.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/search_command.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/search_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,15 +930,15 @@
         body = ""
         try:
             if body_length > 0:
                 body = istream.read(body_length)
         except Exception as error:
             raise RuntimeError('Failed to read body of length {}: {}'.format(body_length, error))
 
-        return metadata, six.ensure_str(body)
+        return metadata, six.ensure_str(body, errors="replace")
 
     _header = re.compile(r'chunked\s+1.0\s*,\s*(\d+)\s*,\s*(\d+)\s*\n')
 
     def _records_protocol_v1(self, ifile):
         return self._read_csv_records(ifile)
 
     def _read_csv_records(self, ifile):
```

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/streaming_command.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/streaming_command.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/searchcommands/validators.py` & `splunk-sdk-1.7.4/splunklib/searchcommands/validators.py`

 * *Files identical despite different names*

### Comparing `splunk-sdk-1.7.3/splunklib/six.py` & `splunk-sdk-1.7.4/splunklib/six.py`

 * *Files identical despite different names*

