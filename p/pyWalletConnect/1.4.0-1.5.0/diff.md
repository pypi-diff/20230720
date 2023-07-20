# Comparing `tmp/pyWalletConnect-1.4.0-py3-none-any.whl.zip` & `tmp/pyWalletConnect-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 41318 bytes, number of entries: 17
+Zip file size: 42033 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      909 b- defN 22-Feb-07 21:32 pywalletconnect/__init__.py
 -rw-rw-rw-  2.0 fat     1196 b- defN 23-Jan-25 19:46 pywalletconnect/base58.py
--rw-rw-rw-  2.0 fat     6978 b- defN 23-Jun-18 16:35 pywalletconnect/client.py
--rw-rw-rw-  2.0 fat     7767 b- defN 23-Jan-25 19:46 pywalletconnect/client_v1.py
--rw-rw-rw-  2.0 fat    15538 b- defN 23-Feb-26 19:08 pywalletconnect/client_v2irn.py
--rw-rw-rw-  2.0 fat    14424 b- defN 23-Jun-18 16:35 pywalletconnect/client_v2waku.py
+-rw-rw-rw-  2.0 fat     7193 b- defN 23-Jul-20 12:54 pywalletconnect/client.py
+-rw-rw-rw-  2.0 fat     8360 b- defN 23-Jul-20 12:54 pywalletconnect/client_v1.py
+-rw-rw-rw-  2.0 fat    16218 b- defN 23-Jul-20 12:54 pywalletconnect/client_v2irn.py
+-rw-rw-rw-  2.0 fat    14843 b- defN 23-Jul-20 12:54 pywalletconnect/client_v2waku.py
 -rw-rw-rw-  2.0 fat     8770 b- defN 23-Jan-25 19:46 pywalletconnect/enc_tunnel.py
--rw-rw-rw-  2.0 fat     2901 b- defN 23-Jun-18 16:35 pywalletconnect/json_rpc.py
+-rw-rw-rw-  2.0 fat     2974 b- defN 23-Jul-20 12:54 pywalletconnect/json_rpc.py
 -rw-rw-rw-  2.0 fat     2282 b- defN 22-Feb-07 21:32 pywalletconnect/tls_socket.py
--rw-rw-rw-  2.0 fat       58 b- defN 23-Jun-18 16:35 pywalletconnect/version.py
+-rw-rw-rw-  2.0 fat       58 b- defN 23-Jul-20 12:54 pywalletconnect/version.py
 -rw-rw-rw-  2.0 fat     7965 b- defN 23-Jan-25 20:08 pywalletconnect/websocket.py
--rw-rw-rw-  2.0 fat     1875 b- defN 23-Jan-25 19:46 pywalletconnect/ws_auth.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11532 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1444 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/RECORD
-17 files, 118896 bytes uncompressed, 38940 bytes compressed:  67.2%
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-Jul-20 12:54 pywalletconnect/ws_auth.py
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-Jul-20 12:56 pyWalletConnect-1.5.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12836 b- defN 23-Jul-20 12:56 pyWalletConnect-1.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 12:56 pyWalletConnect-1.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jul-20 12:56 pyWalletConnect-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1444 b- defN 23-Jul-20 12:56 pyWalletConnect-1.5.0.dist-info/RECORD
+17 files, 122180 bytes uncompressed, 39655 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: pywalletconnect/websocket.py
 Comment: 
 
 Filename: pywalletconnect/ws_auth.py
 Comment: 
 
-Filename: pyWalletConnect-1.4.0.dist-info/LICENSE
+Filename: pyWalletConnect-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyWalletConnect-1.4.0.dist-info/METADATA
+Filename: pyWalletConnect-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: pyWalletConnect-1.4.0.dist-info/WHEEL
+Filename: pyWalletConnect-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyWalletConnect-1.4.0.dist-info/top_level.txt
+Filename: pyWalletConnect-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyWalletConnect-1.4.0.dist-info/RECORD
+Filename: pyWalletConnect-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywalletconnect/client.py

```diff
@@ -45,14 +45,15 @@
 
 class WCClient:
     """WalletConnect wallet v1 and v2 base client."""
 
     wc_uri_pattern = regex_compile(r"^wc:(.+)@(\d)\?(.+)$")
     project_id = ""
     origin_domain = ""
+    wallet_namespace = "eip155"
     wallet_metadata = {
         "description": f"pyWalletConnect v{VERSION} by BitLogiK",
         "url": "https://github.com/bitlogik/pyWalletConnect",
         "icons": [
             "https://raw.githubusercontent.com/bitlogik/pyWalletConnect/master/logo.png"
         ],
         "name": "pyWalletConnect",
@@ -67,26 +68,31 @@
         self.data_queue = None
 
     def __del__(self):
         """Dying gasp and clean close"""
         self.close()
 
     @classmethod
+    def set_wallet_namespace(cls, wallet_namespace):
+        """Can override the default wallet namespace."""
+        cls.wallet_namespace = wallet_namespace
+
+    @classmethod
     def set_wallet_metadata(cls, wallet_metadata):
         """Can override the default wallet metadata."""
         cls.wallet_metadata = wallet_metadata
 
     @classmethod
     def set_project_id(cls, project_id):
         """Set the project id, mandatory for v2, using the central official relay."""
         cls.project_id = project_id
 
     @classmethod
     def set_origin(cls, origin):
-        """Set the Oring header in WS start request."""
+        """Set the Origin header in WS start request."""
         cls.origin_domain = origin
 
     def close(self):
         """Close the WebSocket connection when deleting the object."""
         logger.debug("Closing WalletConnect link.")
         if isinstance(self, WCv1Client):
             # Auto disconnect if v1 and still connected
```

## pywalletconnect/client_v1.py

```diff
@@ -107,15 +107,28 @@
             logger.debug("Get data, WalletConnect message available : %s", msg_ready)
         else:
             msg_ready = (None, "", [])
         return msg_ready
 
     def reply(self, req_id, result):
         """Send a RPC response to the webapp through the relay."""
-        payload_bin = json_rpc_pack_response(req_id, result)
+        self._reply(req_id, result, True)
+
+    def reject(self, req_id, error_code=5002):
+        """Inform the webapp that this request was rejected by the user."""
+        self.reply_error(req_id, "User rejected.", error_code)
+
+    def reply_error(self, req_id, message, error_code):
+        """Send a RPC error to the webapp through the relay."""
+        result = {'code': error_code, 'message': message}
+        self._reply(req_id, result, False)
+
+    def _reply(self, req_id, result, success=True):
+        """Send a RPC response to the webapp through the relay."""
+        payload_bin = json_rpc_pack_response(req_id, result, success)
         datafull = {
             "topic": self.app_peer_id,
             "type": "pub",
             "payload": json_encode(self.enc_channel.encrypt_payload(payload_bin)),
         }
         logger.debug(
             "--> WalletConnect Replying id[%i] : result=%s\nRaw message: %s",
```

## pywalletconnect/client_v2irn.py

```diff
@@ -182,20 +182,29 @@
             cyclew += 1
         if cyclew == CYCLES_TIMEOUT:
             self.close()
             raise WCClientException(f"{resp_type} timeout")
 
     def reply(self, req_id, result):
         """Send a RPC response to the current topic to the webapp through the relay."""
-        self._reply(self.wallet_id, req_id, result)
+        self._reply(self.wallet_id, req_id, result, success=True)
 
-    def _reply(self, topic, req_id, result, tag=0):
+    def reject(self, req_id, error_code=5002):
+        """Inform the webapp that this request was rejected by the user."""
+        self.reply_error(req_id, "User rejected.", error_code)
+
+    def reply_error(self, req_id, message, error_code):
+        """Send a RPC error to the current topic to the webapp through the relay."""
+        result = {'code': error_code, 'message': message}
+        self._reply(self.wallet_id, req_id, result, success=False)
+
+    def _reply(self, topic, req_id, result, tag=0, success=True):
         """Send a RPC response to the webapp through the relay."""
         logger.debug("Sending response result : %s , %s", req_id, result)
-        payload_bin = json_rpc_pack_response(req_id, result)
+        payload_bin = json_rpc_pack_response(req_id, result, success)
         msgbp = self.topics[topic]["secure_channel"].encrypt_payload(payload_bin, None)
         logger.debug("Sending result reply.")
         self.publish(topic, msgbp, tag, "Sending result")
 
     def subscribe(self, topic_id):
         """Start listening to a given topic."""
         logger.debug("Sending a subscription request for %s.", topic_id)
@@ -245,26 +254,29 @@
                 if read_data[1] == "wc_sessionPropose":
                     logger.debug("Session proposal payload received")
                     if read_data[2]["relays"][0]["protocol"] != "irn":
                         raise WCClientException(
                             "Session propose incompatible protocol."
                         )
                     self.peer_pubkey = read_data[2]["proposer"]["publicKey"]
-                    if read_data[2]["requiredNamespaces"].get("eip155") is None:
+                    if read_data[2]["requiredNamespaces"].get(
+                            self.wallet_namespace) is None:
                         raise WCClientException(
-                            "Only compatible with EIP155 namespaces."
+                            f"Wallet namespace ({self.wallet_namespace}) mismatch."
                         )
                     self.proposed_methods = read_data[2]["requiredNamespaces"][
-                        "eip155"
+                        self.wallet_namespace
                     ]["methods"]
-                    self.proposed_events = read_data[2]["requiredNamespaces"]["eip155"][
-                        "events"
-                    ]
+                    self.proposed_events = read_data[2]["requiredNamespaces"][
+                        self.wallet_namespace
+                    ]["events"]
                     peer_meta = read_data[2]["proposer"]["metadata"]
-                    chain_id = read_data[2]["requiredNamespaces"]["eip155"]["chains"][
+                    chain_id = read_data[2]["requiredNamespaces"][
+                        self.wallet_namespace
+                    ]["chains"][
                         0
                     ].split(":")[-1]
                     logger.debug("OK continue : Session proposal payload received")
                     break
             cyclew += 1
         if cyclew == CYCLES_TIMEOUT:
             self.close()
@@ -273,17 +285,16 @@
         return read_data[0], chain_id, peer_meta
 
     def reject_session_request(self, msg_id):
         """Send the sessionRequest rejection."""
 
         respo_neg = json_rpc_pack_response(
             msg_id,
-            {
-                "error": {"code": 5000, "message": "User rejected the session."},
-            },
+            {"code": 5000, "message": "User rejected the session."},
+            success=False
         )
         msgbn = self.topics[self.proposal_topic]["secure_channel"].encrypt_payload(
             respo_neg, None
         )
         logger.debug("Replying the session rejection.")
         self.publish(self.proposal_topic, msgbn, 1109, "Session rejection")
 
@@ -325,28 +336,28 @@
                     "protocol": "irn",
                 },
                 "controller": {
                     "publicKey": pubkey.hex(),
                     "metadata": self.wallet_metadata,
                 },
                 "namespaces": {
-                    "eip155": {
-                        "accounts": [f"eip155:{chain_id}:{account_address}"],
+                    self.wallet_namespace: {
+                        "accounts": [f"{self.wallet_namespace}:{chain_id}:{account_address}"],
                         "methods": self.proposed_methods,
                         "events": self.proposed_events,
                     }
                 },
                 "expiry": now_epoch + 14400,
             },
         )
 
         chat_enc_channel = EncryptedEnvelope(self.local_keypair.shared_key)
         self.topics[chat_topic] = {"secure_channel": chat_enc_channel}
         msgb = chat_enc_channel.encrypt_payload(json_encode(respo))
-        logger.debug("Approving the session proposal.")
+        logger.debug("Approving the session proposal: %s", json_encode(respo))
 
         self.subscribe(chat_topic)
 
         # Send the session approve
         self.publish(self.wallet_id, msgb, 1102, "sessionSettle post")
 
         logger.debug("Waiting for sessionSettle post ack.")
```

## pywalletconnect/client_v2waku.py

```diff
@@ -177,15 +177,24 @@
             cyclew += 1
         if cyclew == CYCLES_TIMEOUT:
             self.close()
             raise WCClientException(f"{resp_type} timeout")
 
     def reply(self, req_id, result):
         """Send a RPC response to the webapp through the relay."""
-        payload_bin = json_rpc_pack_response(req_id, result)
+        self._reply(req_id, result, True)
+
+    def reply_error(self, req_id, message, error_code):
+        """Send a RPC error to the webapp through the relay."""
+        result = {'code': error_code, 'message': message}
+        self._reply(req_id, result, False)
+
+    def _reply(self, req_id, result, success=True):
+        """Send a RPC response to the webapp through the relay."""
+        payload_bin = json_rpc_pack_response(req_id, result, success)
         msgbp = self.enc_channel.encrypt_payload(payload_bin, None)
         logger.debug("Sending result reply.")
         self.publish(self.wallet_id, msgbp, "Sending result")
 
     def subscribe(self, topic_id):
         """Start listening to a given topic."""
         logger.debug("Sending a subscription request for %s.", topic_id)
@@ -310,15 +319,15 @@
             {
                 "relay": {"protocol": "waku"},
                 "responder": {
                     "publicKey": pubkey.hex(),
                     "metadata": self.wallet_metadata,
                 },
                 "expiry": now_epoch + 14400,
-                "state": {"accounts": [f"eip155:{chain_id}:{account_address}"]},
+                "state": {"accounts": [f"{self.wallet_namespace}:{chain_id}:{account_address}"]},
             },
         )
         msgb = self.enc_channel.encrypt_payload(json_encode(respo))
         logger.debug("Approving the session proposal.")
 
         # Recompute keys and topic for the session
         keyassym.compute_shared_key(self.peer_pubkey)
```

## pywalletconnect/json_rpc.py

```diff
@@ -59,20 +59,21 @@
             err_msg = resp_obj["error"]
         raise Exception(err_msg)
     if "result" not in resp_obj:
         raise Exception(f"No result in response {raw_response}")
     return resp_obj["result"]
 
 
-def json_rpc_pack_response(idmsg, result_obj):
+def json_rpc_pack_response(idmsg, result_obj, success=True):
     """Build a JSON-RPC response."""
+    response_type = "result" if success else "error"
     request_obj = {
         "jsonrpc": "2.0",
         "id": idmsg,
-        "result": result_obj,
+        response_type: result_obj,
     }
     return json_encode(request_obj).encode("utf8")
 
 
 def json_rpc_unpack(buffer):
     """Decode a JSON-RPC call query : id, method, params."""
     try:
```

## pywalletconnect/version.py

```diff
@@ -1,3 +1,3 @@
 """pyWalletConnect version info."""
 
-VERSION = "1.4.0"
+VERSION = "1.5.0"
```

## pywalletconnect/ws_auth.py

```diff
@@ -21,15 +21,15 @@
 from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
 from cryptography.hazmat.primitives import serialization as ser
 
 from .base58 import bin_to_base58
 
 
 # WalletConnect central relay authorization needed.
-# But keys are genereted on the fly, so not really an auth.
+# But keys are generated on the fly, so not really an auth.
 
 
 def b64enc(data):
     """Encode in web-base64 without any padding."""
     e = base64.urlsafe_b64encode(data).decode("ascii")
     return e.rstrip("=")
```

## Comparing `pyWalletConnect-1.4.0.dist-info/LICENSE` & `pyWalletConnect-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyWalletConnect-1.4.0.dist-info/METADATA` & `pyWalletConnect-1.5.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyWalletConnect
-Version: 1.4.0
+Version: 1.5.0
 Summary: WalletConnect implementation for Python wallets
 Home-page: https://github.com/bitlogik/pyWalletConnect
 Author: BitLogiK
 Author-email: contact@bitlogik.fr
 License: GPLv3
 Keywords: blockchain wallet cryptography security
 Platform: UNKNOWN
@@ -18,15 +18,14 @@
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography (>=3.3)
 Requires-Dist: wsproto (>=1.0.0)
 
-
 # pyWalletConnect
 
 ![pyWalletConnect logo](logo.png)
 
 ### A WalletConnect implementation for wallets in Python
 
 A Python3 library to link a wallet with a WalletConnect web3 app. This library connects a Python wallet with a web3 app online, using the WalletConnect standard.
@@ -115,15 +114,14 @@
 Use a daemon thread timer for example, to call the `get_message()` method in a short time frequency. 3-6 seconds is an acceptable delay. This can also be performed in a blocking *for* loop with a sleeping time. Then process the Dapp queries for further user wallet actions.
 
 Remember to keep track of the request id, as it is needed for `.reply(req_id, result)` ultimately when sending the processing result back to the dapp service. One way is to provide the id in argument in your processing methods. Also this can be done with global or shared parameters.
 
 When a WCClient object (created from a WC link) is closed or deleted, it will automatically send to the dapp a closing session message.
 
 ```python
-
 def process_sendtransaction(call_id, tx):
     # Processing the RPC query eth_sendTransaction
     # Collect the user approval about the tx query
     < Accept (tx) ? >
     if approved :
         # Build and sign the provided transaction
         <...>
@@ -156,43 +154,53 @@
         if "wc_sessionDelete" == method:
             raise Exception("Disconnected by the Dapp.")
         # Dispatch query processing
         elif "eth_signTypedData" == method:
             result = process_signtypeddata(id_request, parameters[1])
             wallet_dapp.reply(call_id, result)
         elif "eth_sendTransaction" == method:
-            result = process_sendtransaction(id_request, parameters[0])
-            wallet_dapp.reply(call_id, result)
+            approve_ask = input("Approve (y/N)?: ").lower()
+            if approve_ask == 'y':
+                result = process_sendtransaction(id_request, parameters[0])
+                wallet_dapp.reply(call_id, result)
+            else:
+                wallet_dapp.reply_error(call_id, "User rejected request.", 4001)
         elif "eth_sign" == method:
-            result = process_signtransaction(parameters[1])
-            wallet_dapp.reply(call_id, result)
+            approve_ask = input("Approve (y/N)?: ").lower()
+            if approve_ask == 'y':
+                result = process_signtransaction(parameters[1])
+                wallet_dapp.reply(call_id, result)
+            else:
+                wallet_dapp.reject(call_id)
         <...>
         # Next loop
         wc_message = wallet_dapp.get_message()
 
 
 # GUI timer repeated or threading daemon
 # Will call watch_messages every 4 seconds
 apptimer = Timer(4000)
 # Call watch_messages when expires periodically
 apptimer.notify = watch_messages
-
 ```
 
 See also the [RPC methods in WalletConnect](https://docs.walletconnect.org/v/1.0/json-rpc-api-methods/ethereum) to know more about the expected result regarding a specific RPC call.
 
 ## Interface methods of WCClient
 
 `WCClient.set_wallet_metadata( wallet_metadata )`  
 Class method to set the wallet metadata as object (v2). See [the WalletConnect standard for the format details](https://docs.walletconnect.com/2.0/specs/clients/core/pairing/data-structures#metadata).  
 Optional. If not provided, when v2, it sends the default pyWalletConnect metadata as wallet identification.
 
+`WCClient.set_wallet_namespace( wallet_namespace )`  
+Class method to set the wallet [namespace](https://docs.walletconnect.com/2.0/advanced/glossary#namespaces), i.e. supported chain collection.  
+Only for v2, optional. Defaults to 'eip155' aka EVM-based chains.
+
 `WCClient.set_project_id( project_id )`  
-Class method to set the WalletConnect project id. This is mandatory to use a project id when  
-using WC v2 with the official central bridge relay.
+Class method to set the WalletConnect project id. This is mandatory to use a project id when using WC v2 with the official central bridge relay.
 
 `WCClient.set_origin( origin_domain )`  
 Class method to set the origin of the first HTTP query for websocket. Only for v2, optional.
 
 `WCClient.from_wc_uri( wc_uri_str )`  
 Create a WalletConnect wallet client from a wc v1 or v2 URI. (class method constructor)  
 *wc_uri_str* : the wc full EIP1328 URI provided by the Dapp.  
@@ -212,14 +220,25 @@
 When a v2 ping *wc_sessionPing* is received, it is automatically replied when getting it with get_message. In this case, the *get_message* method returns an empty method and no params. So filter *get_message* calls with 'id is None', means no more message left.
 
 `.reply( req_id, result_str )`  
 Send a RPC response to the webapp (through the relay).  
 *req_id* is the JSON-RPC id of the corresponding query request, where the result belongs to. One must kept track this id from the get_message, up to this reply. So a reply result is given back with its associated call query id.  
 *result_str* is the result field to provide in the RPC result response.
 
+`.reject( req_id, error_code=5002 )`  
+Inform the webapp that this request was rejected by the user.  
+*req_id* is the JSON-RPC id of the corresponding query request.  
+*error_code* is a rejection code to send to webapp (default 5002).  
+
+`.reply_error( req_id, message, error_code )`  
+Send a RPC error to the webapp (through the relay).  
+*req_id* is the JSON-RPC id of the corresponding query request.  
+*message* is a string providing a short description of the error.  
+*error_code* is a number that indicates the error type that occurred. See [the WalletConnect standard Error Codes](https://docs.walletconnect.com/2.0/specs/clients/sign/error-codes).   
+
 `.open_session()`  
 Start a WalletConnect session : wait for the session call request message.  
 Must be called right after a WCClient creation.  
 Returns : (message RPCid, chain ID, peerMeta data object).  
 Or throws WalletConnectClientException("sessionRequest timeout")
 after 8 seconds and no sessionRequest received.
 
@@ -229,29 +248,27 @@
 *chain_id* is the integer ideitifying the blockchain.
 *account_address* is a string of the address of the wallet account ("0x...").
 
 `.reject_session_request( req_id )`  
 Send a session rejection message to the dapp (through the relay).
 *req_id* is the RPC id of the session approval request.
 
-
 ## License
 
 Copyright (C) 2021-2023  BitLogiK SAS
 
 This program is free software: you can redistribute it and/or modify  
 it under the terms of the GNU General Public License as published by  
 the Free Software Foundation, version 3 of the License.
 
 This program is distributed in the hope that it will be useful,  
 but WITHOUT ANY WARRANTY; without even the implied warranty of  
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  
 See the GNU General Public License for more details.
 
-
 ## Support
 
 Open an issue in the Github repository for help about its use.
```

## Comparing `pyWalletConnect-1.4.0.dist-info/RECORD` & `pyWalletConnect-1.5.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 pywalletconnect/__init__.py,sha256=twRPUf3Ev6qvN54VuD79HBrxMXZMzwFqJDwJADyFWF8,909
 pywalletconnect/base58.py,sha256=f5ALRFwEFd7IMX946WyQNK5A-yGeOwuU5v6Z-Bnhd6s,1196
-pywalletconnect/client.py,sha256=GGD--bPnYhm1tCZJeIdv2tija1pN-U42gt0fQuM142U,6978
-pywalletconnect/client_v1.py,sha256=TAK5iAoPwcjZcv_44yJ9HIxcaJnXXSDoNTc27Pqo0lY,7767
-pywalletconnect/client_v2irn.py,sha256=cuDXivQhzErYbOg-50Epx7ubA091yehzqQWZ26Gnk1U,15538
-pywalletconnect/client_v2waku.py,sha256=k8d38tV1tmCOZXQXC_ee_2ZV5zNLxuGC6g8XrqNaJqA,14424
+pywalletconnect/client.py,sha256=F4gtGLqsuOFnDvFswGyyeT6wtR2eIHD6sOuqLny4slI,7193
+pywalletconnect/client_v1.py,sha256=tmqWJaDBZATUsdAW9GDPMpRyNdQ5kSUJ0NkY31ufPdU,8360
+pywalletconnect/client_v2irn.py,sha256=Ngt1Vu_SGfoMMwgHfynXFkzE4kX2fXcbKKagnbAAC3A,16218
+pywalletconnect/client_v2waku.py,sha256=6OKsiHNynIqjlAUfsCkT7rWSoRfeEWk1QHTC8Wj3z_U,14843
 pywalletconnect/enc_tunnel.py,sha256=8f-qtBFmqiOgsNgD42DX_ujJSRjOOJPI-gnGfWFyqEI,8770
-pywalletconnect/json_rpc.py,sha256=feF74KmNilFcWOG_N-WKnRrWOsH2iz5T8EM-NCDV8-g,2901
+pywalletconnect/json_rpc.py,sha256=etrzm2gGjXbRDFQsWpMbfVXkpw2UioJCML4g17f8Pkg,2974
 pywalletconnect/tls_socket.py,sha256=8-8uyReJsRv7WqzW43F5RbAvp7FuHFp_HQQU-bVBGbA,2282
-pywalletconnect/version.py,sha256=irvhv0xkqzz8zaIDL-WXidDrhoSuPyGncJnxOWSu-yc,58
+pywalletconnect/version.py,sha256=T4qvdDKtyQLySR3Hx24ziRSzZ1vWTe7UsrlWNV-Ifkw,58
 pywalletconnect/websocket.py,sha256=iE7I2wSLFCG1gSwweyJ23ycWIKGUXABJ_xXA2yk_POY,7965
-pywalletconnect/ws_auth.py,sha256=Et-kzX8ZyeGrrAbMQWMGsU3HW4cGzkteaOSGQdwvID0,1875
-pyWalletConnect-1.4.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pyWalletConnect-1.4.0.dist-info/METADATA,sha256=w0KJK3SCmj5O2EQpmjeKqf18O8gelddy9nbrKc9JBlk,11532
-pyWalletConnect-1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyWalletConnect-1.4.0.dist-info/top_level.txt,sha256=MeiZvwObGZFsa0avWx0Bg--YOWz1SZQF7PV-Q1z3OLo,16
-pyWalletConnect-1.4.0.dist-info/RECORD,,
+pywalletconnect/ws_auth.py,sha256=OOs3pVgujEReGf6Wyd2kIvwkrc_fvMIQ42aEPc7UCTA,1875
+pyWalletConnect-1.5.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pyWalletConnect-1.5.0.dist-info/METADATA,sha256=cZpd5hp7TvntIKWgMy-abjRkzCpK0_BNFwtzGOh92DY,12836
+pyWalletConnect-1.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyWalletConnect-1.5.0.dist-info/top_level.txt,sha256=MeiZvwObGZFsa0avWx0Bg--YOWz1SZQF7PV-Q1z3OLo,16
+pyWalletConnect-1.5.0.dist-info/RECORD,,
```

