# Comparing `tmp/iorclient-0.0.4.tar.gz` & `tmp/iorclient-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iorclient-0.0.4.tar", last modified: Thu Jul 20 09:00:50 2023, max compression
+gzip compressed data, was "iorclient-1.0.2.tar", last modified: Thu Jul 20 17:21:06 2023, max compression
```

## Comparing `iorclient-0.0.4.tar` & `iorclient-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 09:00:50.000031 iorclient-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 iorclient-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 iorclient-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      965 2023-07-20 09:00:49.998593 iorclient-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.963274 iorclient-0.0.4/ior/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 iorclient-0.0.4/ior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.976379 iorclient-0.0.4/ior/client/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 iorclient-0.0.4/ior/client/__init__.py
--rw-rw-rw-   0        0        0    12857 2023-07-19 16:53:06.000000 iorclient-0.0.4/ior/client/certificate_service.py
--rw-rw-rw-   0        0        0     5302 2023-07-20 08:17:33.000000 iorclient-0.0.4/ior/client/contract_template_service.py
--rw-rw-rw-   0        0        0     2539 2023-07-19 05:14:32.000000 iorclient-0.0.4/ior/client/exchange_service.py
--rw-rw-rw-   0        0        0     5056 2023-07-20 08:26:51.000000 iorclient-0.0.4/ior/client/permission_control_service.py
--rw-rw-rw-   0        0        0     5816 2023-07-19 05:30:38.000000 iorclient-0.0.4/ior/client/role_control_service.py
--rw-rw-rw-   0        0        0     5430 2023-07-19 05:15:05.000000 iorclient-0.0.4/ior/client/template_control_service.py
--rw-rw-rw-   0        0        0     2379 2023-07-19 04:47:03.000000 iorclient-0.0.4/ior/iorsdk.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.981241 iorclient-0.0.4/ior/util/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 iorclient-0.0.4/ior/util/__init__.py
--rw-rw-rw-   0        0        0     1490 2023-07-19 15:12:23.000000 iorclient-0.0.4/ior/util/result_utils.py
--rw-rw-rw-   0        0        0     4047 2023-07-17 18:09:55.000000 iorclient-0.0.4/ior/util/web3_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.988947 iorclient-0.0.4/iorclient.egg-info/
--rw-rw-rw-   0        0        0      965 2023-07-20 09:00:49.000000 iorclient-0.0.4/iorclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-07-20 09:00:49.000000 iorclient-0.0.4/iorclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 09:00:49.000000 iorclient-0.0.4/iorclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 09:00:49.000000 iorclient-0.0.4/iorclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 09:00:50.000031 iorclient-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-07-20 09:00:43.000000 iorclient-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:00:49.997492 iorclient-0.0.4/test/
--rw-rw-rw-   0        0        0        0 2023-07-17 16:15:26.000000 iorclient-0.0.4/test/__init__.py
--rw-rw-rw-   0        0        0     2043 2023-07-19 16:51:38.000000 iorclient-0.0.4/test/test_cert.py
--rw-rw-rw-   0        0        0     3809 2023-07-20 08:37:15.000000 iorclient-0.0.4/test/test_role.py
--rw-rw-rw-   0        0        0     2832 2023-07-20 08:25:12.000000 iorclient-0.0.4/test/test_template.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.538165 iorclient-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 iorclient-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 iorclient-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      994 2023-07-20 17:21:06.537168 iorclient-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.511251 iorclient-1.0.2/ior/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 iorclient-1.0.2/ior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.521221 iorclient-1.0.2/ior/client/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 iorclient-1.0.2/ior/client/__init__.py
+-rw-rw-rw-   0        0        0    12857 2023-07-19 16:53:06.000000 iorclient-1.0.2/ior/client/certificate_service.py
+-rw-rw-rw-   0        0        0     5302 2023-07-20 08:17:33.000000 iorclient-1.0.2/ior/client/contract_template_service.py
+-rw-rw-rw-   0        0        0     2539 2023-07-19 05:14:32.000000 iorclient-1.0.2/ior/client/exchange_service.py
+-rw-rw-rw-   0        0        0     5052 2023-07-20 17:16:49.000000 iorclient-1.0.2/ior/client/permission_control_service.py
+-rw-rw-rw-   0        0        0     5816 2023-07-19 05:30:38.000000 iorclient-1.0.2/ior/client/role_control_service.py
+-rw-rw-rw-   0        0        0     5430 2023-07-19 05:15:05.000000 iorclient-1.0.2/ior/client/template_control_service.py
+-rw-rw-rw-   0        0        0     2328 2023-07-20 15:58:18.000000 iorclient-1.0.2/ior/iorsdk.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.525209 iorclient-1.0.2/ior/util/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 iorclient-1.0.2/ior/util/__init__.py
+-rw-rw-rw-   0        0        0     1490 2023-07-19 15:12:23.000000 iorclient-1.0.2/ior/util/result_utils.py
+-rw-rw-rw-   0        0        0     4047 2023-07-17 18:09:55.000000 iorclient-1.0.2/ior/util/web3_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.530188 iorclient-1.0.2/iorclient.egg-info/
+-rw-rw-rw-   0        0        0      994 2023-07-20 17:21:06.000000 iorclient-1.0.2/iorclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-07-20 17:21:06.000000 iorclient-1.0.2/iorclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 17:21:06.000000 iorclient-1.0.2/iorclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 17:21:06.000000 iorclient-1.0.2/iorclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 17:21:06.538165 iorclient-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-07-20 17:18:58.000000 iorclient-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.535171 iorclient-1.0.2/test/
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:15:26.000000 iorclient-1.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     2054 2023-07-20 09:55:38.000000 iorclient-1.0.2/test/test_cert.py
+-rw-rw-rw-   0        0        0     3820 2023-07-20 09:55:42.000000 iorclient-1.0.2/test/test_role.py
+-rw-rw-rw-   0        0        0     2843 2023-07-20 09:55:45.000000 iorclient-1.0.2/test/test_template.py
```

### Comparing `iorclient-0.0.4/LICENSE` & `iorclient-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/PKG-INFO` & `iorclient-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: iorclient
-Version: 0.0.4
+Version: 1.0.2
 Summary: ior client sdk for ior standard
 Home-page: https://github.com/tzspace-ior/iorclient
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IOR SDK Document
+# IOR Client SDK Document
 ## IOR introduction
 
 > The full name of IOR is Internet of Rights, which mainly solves how to manage property rights, resource allocation, and teamwork on the Internet.<p>
 > IOR comes from the 3816 standard under the IEEE organization. It is the logical layer above the blockchain and an overall solution to solve practical problems in real-world scenarios.<p>
-> IOR project address:https://github.com/tzspace-ior/iorclient<p>
-> IOR zh document address:https://github.com/tzspace-ior/iorclient/blob/master/README_ZH.MD<p>
+> IOR client sdk project address:https://github.com/tzspace-ior/iorclient<p>
+> IOR client sdk zh document address:https://github.com/tzspace-ior/iorclient/blob/master/README_ZH.MD<p>
```

### Comparing `iorclient-0.0.4/ior/client/certificate_service.py` & `iorclient-1.0.2/ior/client/certificate_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/ior/client/contract_template_service.py` & `iorclient-1.0.2/ior/client/contract_template_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/ior/client/exchange_service.py` & `iorclient-1.0.2/ior/client/exchange_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/ior/client/permission_control_service.py` & `iorclient-1.0.2/ior/client/permission_control_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def set_api_client(self, server_url, client):
         self._api = RestAPI(api_url=server_url+"/permission/control" ,driver=client)
         endpoints = [
             Endpoint(name="address",path="/get_address",method=HTTPMethod.POST),
             Endpoint(name="hasRole",path="/has_role",method=HTTPMethod.POST),
             Endpoint(name="hasPermission",path="/has_permission",method=HTTPMethod.POST),
-            Endpoint(name="datas",path="/get_dataById",method=HTTPMethod.POST),
+            Endpoint(name="datas",path="/get_dataByName",method=HTTPMethod.POST),
             Endpoint(name="grantRole",path="/estimate_grantRole_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="revokeRole",path="/estimate_revokeRole_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="addPermission",path="/estimate_addPermission_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="delPermission",path="/estimate_delPermission_forReceipt",method=HTTPMethod.POST),
             Endpoint(name="tryForReceipt",path="/try_forReceipt",method=HTTPMethod.POST),
         ]
         self._api.register_endpoints(endpoints)
@@ -52,19 +52,19 @@
                 'permission': _permission, 
                 'data': _data, 
                 'operation': _operation
             })
         return res['data']
 
     @error_handler
-    def datas(self, service_name,  _dataId):
+    def datas(self, service_name,  _data):
         res = self._api.call_endpoint("datas",data=
             {
                 'name': service_name, 
-                'dataId': _dataId
+                'data': _data
             })
         return res['data']
 
 
     @two_ret_error_handler
     def grant_role(self, service_name, pub, sign_func,  _role,_to):
         res = self._api.call_endpoint("grantRole",data=
```

### Comparing `iorclient-0.0.4/ior/client/role_control_service.py` & `iorclient-1.0.2/ior/client/role_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/ior/client/template_control_service.py` & `iorclient-1.0.2/ior/client/template_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/ior/iorsdk.py` & `iorclient-1.0.2/ior/iorsdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,63 +87,60 @@
 00000560: 290d 0a09 0973 656c 662e 7365 7428 2774  )....self.set('t
 00000570: 656d 706c 6174 6527 2c54 656d 706c 6174  emplate',Templat
 00000580: 6543 6f6e 7472 6f6c 5365 7276 6963 6528  eControlService(
 00000590: 2929 0d0a 0909 7365 6c66 2e73 6574 2827  ))....self.set('
 000005a0: 6374 7274 272c 436f 6e74 7261 6374 5465  ctrt',ContractTe
 000005b0: 6d70 6c61 7465 5365 7276 6963 6528 2929  mplateService())
 000005c0: 0d0a 0d0a 0940 7072 6f70 6572 7479 0d0a  .....@property..
-000005d0: 0964 6566 2061 7069 2873 656c 6629 3a0d  .def api(self):.
-000005e0: 0a09 0972 6574 7572 6e20 7365 6c66 2e5f  ...return self._
-000005f0: 6170 690d 0a0d 0a09 4070 726f 7065 7274  api.....@propert
-00000600: 790d 0a09 6465 6620 7733 2873 656c 6629  y...def w3(self)
-00000610: 3a0d 0a09 0972 6574 7572 6e20 7365 6c66  :....return self
-00000620: 2e5f 7733 0d0a 0d0a 0964 6566 2073 6574  ._w3.....def set
-00000630: 2873 656c 662c 206e 616d 652c 2073 6572  (self, name, ser
-00000640: 7669 6365 293a 0d0a 0909 7365 7276 6963  vice):....servic
-00000650: 652e 7365 745f 6170 695f 636c 6965 6e74  e.set_api_client
-00000660: 2873 656c 662e 5f73 6572 7665 725f 7572  (self._server_ur
-00000670: 6c2c 2073 656c 662e 5f63 6c69 656e 7429  l, self._client)
-00000680: 0d0a 0909 7365 6c66 2e5f 7365 7276 6963  ....self._servic
-00000690: 6573 5b6e 616d 655d 203d 2073 6572 7669  es[name] = servi
-000006a0: 6365 0d0a 0d0a 0964 6566 2067 6574 2873  ce.....def get(s
-000006b0: 656c 662c 206e 616d 6529 3a0d 0a09 0969  elf, name):....i
-000006c0: 6620 6e61 6d65 206e 6f74 2069 6e20 7365  f name not in se
-000006d0: 6c66 2e5f 7365 7276 6963 6573 3a0d 0a09  lf._services:...
-000006e0: 0909 7265 7475 726e 204e 6f6e 650d 0a09  ..return None...
-000006f0: 0972 6574 7572 6e20 7365 6c66 2e5f 7365  .return self._se
-00000700: 7276 6963 6573 5b6e 616d 655d 0d0a 0d0a  rvices[name]....
-00000710: 0964 6566 2063 7265 6174 655f 6163 636f  .def create_acco
-00000720: 756e 7428 7365 6c66 293a 0d0a 0909 7265  unt(self):....re
-00000730: 7475 726e 2063 7265 6174 655f 6163 636f  turn create_acco
-00000740: 756e 7428 7365 6c66 2e77 3329 0d0a 0d0a  unt(self.w3)....
-00000750: 0940 6572 726f 725f 6861 6e64 6c65 720d  .@error_handler.
-00000760: 0a09 6465 6620 6465 706c 6f79 5f74 7261  ..def deploy_tra
-00000770: 6e73 6163 7469 6f6e 2873 656c 662c 2072  nsaction(self, r
-00000780: 6177 5478 293a 0d0a 0909 7265 6365 6970  awTx):....receip
-00000790: 7420 3d20 7574 696c 5f73 656e 645f 7261  t = util_send_ra
-000007a0: 775f 7472 616e 7361 6374 696f 6e28 7365  w_transaction(se
-000007b0: 6c66 2e77 332c 2072 6177 5478 2c20 7365  lf.w3, rawTx, se
-000007c0: 6c66 2e5f 636f 6e66 6967 2e74 696d 656f  lf._config.timeo
-000007d0: 7574 2c20 7365 6c66 2e5f 636f 6e66 6967  ut, self._config
-000007e0: 2e70 6f6c 6c5f 6c61 7465 6e63 7929 0d0a  .poll_latency)..
-000007f0: 0909 7265 7475 726e 2072 6563 6569 7074  ..return receipt
-00000800: 2e63 6f6e 7472 6163 7441 6464 7265 7373  .contractAddress
-00000810: 0d0a 0d0a 0940 6572 726f 725f 6861 6e64  .....@error_hand
-00000820: 6c65 720d 0a09 6465 6620 6578 6563 7574  ler...def execut
-00000830: 655f 7472 616e 7361 6374 696f 6e28 7365  e_transaction(se
-00000840: 6c66 2c20 7261 7754 7829 3a0d 0a09 0972  lf, rawTx):....r
-00000850: 6563 6569 7074 203d 2075 7469 6c5f 7365  eceipt = util_se
-00000860: 6e64 5f72 6177 5f74 7261 6e73 6163 7469  nd_raw_transacti
-00000870: 6f6e 2873 656c 662e 7733 2c20 7261 7754  on(self.w3, rawT
-00000880: 782c 2073 656c 662e 5f63 6f6e 6669 672e  x, self._config.
-00000890: 7469 6d65 6f75 742c 2073 656c 662e 5f63  timeout, self._c
-000008a0: 6f6e 6669 672e 706f 6c6c 5f6c 6174 656e  onfig.poll_laten
-000008b0: 6379 290d 0a09 0972 6574 7572 6e20 7265  cy)....return re
-000008c0: 6365 6970 740d 0a0d 0a09 6465 6620 7369  ceipt.....def si
-000008d0: 676e 5f74 7261 6e73 6163 7469 6f6e 2873  gn_transaction(s
-000008e0: 656c 662c 2074 782c 2070 7269 7661 7465  elf, tx, private
-000008f0: 5f6b 6579 293a 0d0a 0909 7369 676e 6564  _key):....signed
-00000900: 5f74 7820 3d20 7574 696c 5f73 6967 6e5f  _tx = util_sign_
-00000910: 7472 616e 7361 6374 696f 6e28 7365 6c66  transaction(self
-00000920: 2e77 332c 2074 782c 2070 7269 7661 7465  .w3, tx, private
-00000930: 5f6b 6579 290d 0a09 0972 6574 7572 6e20  _key)....return 
-00000940: 7369 676e 6564 5f74 780d 0a              signed_tx..
+000005d0: 0964 6566 2077 3328 7365 6c66 293a 0d0a  .def w3(self):..
+000005e0: 0909 7265 7475 726e 2073 656c 662e 5f77  ..return self._w
+000005f0: 330d 0a0d 0a09 6465 6620 7365 7428 7365  3.....def set(se
+00000600: 6c66 2c20 6e61 6d65 2c20 7365 7276 6963  lf, name, servic
+00000610: 6529 3a0d 0a09 0973 6572 7669 6365 2e73  e):....service.s
+00000620: 6574 5f61 7069 5f63 6c69 656e 7428 7365  et_api_client(se
+00000630: 6c66 2e5f 7365 7276 6572 5f75 726c 2c20  lf._server_url, 
+00000640: 7365 6c66 2e5f 636c 6965 6e74 290d 0a09  self._client)...
+00000650: 0973 656c 662e 5f73 6572 7669 6365 735b  .self._services[
+00000660: 6e61 6d65 5d20 3d20 7365 7276 6963 650d  name] = service.
+00000670: 0a0d 0a09 6465 6620 6765 7428 7365 6c66  ....def get(self
+00000680: 2c20 6e61 6d65 293a 0d0a 0909 6966 206e  , name):....if n
+00000690: 616d 6520 6e6f 7420 696e 2073 656c 662e  ame not in self.
+000006a0: 5f73 6572 7669 6365 733a 0d0a 0909 0972  _services:.....r
+000006b0: 6574 7572 6e20 4e6f 6e65 0d0a 0909 7265  eturn None....re
+000006c0: 7475 726e 2073 656c 662e 5f73 6572 7669  turn self._servi
+000006d0: 6365 735b 6e61 6d65 5d0d 0a0d 0a09 6465  ces[name].....de
+000006e0: 6620 6372 6561 7465 5f61 6363 6f75 6e74  f create_account
+000006f0: 2873 656c 6629 3a0d 0a09 0972 6574 7572  (self):....retur
+00000700: 6e20 6372 6561 7465 5f61 6363 6f75 6e74  n create_account
+00000710: 2873 656c 662e 7733 290d 0a0d 0a09 4065  (self.w3).....@e
+00000720: 7272 6f72 5f68 616e 646c 6572 0d0a 0964  rror_handler...d
+00000730: 6566 2064 6570 6c6f 795f 7472 616e 7361  ef deploy_transa
+00000740: 6374 696f 6e28 7365 6c66 2c20 7261 7754  ction(self, rawT
+00000750: 7829 3a0d 0a09 0972 6563 6569 7074 203d  x):....receipt =
+00000760: 2075 7469 6c5f 7365 6e64 5f72 6177 5f74   util_send_raw_t
+00000770: 7261 6e73 6163 7469 6f6e 2873 656c 662e  ransaction(self.
+00000780: 7733 2c20 7261 7754 782c 2073 656c 662e  w3, rawTx, self.
+00000790: 5f63 6f6e 6669 672e 7469 6d65 6f75 742c  _config.timeout,
+000007a0: 2073 656c 662e 5f63 6f6e 6669 672e 706f   self._config.po
+000007b0: 6c6c 5f6c 6174 656e 6379 290d 0a09 0972  ll_latency)....r
+000007c0: 6574 7572 6e20 7265 6365 6970 742e 636f  eturn receipt.co
+000007d0: 6e74 7261 6374 4164 6472 6573 730d 0a0d  ntractAddress...
+000007e0: 0a09 4065 7272 6f72 5f68 616e 646c 6572  ..@error_handler
+000007f0: 0d0a 0964 6566 2065 7865 6375 7465 5f74  ...def execute_t
+00000800: 7261 6e73 6163 7469 6f6e 2873 656c 662c  ransaction(self,
+00000810: 2072 6177 5478 293a 0d0a 0909 7265 6365   rawTx):....rece
+00000820: 6970 7420 3d20 7574 696c 5f73 656e 645f  ipt = util_send_
+00000830: 7261 775f 7472 616e 7361 6374 696f 6e28  raw_transaction(
+00000840: 7365 6c66 2e77 332c 2072 6177 5478 2c20  self.w3, rawTx, 
+00000850: 7365 6c66 2e5f 636f 6e66 6967 2e74 696d  self._config.tim
+00000860: 656f 7574 2c20 7365 6c66 2e5f 636f 6e66  eout, self._conf
+00000870: 6967 2e70 6f6c 6c5f 6c61 7465 6e63 7929  ig.poll_latency)
+00000880: 0d0a 0909 7265 7475 726e 2072 6563 6569  ....return recei
+00000890: 7074 0d0a 0d0a 0964 6566 2073 6967 6e5f  pt.....def sign_
+000008a0: 7472 616e 7361 6374 696f 6e28 7365 6c66  transaction(self
+000008b0: 2c20 7478 2c20 7072 6976 6174 655f 6b65  , tx, private_ke
+000008c0: 7929 3a0d 0a09 0973 6967 6e65 645f 7478  y):....signed_tx
+000008d0: 203d 2075 7469 6c5f 7369 676e 5f74 7261   = util_sign_tra
+000008e0: 6e73 6163 7469 6f6e 2873 656c 662e 7733  nsaction(self.w3
+000008f0: 2c20 7478 2c20 7072 6976 6174 655f 6b65  , tx, private_ke
+00000900: 7929 0d0a 0909 7265 7475 726e 2073 6967  y)....return sig
+00000910: 6e65 645f 7478 0d0a                      ned_tx..
```

### Comparing `iorclient-0.0.4/ior/util/result_utils.py` & `iorclient-1.0.2/ior/util/result_utils.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/ior/util/web3_utils.py` & `iorclient-1.0.2/ior/util/web3_utils.py`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/iorclient.egg-info/PKG-INFO` & `iorclient-1.0.2/iorclient.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: iorclient
-Version: 0.0.4
+Version: 1.0.2
 Summary: ior client sdk for ior standard
 Home-page: https://github.com/tzspace-ior/iorclient
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IOR SDK Document
+# IOR Client SDK Document
 ## IOR introduction
 
 > The full name of IOR is Internet of Rights, which mainly solves how to manage property rights, resource allocation, and teamwork on the Internet.<p>
 > IOR comes from the 3816 standard under the IEEE organization. It is the logical layer above the blockchain and an overall solution to solve practical problems in real-world scenarios.<p>
-> IOR project address:https://github.com/tzspace-ior/iorclient<p>
-> IOR zh document address:https://github.com/tzspace-ior/iorclient/blob/master/README_ZH.MD<p>
+> IOR client sdk project address:https://github.com/tzspace-ior/iorclient<p>
+> IOR client sdk zh document address:https://github.com/tzspace-ior/iorclient/blob/master/README_ZH.MD<p>
```

### Comparing `iorclient-0.0.4/iorclient.egg-info/SOURCES.txt` & `iorclient-1.0.2/iorclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iorclient-0.0.4/setup.py` & `iorclient-1.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.MD", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="iorclient",
-  version="0.0.4",
+  version="1.0.2",
   author="Jie Guan",
   author_email="jguanisme@163.com",
   description="ior client sdk for ior standard",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/tzspace-ior/iorclient",
   packages=setuptools.find_packages(),
```

### Comparing `iorclient-0.0.4/test/test_cert.py` & `iorclient-1.0.2/test/test_cert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ior.iorsdk import IORClient
 from ior.util.web3_utils import keccak256
 import unittest
 
 class TestCertMethods(unittest.TestCase):
     def setUp(self):
         #main test for example        
-        self.ior = IORClient("http://127.0.0.1:5000/v1/api")
+        self.ior = IORClient("http://121.5.19.151:8199/tzspace/v1/api")
         self.ior.init_w3()
         self.ior.init_apis()
 
         self.pub = "0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266"
         self.pk = "0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80"
 
         pub1,pk1 = self.ior.create_account()
```

### Comparing `iorclient-0.0.4/test/test_role.py` & `iorclient-1.0.2/test/test_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ior.iorsdk import IORClient
 from ior.util.web3_utils import keccak256
 import unittest
 
 class TestRoleMethods(unittest.TestCase):
     def setUp(self):
         #main test for example        
-        self.ior = IORClient("http://127.0.0.1:5000/v1/api")
+        self.ior = IORClient("http://121.5.19.151:8199/tzspace/v1/api")
         self.ior.init_w3()
         self.ior.init_apis()
 
         self.pub = "0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266"
         self.pk = "0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80"
 
         pub1,pk1 = self.ior.create_account()
```

### Comparing `iorclient-0.0.4/test/test_template.py` & `iorclient-1.0.2/test/test_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ior.util.web3_utils import to_address,keccak256
 import unittest
 
 
 class TestTemplateMethods(unittest.TestCase):
     def setUp(self):
         #main test for example        
-        self.ior = IORClient("http://127.0.0.1:5000/v1/api")
+        self.ior = IORClient("http://121.5.19.151:8199/tzspace/v1/api")
         self.ior.init_w3()
         self.ior.init_apis()
 
         self.pub = "0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266"
         self.pk = "0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80"
 
         pub1,pk1 = self.ior.create_account()
```

