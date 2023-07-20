# Comparing `tmp/devvio_util-1.6.0.tar.gz` & `tmp/devvio_util-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.6.0.tar", last modified: Mon Jul 10 19:55:49 2023, max compression
+gzip compressed data, was "devvio_util-1.6.1.tar", last modified: Thu Jul 20 15:18:06 2023, max compression
```

## Comparing `devvio_util-1.6.0.tar` & `devvio_util-1.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:49.550386 devvio_util-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 19:55:49.550386 devvio_util-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:42.000000 devvio_util-1.6.0/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:49.550386 devvio_util-1.6.0/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/lib_creds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:49.550386 devvio_util-1.6.0/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:49.550386 devvio_util-1.6.0/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 19:55:49.550386 devvio_util-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-10 19:55:42.000000 devvio_util-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:06.029855 devvio_util-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 15:18:06.029855 devvio_util-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:58.000000 devvio_util-1.6.1/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:06.029855 devvio_util-1.6.1/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/lib_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:06.029855 devvio_util-1.6.1/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:06.029855 devvio_util-1.6.1/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:05.000000 devvio_util-1.6.1/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 15:18:06.029855 devvio_util-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-20 15:17:58.000000 devvio_util-1.6.1/setup.py
```

### Comparing `devvio_util-1.6.0/devvio_util/config.py` & `devvio_util-1.6.1/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/lib_creds.py` & `devvio_util-1.6.1/devvio_util/lib_creds.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,18 +35,26 @@
         myconfig = self._credentials.get("AWS_REGION")
         return myconfig
 
     def get_aws_secret(self):
         myconfig = self._credentials.get("AWS_SECRET_ACCESS_KEY")
         return myconfig
 
-    def get_secrets(self, secret_name):
+    def get_secrets(self, secret_name):  # noqa: max-complexity: 13
         AWS_ACCESS_KEY_ID = self.get_aws_key()
+        if not AWS_ACCESS_KEY_ID:
+            raise Exception("AWS_ACCESS_KEY_ID not informed!")
+
         AWS_SECRET_ACCESS_KEY = self.get_aws_secret()
+        if not AWS_SECRET_ACCESS_KEY:
+            raise Exception("AWS_SECRET_ACCESS_KEY not informed!")
+
         AWS_REGION = self.get_aws_region()
+        if not AWS_REGION:
+            raise Exception("AWS_REGION not informed!")
 
         # Create a Secrets Manager client
         session = boto3.session.Session()
         client = session.client(
             service_name="secretsmanager",
             region_name=AWS_REGION,
             aws_access_key_id=AWS_ACCESS_KEY_ID,
@@ -57,34 +65,27 @@
         # See https://docs.aws.amazon.com/secretsmanager/latest/apireference/API_GetSecretValue.html
         # We rethrow the exception by default.
 
         try:
             get_secret_value_response = client.get_secret_value(SecretId=secret_name)
         except ClientError as e:
             if e.response["Error"]["Code"] == "DecryptionFailureException":
-                # Secrets Manager can't decrypt the protected secret text using the provided KMS key.
-                # Deal with the exception here, and/or rethrow at your discretion.
-                raise e
+                raise Exception("Secrets Manager can't decrypt the protected secret text using the provided KMS key")
             elif e.response["Error"]["Code"] == "InternalServiceErrorException":
-                # An error occurred on the server side.
-                # Deal with the exception here, and/or rethrow at your discretion.
-                raise e
+                raise Exception("An error occurred on the server side.")
             elif e.response["Error"]["Code"] == "InvalidParameterException":
-                # You provided an invalid value for a parameter.
-                # Deal with the exception here, and/or rethrow at your discretion.
-                raise e
+                raise Exception("You provided an invalid value for a parameter.")
             elif e.response["Error"]["Code"] == "InvalidRequestException":
-                # You provided a parameter value that is not valid for the current state of the resource.
-                # Deal with the exception here, and/or rethrow at your discretion.
-                raise e
+                raise Exception(
+                    "You provided a parameter value that is not valid for the current state of the resource.")
             elif e.response["Error"]["Code"] == "ResourceNotFoundException":
-                # We can't find the resource that you asked for.
-                # Deal with the exception here, and/or rethrow at your discretion.
-                raise e
-            return e
+                raise Exception("We can't find the resource that you asked for.")
+            elif e.response["Error"]["Code"] == "InvalidSignatureException":
+                raise Exception("You provided an invalid signature values.")
+            raise e
         else:
             # Decrypts secret using the associated KMS key.
             # Depending on whether the secret is a string or binary, one of these fields will be populated.
             if "SecretString" in get_secret_value_response:
                 secret = get_secret_value_response["SecretString"]
             else:
                 secret = base64.b64decode(get_secret_value_response["SecretBinary"])
```

### Comparing `devvio_util-1.6.0/devvio_util/logging.py` & `devvio_util-1.6.1/devvio_util/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 import logging.handlers
 import os
 import platform
 import threading
 from datetime import datetime as dt
 
+# Import necessary logging functions and variables
+from logging import *  # noqa
+
 
 class HostnameFilter(logging.Filter):
     """
     A logging filter that adds the hostname as an additional attribute to each log record.
     This class inherits from `logging.Filter` and is designed to be used with Python's logging module to filter
     log records based on the hostname where the program is running.
     hostname: The name of the host where the program is running.
```

### Comparing `devvio_util-1.6.0/devvio_util/primitives/address.py` & `devvio_util-1.6.1/devvio_util/primitives/address.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/chainstate.py` & `devvio_util-1.6.1/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/devv_constants.py` & `devvio_util-1.6.1/devvio_util/primitives/devv_constants.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/devv_sign.py` & `devvio_util-1.6.1/devvio_util/primitives/devv_sign.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/final_block.py` & `devvio_util-1.6.1/devvio_util/primitives/final_block.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/signature.py` & `devvio_util-1.6.1/devvio_util/primitives/signature.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/smart_coin.py` & `devvio_util-1.6.1/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/summary.py` & `devvio_util-1.6.1/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/transaction.py` & `devvio_util-1.6.1/devvio_util/primitives/transaction.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/transfer.py` & `devvio_util-1.6.1/devvio_util/primitives/transfer.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/utils.py` & `devvio_util-1.6.1/devvio_util/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/primitives/validation.py` & `devvio_util-1.6.1/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/devvio_util/psql_mixin.py` & `devvio_util-1.6.1/devvio_util/psql_mixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -112,13 +112,31 @@
         db_user = self._db_secrets.get("DEVV_DB_USER")
         db_pass = self._db_secrets.get("DEVV_DB_PASS")
         db_name = self._db_secrets.get("DEVV_DB_NAME")
         db_port = self._db_secrets.get("DEVV_DB_PORT")
         return db_host, db_user, db_pass, db_name, db_port
 
     def get_vault_cred(self):
-        vault_host = self._db_secrets.get("DEVV_VAULT_HOST")
-        vault_user = self._db_secrets.get("DEVV_VAULT_USER")
-        vault_pass = self._db_secrets.get("DEVV_VAULT_PASS")
-        vault_name = self._db_secrets.get("DEVV_VAULT_NAME")
-        vault_port = self._db_secrets.get("DEVV_VAULT_PORT")
+        try:
+            vault_host = self._db_secrets.get("DEVV_VAULT_HOST")
+            if not vault_host:
+                raise Exception("DEVV_VAULT_HOST is not defined")
+            vault_user = self._db_secrets.get("DEVV_VAULT_USER")
+            if not vault_user:
+                raise Exception("DEVV_VAULT_USER is not defined")
+            vault_pass = self._db_secrets.get("DEVV_VAULT_PASS")
+            if not vault_pass:
+                raise Exception("DEVV_VAULT_PASS is not defined")
+            vault_name = self._db_secrets.get("DEVV_VAULT_NAME")
+            if not vault_name:
+                raise Exception("DEVV_VAULT_NAME is not defined")
+            vault_port = self._db_secrets.get("DEVV_VAULT_PORT")
+            if not vault_port:
+                raise Exception("DEVV_VAULT_PORT is not defined")
+        except Exception as e:
+            self._logger.exception("Vault params not set, defaulting to cache DB.", e)
+            vault_host = self._db_secrets.get("DEVV_DB_HOST")
+            vault_user = self._db_secrets.get("DEVV_DB_USER")
+            vault_pass = self._db_secrets.get("DEVV_DB_PASS")
+            vault_name = self._db_secrets.get("DEVV_DB_NAME")
+            vault_port = self._db_secrets.get("DEVV_DB_PORT")
         return vault_host, vault_user, vault_pass, vault_name, vault_port
```

### Comparing `devvio_util-1.6.0/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.6.1/devvio_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.0/setup.py` & `devvio_util-1.6.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup
-VERSION = 'v1.6.0'
+VERSION = 'v1.6.1'
 
 setup(name='devvio_util',
       version=VERSION,
       long_description=open('README.txt').read(),
       long_description_content_type='text/markdown',
       description='Utility to be used inside Devvio projects',
       author='Devvio Team',
```

