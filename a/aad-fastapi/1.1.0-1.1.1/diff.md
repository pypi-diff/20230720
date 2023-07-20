# Comparing `tmp/aad_fastapi-1.1.0.tar.gz` & `tmp/aad_fastapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aad_fastapi-1.1.0.tar", last modified: Mon Apr  3 06:19:38 2023, max compression
+gzip compressed data, was "aad_fastapi-1.1.1.tar", last modified: Thu Jul 20 09:51:33 2023, max compression
```

## Comparing `aad_fastapi-1.1.0.tar` & `aad_fastapi-1.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:19:38.870163 aad_fastapi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-03 06:19:38.870163 aad_fastapi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:19:38.866163 aad_fastapi-1.1.0/aad_fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_auth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_bearer_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_discover_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/aad_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:19:38.866163 aad_fastapi-1.1.0/aad_fastapi/roles/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/roles/all_role_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/roles/any_role_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/roles/role_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/roles/role_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/aad_fastapi/roles/role_validator_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:19:38.866163 aad_fastapi-1.1.0/aad_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-03 06:19:38.000000 aad_fastapi-1.1.0/aad_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-03 06:19:38.000000 aad_fastapi-1.1.0/aad_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 06:19:38.000000 aad_fastapi-1.1.0/aad_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-03 06:19:38.000000 aad_fastapi-1.1.0/aad_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 06:19:38.000000 aad_fastapi-1.1.0/aad_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 06:19:38.870163 aad_fastapi-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:19:38.870163 aad_fastapi-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/test_aad_auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/test_aad_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/test_aad_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/test_authorize_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/test_oauth2_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-03 06:19:26.000000 aad_fastapi-1.1.0/tests/test_role_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:51:33.454457 aad_fastapi-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-20 09:51:33.454457 aad_fastapi-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:51:33.454457 aad_fastapi-1.1.1/aad_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_auth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_bearer_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_discover_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/aad_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:51:33.454457 aad_fastapi-1.1.1/aad_fastapi/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/roles/all_role_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/roles/any_role_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/roles/role_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/roles/role_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/aad_fastapi/roles/role_validator_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:51:33.454457 aad_fastapi-1.1.1/aad_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-20 09:51:33.000000 aad_fastapi-1.1.1/aad_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-20 09:51:33.000000 aad_fastapi-1.1.1/aad_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:51:33.000000 aad_fastapi-1.1.1/aad_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 09:51:33.000000 aad_fastapi-1.1.1/aad_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 09:51:33.000000 aad_fastapi-1.1.1/aad_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 09:51:33.458457 aad_fastapi-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:51:33.454457 aad_fastapi-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/test_aad_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/test_aad_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/test_aad_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/test_authorize_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/test_oauth2_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-20 09:51:20.000000 aad_fastapi-1.1.1/tests/test_role_validator.py
```

### Comparing `aad_fastapi-1.1.0/HISTORY.md` & `aad_fastapi-1.1.1/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Release: version ${TAG} ≡ƒÜÇ. [Dor Lugasi-Gal]
+- Added multidict. [Dor Lugasi-Gal]
+
+
+1.1.0 (2023-04-03)
+------------------
+- Release: version 1.1.0 🚀 [Dor Lugasi-Gal]
 - Added role_requirements.Any\All behaviour to the authorize decorator
   (#7) [Dor Lugasi-Gal]
 
   * added role_requirements.Any\All behavior to the authorized decorator
   * Added some docstrings
   * formatting
   * merge tests with parametrize
```

### Comparing `aad_fastapi-1.1.0/LICENSE` & `aad_fastapi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/PKG-INFO` & `aad_fastapi-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aad_fastapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: aad_fastapi middleware backend helper for bearer verification with FastAPI and Azure AD
 Home-page: https://github.com/Mimetis/aad_fastapi
 Author: Sébastien Pertus, Dor Lugasi-Gal
 Author-email: sebastien.pertus@gmail.com, dorlugasigal@gmail.com
 Project-URL: Homepage, https://github.com/Mimetis/aad_fastapi
 Project-URL: Bug Tracker, https://github.com/Mimetis/aad_fastapi/issues
 Keywords: python
```

### Comparing `aad_fastapi-1.1.0/README.md` & `aad_fastapi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/__init__.py` & `aad_fastapi-1.1.1/aad_fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/aad_auth_error.py` & `aad_fastapi-1.1.1/aad_fastapi/aad_auth_error.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/aad_bearer_backend.py` & `aad_fastapi-1.1.1/aad_fastapi/aad_bearer_backend.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/aad_decorators.py` & `aad_fastapi-1.1.1/aad_fastapi/aad_decorators.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/aad_helpers.py` & `aad_fastapi-1.1.1/aad_fastapi/aad_helpers.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/aad_options.py` & `aad_fastapi-1.1.1/aad_fastapi/aad_options.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/aad_token.py` & `aad_fastapi-1.1.1/aad_fastapi/aad_token.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/aad_user.py` & `aad_fastapi-1.1.1/aad_fastapi/aad_user.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/aad_vault.py` & `aad_fastapi-1.1.1/aad_fastapi/aad_vault.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi/roles/role_validator.py` & `aad_fastapi-1.1.1/aad_fastapi/roles/role_validator.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/aad_fastapi.egg-info/PKG-INFO` & `aad_fastapi-1.1.1/aad_fastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aad-fastapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: aad_fastapi middleware backend helper for bearer verification with FastAPI and Azure AD
 Home-page: https://github.com/Mimetis/aad_fastapi
 Author: Sébastien Pertus, Dor Lugasi-Gal
 Author-email: sebastien.pertus@gmail.com, dorlugasigal@gmail.com
 Project-URL: Homepage, https://github.com/Mimetis/aad_fastapi
 Project-URL: Bug Tracker, https://github.com/Mimetis/aad_fastapi/issues
 Keywords: python
```

### Comparing `aad_fastapi-1.1.0/aad_fastapi.egg-info/SOURCES.txt` & `aad_fastapi-1.1.1/aad_fastapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/setup.py` & `aad_fastapi-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/README.md` & `aad_fastapi-1.1.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/conftest.py` & `aad_fastapi-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/helpers.py` & `aad_fastapi-1.1.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/http_client.py` & `aad_fastapi-1.1.1/tests/http_client.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/test_aad_auth_token.py` & `aad_fastapi-1.1.1/tests/test_aad_auth_token.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/test_aad_helpers.py` & `aad_fastapi-1.1.1/tests/test_aad_helpers.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/test_aad_vault.py` & `aad_fastapi-1.1.1/tests/test_aad_vault.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/test_authorize_decorator.py` & `aad_fastapi-1.1.1/tests/test_authorize_decorator.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/test_oauth2_scheme.py` & `aad_fastapi-1.1.1/tests/test_oauth2_scheme.py`

 * *Files identical despite different names*

### Comparing `aad_fastapi-1.1.0/tests/test_role_validator.py` & `aad_fastapi-1.1.1/tests/test_role_validator.py`

 * *Files identical despite different names*

