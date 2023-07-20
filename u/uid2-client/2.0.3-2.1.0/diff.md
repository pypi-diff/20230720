# Comparing `tmp/uid2_client-2.0.3.tar.gz` & `tmp/uid2_client-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uid2_client-2.0.3.tar", last modified: Wed Jun 21 16:25:00 2023, max compression
+gzip compressed data, was "uid2_client-2.1.0.tar", last modified: Thu Jul 20 21:08:29 2023, max compression
```

## Comparing `uid2_client-2.0.3.tar` & `uid2_client-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:00.654642 uid2_client-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-21 16:24:53.000000 uid2_client-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-21 16:25:00.654642 uid2_client-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-21 16:24:53.000000 uid2_client-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-21 16:24:53.000000 uid2_client-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 16:25:00.654642 uid2_client-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 16:24:53.000000 uid2_client-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:00.650642 uid2_client-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-06-21 16:24:53.000000 uid2_client-2.0.3/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-21 16:24:53.000000 uid2_client-2.0.3/tests/test_key_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-21 16:24:53.000000 uid2_client-2.0.3/tests/test_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:00.654642 uid2_client-2.0.3/uid2_client/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/advertising_token_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/auto_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/identity_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/identity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-21 16:24:53.000000 uid2_client-2.0.3/uid2_client/uid2_base64_url_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:00.654642 uid2_client-2.0.3/uid2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:25:00.000000 uid2_client-2.0.3/uid2_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:08:29.198895 uid2_client-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-20 21:08:21.000000 uid2_client-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-20 21:08:29.198895 uid2_client-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-20 21:08:21.000000 uid2_client-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-20 21:08:21.000000 uid2_client-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-20 21:08:29.202895 uid2_client-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 21:08:21.000000 uid2_client-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:08:29.198895 uid2_client-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29296 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_key_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:08:29.198895 uid2_client-2.1.0/uid2_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/advertising_token_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/auto_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/euid_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/identity_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/identity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/request_response_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/uid2_base64_url_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/uid2_client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:08:29.198895 uid2_client-2.1.0/uid2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:08:28.000000 uid2_client-2.1.0/uid2_client.egg-info/zip-safe
```

### Comparing `uid2_client-2.0.3/LICENSE` & `uid2_client-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.3/PKG-INFO` & `uid2_client-2.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,77 @@
-Metadata-Version: 2.1
-Name: uid2_client
-Version: 2.0.3
-Summary: UID2 SDK for Python
-Home-page: https://iabtechlab.com
-Author: UID2 team
-Author-email: UID2 team <unifiedid-admin@thetradedesk.com>
-License: Apache 2.0
-Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
-Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
-Keywords: uid2
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # UID2 SDK for Python
 
 The UID 2 Project is subject to Tech Lab IPR’s Policy and is managed by the IAB Tech Lab Addressability Working Group and Privacy & Rearc Commit Group. Please review [the governance rules](https://github.com/IABTechLab/uid2-core/blob/master/Software%20Development%20and%20Release%20Procedures.md).
 
-This SDK simplifies integration with UID2 for those using Python.
+This document includes:
+* [Who Is this SDK for?](#who-is-this-sdk-for)
+* [Requirements](#requirements)
+* [Install](#install)
+* [Usage for DSPs](#usage-for-dsps)
+* [Usage for UID2 Sharers](#usage-for-uid2-sharers)
+* [Development](#development)
+  * [Example Usage](#example-usage)
+
+## Who Is this SDK for?
+
+This SDK simplifies integration with UID2 for DSPs and UID Sharers, as described in [UID2 Integration Guides](https://unifiedid.com/docs/category/integration-guides).
 
-## Dependencies
+## Requirements
 
 This SDK supports Python 3.6 and above.
 
-## Quick Start
+## Install
 
-Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
+The SDK can be installed using pip.
+```
+pip install uid2-client
+```
+
+## Usage for DSPs
 
+Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
+For examples of usage for DSPs, see [sample_client.py](examples/sample_client.py) and [sample_auto_refresh.py](examples/sample_auto_refresh.py)
 ```
-from uid2_client import Uid2Client, decrypt
+from uid2_client import Uid2ClientFactory
 
-client = Uid2Client('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
-keys = client.refresh_keys()
+# for UID2 (for EUID use EuidClientFactory)
+client = Uid2ClientFactory.create('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
+client.refresh_keys()
 advertising_token = 'AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A=='
-decrypted_token = decrypt(advertising_token, keys)
+decrypted_token = client.decrypt(advertising_token)
 print(decrypted_token.uid2)
 ```
 
-Additional examples are in the [examples] directory:
-* [sample_auto_refresh.py](examples/sample_auto_refresh.py)
-* [sample_client.py](examples/sample_client.py)
-  * Includes an example to encrypt a raw UID2 into an advertising token for UID2 sharing.
+## Usage for Sharers
+
+A UID2 sharer is a participant that wants to share UID2s or EUIDs with another participant. Raw UID2s must be encrypted into UID2 tokens before sending them to another participant. 
+For examples of usage, see [sample_sharing.py](examples/sample_sharing.py) and [sample_auto_refresh.py](examples/sample_auto_refresh.py)
+
+```
+from uid2_client import Uid2ClientFactory
+
+# for UID2 (for EUID use EuidClientFactory)
+client = Uid2ClientFactory.create('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
+client.refresh_keys()
+```
+Senders:
+
+1. Call the following:
+```
+encrypted = client.encrypt(raw_uid)
+ ```
+2. If encryption was successful, send the token `encrypted.uid2` to the receiver.
+
+Receivers:
+
+1. Call the following:
+```
+decrypted = client.decrypt(uid_token)
+```
+2. If decryption was successful, use the token `decrypted.uid2`.
 
 ## Development
 
 First, build the Docker image with Python 3.6 and all dev dependencies. This is required for all subsequent commands. Run the following:
 
 ```
 make docker
@@ -68,21 +91,22 @@
 
 Get access to an interactive shell within the Python 3.6 Docker image:
 
 ```
 make shell
 ```
 
-## Example Usage
+### Example Usage
 
 To run all the example applications:
 
 ```
 make examples BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
-	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
+	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A== \
+	RAW_UID=JCqmlLXpbbu/jTdpB2a1cNAVs8O72eMXPaQzC9Ic9mE=
 ```
 
 Alternatively, you can run specific examples:
 
 ```
 make example_client BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
```

### Comparing `uid2_client-2.0.3/pyproject.toml` & `uid2_client-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 40.9.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uid2_client"
-version = "2.0.3"
+version = "2.1.0"
 authors = [
     { name = "UID2 team", email = "unifiedid-admin@thetradedesk.com" }
 ]
 description = "UID2 SDK for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `uid2_client-2.0.3/setup.cfg` & `uid2_client-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.3/tests/test_encryption.py` & `uid2_client-2.1.0/tests/test_encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import base64
-import datetime as dt
-from datetime import timezone
 import unittest
 
 from tests.uid2_token_generator import UID2TokenGenerator, Params
 from uid2_client import *
+from uid2_client.encryption import _encrypt_token
 from uid2_client.identity_scope import IdentityScope
 from uid2_client.identity_type import IdentityType
 from uid2_client.keys import *
 
 _master_secret = bytes([139, 37, 241, 173, 18, 92, 36, 232, 165, 168, 23, 18, 38, 195, 123, 92, 160, 136, 185, 40, 91, 173, 165, 221, 168, 16, 169, 164, 38, 139, 8, 155])
 _site_secret =   bytes([32, 251, 7, 194, 132, 154, 250, 86, 202, 116, 104, 29, 131, 192, 139, 215, 48, 164, 11, 65, 226, 110, 167, 14, 108, 51, 254, 125, 65, 24, 23, 133])
 _master_key_id = 164
@@ -336,24 +334,26 @@
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys, now=expiry + dt.timedelta(seconds=1))
 
         result = decrypt(token, keys, now=expiry - dt.timedelta(seconds=1))
         self.assertEqual(_example_id, result.uid2)
 
-
     def test_smoke_token_v3(self):
         uid2 = _example_id
         identity_scope = IdentityScope.UID2
         now = dt.datetime.now(tz=timezone.utc)
 
         keys = EncryptionKeysCollection([_master_key, _site_key, _keyset_key], default_keyset_id=20,
                                         master_keyset_id=9999, caller_site_id=20)
 
-        result = encrypt(uid2, identity_scope, keys, now=now, ad_token_version=AdvertisingTokenVersion.ADVERTISING_TOKEN_V3)
+        result = _encrypt_token(uid2, identity_scope, _master_key, _site_key, _site_id, now=now,
+                                token_expiry=now + dt.timedelta(days=30) if keys.get_token_expiry_seconds() is None \
+                                    else now + dt.timedelta(seconds=int(keys.get_token_expiry_seconds())),
+                         ad_token_version=AdvertisingTokenVersion.ADVERTISING_TOKEN_V3)
         final = decrypt(result, keys, now=now)
 
         self.assertEqual(uid2, final.uid2)
 
     def test_smoke_token_v4(self):
         uid2 = _example_id
         identity_scope = IdentityScope.UID2
@@ -615,15 +615,15 @@
         keys = EncryptionKeysCollection([key])
         encrypted = UID2TokenGenerator.encrypt_data_v2(data, key=key, site_id=12345, now=now)
         decrypted = decrypt_data(encrypted, keys)
         self.assertEqual(data, decrypted.data)
         self.assertEqual(format_time(now), format_time(decrypted.encrypted_at))
 
 
-    # TODO - deduplicate the logic in sharing_test.py that has been copied from this file
+    # TODO - deduplicate the logic in test_sharing.py that has been copied from this file
     def test_raw_uid_produces_correct_identity_type_in_token(self):
         #v2 +12345678901. Although this was generated from a phone number, it's a v2 raw UID which doesn't encode this
         # information, so token assumes email by default.
         self.verify_identity_type("Q4bGug8t1xjsutKLCNjnb5fTlXSvIQukmahYDJeLBtk=",
                                                       IdentityType.Email.value)
         self.verify_identity_type("BEOGxroPLdcY7LrSiwjY52+X05V0ryELpJmoWAyXiwbZ",
                                                       IdentityType.Phone.value) #v3 +12345678901
```

### Comparing `uid2_client-2.0.3/tests/test_key_parse.py` & `uid2_client-2.1.0/tests/test_key_parse.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.3/tests/test_keys.py` & `uid2_client-2.1.0/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.3/uid2_client/auto_refresh.py` & `uid2_client-2.1.0/uid2_client/auto_refresh.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.3/uid2_client/encryption.py` & `uid2_client-2.1.0/uid2_client/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Internal module for keeping encryption/decryption logic.
 
 Do not use this module directly, import from uid2_client instead, e.g.
 >>> from uid2_client import decrypt
 """
 
-
 import base64
 import datetime as dt
 from datetime import timezone
 import os
 from Crypto.Cipher import AES
 from enum import Enum
 
@@ -25,16 +24,19 @@
 
 
 class _PayloadType(Enum):
     """Enum for types of payload that can be encoded in opaque strings"""
     ENCRYPTED_DATA = 128
     ENCRYPTED_DATA_V3 = 96
 
+
 base64_url_special_chars = {"-", "_"}
 
+
+# DEPRECATED, DO NOT CALL DIRECTLY. PLEASE USE Uid2Client's client.decrypt()
 def decrypt(token, keys, now=dt.datetime.now(tz=timezone.utc)):
     """Decrypt advertising token to extract UID2 details.
 
     Args:
         token (str): advertising token to decrypt
         keys (EncryptionKeysCollection): collection of keys to decrypt the token
         now (datetime): date/time to use as "now" when doing token expiration check
@@ -96,18 +98,18 @@
 
     identity_iv = master_payload[12:28]
     identity = _decrypt(master_payload[28:], identity_iv, site_key)
 
     site_id = int.from_bytes(identity[0:4], 'big')
 
     id_len = int.from_bytes(identity[4:8], 'big')
-    id_str = identity[8:8+id_len].decode('utf-8')
+    id_str = identity[8:8 + id_len].decode('utf-8')
 
     idx = 8 + id_len + 4
-    established_ms = int.from_bytes(identity[idx:idx+8], 'big')
+    established_ms = int.from_bytes(identity[idx:idx + 8], 'big')
     established = dt.datetime.fromtimestamp(established_ms / 1000.0, tz=timezone.utc)
 
     return DecryptedToken(id_str, established, site_id, site_key.site_id)
 
 
 def _decrypt_token_v3(token_bytes, keys, now):
     master_key_id = int.from_bytes(token_bytes[2:6], 'big')
@@ -153,71 +155,69 @@
     site_payload = bytearray(128)
     # Publisher Data
     site_payload[0:4] = int.to_bytes(site_id, byteorder='big', length=4)  # Site id
     site_payload[4:12] = int.to_bytes(0, byteorder='big', length=8)  # Publisher ID
     site_payload[12:16] = int.to_bytes(0, byteorder='big', length=4)  # Client Key ID
     # User Identity Data
     site_payload[16:20] = int.to_bytes(0, byteorder='big', length=4)  # Privacy Bits
-    site_payload[20:28] = int.to_bytes(int((now-dt.timedelta(hours=1)).timestamp())*1000, byteorder='big', length=8)  # Established
-    site_payload[28:36] = int.to_bytes(int(now.timestamp())*1000, byteorder='big', length=8)  # last refresh
+    site_payload[20:28] = int.to_bytes(int((now - dt.timedelta(hours=1)).timestamp()) * 1000, byteorder='big',
+                                       length=8)  # Established
+    site_payload[28:36] = int.to_bytes(int(now.timestamp()) * 1000, byteorder='big', length=8)  # last refresh
     site_payload[36:] = bytes(base64.b64decode(uid2))
 
     id_payload = _encrypt_gcm(bytes(site_payload), None, site_key.secret)
 
     # Operator Identity Data
     master_payload = bytearray(256)
-    master_payload[:8] = int.to_bytes(int(token_expiry.timestamp())*1000, byteorder='big', length=8)  # Expiry
+    master_payload[:8] = int.to_bytes(int(token_expiry.timestamp()) * 1000, byteorder='big', length=8)  # Expiry
     master_payload[8:16] = int.to_bytes(int(now.timestamp()), byteorder='big', length=8)  # Token Created
     master_payload[16:20] = int.to_bytes(0, byteorder='big', length=4)  # Site ID
     master_payload[20:21] = int.to_bytes(1, byteorder='big', length=1)  # Operator Type
     master_payload[21:25] = int.to_bytes(0, byteorder='big', length=4)  # Operator Version
     master_payload[25:29] = int.to_bytes(0, byteorder='big', length=4)  # Operator Key ID
-    master_payload[29:33] = int.to_bytes(site_key.key_id, byteorder='big', length=4) # Site Key ID
+    master_payload[29:33] = int.to_bytes(site_key.key_id, byteorder='big', length=4)  # Site Key ID
     master_payload[33:] = bytes(id_payload)
 
     encrypted_master_payload = _encrypt_gcm(bytes(master_payload), None, master_key.secret)
 
-    root_writer = bytearray(len(encrypted_master_payload)+6)
+    root_writer = bytearray(len(encrypted_master_payload) + 6)
     first_char = uid2[0]
     identity_type = IdentityType.Phone if first_char == 'F' or first_char == 'B' else IdentityType.Email
     root_writer[0:1] = int.to_bytes((int(identity_scope) << 4 | int(identity_type) << 2), byteorder='big', length=1)
-    root_writer[1:2] = int.to_bytes(ad_token_version, byteorder='big', length=1)
+    root_writer[1:2] = int.to_bytes(ad_token_version.value, byteorder='big', length=1)
     root_writer[2:6] = int.to_bytes(master_key.key_id, byteorder='big', length=4)
     root_writer[6:] = bytes(encrypted_master_payload)
 
     if ad_token_version == AdvertisingTokenVersion.ADVERTISING_TOKEN_V4:
         return Uid2Base64UrlCoder.encode(root_writer)
 
     return base64.b64encode(root_writer)
 
 
-
+# DEPRECATED, DO NOT CALL DIRECTLY. PLEASE USE Uid2Client's client.encrypt()
 def encrypt(uid2, identity_scope, keys, keyset_id=None, **kwargs):
     """ Encrypt an UID2 into a sharing token
 
     Args:
         uid2: the UID2 or EUID to be encrypted
         identity_scope (IdentityScope): indicates whether the output will be for UID2 or EUID
         keys (EncryptionKeysCollection): collection of keys to choose from for encryption
         keyset_id (int) : An optional keyset id to use for the encryption. Will use default keyset if left blank
 
     Keyword Args:
         now (Datetime): the datettime to use for now. Defaults to utc now
-        ad_token_version (AdvertisingTokenVersion): Defaults to v4
 
     Returns (str): Sharing Token
 
     """
     now = kwargs.get("now")
     if now is None:
         now = dt.datetime.now(tz=timezone.utc)
 
-    ad_token_version = kwargs.get("ad_token_version")
-    if ad_token_version is None:
-        ad_token_version = AdvertisingTokenVersion.ADVERTISING_TOKEN_V4
+    ad_token_version = AdvertisingTokenVersion.ADVERTISING_TOKEN_V4
 
     key = keys.get_default_keyset_key(now) if keyset_id is None else keys.get_by_keyset_key(keyset_id, now)
     master_key = keys.get_by_keyset_key(keys.get_master_keyset_id(), now)
 
     token_expiry = now + dt.timedelta(days=30) if keys.get_token_expiry_seconds() is None \
         else now + dt.timedelta(seconds=int(keys.get_token_expiry_seconds()))
 
@@ -245,15 +245,15 @@
     Keyword Args:
         key (EncryptionKey): key to encrypt the data with; if this is specified,
                              you should not specify keys, site_id, or advertising_token
         keys (EncryptionKeysCollection): collection of keys to choose the encryption
                                          key from; the key will be selected using site_id
         site_id (int): ID of the site for which the encryption key is to be used;
                        the key will be looked up from the keys collection;
-                       if this is specified, you can't specificy advertising_token
+                       if this is specified, you can't specify advertising_token
         advertising_token (str): token to decrypt in order to obtain the site_id
         now (datetime): date/time to use as "now" for checking whether advertising_token
                         or site encryption key have expired (default: UTC now) as well as
                         for timestamp of the encrypted data
         iv (bytes): custom initialization vector for the encryption; if not specified,
                     the function will generate one using urandom
 
@@ -384,15 +384,15 @@
     # site id 8:12
 
     return DecryptedData(payload[12:], encrypted_at)
 
 
 def _add_pkcs7_padding(data, block_size):
     pad_len = block_size - (len(data) % block_size)
-    return data + bytes([pad_len])*pad_len
+    return data + bytes([pad_len]) * pad_len
 
 
 def _encrypt(data, iv, key):
     cipher = AES.new(key.secret, AES.MODE_CBC, IV=iv)
     return cipher.encrypt(_add_pkcs7_padding(data, AES.block_size))
 
 
@@ -428,24 +428,26 @@
 
     Attrs:
         uid2 (str): universal ID string
         established (datetime): UTC date/time for when the token was first generated
         site_id (int): site ID which the token is originating from
         site_key_site_id (int): site ID of the site key which the token is encrypted with
     """
+
     def __init__(self, uid2, established, site_id, site_key_site_id):
         self.uid2 = uid2
         self.established = established
         self.site_id = site_id
         self.site_key_site_id = site_key_site_id
 
 
 class DecryptedData:
     """Details extracted from the encrypted data string.
 
     Attrs:
         data (bytes): data decrypted from the string
         encrypted_at (datetime): UTC date/time for when the data was encrypted
     """
+
     def __init__(self, data, encrypted_at):
         self.data = data
         self.encrypted_at = encrypted_at
```

### Comparing `uid2_client-2.0.3/uid2_client/keys.py` & `uid2_client-2.1.0/uid2_client/keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.3/uid2_client/uid2_base64_url_coder.py` & `uid2_client-2.1.0/uid2_client/uid2_base64_url_coder.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.3/uid2_client.egg-info/PKG-INFO` & `uid2_client-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uid2-client
-Version: 2.0.3
+Name: uid2_client
+Version: 2.1.0
 Summary: UID2 SDK for Python
 Home-page: https://iabtechlab.com
 Author: UID2 team
 Author-email: UID2 team <unifiedid-admin@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
@@ -17,38 +17,80 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UID2 SDK for Python
 
 The UID 2 Project is subject to Tech Lab IPR’s Policy and is managed by the IAB Tech Lab Addressability Working Group and Privacy & Rearc Commit Group. Please review [the governance rules](https://github.com/IABTechLab/uid2-core/blob/master/Software%20Development%20and%20Release%20Procedures.md).
 
-This SDK simplifies integration with UID2 for those using Python.
+This document includes:
+* [Who Is this SDK for?](#who-is-this-sdk-for)
+* [Requirements](#requirements)
+* [Install](#install)
+* [Usage for DSPs](#usage-for-dsps)
+* [Usage for UID2 Sharers](#usage-for-uid2-sharers)
+* [Development](#development)
+  * [Example Usage](#example-usage)
 
-## Dependencies
+## Who Is this SDK for?
+
+This SDK simplifies integration with UID2 for DSPs and UID Sharers, as described in [UID2 Integration Guides](https://unifiedid.com/docs/category/integration-guides).
+
+## Requirements
 
 This SDK supports Python 3.6 and above.
 
-## Quick Start
+## Install
 
-Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
+The SDK can be installed using pip.
+```
+pip install uid2-client
+```
 
+## Usage for DSPs
+
+Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
+For examples of usage for DSPs, see [sample_client.py](examples/sample_client.py) and [sample_auto_refresh.py](examples/sample_auto_refresh.py)
 ```
-from uid2_client import Uid2Client, decrypt
+from uid2_client import Uid2ClientFactory
 
-client = Uid2Client('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
-keys = client.refresh_keys()
+# for UID2 (for EUID use EuidClientFactory)
+client = Uid2ClientFactory.create('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
+client.refresh_keys()
 advertising_token = 'AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A=='
-decrypted_token = decrypt(advertising_token, keys)
+decrypted_token = client.decrypt(advertising_token)
 print(decrypted_token.uid2)
 ```
 
-Additional examples are in the [examples] directory:
-* [sample_auto_refresh.py](examples/sample_auto_refresh.py)
-* [sample_client.py](examples/sample_client.py)
-  * Includes an example to encrypt a raw UID2 into an advertising token for UID2 sharing.
+## Usage for Sharers
+
+A UID2 sharer is a participant that wants to share UID2s or EUIDs with another participant. Raw UID2s must be encrypted into UID2 tokens before sending them to another participant. 
+For examples of usage, see [sample_sharing.py](examples/sample_sharing.py) and [sample_auto_refresh.py](examples/sample_auto_refresh.py)
+
+```
+from uid2_client import Uid2ClientFactory
+
+# for UID2 (for EUID use EuidClientFactory)
+client = Uid2ClientFactory.create('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
+client.refresh_keys()
+```
+Senders:
+
+1. Call the following:
+```
+encrypted = client.encrypt(raw_uid)
+ ```
+2. If encryption was successful, send the token `encrypted.uid2` to the receiver.
+
+Receivers:
+
+1. Call the following:
+```
+decrypted = client.decrypt(uid_token)
+```
+2. If decryption was successful, use the token `decrypted.uid2`.
 
 ## Development
 
 First, build the Docker image with Python 3.6 and all dev dependencies. This is required for all subsequent commands. Run the following:
 
 ```
 make docker
@@ -68,21 +110,22 @@
 
 Get access to an interactive shell within the Python 3.6 Docker image:
 
 ```
 make shell
 ```
 
-## Example Usage
+### Example Usage
 
 To run all the example applications:
 
 ```
 make examples BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
-	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
+	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A== \
+	RAW_UID=JCqmlLXpbbu/jTdpB2a1cNAVs8O72eMXPaQzC9Ic9mE=
 ```
 
 Alternatively, you can run specific examples:
 
 ```
 make example_client BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
```

### Comparing `uid2_client-2.0.3/uid2_client.egg-info/SOURCES.txt` & `uid2_client-2.1.0/uid2_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+tests/test_client.py
 tests/test_encryption.py
 tests/test_key_parse.py
 tests/test_keys.py
+tests/test_sharing.py
+tests/test_utils.py
 uid2_client/__init__.py
 uid2_client/advertising_token_version.py
 uid2_client/auto_refresh.py
 uid2_client/client.py
 uid2_client/encryption.py
+uid2_client/euid_client_factory.py
 uid2_client/identity_scope.py
 uid2_client/identity_type.py
 uid2_client/keys.py
+uid2_client/request_response_util.py
 uid2_client/uid2_base64_url_coder.py
+uid2_client/uid2_client_factory.py
 uid2_client.egg-info/PKG-INFO
 uid2_client.egg-info/SOURCES.txt
 uid2_client.egg-info/dependency_links.txt
 uid2_client.egg-info/requires.txt
 uid2_client.egg-info/top_level.txt
 uid2_client.egg-info/zip-safe
```

