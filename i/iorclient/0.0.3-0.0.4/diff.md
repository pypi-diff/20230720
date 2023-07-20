# Comparing `tmp/iorclient-0.0.3.tar.gz` & `tmp/iorclient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iorclient-0.0.3.tar", last modified: Wed Jul 19 05:43:38 2023, max compression
+gzip compressed data, was "iorclient-0.0.4.tar", last modified: Thu Jul 20 09:00:50 2023, max compression
```

## Comparing `iorclient-0.0.3.tar` & `iorclient-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 05:43:38.598982 iorclient-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 iorclient-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 iorclient-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      965 2023-07-19 05:43:38.598982 iorclient-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 05:43:38.576673 iorclient-0.0.3/ior/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 iorclient-0.0.3/ior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:43:38.585686 iorclient-0.0.3/ior/client/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 iorclient-0.0.3/ior/client/__init__.py
--rw-rw-rw-   0        0        0    11457 2023-07-19 05:12:47.000000 iorclient-0.0.3/ior/client/certificate_service.py
--rw-rw-rw-   0        0        0     4903 2023-07-19 05:13:21.000000 iorclient-0.0.3/ior/client/contract_template_service.py
--rw-rw-rw-   0        0        0     2539 2023-07-19 05:14:32.000000 iorclient-0.0.3/ior/client/exchange_service.py
--rw-rw-rw-   0        0        0     5095 2023-07-19 05:14:41.000000 iorclient-0.0.3/ior/client/permission_control_service.py
--rw-rw-rw-   0        0        0     5816 2023-07-19 05:30:38.000000 iorclient-0.0.3/ior/client/role_control_service.py
--rw-rw-rw-   0        0        0     5430 2023-07-19 05:15:05.000000 iorclient-0.0.3/ior/client/template_control_service.py
--rw-rw-rw-   0        0        0     2379 2023-07-19 04:47:03.000000 iorclient-0.0.3/ior/iorsdk.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:43:38.589017 iorclient-0.0.3/ior/util/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 iorclient-0.0.3/ior/util/__init__.py
--rw-rw-rw-   0        0        0     1490 2023-07-19 04:30:56.000000 iorclient-0.0.3/ior/util/result_utils.py
--rw-rw-rw-   0        0        0     4047 2023-07-17 18:09:55.000000 iorclient-0.0.3/ior/util/web3_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:43:38.592993 iorclient-0.0.3/iorclient.egg-info/
--rw-rw-rw-   0        0        0      965 2023-07-19 05:43:38.000000 iorclient-0.0.3/iorclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-07-19 05:43:38.000000 iorclient-0.0.3/iorclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 05:43:38.000000 iorclient-0.0.3/iorclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-19 05:43:38.000000 iorclient-0.0.3/iorclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 05:43:38.599849 iorclient-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-07-19 05:40:03.000000 iorclient-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:43:38.596774 iorclient-0.0.3/test/
--rw-rw-rw-   0        0        0        0 2023-07-17 16:15:26.000000 iorclient-0.0.3/test/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-07-19 05:24:41.000000 iorclient-0.0.3/test/test_cert.py
--rw-rw-rw-   0        0        0     3418 2023-07-19 05:37:19.000000 iorclient-0.0.3/test/test_role.py
--rw-rw-rw-   0        0        0     2334 2023-07-19 05:22:40.000000 iorclient-0.0.3/test/test_template.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:00:50.000031 iorclient-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 iorclient-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 iorclient-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      965 2023-07-20 09:00:49.998593 iorclient-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.963274 iorclient-0.0.4/ior/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 iorclient-0.0.4/ior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.976379 iorclient-0.0.4/ior/client/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 iorclient-0.0.4/ior/client/__init__.py
+-rw-rw-rw-   0        0        0    12857 2023-07-19 16:53:06.000000 iorclient-0.0.4/ior/client/certificate_service.py
+-rw-rw-rw-   0        0        0     5302 2023-07-20 08:17:33.000000 iorclient-0.0.4/ior/client/contract_template_service.py
+-rw-rw-rw-   0        0        0     2539 2023-07-19 05:14:32.000000 iorclient-0.0.4/ior/client/exchange_service.py
+-rw-rw-rw-   0        0        0     5056 2023-07-20 08:26:51.000000 iorclient-0.0.4/ior/client/permission_control_service.py
+-rw-rw-rw-   0        0        0     5816 2023-07-19 05:30:38.000000 iorclient-0.0.4/ior/client/role_control_service.py
+-rw-rw-rw-   0        0        0     5430 2023-07-19 05:15:05.000000 iorclient-0.0.4/ior/client/template_control_service.py
+-rw-rw-rw-   0        0        0     2379 2023-07-19 04:47:03.000000 iorclient-0.0.4/ior/iorsdk.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.981241 iorclient-0.0.4/ior/util/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 iorclient-0.0.4/ior/util/__init__.py
+-rw-rw-rw-   0        0        0     1490 2023-07-19 15:12:23.000000 iorclient-0.0.4/ior/util/result_utils.py
+-rw-rw-rw-   0        0        0     4047 2023-07-17 18:09:55.000000 iorclient-0.0.4/ior/util/web3_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.988947 iorclient-0.0.4/iorclient.egg-info/
+-rw-rw-rw-   0        0        0      965 2023-07-20 09:00:49.000000 iorclient-0.0.4/iorclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-07-20 09:00:49.000000 iorclient-0.0.4/iorclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 09:00:49.000000 iorclient-0.0.4/iorclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 09:00:49.000000 iorclient-0.0.4/iorclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 09:00:50.000031 iorclient-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-07-20 09:00:43.000000 iorclient-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.997492 iorclient-0.0.4/test/
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:15:26.000000 iorclient-0.0.4/test/__init__.py
+-rw-rw-rw-   0        0        0     2043 2023-07-19 16:51:38.000000 iorclient-0.0.4/test/test_cert.py
+-rw-rw-rw-   0        0        0     3809 2023-07-20 08:37:15.000000 iorclient-0.0.4/test/test_role.py
+-rw-rw-rw-   0        0        0     2832 2023-07-20 08:25:12.000000 iorclient-0.0.4/test/test_template.py
```

### Comparing `iorclient-0.0.3/LICENSE` & `iorclient-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.3/PKG-INFO` & `iorclient-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iorclient
-Version: 0.0.3
+Version: 0.0.4
 Summary: ior client sdk for ior standard
 Home-page: https://github.com/tzspace-ior/iorclient
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iorclient-0.0.3/ior/client/certificate_service.py` & `iorclient-0.0.4/ior/client/certificate_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,26 @@
     def __init__(self):
         None
 
     def set_api_client(self, server_url, client):
         self._api = RestAPI(api_url=server_url+"/certificate" ,driver=client)
         endpoints = [
             Endpoint(name="address",path="/get_address",method=HTTPMethod.POST),
-            Endpoint(name="tokens",path="/get_tokenById",method=HTTPMethod.POST),
+            Endpoint(name="pretokens",path="/get_preTokenById",method=HTTPMethod.POST),
             Endpoint(name="recreations",path="/get_recreationById",method=HTTPMethod.POST),
             Endpoint(name="isApproved",path="/is_authorizeApproved",method=HTTPMethod.POST),
             Endpoint(name="tokenUri",path="/get_tokenUri",method=HTTPMethod.POST),
+            Endpoint(name="verifyOwner",path="/verify_owner",method=HTTPMethod.POST),
+            Endpoint(name="verifyHash",path="/verify_hash",method=HTTPMethod.POST),
+            Endpoint(name="updateHash",path="/estimate_updateHash_forReceipt",method=HTTPMethod.POST),
+            Endpoint(name="updateBaseUri",path="/estimate_updateBaseUri_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="setAuthorizeApproval",path="/estimate_setAuthorizeApproval_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="bindOption",path="/estimate_bindOption_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="setApproveForAll",path="/estimate_setApproveForAll_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="approve",path="/estimate_approve_forReceipt",method=HTTPMethod.POST),
-            Endpoint(name="updateTokenIdMapping",path="/prepare_updateTokenIdMapping_forResult",method=HTTPMethod.POST),
             Endpoint(name="recreateCrossChain",path="/prepare_recreateCrossChain_forResult",method=HTTPMethod.POST),
             Endpoint(name="recreateInChain",path="/prepare_recreateInChain_forResult",method=HTTPMethod.POST),
             Endpoint(name="recreate",path="/prepare_recreate_forResult",method=HTTPMethod.POST),
             Endpoint(name="authorizeOption",path="/prepare_authorizeOption_forResult",method=HTTPMethod.POST),
             Endpoint(name="createOption",path="/prepare_createOption_forResult",method=HTTPMethod.POST),
             Endpoint(name="authorize",path="/prepare_authorize_forResult",method=HTTPMethod.POST),
             Endpoint(name="safeTransferFrom",path="/prepare_safeTransferFrom_forResult",method=HTTPMethod.POST),
@@ -42,16 +45,16 @@
         res = self._api.call_endpoint("address",data=
             {
                 'name': service_name
             })
         return res['data']
 
     @error_handler
-    def tokens(self, service_name, _certId):
-        res = self._api.call_endpoint("tokens",data=
+    def pretokens(self, service_name, _certId):
+        res = self._api.call_endpoint("pretokens",data=
             {
                 'name': service_name, 
                 'certId': _certId
             })
         return res['data']
 
     @error_handler
@@ -79,14 +82,64 @@
             {
                 'name': service_name, 
                 'certId': _certId, 
                 'sender': pub
             })
         return res['data']
 
+    @error_handler
+    def verify_owner(self, service_name, _certId, _to):
+        res = self._api.call_endpoint("verifyOwner",data=
+            {
+                'name': service_name, 
+                'certId': _certId, 
+                'to': _to
+            })
+        return res['data']
+
+
+    @error_handler
+    def verify_hash(self, service_name, _certId, _hash):
+        res = self._api.call_endpoint("verifyHash",data=
+            {
+                'name': service_name, 
+                'certId': _certId, 
+                'hash': _hash
+            })
+        return res['data']
+
+    @two_ret_error_handler
+    def update_hash(self, service_name, pub, sign_func,  _certId,_hash):
+        res = self._api.call_endpoint("updateHash",data=
+            {
+                'name': service_name, 
+                'certId': _certId, 
+                'hash': _hash, 
+                'sender': pub
+            })
+        tx = res['data']['transaction']
+
+        raw = sign_func(pub, tx)
+        result = self._api.call_endpoint("tryForReceipt",data={'name': service_name, 'tx': raw})
+        return result['data']['code'],result['data']['receipt']
+
+    @two_ret_error_handler
+    def update_base_uri(self, service_name, pub, sign_func,  _uri):
+        res = self._api.call_endpoint("updateBaseUri",data=
+            {
+                'name': service_name, 
+                'uri': _uri, 
+                'sender': pub
+            })
+        tx = res['data']['transaction']
+
+        raw = sign_func(pub, tx)
+        result = self._api.call_endpoint("tryForReceipt",data={'name': service_name, 'tx': raw})
+        return result['data']['code'],result['data']['receipt']
+
     @two_ret_error_handler
     def set_authorize_approval(self, service_name, pub, sign_func,  _certId,_to,_approved):
         res = self._api.call_endpoint("setAuthorizeApproval",data=
             {
                 'name': service_name, 
                 'certId': _certId, 
                 'to': _to, 
@@ -138,30 +191,14 @@
                 'sender': pub
             })
         tx = res['data']['transaction']
 
         raw = sign_func(pub, tx)
         result = self._api.call_endpoint("tryForResult",data={'name': service_name, 'tx': raw})
         res = result['data']['res']
-        return res
-
-    @error_handler
-    def update_token_id_mapping(self, service_name, pub, sign_func,  _certId,_original):
-        res = self._api.call_endpoint("updateTokenIdMapping",data=
-            {
-                'name': service_name, 
-                'certId': _certId, 
-                'original': _original, 
-                'sender': pub
-            })
-        tx = res['data']['transaction']
-
-        raw = sign_func(pub, tx)
-        result = self._api.call_endpoint("tryForResult",data={'name': service_name, 'tx': raw})
-        res = result['data']['res']
         return res
 
     @error_handler
     def recreate_cross_chain(self, service_name, pub, sign_func,   _to,_chains,_certs,_certIds):
         res = self._api.call_endpoint("recreateCrossChain",data=
             {
                 'name': service_name,
```

### Comparing `iorclient-0.0.3/ior/client/contract_template_service.py` & `iorclient-0.0.4/ior/client/contract_template_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     def __init__(self):
         None
 
     def set_api_client(self, server_url, client):
         self._api = RestAPI(api_url=server_url+"/contract/template" ,driver=client)
         endpoints = [
             Endpoint(name="address",path="/get_address",method=HTTPMethod.POST),
+            Endpoint(name="verifyHash",path="/verify_hash",method=HTTPMethod.POST),
             Endpoint(name="canPay",path="/can_pay",method=HTTPMethod.POST),
             Endpoint(name="getPayees",path="/get_payees",method=HTTPMethod.POST),
             Endpoint(name="getRatioByPayee",path="/get_ratioByPayee",method=HTTPMethod.POST),
             Endpoint(name="init",path="/estimate_init_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="sign",path="/prepare_sign_forSign",method=HTTPMethod.POST),
             Endpoint(name="start",path="/prepare_start_forState",method=HTTPMethod.POST),
             Endpoint(name="end",path="/prepare_end_forState",method=HTTPMethod.POST),
@@ -33,18 +34,28 @@
         res = self._api.call_endpoint("address",data=
             {
                 'name': service_name
             })
         return res['data']
 
     @error_handler
+    def verify_hash(self, service_name, _instanceId, _hash):
+        res = self._api.call_endpoint("verifyHash",data=
+            {
+                'name': service_name,
+                'instanceId': _instanceId,
+                'hash': _hash
+            })
+        return res['data']
+
+    @error_handler
     def can_pay(self, service_name, _instanceId, _payerAddress):
         res = self._api.call_endpoint("canPay",data=
             {
-                'name': service_name, 
+                'name': service_name,
                 'instanceId': _instanceId,
                 'payerAddress': _payerAddress
             })
         return res['data']
 
     @error_handler
     def get_payees(self, service_name, _instanceId):
```

### Comparing `iorclient-0.0.3/ior/client/exchange_service.py` & `iorclient-0.0.4/ior/client/exchange_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.3/ior/client/permission_control_service.py` & `iorclient-0.0.4/ior/client/permission_control_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,18 @@
                 'name': service_name, 
                 'role': _role, 
                 'to': _to
             })
         return res['data']
 
     @error_handler
-    def has_permission(self, service_name,  _role, _permission, _data, _operation):
+    def has_permission(self, service_name,  _permission, _data, _operation):
         res = self._api.call_endpoint("hasPermission",data=
             {
                 'name': service_name, 
-                'role': _role,
                 'permission': _permission, 
                 'data': _data, 
                 'operation': _operation
             })
         return res['data']
 
     @error_handler
```

### Comparing `iorclient-0.0.3/ior/client/role_control_service.py` & `iorclient-0.0.4/ior/client/role_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.3/ior/client/template_control_service.py` & `iorclient-0.0.4/ior/client/template_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.3/ior/iorsdk.py` & `iorclient-0.0.4/ior/iorsdk.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.3/ior/util/result_utils.py` & `iorclient-0.0.4/ior/util/result_utils.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.3/ior/util/web3_utils.py` & `iorclient-0.0.4/ior/util/web3_utils.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.3/iorclient.egg-info/PKG-INFO` & `iorclient-0.0.4/iorclient.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iorclient
-Version: 0.0.3
+Version: 0.0.4
 Summary: ior client sdk for ior standard
 Home-page: https://github.com/tzspace-ior/iorclient
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iorclient-0.0.3/iorclient.egg-info/SOURCES.txt` & `iorclient-0.0.4/iorclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.3/setup.py` & `iorclient-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.MD", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="iorclient",
-  version="0.0.3",
+  version="0.0.4",
   author="Jie Guan",
   author_email="jguanisme@163.com",
   description="ior client sdk for ior standard",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/tzspace-ior/iorclient",
   packages=setuptools.find_packages(),
```

### Comparing `iorclient-0.0.3/test/test_cert.py` & `iorclient-0.0.4/test/test_cert.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ior.iorsdk import IORClient
+from ior.util.web3_utils import keccak256
 import unittest
 
 class TestCertMethods(unittest.TestCase):
     def setUp(self):
         #main test for example        
         self.ior = IORClient("http://127.0.0.1:5000/v1/api")
         self.ior.init_w3()
@@ -23,27 +24,36 @@
         def sign_tx(pub,tx):
             stx = self.ior.sign_transaction(tx,self.pks[pub])
             return stx.rawTransaction.hex()
 
         pub = self.pubs[0]
         cert = self.ior.get('cert')
 
-        _,certId = cert.mint('stcc',pub,sign_tx, pub)
-        print(certId)
-
-        ret,_,_ = cert.set_authorize_approval('stcc',pub,sign_tx, certId,self.pubs[1],True)
-        print(ret)
-        _,ret = cert.is_authorize_approved('stcc', certId,self.pubs[1])
-        print(ret)
-        _,ret = cert.tokens('stcc',certId)
-        print(ret)
-        _,nId = cert.authorize('stcc',self.pubs[1],sign_tx, self.pubs[2],certId)
+        ret,certId = cert.mint('stcc',pub,sign_tx, pub)
+        print('mint',ret,certId)
+        
+        hashValue = keccak256('cert').hex()
+        ret,res,receipt = cert.update_hash('stcc',pub,sign_tx, certId,hashValue)
+        print('update_hash',res)
+
+        hashValue = keccak256('cert2').hex()
+        ret,res = cert.verify_hash('stcc',certId,hashValue)
+        print('verify_hash',res)
+
+        ret,res = cert.pretokens('stcc',certId)
+        print('pretokens',res)
+
+        ret,res,receipt = cert.set_authorize_approval('stcc',pub,sign_tx, certId,self.pubs[1],True)
+        print(res)
+        ret,res = cert.is_authorize_approved('stcc', certId,self.pubs[1])
+        print(res)
+        ret,nId = cert.authorize('stcc',self.pubs[1],sign_tx, self.pubs[2],certId)
         print(nId)
-        _,nxId = cert.tokens('stcc',nId)
-        print(nxId)
-        _,ret = cert.safe_transfer_from('stcc',self.pubs[2],sign_tx, self.pubs[2],self.pubs[3],nId)
-        print(ret)
+        ret,nxId = cert.pretokens('stcc',nId)
+        print('pretokens',nxId)
+        ret,res = cert.safe_transfer_from('stcc',self.pubs[2],sign_tx, self.pubs[2],self.pubs[3],nId)
+        print(res)
 
 
  
 if __name__=='__main__':
     unittest.main()
```

### Comparing `iorclient-0.0.3/test/test_role.py` & `iorclient-0.0.4/test/test_role.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ior.iorsdk import IORClient
+from ior.util.web3_utils import keccak256
 import unittest
 
 class TestRoleMethods(unittest.TestCase):
     def setUp(self):
         #main test for example        
         self.ior = IORClient("http://127.0.0.1:5000/v1/api")
         self.ior.init_w3()
@@ -30,65 +31,66 @@
 
         permission = "AddData"
         permissions = [permission]
         roleName = "Role1"
         adminRoleName = "AdminRole"
         permissionRoleName = "PermissionRole"
 
-        _,addr = pctrl.address('permission')
-        print(addr)
+        ret,addr = pctrl.address('pctrl')
         permissionContractAddrs = [addr]
 
         #只需要添加一次
-        #rolectrl.add_role('role',pub,sign_tx, roleName,adminRoleName,permissionRoleName,permissions,permissionContractAddrs)
-        
-
-        ret,_,_=rolectrl.grant_role('role',pub,sign_tx, adminRoleName,self.pubs[1])
-
-        ret,_,_=rolectrl.grant_role('role',self.pubs[1],sign_tx, permissionRoleName,self.pubs[2])
-        
-        ret,_,_ = rolectrl.grant_role('role',self.pubs[1],sign_tx, roleName,self.pubs[3])
-        print('grant all roles')
+        ret,res,receipt = rolectrl.add_role('rolectrl',pub,sign_tx, roleName,adminRoleName,permissionRoleName,permissions,permissionContractAddrs)
+        print('add_role', res)
+        ret,res = rolectrl.roles('rolectrl', keccak256(roleName).hex())
+        print('roles', res)
+        ret,res,receipt = rolectrl.grant_role('rolectrl',pub,sign_tx, adminRoleName,self.pubs[1])
+        ret,res,receipt = rolectrl.grant_role('rolectrl',self.pubs[1],sign_tx, permissionRoleName,self.pubs[2])
+        ret,res,receipt = rolectrl.grant_role('rolectrl',self.pubs[1],sign_tx, roleName,self.pubs[3])
+        print('grant all roles',res)
         permissionAdmin = "AdminRole"
-        ret,_,_ = pctrl.grant_role('permission',pub,sign_tx, permissionAdmin,self.pubs[2])
-        print('grant first permission',ret)
+        ret,res,receipt = pctrl.grant_role('pctrl',pub,sign_tx, permissionAdmin,self.pubs[2])
+        print('grant first permission',res)
 
         permissionAdmin2 = "AdminRole2"
-        ret,_,_ = pctrl.grant_role('permission',pub,sign_tx, permissionAdmin2,self.pubs[2])
+        ret,res,receipt = pctrl.grant_role('pctrl',pub,sign_tx, permissionAdmin2,self.pubs[2])
         print('grant all permission',ret)
 
-        ret,_,_ = rolectrl.add_permission('role',self.pubs[2],sign_tx, roleName,permissions,permissionContractAddrs)
+        ret,res,receipt = rolectrl.add_permission('rolectrl',self.pubs[2],sign_tx, roleName,permissions,permissionContractAddrs)
         
         #read 0x01, write 0x02, read and write 0x03
         data = ["username","idcard"]
         operations = [0x02,0x03]
         defaultOperations = [0x01,0x02]
         parent = ["1.2.121.1.3.21.2","1.2.121.1.3.21.2"]
         dhash = data;
 
-        ret,_,_ = pctrl.add_permission('permission',self.pubs[2],sign_tx, permission,data,operations,defaultOperations,parent,dhash)
+        ret,res,receipt = pctrl.add_permission('pctrl',self.pubs[2],sign_tx, permission,data,operations,defaultOperations,parent,dhash)
        
         data1 = "username"
         operation = 0x02
-        _,h = rolectrl.has_permission('role',roleName,permission,data1,operation)
-        print(h, roleName, permission, data1, operation)
+        ret,res = rolectrl.has_permission('rolectrl',roleName,permission,data1,operation)
+        print(res, roleName, permission, data1, operation)
 
+        operation0 = 0x02
+        ret,res = pctrl.has_permission('pctrl',permission,data1,operation0)
+        print(res)
 
         data2 = "idcard"
         operation2 = 0x02
-        _,h = rolectrl.has_permission('role',roleName,permission,data2,operation2)
-        print(h)
+        ret,res = rolectrl.has_permission('rolectrl',roleName,permission,data2,operation2)
+        print(res)
 
         operation3 = 0x01
-        _,h = rolectrl.has_permission('role',roleName,permission,data2,operation3)
-        print(h)
+        ret,res = rolectrl.has_permission('rolectrl',roleName,permission,data2,operation3)
+        print(res)
 
-        ret,_,_ = rolectrl.del_permission('role',self.pubs[2],sign_tx, roleName,[permission])
+        ret,res,receipt = rolectrl.del_permission('rolectrl',self.pubs[2],sign_tx, roleName,[permission])
         
         operation4 = 0x01
-        _,h = rolectrl.has_permission('role',roleName,permission,data1,operation4)
-        print(h)
+        ret,res = rolectrl.has_permission('rolectrl',roleName,permission,data1,operation4)
+        print(res)
 
 
  
 if __name__=='__main__':
     unittest.main()
```

### Comparing `iorclient-0.0.3/test/test_template.py` & `iorclient-0.0.4/test/test_template.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ior.iorsdk import IORClient
-from ior.util.web3_utils import to_address
+from ior.util.web3_utils import to_address,keccak256
 import unittest
 
 
 class TestTemplateMethods(unittest.TestCase):
     def setUp(self):
         #main test for example        
         self.ior = IORClient("http://127.0.0.1:5000/v1/api")
@@ -30,36 +30,48 @@
         tempctrl = self.ior.get('template')
         contract = self.ior.get('ctrt')
 
         #初始化模板Id
         tmp_id = 1
         ins_id = 0
         #只需要启动一次
-        #tempctrl.start('tempctrl',pub,sign_tx, tmp_id)
-        
+        ret,res = tempctrl.start('tempctrl',pub,sign_tx, tmp_id)
+        print('start',res)  
+
+        ret,res = tempctrl.templates('tempctrl',tmp_id)
+        print('templates',res)  
+
+        contract_identity = keccak256('测试').hex()
 
         #注册的结果返回0，需要根据实际结果查看, pub和pk可以是任意用户, 根据模板设计
-        _,ins_id = tempctrl.request_template('tempctrl',pub,sign_tx, tmp_id,'测试',2669296503)
-        
-        ret,_,_ = contract.init('contract1',pub,sign_tx, ins_id
+        ret,ins_id = tempctrl.request_template('tempctrl',pub,sign_tx, tmp_id, contract_identity, 2669296503)
+        print('request_template',ret,ins_id)
+
+        ret,res,receipt = contract.init('contract1',pub,sign_tx, ins_id
             , ['0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266']
             , '0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266'
             , ['0xb5A3426f9AB8751B868f9492a56A35ccE8a8dBfb','0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266']
             , [8000,2000]
             )
-        
-        _,state = contract.start('contract1',pub,sign_tx, ins_id)
-        
-        _,state = contract.sign('contract1',pub,sign_tx, ins_id)
-        
-        _,state = contract.end('contract1',pub,sign_tx, ins_id)
-        
-        _,can = contract.can_pay('contract1',ins_id,pub)
-        print(can)
-        _,payees = contract.get_payees('contract1',ins_id)
+        print('init',res)
+
+        ret,res = contract.verify_hash('contract1', ins_id, contract_identity)
+        print('verify_hash',res)
+
+        ret,state = contract.start('contract1',pub,sign_tx, ins_id)
+        print('start',state)
+        ret,state = contract.sign('contract1',pub,sign_tx, ins_id)
+        print('sign',state)
+        ret,state = contract.end('contract1',pub,sign_tx, ins_id)
+        print('end',state)
+        ret,can = contract.can_pay('contract1',ins_id,pub)
+        print('can pay',can)
+        ret,payees = contract.get_payees('contract1',ins_id)
+        print('get_payees',payees)
+
         for payee in payees:
             _,ratio = contract.get_ratio_by_payee('contract1',ins_id, payee)
             print(payee,ratio)
 
  
 if __name__=='__main__':
     unittest.main()
```

