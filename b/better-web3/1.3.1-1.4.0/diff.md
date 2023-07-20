# Comparing `tmp/better_web3-1.3.1.tar.gz` & `tmp/better_web3-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-1.3.1.tar", max compression
+gzip compressed data, was "better_web3-1.4.0.tar", max compression
```

## Comparing `better_web3-1.3.1.tar` & `better_web3-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0      377 2023-07-07 12:41:36.289000 better_web3-1.3.1/better_web3/__init__.py
--rw-r--r--   0        0        0    10484 2023-07-07 13:10:10.895000 better_web3-1.3.1/better_web3/batch_call.py
--rw-r--r--   0        0        0    14905 2023-07-07 12:24:04.882000 better_web3-1.3.1/better_web3/chain.py
--rw-r--r--   0        0        0      251 2023-07-07 12:10:25.885000 better_web3-1.3.1/better_web3/contract/__init__.py
--rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.3.1/better_web3/contract/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.3.1/better_web3/contract/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0     2861 2023-06-28 12:47:45.841000 better_web3-1.3.1/better_web3/contract/__pycache__/contract.cpython-311.pyc
--rw-r--r--   0        0        0     3766 2023-06-22 18:24:06.215000 better_web3-1.3.1/better_web3/contract/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     5344 2023-06-22 18:24:06.241000 better_web3-1.3.1/better_web3/contract/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0     9591 2023-06-22 17:42:59.377000 better_web3-1.3.1/better_web3/contract/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0      352 2023-07-07 12:03:06.296000 better_web3-1.3.1/better_web3/contract/_abi.py
--rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.3.1/better_web3/contract/_paths.py
--rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-1.3.1/better_web3/contract/abi/disperse.json
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.3.1/better_web3/contract/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.3.1/better_web3/contract/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.3.1/better_web3/contract/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.3.1/better_web3/contract/abi/multicall_v3.json
--rw-r--r--   0        0        0     1217 2023-06-28 12:35:30.364000 better_web3-1.3.1/better_web3/contract/contract.py
--rw-r--r--   0        0        0      974 2023-07-07 12:13:30.821000 better_web3-1.3.1/better_web3/contract/disperse.py
--rw-r--r--   0        0        0     1750 2023-07-07 12:07:18.371000 better_web3-1.3.1/better_web3/contract/erc20.py
--rw-r--r--   0        0        0     2874 2023-07-07 12:07:18.593000 better_web3-1.3.1/better_web3/contract/erc721.py
--rw-r--r--   0        0        0     6201 2023-07-07 12:07:18.259000 better_web3-1.3.1/better_web3/contract/multicall.py
--rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.3.1/better_web3/enums.py
--rw-r--r--   0        0        0      199 2023-06-28 11:42:15.433000 better_web3-1.3.1/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      445 2023-06-28 12:32:10.840000 better_web3-1.3.1/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3500 2023-06-19 18:50:51.812000 better_web3-1.3.1/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.3.1/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     1519 2023-06-28 12:32:10.893000 better_web3-1.3.1/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0     1907 2023-06-19 15:51:51.887000 better_web3-1.3.1/better_web3/utils/eth.py
--rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.3.1/better_web3/utils/file.py
--rw-r--r--   0        0        0      733 2023-06-28 11:42:15.546000 better_web3-1.3.1/better_web3/utils/other.py
--rw-r--r--   0        0        0     2323 2023-07-07 16:15:52.744000 better_web3-1.3.1/better_web3/wallet.py
--rw-r--r--   0        0        0      412 2023-07-07 16:15:52.791000 better_web3-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      406 2023-07-07 13:10:55.766000 better_web3-1.3.1/README.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 better_web3-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      403 2023-07-17 08:30:00.413000 better_web3-1.4.0/better_web3/__init__.py
+-rw-r--r--   0        0        0    10461 2023-07-17 08:28:26.368000 better_web3-1.4.0/better_web3/batch_call.py
+-rw-r--r--   0        0        0    15896 2023-07-15 15:58:01.098000 better_web3-1.4.0/better_web3/chain.py
+-rw-r--r--   0        0        0      251 2023-07-07 12:10:25.885000 better_web3-1.4.0/better_web3/contract/__init__.py
+-rw-r--r--   0        0        0      525 2023-07-11 06:39:31.842000 better_web3-1.4.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      687 2023-07-11 06:39:33.730000 better_web3-1.4.0/better_web3/contract/__pycache__/_abi.cpython-311.pyc
+-rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.4.0/better_web3/contract/__pycache__/_paths.cpython-311.pyc
+-rw-r--r--   0        0        0     2938 2023-07-11 06:39:31.913000 better_web3-1.4.0/better_web3/contract/__pycache__/contract.cpython-311.pyc
+-rw-r--r--   0        0        0     1938 2023-07-11 06:39:34.027000 better_web3-1.4.0/better_web3/contract/__pycache__/disperse.cpython-311.pyc
+-rw-r--r--   0        0        0     3687 2023-07-11 06:39:34.086000 better_web3-1.4.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc
+-rw-r--r--   0        0        0     5293 2023-07-11 06:39:34.163000 better_web3-1.4.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc
+-rw-r--r--   0        0        0     9601 2023-07-11 06:39:33.679000 better_web3-1.4.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc
+-rw-r--r--   0        0        0      352 2023-07-07 12:03:06.296000 better_web3-1.4.0/better_web3/contract/_abi.py
+-rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.4.0/better_web3/contract/_paths.py
+-rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-1.4.0/better_web3/contract/abi/disperse.json
+-rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.4.0/better_web3/contract/abi/erc1155.json
+-rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.4.0/better_web3/contract/abi/erc20.json
+-rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.4.0/better_web3/contract/abi/erc721.json
+-rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.4.0/better_web3/contract/abi/multicall_v3.json
+-rw-r--r--   0        0        0     1264 2023-07-10 08:18:27.356000 better_web3-1.4.0/better_web3/contract/contract.py
+-rw-r--r--   0        0        0      974 2023-07-07 12:13:30.821000 better_web3-1.4.0/better_web3/contract/disperse.py
+-rw-r--r--   0        0        0     1747 2023-07-07 20:11:33.426000 better_web3-1.4.0/better_web3/contract/erc20.py
+-rw-r--r--   0        0        0     2876 2023-07-07 20:11:33.364000 better_web3-1.4.0/better_web3/contract/erc721.py
+-rw-r--r--   0        0        0     6201 2023-07-07 12:07:18.259000 better_web3-1.4.0/better_web3/contract/multicall.py
+-rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.4.0/better_web3/enums.py
+-rw-r--r--   0        0        0     4037 2023-07-17 10:02:59.828000 better_web3-1.4.0/better_web3/proxy.py
+-rw-r--r--   0        0        0      730 2023-07-17 08:28:26.473000 better_web3-1.4.0/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-07-17 08:28:28.447000 better_web3-1.4.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4132 2023-07-17 08:28:28.496000 better_web3-1.4.0/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.4.0/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     1398 2023-07-11 06:39:33.869000 better_web3-1.4.0/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0     2131 2023-07-17 08:28:26.617000 better_web3-1.4.0/better_web3/utils/eth.py
+-rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.4.0/better_web3/utils/file.py
+-rw-r--r--   0        0        0      663 2023-07-07 20:05:19.087000 better_web3-1.4.0/better_web3/utils/other.py
+-rw-r--r--   0        0        0     3172 2023-07-17 10:00:37.875000 better_web3-1.4.0/better_web3/wallet.py
+-rw-r--r--   0        0        0      412 2023-07-17 09:38:47.230000 better_web3-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      479 2023-07-07 17:47:32.398000 better_web3-1.4.0/README.md
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 better_web3-1.4.0/PKG-INFO
```

### Comparing `better_web3-1.3.1/better_web3/batch_call.py` & `better_web3-1.4.0/better_web3/batch_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     BlockIdentifier,
     TxData,
     TxParams,
     TxReceipt,
     Wei,
 )
 
-from .utils import chunks
-from .utils.eth import hex_block_identifier
+from .utils import chunks, hex_block_identifier
 
 if TYPE_CHECKING:
     from .chain import Chain
 
 
 def build_payload(index: int, method: str, params: list) -> dict:
     return {"id": index, "jsonrpc": "2.0", "method": method, "params": params}
```

### Comparing `better_web3-1.3.1/better_web3/chain.py` & `better_web3-1.4.0/better_web3/chain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from dataclasses import dataclass
+from functools import cached_property
+from time import sleep
 
 import requests
 from eth_account.signers.local import LocalAccount
 from eth_typing import BlockNumber, ChecksumAddress, HexStr, Address, Hash32
 from hexbytes import HexBytes
 from requests.adapters import HTTPAdapter
 from web3 import HTTPProvider, Web3
@@ -17,15 +19,15 @@
     TxReceipt,
     Wei,
 )
 
 from .batch_call import BatchCallManager
 from .contract import Contract, Multicall, Disperse, ERC20, ERC721
 from .enums import TxSpeed
-from .utils import cache, link_by_tx_hash
+from .utils import link_by_tx_hash
 
 
 @dataclass
 class NativeToken:
     symbol: str = "ETH"
     decimals: int = 18
 
@@ -33,14 +35,15 @@
 class Chain:
     def __init__(
             self,
             rpc: str,
             *,
             name: str = "EVM Chain",
             is_testnet: bool = False,
+            use_eip1559: bool = True,
             # Native token
             symbol: str = "ETH",
             decimals: int = 18,
             # Explorer
             explorer_url: str = None,
             # Connection settings
             provider_timeout: int = 15,
@@ -59,14 +62,15 @@
             gas_price: Wei | int = None,
     ):
         self._rpc = rpc
         self.name = name
         self.is_testnet = is_testnet
         self.token = NativeToken(symbol=symbol, decimals=decimals)
         self.explorer_url = explorer_url
+        self.use_eip1559 = use_eip1559
 
         self.http_session = self._prepare_http_session(retry_count)
         self.timeout = provider_timeout
         self.slow_timeout = slow_provider_timeout
 
         self.w3_provider = self._create_http_provider(provider_timeout)
         self.w3_slow_provider = self._create_http_provider(slow_provider_timeout)
@@ -118,17 +122,20 @@
         session.mount("https://", adapter)
         return session
 
     @property
     def rpc(self):
         return self._rpc
 
-    def get_link_by_tx_hash(self, tx_hash: HexStr | str):
+    def get_link_by_tx_hash(self, tx_hash: HexBytes | HexStr | str):
         if self.explorer_url is None:
             raise ValueError("Set explorer_url before using this method")
+
+        if isinstance(tx_hash, HexBytes):
+            tx_hash = tx_hash.hex()
         return link_by_tx_hash(self.explorer_url, tx_hash)
 
     ################################################################################
     # Contract creation shortcuts
     ################################################################################
 
     def contract(self, address, abi) -> Contract:
@@ -140,26 +147,23 @@
     def erc721(self, address) -> ERC721:
         return ERC721(self, address)
 
     ################################################################################
     # Shortcuts
     ################################################################################
 
-    @property
-    @cache
+    @cached_property
     def chain_id(self) -> int:
         return self.w3.eth.chain_id
 
-    @property
-    @cache
+    @cached_property
     def client_version(self) -> str:
         return self.w3.client_version
 
-    @property
-    @cache
+    @cached_property
     def is_eip1559_supported(self) -> bool:
         """
         :return: True if EIP1559 is supported by the node, False otherwise
         """
         last_block = self.get_block("latest")
         return True if "baseFeePerGas" in last_block else False
 
@@ -193,15 +197,19 @@
     ) -> TxReceipt:
         """
         raises: TimeExhausted:
                  Raised when a method has not retrieved the desired result within a specified timeout.
                  TransactionNotFound:
                  Raised when a tx hash used to look up a tx in a jsonrpc call cannot be found.
         """
-        return self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout, poll_latency)
+        tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout, poll_latency)
+
+        # Add extra sleep to let tx propogate correctly
+        sleep(1)
+        return tx_receipt
 
     def get_block(
             self,
             block_identifier: BlockIdentifier,
             full_transactions: bool = False
     ) -> BlockData:
         return self.w3.eth.get_block(block_identifier, full_transactions=full_transactions)
@@ -256,15 +264,15 @@
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
             max_fee_per_gas: Wei = None,
             max_priority_fee_per_gas: Wei = None,
             tx_speed: TxSpeed = TxSpeed.NORMAL,
     ):
-        ...  # TODO Реализовать метод Chain.transfer_all()
+        raise NotImplementedError  # TODO Реализовать метод Chain.transfer_all()
 
     ################################################################################
     # Gas price shortcuts
     ################################################################################
 
     def get_gas_price(self) -> Wei:
         return self.w3.eth.gas_price
@@ -287,14 +295,20 @@
         max_fee_per_gas = base_fee_per_gas + max_priority_fee_per_gas
         return max_fee_per_gas, max_priority_fee_per_gas
 
     ################################################################################
     # Working with transactions
     ################################################################################
 
+    def _send_tx(self, tx: TxParams) -> HexBytes:
+        return self.w3.eth.send_transaction(tx)
+
+    def _send_raw_tx(self, raw_tx: bytes | HexStr) -> HexBytes:
+        return self.w3.eth.send_raw_transaction(bytes(raw_tx))
+
     def _build_tx_base_params(
             self,
             gas: int = None,
             address_from: Address | ChecksumAddress | str = None,
             address_to: Address | ChecksumAddress | str = None,
             nonce: Nonce | int = None,
             value: Wei = None,
@@ -334,15 +348,18 @@
             *,
             tx_params: TxParams = None,
     ) -> TxParams:
         if tx_params is None:
             tx_params = dict()
         tx_params = tx_params.copy()
 
-        if self.is_eip1559_supported and gas_price is None:
+        if (self.is_eip1559_supported and
+                ((gas_price is None and self.use_eip1559)
+                 or max_fee_per_gas is not None
+                 or max_priority_fee_per_gas is not None)):
             if max_fee_per_gas is None or max_priority_fee_per_gas is None:
                 estimated_max_fee_per_gas, estimated_max_priority_fee_per_gas = self.estimate_eip1559_fees(tx_speed)
                 max_fee_per_gas = max_fee_per_gas or estimated_max_fee_per_gas
                 max_priority_fee_per_gas = max_priority_fee_per_gas or estimated_max_priority_fee_per_gas
             tx_params["maxFeePerGas"] = max_fee_per_gas
             tx_params["maxPriorityFeePerGas"] = max_priority_fee_per_gas
         else:
@@ -357,16 +374,16 @@
             address_from: Address | ChecksumAddress | str = None,
             address_to: Address | ChecksumAddress | str = None,
             nonce: Nonce | int = None,
             value: Wei | int = None,
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
-            max_fee_per_gas: Wei = None,
-            max_priority_fee_per_gas: Wei = None,
+            max_fee_per_gas: Wei | int = None,
+            max_priority_fee_per_gas: Wei | int = None,
             tx_speed: TxSpeed = TxSpeed.NORMAL,
     ) -> TxParams:
         gas_price = gas_price or self.gas_price
         tx_params = self._build_tx_base_params(gas, address_from, address_to, nonce, value)
         gas = contract_function.estimate_gas(tx_params)
         tx_params = self._build_tx_base_params(gas, tx_params=tx_params)
         tx_params = self._build_tx_fee_params(
@@ -374,24 +391,34 @@
         return contract_function.build_transaction(tx_params)
 
     def sign_and_send_tx(self, account: LocalAccount, tx: TxParams) -> HexStr:
         signed_tx = account.sign_transaction(tx)
         tx_hash = self._send_raw_tx(signed_tx.rawTransaction)
         return HexStr(tx_hash.hex())
 
-    def _send_tx(self, tx: TxParams) -> HexBytes:
-        return self.w3.eth.send_transaction(tx)
-
-    def _send_raw_tx(self, raw_tx: bytes | HexStr) -> HexBytes:
-        return self.w3.eth.send_raw_transaction(bytes(raw_tx))
-
     def execute_fn(
             self,
             account: LocalAccount,
             fn: ContractFunction,
             *,
-            value: Wei = None,
-    ) -> tuple[TxReceipt, HexStr]:
-        tx = self.build_tx(fn, address_from=account.address, value=value)
+            gas: int = None,
+            nonce: Nonce | int = None,
+            value: Wei | int = None,
+            # legacy pricing
+            gas_price: Wei | int = None,
+            # dynamic fee pricing
+            max_fee_per_gas: Wei | int = None,
+            max_priority_fee_per_gas: Wei | int = None,
+            tx_speed: TxSpeed = TxSpeed.NORMAL,
+    ) -> HexStr:
+        tx = self.build_tx(
+            fn,
+            gas=gas,
+            nonce=nonce,
+            value=value,
+            gas_price=gas_price,
+            max_fee_per_gas=max_fee_per_gas,
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
+            tx_speed=tx_speed,
+        )
         tx_hash = self.sign_and_send_tx(account, tx)
-        tx_receipt = self.wait_for_tx_receipt(tx_hash)
-        return tx_receipt, tx_hash
+        return tx_hash
```

### Comparing `better_web3-1.3.1/better_web3/contract/__pycache__/contract.cpython-311.pyc` & `better_web3-1.4.0/better_web3/contract/__pycache__/contract.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x12299c64 (Wed Jun 28 12:35:30 2023 UTC)
-files sz: 1217
+moddate:  0xd3beab64 (Mon Jul 10 08:18:27 2023 UTC)
+files sz: 1264
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c066d075a070100640064056c086d095a
-      0a0100640064066c086d0b5a0b6d0c5a0c010065017206640764086c0d6d
-      0e5a0e01000200470064098400640aa6020000ab0200000000000000005a
-      09640b5300
+      0a0100640064066c086d0b5a0b6d0c5a0c0100640064076c0d6d0e5a0e01
+      0065017206640864096c0f6d105a10010002004700640a8400640ba60200
+      00ab0200000000000000005a09640c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('TYPE_CHECKING',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (TYPE_CHECKING)
                 10 STORE_NAME               1 (TYPE_CHECKING)
@@ -54,162 +54,173 @@
                 66 IMPORT_NAME              8 (web3.contract.contract)
                 68 IMPORT_FROM             11 (ContractEvents)
                 70 STORE_NAME              11 (ContractEvents)
                 72 IMPORT_FROM             12 (ContractFunctions)
                 74 STORE_NAME              12 (ContractFunctions)
                 76 POP_TOP
    
-     9          78 LOAD_NAME                1 (TYPE_CHECKING)
-                80 POP_JUMP_FORWARD_IF_FALSE     6 (to 94)
+     8          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               7 (('ABI',))
+                82 IMPORT_NAME             13 (web3.types)
+                84 IMPORT_FROM             14 (ABI)
+                86 STORE_NAME              14 (ABI)
+                88 POP_TOP
    
-    10          82 LOAD_CONST               7 (2)
-                84 LOAD_CONST               8 (('Chain',))
-                86 IMPORT_NAME             13 (chain)
-                88 IMPORT_FROM             14 (Chain)
-                90 STORE_NAME              14 (Chain)
-                92 POP_TOP
+    10          90 LOAD_NAME                1 (TYPE_CHECKING)
+                92 POP_JUMP_FORWARD_IF_FALSE     6 (to 106)
    
-    13     >>   94 PUSH_NULL
-                96 LOAD_BUILD_CLASS
-                98 LOAD_CONST               9 (<code object Contract, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 13>)
-               100 MAKE_FUNCTION            0
-               102 LOAD_CONST              10 ('Contract')
-               104 PRECALL                  2
-               108 CALL                     2
-               118 STORE_NAME               9 (Contract)
-               120 LOAD_CONST              11 (None)
-               122 RETURN_VALUE
+    11          94 LOAD_CONST               8 (2)
+                96 LOAD_CONST               9 (('Chain',))
+                98 IMPORT_NAME             15 (chain)
+               100 IMPORT_FROM             16 (Chain)
+               102 STORE_NAME              16 (Chain)
+               104 POP_TOP
+   
+    14     >>  106 PUSH_NULL
+               108 LOAD_BUILD_CLASS
+               110 LOAD_CONST              10 (<code object Contract, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 14>)
+               112 MAKE_FUNCTION            0
+               114 LOAD_CONST              11 ('Contract')
+               116 PRECALL                  2
+               120 CALL                     2
+               130 STORE_NAME               9 (Contract)
+               132 LOAD_CONST              12 (None)
+               134 RETURN_VALUE
    consts
       0
       ('TYPE_CHECKING',)
       ('ChecksumAddress',)
       ('to_checksum_address',)
       ('Web3',)
       ('Contract',)
       ('ContractEvents', 'ContractFunctions')
+      ('ABI',)
       2
       ('Chain',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02640164026403650365047a0700006604640484
             045a05650664056507660264068404a6000000ab0000000000000000005a
             086506640e64078404a6000000ab0000000000000000005a096506640565
-            0a660264088404a6000000ab0000000000000000005a0b65066405650466
-            0264098404a6000000ab0000000000000000005a0c6506640a8400a60000
-            00ab0000000000000000005a0d65066405650e6602640b8404a6000000ab
-            0000000000000000005a0f6506640565106602640c8404a6000000ab0000
-            000000000000005a11640d5300
-          13           0 RESUME                   0
+            0a660264088404a6000000ab0000000000000000005a0b65066405650366
+            0264098404a6000000ab0000000000000000005a0c65066405650d660264
+            0a8404a6000000ab0000000000000000005a0e65066405650f6602640b84
+            04a6000000ab0000000000000000005a106506640565116602640c8404a6
+            000000ab0000000000000000005a12640d5300
+          14           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Contract')
                        8 STORE_NAME               2 (__qualname__)
          
-          14          10 LOAD_CONST               1 ('chain')
+          15          10 LOAD_CONST               1 ('chain')
                       12 LOAD_CONST               2 ('Chain')
                       14 LOAD_CONST               3 ('address')
                       16 LOAD_NAME                3 (ChecksumAddress)
                       18 LOAD_NAME                4 (str)
                       20 BINARY_OP                7 (|)
                       24 BUILD_TUPLE              4
-                      26 LOAD_CONST               4 (<code object __init__, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 14>)
+                      26 LOAD_CONST               4 (<code object __init__, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 15>)
                       28 MAKE_FUNCTION            4 (annotations)
                       30 STORE_NAME               5 (__init__)
          
-          20          32 LOAD_NAME                6 (property)
+          21          32 LOAD_NAME                6 (property)
          
-          21          34 LOAD_CONST               5 ('return')
+          22          34 LOAD_CONST               5 ('return')
                       36 LOAD_NAME                7 (Web3)
                       38 BUILD_TUPLE              2
-                      40 LOAD_CONST               6 (<code object w3, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 20>)
+                      40 LOAD_CONST               6 (<code object w3, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 21>)
                       42 MAKE_FUNCTION            4 (annotations)
          
-          20          44 PRECALL                  0
+          21          44 PRECALL                  0
                       48 CALL                     0
          
-          21          58 STORE_NAME               8 (w3)
+          22          58 STORE_NAME               8 (w3)
          
-          24          60 LOAD_NAME                6 (property)
+          25          60 LOAD_NAME                6 (property)
          
-          25          62 LOAD_CONST              14 (('return', 'Chain'))
-                      64 LOAD_CONST               7 (<code object chain, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 24>)
+          26          62 LOAD_CONST              14 (('return', 'Chain'))
+                      64 LOAD_CONST               7 (<code object chain, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 25>)
                       66 MAKE_FUNCTION            4 (annotations)
          
-          24          68 PRECALL                  0
+          25          68 PRECALL                  0
                       72 CALL                     0
          
-          25          82 STORE_NAME               9 (chain)
+          26          82 STORE_NAME               9 (chain)
          
-          28          84 LOAD_NAME                6 (property)
+          29          84 LOAD_NAME                6 (property)
          
-          29          86 LOAD_CONST               5 ('return')
+          30          86 LOAD_CONST               5 ('return')
                       88 LOAD_NAME               10 (Web3Contract)
                       90 BUILD_TUPLE              2
-                      92 LOAD_CONST               8 (<code object contract, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 28>)
+                      92 LOAD_CONST               8 (<code object contract, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 29>)
                       94 MAKE_FUNCTION            4 (annotations)
          
-          28          96 PRECALL                  0
+          29          96 PRECALL                  0
                      100 CALL                     0
          
-          29         110 STORE_NAME              11 (contract)
+          30         110 STORE_NAME              11 (contract)
          
-          32         112 LOAD_NAME                6 (property)
+          33         112 LOAD_NAME                6 (property)
          
-          33         114 LOAD_CONST               5 ('return')
-                     116 LOAD_NAME                4 (str)
+          34         114 LOAD_CONST               5 ('return')
+                     116 LOAD_NAME                3 (ChecksumAddress)
                      118 BUILD_TUPLE              2
-                     120 LOAD_CONST               9 (<code object address, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 32>)
+                     120 LOAD_CONST               9 (<code object address, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 33>)
                      122 MAKE_FUNCTION            4 (annotations)
          
-          32         124 PRECALL                  0
+          33         124 PRECALL                  0
                      128 CALL                     0
          
-          33         138 STORE_NAME              12 (address)
+          34         138 STORE_NAME              12 (address)
          
-          36         140 LOAD_NAME                6 (property)
+          37         140 LOAD_NAME                6 (property)
          
-          37         142 LOAD_CONST              10 (<code object abi, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 36>)
-                     144 MAKE_FUNCTION            0
+          38         142 LOAD_CONST               5 ('return')
+                     144 LOAD_NAME               13 (ABI)
+                     146 BUILD_TUPLE              2
+                     148 LOAD_CONST              10 (<code object abi, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 37>)
+                     150 MAKE_FUNCTION            4 (annotations)
          
-          36         146 PRECALL                  0
-                     150 CALL                     0
+          37         152 PRECALL                  0
+                     156 CALL                     0
          
-          37         160 STORE_NAME              13 (abi)
+          38         166 STORE_NAME              14 (abi)
          
-          40         162 LOAD_NAME                6 (property)
+          41         168 LOAD_NAME                6 (property)
          
-          41         164 LOAD_CONST               5 ('return')
-                     166 LOAD_NAME               14 (ContractFunctions)
-                     168 BUILD_TUPLE              2
-                     170 LOAD_CONST              11 (<code object functions, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 40>)
-                     172 MAKE_FUNCTION            4 (annotations)
+          42         170 LOAD_CONST               5 ('return')
+                     172 LOAD_NAME               15 (ContractFunctions)
+                     174 BUILD_TUPLE              2
+                     176 LOAD_CONST              11 (<code object functions, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 41>)
+                     178 MAKE_FUNCTION            4 (annotations)
          
-          40         174 PRECALL                  0
-                     178 CALL                     0
+          41         180 PRECALL                  0
+                     184 CALL                     0
          
-          41         188 STORE_NAME              15 (functions)
+          42         194 STORE_NAME              16 (functions)
          
-          44         190 LOAD_NAME                6 (property)
+          45         196 LOAD_NAME                6 (property)
          
-          45         192 LOAD_CONST               5 ('return')
-                     194 LOAD_NAME               16 (ContractEvents)
-                     196 BUILD_TUPLE              2
-                     198 LOAD_CONST              12 (<code object events, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 44>)
-                     200 MAKE_FUNCTION            4 (annotations)
+          46         198 LOAD_CONST               5 ('return')
+                     200 LOAD_NAME               17 (ContractEvents)
+                     202 BUILD_TUPLE              2
+                     204 LOAD_CONST              12 (<code object events, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 45>)
+                     206 MAKE_FUNCTION            4 (annotations)
          
-          44         202 PRECALL                  0
-                     206 CALL                     0
+          45         208 PRECALL                  0
+                     212 CALL                     0
          
-          45         216 STORE_NAME              17 (events)
-                     218 LOAD_CONST              13 (None)
-                     220 RETURN_VALUE
+          46         222 STORE_NAME              18 (events)
+                     224 LOAD_CONST              13 (None)
+                     226 RETURN_VALUE
          consts
             'Contract'
             'chain'
             'Chain'
             'address'
             code
                argcount  : 4
@@ -219,34 +230,34 @@
                code
                   0x97007401000000000000000000007c02740200000000000000000000a6
                   020000ab020000000000000000720f7405000000000000000000007c02a6
                   010000ab0100000000000000007d027c017c005f0300000000000000007c
                   006a0300000000000000006a0400000000000000006a0500000000000000
                   00a00600000000000000000000000000000000000000007c027c03ac01a6
                   020000ab0200000000000000007c005f07000000000000000064005300
-                14           0 RESUME                   0
+                15           0 RESUME                   0
                
-                15           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                16           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                2 (address)
                             16 LOAD_GLOBAL              2 (str)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE    15 (to 74)
                
-                16          44 LOAD_GLOBAL              5 (NULL + to_checksum_address)
+                17          44 LOAD_GLOBAL              5 (NULL + to_checksum_address)
                             56 LOAD_FAST                2 (address)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               2 (address)
                
-                17     >>   74 LOAD_FAST                1 (chain)
+                18     >>   74 LOAD_FAST                1 (chain)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (_chain)
                
-                18          88 LOAD_FAST                0 (self)
+                19          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                3 (_chain)
                            100 LOAD_ATTR                4 (w3)
                            110 LOAD_ATTR                5 (eth)
                            120 LOAD_METHOD              6 (contract)
                            142 LOAD_FAST                2 (address)
                            144 LOAD_FAST                3 (abi)
                            146 KW_NAMES                 1
@@ -261,184 +272,184 @@
                   ('abi',)
                names      ('isinstance', 'str', 'to_checksum_address', '_chain', 'w3', 'eth', 'contract', '_contract')
                varnames   ('self', 'chain', 'address', 'abi')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       '__init__'
-               firstlineno 14
+               firstlineno 15
                lnotab 0x02012a011e010e01
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                20           0 RESUME                   0
+                21           0 RESUME                   0
                
-                22           2 LOAD_FAST                0 (self)
+                23           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_chain)
                             14 LOAD_ATTR                1 (w3)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_chain', 'w3')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'w3'
-               firstlineno 20
+               firstlineno 21
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-                24           0 RESUME                   0
+                25           0 RESUME                   0
                
-                26           2 LOAD_FAST                0 (self)
+                27           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_chain)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_chain',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'chain'
-               firstlineno 24
+               firstlineno 25
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-                28           0 RESUME                   0
+                29           0 RESUME                   0
                
-                30           2 LOAD_FAST                0 (self)
+                31           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_contract',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'contract'
-               firstlineno 28
+               firstlineno 29
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                32           0 RESUME                   0
+                33           0 RESUME                   0
                
-                34           2 LOAD_FAST                0 (self)
+                35           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 LOAD_ATTR                1 (address)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_contract', 'address')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'address'
-               firstlineno 32
+               firstlineno 33
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                36           0 RESUME                   0
+                37           0 RESUME                   0
                
-                38           2 LOAD_FAST                0 (self)
+                39           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 LOAD_ATTR                1 (abi)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_contract', 'abi')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'abi'
-               firstlineno 36
+               firstlineno 37
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                40           0 RESUME                   0
+                41           0 RESUME                   0
                
-                42           2 LOAD_FAST                0 (self)
+                43           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 LOAD_ATTR                1 (functions)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_contract', 'functions')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'functions'
-               firstlineno 40
+               firstlineno 41
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                44           0 RESUME                   0
+                45           0 RESUME                   0
                
-                46           2 LOAD_FAST                0 (self)
+                47           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 LOAD_ATTR                1 (events)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_contract', 'events')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'events'
-               firstlineno 44
+               firstlineno 45
                lnotab 0x0202
             None
             ('return', 'Chain')
-         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'property', 'Web3', 'w3', 'chain', 'Web3Contract', 'contract', 'address', 'abi', 'ContractFunctions', 'functions', 'ContractEvents', 'events')
+         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'property', 'Web3', 'w3', 'chain', 'Web3Contract', 'contract', 'address', 'ABI', 'abi', 'ContractFunctions', 'functions', 'ContractEvents', 'events')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
          name       'Contract'
-         firstlineno 13
+         firstlineno 14
          lnotab
             0x0a01160602010aff0e010203020106ff0e01020302010aff0e01020302
-            010aff0e010203020104ff0e01020302010aff0e01020302010aff0e01
+            010aff0e01020302010aff0e01020302010aff0e01020302010aff0e01
       'Contract'
       None
-   names      ('typing', 'TYPE_CHECKING', 'eth_typing', 'ChecksumAddress', 'eth_utils', 'to_checksum_address', 'web3', 'Web3', 'web3.contract.contract', 'Contract', 'Web3Contract', 'ContractEvents', 'ContractFunctions', 'chain', 'Chain')
+   names      ('typing', 'TYPE_CHECKING', 'eth_typing', 'ChecksumAddress', 'eth_utils', 'to_checksum_address', 'web3', 'Web3', 'web3.contract.contract', 'Contract', 'Web3Contract', 'ContractEvents', 'ContractFunctions', 'web3.types', 'ABI', 'chain', 'Chain')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c020c010c010c010c01100204010c03
+   lnotab 0x00ff02010c020c010c010c010c0110010c0204010c03
```

### Comparing `better_web3-1.3.1/better_web3/contract/__pycache__/erc20.cpython-311.pyc` & `better_web3-1.4.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,117 +1,115 @@
 magic:    0xa70d0d0a
-moddate:  0xb6919464 (Thu Jun 22 18:23:50 2023 UTC)
-files sz: 1749
+moddate:  0x7571a864 (Fri Jul  7 20:11:33 2023 UTC)
+files sz: 1747
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a020100640064026c036d045a046d
-      055a050100640064036c066d075a070100640464056c086d095a09010064
-      0464066c0a6d0b5a0b0100640764086c0c6d0d5a0d010065017206640764
-      096c0e6d0f5a0f010002004700640a8400640b650ba6030000ab03000000
+      0x9700640064016c006d015a010100640064026c026d035a036d045a0401
+      00640064036c056d065a066d075a070100640064046c086d095a09010064
+      0564066c0a6d0b5a0b0100640564076c0c6d0d5a0d010065037206640864
+      096c0e6d0f5a0f010002004700640a8400640b650da6030000ab03000000
       00000000005a10640c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('TYPE_CHECKING', 'Iterable'))
-                 6 IMPORT_NAME              0 (typing)
-                 8 IMPORT_FROM              1 (TYPE_CHECKING)
-                10 STORE_NAME               1 (TYPE_CHECKING)
-                12 IMPORT_FROM              2 (Iterable)
-                14 STORE_NAME               2 (Iterable)
-                16 POP_TOP
+                 4 LOAD_CONST               1 (('cached_property',))
+                 6 IMPORT_NAME              0 (functools)
+                 8 IMPORT_FROM              1 (cached_property)
+                10 STORE_NAME               1 (cached_property)
+                12 POP_TOP
    
-     3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('ChecksumAddress', 'BlockIdentifier'))
-                22 IMPORT_NAME              3 (eth_typing)
-                24 IMPORT_FROM              4 (ChecksumAddress)
-                26 STORE_NAME               4 (ChecksumAddress)
-                28 IMPORT_FROM              5 (BlockIdentifier)
-                30 STORE_NAME               5 (BlockIdentifier)
-                32 POP_TOP
+     2          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('TYPE_CHECKING', 'Iterable'))
+                18 IMPORT_NAME              2 (typing)
+                20 IMPORT_FROM              3 (TYPE_CHECKING)
+                22 STORE_NAME               3 (TYPE_CHECKING)
+                24 IMPORT_FROM              4 (Iterable)
+                26 STORE_NAME               4 (Iterable)
+                28 POP_TOP
    
-     4          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (('Wei',))
-                38 IMPORT_NAME              6 (web3.types)
-                40 IMPORT_FROM              7 (Wei)
-                42 STORE_NAME               7 (Wei)
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('ChecksumAddress', 'BlockIdentifier'))
+                34 IMPORT_NAME              5 (eth_typing)
+                36 IMPORT_FROM              6 (ChecksumAddress)
+                38 STORE_NAME               6 (ChecksumAddress)
+                40 IMPORT_FROM              7 (BlockIdentifier)
+                42 STORE_NAME               7 (BlockIdentifier)
                 44 POP_TOP
    
-     6          46 LOAD_CONST               4 (1)
-                48 LOAD_CONST               5 (('ERC20_ABI',))
-                50 IMPORT_NAME              8 (abi)
-                52 IMPORT_FROM              9 (ERC20_ABI)
-                54 STORE_NAME               9 (ERC20_ABI)
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('Wei',))
+                50 IMPORT_NAME              8 (web3.types)
+                52 IMPORT_FROM              9 (Wei)
+                54 STORE_NAME               9 (Wei)
                 56 POP_TOP
    
-     7          58 LOAD_CONST               4 (1)
-                60 LOAD_CONST               6 (('Contract',))
-                62 IMPORT_NAME             10 (contract)
-                64 IMPORT_FROM             11 (Contract)
-                66 STORE_NAME              11 (Contract)
+     7          58 LOAD_CONST               5 (1)
+                60 LOAD_CONST               6 (('ERC20_ABI',))
+                62 IMPORT_NAME             10 (_abi)
+                64 IMPORT_FROM             11 (ERC20_ABI)
+                66 STORE_NAME              11 (ERC20_ABI)
                 68 POP_TOP
    
-     8          70 LOAD_CONST               7 (2)
-                72 LOAD_CONST               8 (('cache',))
-                74 IMPORT_NAME             12 (utils)
-                76 IMPORT_FROM             13 (cache)
-                78 STORE_NAME              13 (cache)
+     8          70 LOAD_CONST               5 (1)
+                72 LOAD_CONST               7 (('Contract',))
+                74 IMPORT_NAME             12 (contract)
+                76 IMPORT_FROM             13 (Contract)
+                78 STORE_NAME              13 (Contract)
                 80 POP_TOP
    
-    10          82 LOAD_NAME                1 (TYPE_CHECKING)
+    10          82 LOAD_NAME                3 (TYPE_CHECKING)
                 84 POP_JUMP_FORWARD_IF_FALSE     6 (to 98)
    
-    11          86 LOAD_CONST               7 (2)
+    11          86 LOAD_CONST               8 (2)
                 88 LOAD_CONST               9 (('Chain',))
                 90 IMPORT_NAME             14 (chain)
                 92 IMPORT_FROM             15 (Chain)
                 94 STORE_NAME              15 (Chain)
                 96 POP_TOP
    
     14     >>   98 PUSH_NULL
                100 LOAD_BUILD_CLASS
                102 LOAD_CONST              10 (<code object ERC20, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 14>)
                104 MAKE_FUNCTION            0
                106 LOAD_CONST              11 ('ERC20')
-               108 LOAD_NAME               11 (Contract)
+               108 LOAD_NAME               13 (Contract)
                110 PRECALL                  3
                114 CALL                     3
                124 STORE_NAME              16 (ERC20)
                126 LOAD_CONST              12 (None)
                128 RETURN_VALUE
    consts
       0
+      ('cached_property',)
       ('TYPE_CHECKING', 'Iterable')
       ('ChecksumAddress', 'BlockIdentifier')
       ('Wei',)
       1
       ('ERC20_ABI',)
       ('Contract',)
       2
-      ('cache',)
       ('Chain',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
             0x8700970065005a0164005a020900640f640264036404650365047a0700
-            006604880066016405840d5a056506650764066504660264078404a60000
-            00ab000000000000000000a6000000ab0000000000000000005a08650665
-            0764066504660264088404a6000000ab000000000000000000a6000000ab
-            0000000000000000005a09650665076406650a660264098404a6000000ab
-            000000000000000000a6000000ab0000000000000000005a0b0900641064
-            046503640b650c6406650d6606640c84055a0e09006410640d650f650319
-            000000000000000000640b650c6406650f65106504650365047a07000085
-            026504650d85026602190000000000000000001900000000000000000066
-            06640e84055a11880078015a125300
+            006604880066016405840d5a05650664066504660264078404a6000000ab
+            0000000000000000005a07650664066504660264088404a6000000ab0000
+            000000000000005a08650664066509660264098404a6000000ab00000000
+            00000000005a0a0900641064046503640b650b6406650c6606640c84055a
+            0d09006410640d650e650319000000000000000000640b650b6406650e65
+            0f6504650365047a07000085026504650c85026602190000000000000000
+            00190000000000000000006606640e84055a10880078015a115300
                        0 MAKE_CELL                0 (__class__)
          
           14           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ERC20')
                       10 STORE_NAME               2 (__qualname__)
@@ -132,125 +130,110 @@
           15          30 BUILD_TUPLE              4
                       32 LOAD_CLOSURE             0 (__class__)
                       34 BUILD_TUPLE              1
                       36 LOAD_CONST               5 (<code object __init__, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 15>)
                       38 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       40 STORE_NAME               5 (__init__)
          
-          24          42 LOAD_NAME                6 (property)
+          24          42 LOAD_NAME                6 (cached_property)
          
-          25          44 LOAD_NAME                7 (cache)
+          25          44 LOAD_CONST               6 ('return')
+                      46 LOAD_NAME                4 (str)
+                      48 BUILD_TUPLE              2
+                      50 LOAD_CONST               7 (<code object name, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 24>)
+                      52 MAKE_FUNCTION            4 (annotations)
          
-          26          46 LOAD_CONST               6 ('return')
-                      48 LOAD_NAME                4 (str)
-                      50 BUILD_TUPLE              2
-                      52 LOAD_CONST               7 (<code object name, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 24>)
-                      54 MAKE_FUNCTION            4 (annotations)
+          24          54 PRECALL                  0
+                      58 CALL                     0
          
-          25          56 PRECALL                  0
-                      60 CALL                     0
+          25          68 STORE_NAME               7 (name)
          
-          24          70 PRECALL                  0
-                      74 CALL                     0
+          28          70 LOAD_NAME                6 (cached_property)
          
-          26          84 STORE_NAME               8 (name)
+          29          72 LOAD_CONST               6 ('return')
+                      74 LOAD_NAME                4 (str)
+                      76 BUILD_TUPLE              2
+                      78 LOAD_CONST               8 (<code object symbol, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 28>)
+                      80 MAKE_FUNCTION            4 (annotations)
          
-          29          86 LOAD_NAME                6 (property)
+          28          82 PRECALL                  0
+                      86 CALL                     0
          
-          30          88 LOAD_NAME                7 (cache)
+          29          96 STORE_NAME               8 (symbol)
          
-          31          90 LOAD_CONST               6 ('return')
-                      92 LOAD_NAME                4 (str)
-                      94 BUILD_TUPLE              2
-                      96 LOAD_CONST               8 (<code object symbol, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 29>)
-                      98 MAKE_FUNCTION            4 (annotations)
+          32          98 LOAD_NAME                6 (cached_property)
          
-          30         100 PRECALL                  0
-                     104 CALL                     0
+          33         100 LOAD_CONST               6 ('return')
+                     102 LOAD_NAME                9 (int)
+                     104 BUILD_TUPLE              2
+                     106 LOAD_CONST               9 (<code object decimals, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 32>)
+                     108 MAKE_FUNCTION            4 (annotations)
          
-          29         114 PRECALL                  0
-                     118 CALL                     0
+          32         110 PRECALL                  0
+                     114 CALL                     0
          
-          31         128 STORE_NAME               9 (symbol)
+          33         124 STORE_NAME              10 (decimals)
          
-          34         130 LOAD_NAME                6 (property)
+          39         126 NOP
          
-          35         132 LOAD_NAME                7 (cache)
+          36         128 LOAD_CONST              16 (('latest',))
+                     130 LOAD_CONST               4 ('address')
          
-          36         134 LOAD_CONST               6 ('return')
-                     136 LOAD_NAME               10 (int)
-                     138 BUILD_TUPLE              2
-                     140 LOAD_CONST               9 (<code object decimals, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 34>)
-                     142 MAKE_FUNCTION            4 (annotations)
+          38         132 LOAD_NAME                3 (ChecksumAddress)
          
-          35         144 PRECALL                  0
-                     148 CALL                     0
+          36         134 LOAD_CONST              11 ('block_identifier')
          
-          34         158 PRECALL                  0
-                     162 CALL                     0
+          39         136 LOAD_NAME               11 (BlockIdentifier)
          
-          36         172 STORE_NAME              11 (decimals)
+          36         138 LOAD_CONST               6 ('return')
          
-          42         174 NOP
+          40         140 LOAD_NAME               12 (Wei)
          
-          39         176 LOAD_CONST              16 (('latest',))
-                     178 LOAD_CONST               4 ('address')
+          36         142 BUILD_TUPLE              6
+                     144 LOAD_CONST              12 (<code object get_balance, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 36>)
+                     146 MAKE_FUNCTION            5 (defaults, annotations)
+                     148 STORE_NAME              13 (get_balance)
          
-          41         180 LOAD_NAME                3 (ChecksumAddress)
+          47         150 NOP
          
-          39         182 LOAD_CONST              11 ('block_identifier')
+          44         152 LOAD_CONST              16 (('latest',))
+                     154 LOAD_CONST              13 ('addresses')
          
-          42         184 LOAD_NAME               12 (BlockIdentifier)
+          46         156 LOAD_NAME               14 (Iterable)
+                     158 LOAD_NAME                3 (ChecksumAddress)
+                     160 BINARY_SUBSCR
          
-          39         186 LOAD_CONST               6 ('return')
+          44         170 LOAD_CONST              11 ('block_identifier')
          
-          43         188 LOAD_NAME               13 (Wei)
+          47         172 LOAD_NAME               11 (BlockIdentifier)
          
-          39         190 BUILD_TUPLE              6
-                     192 LOAD_CONST              12 (<code object get_balance, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 39>)
-                     194 MAKE_FUNCTION            5 (defaults, annotations)
-                     196 STORE_NAME              14 (get_balance)
+          44         174 LOAD_CONST               6 ('return')
          
-          50         198 NOP
+          49         176 LOAD_NAME               14 (Iterable)
+                     178 LOAD_NAME               15 (dict)
+                     180 LOAD_NAME                4 (str)
+                     182 LOAD_NAME                3 (ChecksumAddress)
+                     184 LOAD_NAME                4 (str)
+                     186 BINARY_OP                7 (|)
+                     190 BUILD_SLICE              2
+                     192 LOAD_NAME                4 (str)
+                     194 LOAD_NAME               12 (Wei)
+                     196 BUILD_SLICE              2
+                     198 BUILD_TUPLE              2
+                     200 BINARY_SUBSCR
+                     210 BINARY_SUBSCR
          
-          47         200 LOAD_CONST              16 (('latest',))
-                     202 LOAD_CONST              13 ('addresses')
-         
-          49         204 LOAD_NAME               15 (Iterable)
-                     206 LOAD_NAME                3 (ChecksumAddress)
-                     208 BINARY_SUBSCR
-         
-          47         218 LOAD_CONST              11 ('block_identifier')
-         
-          50         220 LOAD_NAME               12 (BlockIdentifier)
-         
-          47         222 LOAD_CONST               6 ('return')
-         
-          52         224 LOAD_NAME               15 (Iterable)
-                     226 LOAD_NAME               16 (dict)
-                     228 LOAD_NAME                4 (str)
-                     230 LOAD_NAME                3 (ChecksumAddress)
-                     232 LOAD_NAME                4 (str)
-                     234 BINARY_OP                7 (|)
-                     238 BUILD_SLICE              2
-                     240 LOAD_NAME                4 (str)
-                     242 LOAD_NAME               13 (Wei)
-                     244 BUILD_SLICE              2
-                     246 BUILD_TUPLE              2
-                     248 BINARY_SUBSCR
-                     258 BINARY_SUBSCR
-         
-          47         268 BUILD_TUPLE              6
-                     270 LOAD_CONST              14 (<code object get_balances, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 47>)
-                     272 MAKE_FUNCTION            5 (defaults, annotations)
-                     274 STORE_NAME              17 (get_balances)
-                     276 LOAD_CLOSURE             0 (__class__)
-                     278 COPY                     1
-                     280 STORE_NAME              18 (__classcell__)
-                     282 RETURN_VALUE
+          44         220 BUILD_TUPLE              6
+                     222 LOAD_CONST              14 (<code object get_balances, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 44>)
+                     224 MAKE_FUNCTION            5 (defaults, annotations)
+                     226 STORE_NAME              16 (get_balances)
+                     228 LOAD_CLOSURE             0 (__class__)
+                     230 COPY                     1
+                     232 STORE_NAME              17 (__classcell__)
+                     234 RETURN_VALUE
          consts
             'ERC20'
             None
             'chain'
             'Chain'
             'address'
             code
@@ -302,15 +285,15 @@
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000a00200000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
                 24           0 RESUME                   0
                
-                27           2 LOAD_FAST                0 (self)
+                26           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (functions)
                             14 LOAD_METHOD              1 (name)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 LOAD_METHOD              2 (call)
                             72 PRECALL                  0
                             76 CALL                     0
@@ -320,27 +303,27 @@
                names      ('functions', 'name', 'call')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc20.py'
                name       'name'
                firstlineno 24
-               lnotab 0x0203
+               lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000a00200000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-                29           0 RESUME                   0
+                28           0 RESUME                   0
                
-                32           2 LOAD_FAST                0 (self)
+                30           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (functions)
                             14 LOAD_METHOD              1 (symbol)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 LOAD_METHOD              2 (call)
                             72 PRECALL                  0
                             76 CALL                     0
@@ -349,28 +332,28 @@
                   None
                names      ('functions', 'symbol', 'call')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc20.py'
                name       'symbol'
-               firstlineno 29
-               lnotab 0x0203
+               firstlineno 28
+               lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000a00200000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-                34           0 RESUME                   0
+                32           0 RESUME                   0
                
-                37           2 LOAD_FAST                0 (self)
+                34           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (functions)
                             14 LOAD_METHOD              1 (decimals)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 LOAD_METHOD              2 (call)
                             72 PRECALL                  0
                             76 CALL                     0
@@ -379,55 +362,55 @@
                   None
                names      ('functions', 'decimals', 'call')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc20.py'
                name       'decimals'
-               firstlineno 34
-               lnotab 0x0203
+               firstlineno 32
+               lnotab 0x0202
             'latest'
             'block_identifier'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000a0020000000000
                   0000000000000000000000000000007c02ac01a6010000ab010000000000
                   0000007d037c035300
-                39           0 RESUME                   0
+                36           0 RESUME                   0
                
-                44           2 LOAD_FAST                0 (self)
+                41           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (functions)
                             14 LOAD_METHOD              1 (balanceOf)
                             36 LOAD_FAST                1 (address)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (call)
                             74 LOAD_FAST                2 (block_identifier)
                             76 KW_NAMES                 1
                             78 PRECALL                  1
                             82 CALL                     1
                             92 STORE_FAST               3 (balance)
                
-                45          94 LOAD_FAST                3 (balance)
+                42          94 LOAD_FAST                3 (balance)
                             96 RETURN_VALUE
                consts
                   None
                   ('block_identifier',)
                names      ('functions', 'balanceOf', 'call')
                varnames   ('self', 'address', 'block_identifier', 'balance')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc20.py'
                name       'get_balance'
-               firstlineno 39
+               firstlineno 36
                lnotab 0x02055c01
             'addresses'
             code
                argcount  : 3
                nlocals   : 7
                stacksize : 5
                flags     : 43
@@ -436,88 +419,88 @@
                   006a0100000000000000006a02000000000000000088006601640184087c
                   014400a6000000ab0000000000000000007c02660269007c03a4018e017d
                   047407000000000000000000007c017c04a6020000ab0200000000000000
                   0044005d125c0200007d057d067c057c0664021900000000000000000064
                   039c025600970101008c1364005300
                              0 MAKE_CELL                0 (self)
                
-                47           2 RETURN_GENERATOR
+                44           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                53           8 LOAD_FAST                1 (addresses)
+                50           8 LOAD_FAST                1 (addresses)
                             10 POP_JUMP_FORWARD_IF_TRUE     2 (to 16)
                
-                54          12 BUILD_LIST               0
+                51          12 BUILD_LIST               0
                             14 RETURN_VALUE
                
-                56     >>   16 PUSH_NULL
+                53     >>   16 PUSH_NULL
                             18 LOAD_DEREF               0 (self)
                             20 LOAD_ATTR                0 (chain)
                             30 LOAD_ATTR                1 (batch_request)
                             40 LOAD_ATTR                2 (contract_request)
                
-                57          50 LOAD_CLOSURE             0 (self)
+                54          50 LOAD_CLOSURE             0 (self)
                             52 BUILD_TUPLE              1
-                            54 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 57>)
+                            54 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc20.py", line 54>)
                             56 MAKE_FUNCTION            8 (closure)
                             58 LOAD_FAST                1 (addresses)
                             60 GET_ITER
                             62 PRECALL                  0
                             66 CALL                     0
                
-                58          76 LOAD_FAST                2 (block_identifier)
+                55          76 LOAD_FAST                2 (block_identifier)
                
-                56          78 BUILD_TUPLE              2
+                53          78 BUILD_TUPLE              2
                             80 BUILD_MAP                0
                
-                59          82 LOAD_FAST                3 (kwargs)
+                56          82 LOAD_FAST                3 (kwargs)
                
-                56          84 DICT_MERGE               1
+                53          84 DICT_MERGE               1
                             86 CALL_FUNCTION_EX         1
                             88 STORE_FAST               4 (balances)
                
-                61          90 LOAD_GLOBAL              7 (NULL + zip)
+                58          90 LOAD_GLOBAL              7 (NULL + zip)
                            102 LOAD_FAST                1 (addresses)
                            104 LOAD_FAST                4 (balances)
                            106 PRECALL                  2
                            110 CALL                     2
                            120 GET_ITER
                        >>  122 FOR_ITER                18 (to 160)
                            124 UNPACK_SEQUENCE          2
                            128 STORE_FAST               5 (address)
                            130 STORE_FAST               6 (balance_data)
                
-                62         132 LOAD_FAST                5 (address)
+                59         132 LOAD_FAST                5 (address)
                            134 LOAD_FAST                6 (balance_data)
                            136 LOAD_CONST               2 ('result')
                            138 BINARY_SUBSCR
                            148 LOAD_CONST               3 (('address', 'balance'))
                            150 BUILD_CONST_KEY_MAP      2
                            152 YIELD_VALUE
                            154 RESUME                   1
                            156 POP_TOP
                            158 JUMP_BACKWARD           19 (to 122)
                
-                61     >>  160 LOAD_CONST               0 (None)
+                58     >>  160 LOAD_CONST               0 (None)
                            162 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d1c7d0189026a000000000000000000a001000000
                         00000000000000000000000000000000007c01a6010000ab010000000000
                         00000091028c1d5300
                                    0 COPY_FREE_VARS           1
                      
-                      57           2 RESUME                   0
+                      54           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                28 (to 66)
                                   10 STORE_FAST               1 (address)
                                   12 LOAD_DEREF               2 (self)
                                   14 LOAD_ATTR                0 (functions)
                                   24 LOAD_METHOD              1 (balanceOf)
@@ -530,42 +513,42 @@
                      consts
                      names      ('functions', 'balanceOf')
                      varnames   ('.0', 'address')
                      freevars   ('self',)
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc20.py'
                      name       '<listcomp>'
-                     firstlineno 57
+                     firstlineno 54
                      lnotab 0x
                   'result'
                   ('address', 'balance')
                names      ('chain', 'batch_request', 'contract_request', 'zip')
                varnames   ('self', 'addresses', 'block_identifier', 'kwargs', 'balances', 'address', 'balance_data')
                freevars   ()
                cellvars   ('self',)
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc20.py'
                name       'get_balances'
-               firstlineno 47
+               firstlineno 44
                lnotab 0x08060401040222011a0102fe040302fd06052a011cff
             (None,)
             ('latest',)
-         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'property', 'cache', 'name', 'symbol', 'int', 'decimals', 'BlockIdentifier', 'Wei', 'get_balance', 'Iterable', 'dict', 'get_balances', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'cached_property', 'name', 'symbol', 'int', 'decimals', 'BlockIdentifier', 'Wei', 'get_balance', 'Iterable', 'dict', 'get_balances', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc20.py'
          name       'ERC20'
          firstlineno 14
          lnotab
-            0x0c0502fc040202fe020308fd0c09020102010aff0eff0e020203020102
-            010aff0eff0e020203020102010aff0eff0e02020602fd040202fe020302
-            fd020402fc080b02fd04020efe020302fd02052cfb
+            0x0c0502fc040202fe020308fd0c0902010aff0e01020302010aff0e0102
+            0302010aff0e01020602fd040202fe020302fd020402fc080b02fd04020e
+            fe020302fd02052cfb
       'ERC20'
       None
-   names      ('typing', 'TYPE_CHECKING', 'Iterable', 'eth_typing', 'ChecksumAddress', 'BlockIdentifier', 'web3.types', 'Wei', 'abi', 'ERC20_ABI', 'contract', 'Contract', 'utils', 'cache', 'chain', 'Chain', 'ERC20')
+   names      ('functools', 'cached_property', 'typing', 'TYPE_CHECKING', 'Iterable', 'eth_typing', 'ChecksumAddress', 'BlockIdentifier', 'web3.types', 'Wei', '_abi', 'ERC20_ABI', 'contract', 'Contract', 'chain', 'Chain', 'ERC20')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc20.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201100210010c020c010c010c0204010c03
+   lnotab 0x00ff02010c01100210010c020c010c0204010c03
```

### Comparing `better_web3-1.3.1/better_web3/contract/__pycache__/erc721.cpython-311.pyc` & `better_web3-1.4.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,120 +1,119 @@
 magic:    0xa70d0d0a
-moddate:  0xb6919464 (Thu Jun 22 18:23:50 2023 UTC)
-files sz: 2873
+moddate:  0x7571a864 (Fri Jul  7 20:11:33 2023 UTC)
+files sz: 2876
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a020100640064026c036d045a046d
-      055a050100640064036c066d075a070100640464056c086d095a09010064
-      0464066c0a6d0b5a0b0100640764086c0c6d0d5a0d010065017206640764
-      096c0e6d0f5a0f010002004700640a8400640b650ba6030000ab03000000
+      0x9700640064016c006d015a010100640064026c026d035a036d045a0401
+      00640064036c056d065a066d075a070100640064046c086d095a09010064
+      0564066c0a6d0b5a0b0100640564076c0c6d0d5a0d010065037206640864
+      096c0e6d0f5a0f010002004700640a8400640b650da6030000ab03000000
       00000000005a10640c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('TYPE_CHECKING', 'Iterable'))
-                 6 IMPORT_NAME              0 (typing)
-                 8 IMPORT_FROM              1 (TYPE_CHECKING)
-                10 STORE_NAME               1 (TYPE_CHECKING)
-                12 IMPORT_FROM              2 (Iterable)
-                14 STORE_NAME               2 (Iterable)
-                16 POP_TOP
+                 4 LOAD_CONST               1 (('cached_property',))
+                 6 IMPORT_NAME              0 (functools)
+                 8 IMPORT_FROM              1 (cached_property)
+                10 STORE_NAME               1 (cached_property)
+                12 POP_TOP
    
-     3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('ChecksumAddress', 'BlockIdentifier'))
-                22 IMPORT_NAME              3 (eth_typing)
-                24 IMPORT_FROM              4 (ChecksumAddress)
-                26 STORE_NAME               4 (ChecksumAddress)
-                28 IMPORT_FROM              5 (BlockIdentifier)
-                30 STORE_NAME               5 (BlockIdentifier)
-                32 POP_TOP
+     2          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('TYPE_CHECKING', 'Iterable'))
+                18 IMPORT_NAME              2 (typing)
+                20 IMPORT_FROM              3 (TYPE_CHECKING)
+                22 STORE_NAME               3 (TYPE_CHECKING)
+                24 IMPORT_FROM              4 (Iterable)
+                26 STORE_NAME               4 (Iterable)
+                28 POP_TOP
    
-     4          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (('to_checksum_address',))
-                38 IMPORT_NAME              6 (eth_utils)
-                40 IMPORT_FROM              7 (to_checksum_address)
-                42 STORE_NAME               7 (to_checksum_address)
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('ChecksumAddress', 'BlockIdentifier'))
+                34 IMPORT_NAME              5 (eth_typing)
+                36 IMPORT_FROM              6 (ChecksumAddress)
+                38 STORE_NAME               6 (ChecksumAddress)
+                40 IMPORT_FROM              7 (BlockIdentifier)
+                42 STORE_NAME               7 (BlockIdentifier)
                 44 POP_TOP
    
-     6          46 LOAD_CONST               4 (1)
-                48 LOAD_CONST               5 (('ERC721_ABI',))
-                50 IMPORT_NAME              8 (abi)
-                52 IMPORT_FROM              9 (ERC721_ABI)
-                54 STORE_NAME               9 (ERC721_ABI)
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('to_checksum_address',))
+                50 IMPORT_NAME              8 (eth_utils)
+                52 IMPORT_FROM              9 (to_checksum_address)
+                54 STORE_NAME               9 (to_checksum_address)
                 56 POP_TOP
    
-     7          58 LOAD_CONST               4 (1)
-                60 LOAD_CONST               6 (('Contract',))
-                62 IMPORT_NAME             10 (contract)
-                64 IMPORT_FROM             11 (Contract)
-                66 STORE_NAME              11 (Contract)
+     7          58 LOAD_CONST               5 (1)
+                60 LOAD_CONST               6 (('ERC721_ABI',))
+                62 IMPORT_NAME             10 (_abi)
+                64 IMPORT_FROM             11 (ERC721_ABI)
+                66 STORE_NAME              11 (ERC721_ABI)
                 68 POP_TOP
    
-     8          70 LOAD_CONST               7 (2)
-                72 LOAD_CONST               8 (('cache',))
-                74 IMPORT_NAME             12 (utils)
-                76 IMPORT_FROM             13 (cache)
-                78 STORE_NAME              13 (cache)
+     8          70 LOAD_CONST               5 (1)
+                72 LOAD_CONST               7 (('Contract',))
+                74 IMPORT_NAME             12 (contract)
+                76 IMPORT_FROM             13 (Contract)
+                78 STORE_NAME              13 (Contract)
                 80 POP_TOP
    
-    10          82 LOAD_NAME                1 (TYPE_CHECKING)
+    10          82 LOAD_NAME                3 (TYPE_CHECKING)
                 84 POP_JUMP_FORWARD_IF_FALSE     6 (to 98)
    
-    11          86 LOAD_CONST               7 (2)
+    11          86 LOAD_CONST               8 (2)
                 88 LOAD_CONST               9 (('Chain',))
                 90 IMPORT_NAME             14 (chain)
                 92 IMPORT_FROM             15 (Chain)
                 94 STORE_NAME              15 (Chain)
                 96 POP_TOP
    
     14     >>   98 PUSH_NULL
                100 LOAD_BUILD_CLASS
                102 LOAD_CONST              10 (<code object ERC721, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 14>)
                104 MAKE_FUNCTION            0
                106 LOAD_CONST              11 ('ERC721')
-               108 LOAD_NAME               11 (Contract)
+               108 LOAD_NAME               13 (Contract)
                110 PRECALL                  3
                114 CALL                     3
                124 STORE_NAME              16 (ERC721)
                126 LOAD_CONST              12 (None)
                128 RETURN_VALUE
    consts
       0
+      ('cached_property',)
       ('TYPE_CHECKING', 'Iterable')
       ('ChecksumAddress', 'BlockIdentifier')
       ('to_checksum_address',)
       1
       ('ERC721_ABI',)
       ('Contract',)
       2
-      ('cache',)
       ('Chain',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
             0x8700970065005a0164005a0209006411640264036404650365047a0700
-            006604880066016405840d5a056506650764066504660264078404a60000
-            00ab000000000000000000a6000000ab0000000000000000005a08650665
-            0764066504660264088404a6000000ab000000000000000000a6000000ab
-            0000000000000000005a090900641264046503640a650a6406650b660664
-            0b84055a0c09006412640c650d650319000000000000000000640a650a64
-            06650d650e6504650385026504650b850266021900000000000000000019
-            0000000000000000006606640d84055a0f09006412640e650d650b190000
-            00000000000000640a650a6406650d650e6504650b850265046503850266
-            0219000000000000000000190000000000000000006606640f84055a1009
-            006412640e650d650b19000000000000000000640a650a6406650d650e65
-            04650b850265046504850266021900000000000000000019000000000000
-            0000006606641084055a11880078015a125300
+            006604880066016405840d5a05650664066504660264078404a6000000ab
+            0000000000000000005a07650664066504660264088404a6000000ab0000
+            000000000000005a080900641264046503640a65096406650a6606640b84
+            055a0b09006412640c650c650319000000000000000000640a6509640665
+            0c650d6504650385026504650a8502660219000000000000000000190000
+            000000000000006606640d84055a0e09006412640e650c650a1900000000
+            0000000000640a65096406650c650d6504650a8502650465038502660219
+            000000000000000000190000000000000000006606640f84055a0f090064
+            12640e650c650a19000000000000000000640a65096406650c650d650465
+            0a8502650465048502660219000000000000000000190000000000000000
+            006606641084055a10880078015a115300
                        0 MAKE_CELL                0 (__class__)
          
           14           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ERC721')
                       10 STORE_NAME               2 (__qualname__)
@@ -135,169 +134,159 @@
           15          30 BUILD_TUPLE              4
                       32 LOAD_CLOSURE             0 (__class__)
                       34 BUILD_TUPLE              1
                       36 LOAD_CONST               5 (<code object __init__, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 15>)
                       38 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       40 STORE_NAME               5 (__init__)
          
-          24          42 LOAD_NAME                6 (property)
+          24          42 LOAD_NAME                6 (cached_property)
          
-          25          44 LOAD_NAME                7 (cache)
+          25          44 LOAD_CONST               6 ('return')
+                      46 LOAD_NAME                4 (str)
+                      48 BUILD_TUPLE              2
+                      50 LOAD_CONST               7 (<code object name, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 24>)
+                      52 MAKE_FUNCTION            4 (annotations)
          
-          26          46 LOAD_CONST               6 ('return')
-                      48 LOAD_NAME                4 (str)
-                      50 BUILD_TUPLE              2
-                      52 LOAD_CONST               7 (<code object name, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 24>)
-                      54 MAKE_FUNCTION            4 (annotations)
+          24          54 PRECALL                  0
+                      58 CALL                     0
          
-          25          56 PRECALL                  0
-                      60 CALL                     0
+          25          68 STORE_NAME               7 (name)
          
-          24          70 PRECALL                  0
-                      74 CALL                     0
+          28          70 LOAD_NAME                6 (cached_property)
          
-          26          84 STORE_NAME               8 (name)
+          29          72 LOAD_CONST               6 ('return')
+                      74 LOAD_NAME                4 (str)
+                      76 BUILD_TUPLE              2
+                      78 LOAD_CONST               8 (<code object symbol, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 28>)
+                      80 MAKE_FUNCTION            4 (annotations)
          
-          29          86 LOAD_NAME                6 (property)
+          28          82 PRECALL                  0
+                      86 CALL                     0
          
-          30          88 LOAD_NAME                7 (cache)
+          29          96 STORE_NAME               8 (symbol)
          
-          31          90 LOAD_CONST               6 ('return')
-                      92 LOAD_NAME                4 (str)
-                      94 BUILD_TUPLE              2
-                      96 LOAD_CONST               8 (<code object symbol, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 29>)
-                      98 MAKE_FUNCTION            4 (annotations)
+          35          98 NOP
          
-          30         100 PRECALL                  0
-                     104 CALL                     0
+          32         100 LOAD_CONST              18 (('latest',))
+                     102 LOAD_CONST               4 ('address')
          
-          29         114 PRECALL                  0
-                     118 CALL                     0
+          34         104 LOAD_NAME                3 (ChecksumAddress)
          
-          31         128 STORE_NAME               9 (symbol)
+          32         106 LOAD_CONST              10 ('block_identifier')
          
-          37         130 NOP
+          35         108 LOAD_NAME                9 (BlockIdentifier)
          
-          34         132 LOAD_CONST              18 (('latest',))
-                     134 LOAD_CONST               4 ('address')
+          32         110 LOAD_CONST               6 ('return')
          
-          36         136 LOAD_NAME                3 (ChecksumAddress)
+          36         112 LOAD_NAME               10 (int)
          
-          34         138 LOAD_CONST              10 ('block_identifier')
+          32         114 BUILD_TUPLE              6
+                     116 LOAD_CONST              11 (<code object get_balance, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 32>)
+                     118 MAKE_FUNCTION            5 (defaults, annotations)
+                     120 STORE_NAME              11 (get_balance)
          
-          37         140 LOAD_NAME               10 (BlockIdentifier)
+          42         122 NOP
          
-          34         142 LOAD_CONST               6 ('return')
+          39         124 LOAD_CONST              18 (('latest',))
+                     126 LOAD_CONST              12 ('addresses')
          
-          38         144 LOAD_NAME               11 (int)
+          41         128 LOAD_NAME               12 (Iterable)
+                     130 LOAD_NAME                3 (ChecksumAddress)
+                     132 BINARY_SUBSCR
          
-          34         146 BUILD_TUPLE              6
-                     148 LOAD_CONST              11 (<code object get_balance, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 34>)
-                     150 MAKE_FUNCTION            5 (defaults, annotations)
-                     152 STORE_NAME              12 (get_balance)
+          39         142 LOAD_CONST              10 ('block_identifier')
          
-          44         154 NOP
+          42         144 LOAD_NAME                9 (BlockIdentifier)
          
-          41         156 LOAD_CONST              18 (('latest',))
-                     158 LOAD_CONST              12 ('addresses')
+          39         146 LOAD_CONST               6 ('return')
          
-          43         160 LOAD_NAME               13 (Iterable)
-                     162 LOAD_NAME                3 (ChecksumAddress)
-                     164 BINARY_SUBSCR
+          44         148 LOAD_NAME               12 (Iterable)
+                     150 LOAD_NAME               13 (dict)
+                     152 LOAD_NAME                4 (str)
+                     154 LOAD_NAME                3 (ChecksumAddress)
+                     156 BUILD_SLICE              2
+                     158 LOAD_NAME                4 (str)
+                     160 LOAD_NAME               10 (int)
+                     162 BUILD_SLICE              2
+                     164 BUILD_TUPLE              2
+                     166 BINARY_SUBSCR
+                     176 BINARY_SUBSCR
          
-          41         174 LOAD_CONST              10 ('block_identifier')
+          39         186 BUILD_TUPLE              6
+                     188 LOAD_CONST              13 (<code object get_balances, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 39>)
+                     190 MAKE_FUNCTION            5 (defaults, annotations)
+                     192 STORE_NAME              14 (get_balances)
          
-          44         176 LOAD_NAME               10 (BlockIdentifier)
+          59         194 NOP
          
-          41         178 LOAD_CONST               6 ('return')
+          56         196 LOAD_CONST              18 (('latest',))
+                     198 LOAD_CONST              14 ('token_ids')
          
-          46         180 LOAD_NAME               13 (Iterable)
-                     182 LOAD_NAME               14 (dict)
-                     184 LOAD_NAME                4 (str)
-                     186 LOAD_NAME                3 (ChecksumAddress)
-                     188 BUILD_SLICE              2
-                     190 LOAD_NAME                4 (str)
-                     192 LOAD_NAME               11 (int)
-                     194 BUILD_SLICE              2
-                     196 BUILD_TUPLE              2
-                     198 BINARY_SUBSCR
-                     208 BINARY_SUBSCR
+          58         200 LOAD_NAME               12 (Iterable)
+                     202 LOAD_NAME               10 (int)
+                     204 BINARY_SUBSCR
          
-          41         218 BUILD_TUPLE              6
-                     220 LOAD_CONST              13 (<code object get_balances, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 41>)
-                     222 MAKE_FUNCTION            5 (defaults, annotations)
-                     224 STORE_NAME              15 (get_balances)
+          56         214 LOAD_CONST              10 ('block_identifier')
          
-          61         226 NOP
+          59         216 LOAD_NAME                9 (BlockIdentifier)
          
-          58         228 LOAD_CONST              18 (('latest',))
-                     230 LOAD_CONST              14 ('token_ids')
+          56         218 LOAD_CONST               6 ('return')
          
-          60         232 LOAD_NAME               13 (Iterable)
-                     234 LOAD_NAME               11 (int)
-                     236 BINARY_SUBSCR
+          61         220 LOAD_NAME               12 (Iterable)
+                     222 LOAD_NAME               13 (dict)
+                     224 LOAD_NAME                4 (str)
+                     226 LOAD_NAME               10 (int)
+                     228 BUILD_SLICE              2
+                     230 LOAD_NAME                4 (str)
+                     232 LOAD_NAME                3 (ChecksumAddress)
+                     234 BUILD_SLICE              2
+                     236 BUILD_TUPLE              2
+                     238 BINARY_SUBSCR
+                     248 BINARY_SUBSCR
          
-          58         246 LOAD_CONST              10 ('block_identifier')
+          56         258 BUILD_TUPLE              6
+                     260 LOAD_CONST              15 (<code object get_owners, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 56>)
+                     262 MAKE_FUNCTION            5 (defaults, annotations)
+                     264 STORE_NAME              15 (get_owners)
          
-          61         248 LOAD_NAME               10 (BlockIdentifier)
+          76         266 NOP
          
-          58         250 LOAD_CONST               6 ('return')
+          73         268 LOAD_CONST              18 (('latest',))
+                     270 LOAD_CONST              14 ('token_ids')
          
-          63         252 LOAD_NAME               13 (Iterable)
-                     254 LOAD_NAME               14 (dict)
-                     256 LOAD_NAME                4 (str)
-                     258 LOAD_NAME               11 (int)
-                     260 BUILD_SLICE              2
-                     262 LOAD_NAME                4 (str)
-                     264 LOAD_NAME                3 (ChecksumAddress)
-                     266 BUILD_SLICE              2
-                     268 BUILD_TUPLE              2
-                     270 BINARY_SUBSCR
-                     280 BINARY_SUBSCR
+          75         272 LOAD_NAME               12 (Iterable)
+                     274 LOAD_NAME               10 (int)
+                     276 BINARY_SUBSCR
          
-          58         290 BUILD_TUPLE              6
-                     292 LOAD_CONST              15 (<code object get_owners, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 58>)
-                     294 MAKE_FUNCTION            5 (defaults, annotations)
-                     296 STORE_NAME              16 (get_owners)
+          73         286 LOAD_CONST              10 ('block_identifier')
          
-          78         298 NOP
+          76         288 LOAD_NAME                9 (BlockIdentifier)
          
-          75         300 LOAD_CONST              18 (('latest',))
-                     302 LOAD_CONST              14 ('token_ids')
+          73         290 LOAD_CONST               6 ('return')
          
-          77         304 LOAD_NAME               13 (Iterable)
-                     306 LOAD_NAME               11 (int)
-                     308 BINARY_SUBSCR
+          78         292 LOAD_NAME               12 (Iterable)
+                     294 LOAD_NAME               13 (dict)
+                     296 LOAD_NAME                4 (str)
+                     298 LOAD_NAME               10 (int)
+                     300 BUILD_SLICE              2
+                     302 LOAD_NAME                4 (str)
+                     304 LOAD_NAME                4 (str)
+                     306 BUILD_SLICE              2
+                     308 BUILD_TUPLE              2
+                     310 BINARY_SUBSCR
+                     320 BINARY_SUBSCR
          
-          75         318 LOAD_CONST              10 ('block_identifier')
-         
-          78         320 LOAD_NAME               10 (BlockIdentifier)
-         
-          75         322 LOAD_CONST               6 ('return')
-         
-          80         324 LOAD_NAME               13 (Iterable)
-                     326 LOAD_NAME               14 (dict)
-                     328 LOAD_NAME                4 (str)
-                     330 LOAD_NAME               11 (int)
-                     332 BUILD_SLICE              2
-                     334 LOAD_NAME                4 (str)
-                     336 LOAD_NAME                4 (str)
-                     338 BUILD_SLICE              2
-                     340 BUILD_TUPLE              2
-                     342 BINARY_SUBSCR
-                     352 BINARY_SUBSCR
-         
-          75         362 BUILD_TUPLE              6
-                     364 LOAD_CONST              16 (<code object get_token_uris, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 75>)
-                     366 MAKE_FUNCTION            5 (defaults, annotations)
-                     368 STORE_NAME              17 (get_token_uris)
-                     370 LOAD_CLOSURE             0 (__class__)
-                     372 COPY                     1
-                     374 STORE_NAME              18 (__classcell__)
-                     376 RETURN_VALUE
+          73         330 BUILD_TUPLE              6
+                     332 LOAD_CONST              16 (<code object get_token_uris, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 73>)
+                     334 MAKE_FUNCTION            5 (defaults, annotations)
+                     336 STORE_NAME              16 (get_token_uris)
+                     338 LOAD_CLOSURE             0 (__class__)
+                     340 COPY                     1
+                     342 STORE_NAME              17 (__classcell__)
+                     344 RETURN_VALUE
          consts
             'ERC721'
             None
             'chain'
             'Chain'
             'address'
             code
@@ -349,15 +338,15 @@
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000a00200000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
                 24           0 RESUME                   0
                
-                27           2 LOAD_FAST                0 (self)
+                26           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (functions)
                             14 LOAD_METHOD              1 (name)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 LOAD_METHOD              2 (call)
                             72 PRECALL                  0
                             76 CALL                     0
@@ -367,27 +356,27 @@
                names      ('functions', 'name', 'call')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                name       'name'
                firstlineno 24
-               lnotab 0x0203
+               lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000a00200000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-                29           0 RESUME                   0
+                28           0 RESUME                   0
                
-                32           2 LOAD_FAST                0 (self)
+                30           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (functions)
                             14 LOAD_METHOD              1 (symbol)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 LOAD_METHOD              2 (call)
                             72 PRECALL                  0
                             76 CALL                     0
@@ -396,31 +385,31 @@
                   None
                names      ('functions', 'symbol', 'call')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                name       'symbol'
-               firstlineno 29
-               lnotab 0x0203
+               firstlineno 28
+               lnotab 0x0202
             'latest'
             'block_identifier'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000a0020000000000
                   0000000000000000000000000000007c02ac01a6010000ab010000000000
                   0000005300
-                34           0 RESUME                   0
+                32           0 RESUME                   0
                
-                39           2 LOAD_FAST                0 (self)
+                37           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (functions)
                             14 LOAD_METHOD              1 (balanceOf)
                             36 LOAD_FAST                1 (address)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (call)
                             74 LOAD_FAST                2 (block_identifier)
@@ -433,15 +422,15 @@
                   ('block_identifier',)
                names      ('functions', 'balanceOf', 'call')
                varnames   ('self', 'address', 'block_identifier')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                name       'get_balance'
-               firstlineno 34
+               firstlineno 32
                lnotab 0x0205
             'addresses'
             code
                argcount  : 3
                nlocals   : 7
                stacksize : 5
                flags     : 43
@@ -450,88 +439,88 @@
                   006a0100000000000000006a02000000000000000088006601640184087c
                   014400a6000000ab0000000000000000007c02660269007c03a4018e017d
                   047407000000000000000000007c017c04a6020000ab0200000000000000
                   0044005d125c0200007d057d067c057c0664021900000000000000000064
                   039c025600970101008c1364005300
                              0 MAKE_CELL                0 (self)
                
-                41           2 RETURN_GENERATOR
+                39           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                47           8 LOAD_FAST                1 (addresses)
+                45           8 LOAD_FAST                1 (addresses)
                             10 POP_JUMP_FORWARD_IF_TRUE     2 (to 16)
                
-                48          12 BUILD_LIST               0
+                46          12 BUILD_LIST               0
                             14 RETURN_VALUE
                
-                50     >>   16 PUSH_NULL
+                48     >>   16 PUSH_NULL
                             18 LOAD_DEREF               0 (self)
                             20 LOAD_ATTR                0 (chain)
                             30 LOAD_ATTR                1 (batch_request)
                             40 LOAD_ATTR                2 (contract_request)
                
-                51          50 LOAD_CLOSURE             0 (self)
+                49          50 LOAD_CLOSURE             0 (self)
                             52 BUILD_TUPLE              1
-                            54 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 51>)
+                            54 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 49>)
                             56 MAKE_FUNCTION            8 (closure)
                             58 LOAD_FAST                1 (addresses)
                             60 GET_ITER
                             62 PRECALL                  0
                             66 CALL                     0
                
-                52          76 LOAD_FAST                2 (block_identifier)
+                50          76 LOAD_FAST                2 (block_identifier)
                
-                50          78 BUILD_TUPLE              2
+                48          78 BUILD_TUPLE              2
                             80 BUILD_MAP                0
                
-                53          82 LOAD_FAST                3 (kwargs)
+                51          82 LOAD_FAST                3 (kwargs)
                
-                50          84 DICT_MERGE               1
+                48          84 DICT_MERGE               1
                             86 CALL_FUNCTION_EX         1
                             88 STORE_FAST               4 (balances)
                
-                55          90 LOAD_GLOBAL              7 (NULL + zip)
+                53          90 LOAD_GLOBAL              7 (NULL + zip)
                            102 LOAD_FAST                1 (addresses)
                            104 LOAD_FAST                4 (balances)
                            106 PRECALL                  2
                            110 CALL                     2
                            120 GET_ITER
                        >>  122 FOR_ITER                18 (to 160)
                            124 UNPACK_SEQUENCE          2
                            128 STORE_FAST               5 (address)
                            130 STORE_FAST               6 (balance_data)
                
-                56         132 LOAD_FAST                5 (address)
+                54         132 LOAD_FAST                5 (address)
                            134 LOAD_FAST                6 (balance_data)
                            136 LOAD_CONST               2 ('result')
                            138 BINARY_SUBSCR
                            148 LOAD_CONST               3 (('address', 'balance'))
                            150 BUILD_CONST_KEY_MAP      2
                            152 YIELD_VALUE
                            154 RESUME                   1
                            156 POP_TOP
                            158 JUMP_BACKWARD           19 (to 122)
                
-                55     >>  160 LOAD_CONST               0 (None)
+                53     >>  160 LOAD_CONST               0 (None)
                            162 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d1c7d0189026a000000000000000000a001000000
                         00000000000000000000000000000000007c01a6010000ab010000000000
                         00000091028c1d5300
                                    0 COPY_FREE_VARS           1
                      
-                      51           2 RESUME                   0
+                      49           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                28 (to 66)
                                   10 STORE_FAST               1 (address)
                                   12 LOAD_DEREF               2 (self)
                                   14 LOAD_ATTR                0 (functions)
                                   24 LOAD_METHOD              1 (balanceOf)
@@ -544,25 +533,25 @@
                      consts
                      names      ('functions', 'balanceOf')
                      varnames   ('.0', 'address')
                      freevars   ('self',)
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                      name       '<listcomp>'
-                     firstlineno 51
+                     firstlineno 49
                      lnotab 0x
                   'result'
                   ('address', 'balance')
                names      ('chain', 'batch_request', 'contract_request', 'zip')
                varnames   ('self', 'addresses', 'block_identifier', 'kwargs', 'balances', 'address', 'balance_data')
                freevars   ()
                cellvars   ('self',)
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                name       'get_balances'
-               firstlineno 41
+               firstlineno 39
                lnotab 0x08060401040222011a0102fe040302fd06052a011cff
             'token_ids'
             code
                argcount  : 3
                nlocals   : 7
                stacksize : 6
                flags     : 43
@@ -572,91 +561,91 @@
                   014400a6000000ab0000000000000000007c02660269007c03a4018e017d
                   047407000000000000000000007c017c04a6020000ab0200000000000000
                   0044005d1f5c0200007d057d067c057409000000000000000000007c0664
                   0219000000000000000000a6010000ab01000000000000000064039c0256
                   00970101008c2064005300
                              0 MAKE_CELL                0 (self)
                
-                58           2 RETURN_GENERATOR
+                56           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                64           8 LOAD_FAST                1 (token_ids)
+                62           8 LOAD_FAST                1 (token_ids)
                             10 POP_JUMP_FORWARD_IF_TRUE     2 (to 16)
                
-                65          12 BUILD_LIST               0
+                63          12 BUILD_LIST               0
                             14 RETURN_VALUE
                
-                67     >>   16 PUSH_NULL
+                65     >>   16 PUSH_NULL
                             18 LOAD_DEREF               0 (self)
                             20 LOAD_ATTR                0 (chain)
                             30 LOAD_ATTR                1 (batch_request)
                             40 LOAD_ATTR                2 (contract_request)
                
-                68          50 LOAD_CLOSURE             0 (self)
+                66          50 LOAD_CLOSURE             0 (self)
                             52 BUILD_TUPLE              1
-                            54 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 68>)
+                            54 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 66>)
                             56 MAKE_FUNCTION            8 (closure)
                             58 LOAD_FAST                1 (token_ids)
                             60 GET_ITER
                             62 PRECALL                  0
                             66 CALL                     0
                
-                69          76 LOAD_FAST                2 (block_identifier)
+                67          76 LOAD_FAST                2 (block_identifier)
                
-                67          78 BUILD_TUPLE              2
+                65          78 BUILD_TUPLE              2
                             80 BUILD_MAP                0
                
-                70          82 LOAD_FAST                3 (kwargs)
+                68          82 LOAD_FAST                3 (kwargs)
                
-                67          84 DICT_MERGE               1
+                65          84 DICT_MERGE               1
                             86 CALL_FUNCTION_EX         1
                             88 STORE_FAST               4 (owners)
                
-                72          90 LOAD_GLOBAL              7 (NULL + zip)
+                70          90 LOAD_GLOBAL              7 (NULL + zip)
                            102 LOAD_FAST                1 (token_ids)
                            104 LOAD_FAST                4 (owners)
                            106 PRECALL                  2
                            110 CALL                     2
                            120 GET_ITER
                        >>  122 FOR_ITER                31 (to 186)
                            124 UNPACK_SEQUENCE          2
                            128 STORE_FAST               5 (token_id)
                            130 STORE_FAST               6 (owner_data)
                
-                73         132 LOAD_FAST                5 (token_id)
+                71         132 LOAD_FAST                5 (token_id)
                            134 LOAD_GLOBAL              9 (NULL + to_checksum_address)
                            146 LOAD_FAST                6 (owner_data)
                            148 LOAD_CONST               2 ('result')
                            150 BINARY_SUBSCR
                            160 PRECALL                  1
                            164 CALL                     1
                            174 LOAD_CONST               3 (('token_id', 'owner'))
                            176 BUILD_CONST_KEY_MAP      2
                            178 YIELD_VALUE
                            180 RESUME                   1
                            182 POP_TOP
                            184 JUMP_BACKWARD           32 (to 122)
                
-                72     >>  186 LOAD_CONST               0 (None)
+                70     >>  186 LOAD_CONST               0 (None)
                            188 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d1c7d0189026a000000000000000000a001000000
                         00000000000000000000000000000000007c01a6010000ab010000000000
                         00000091028c1d5300
                                    0 COPY_FREE_VARS           1
                      
-                      68           2 RESUME                   0
+                      66           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                28 (to 66)
                                   10 STORE_FAST               1 (token_id)
                                   12 LOAD_DEREF               2 (self)
                                   14 LOAD_ATTR                0 (functions)
                                   24 LOAD_METHOD              1 (ownerOf)
@@ -669,25 +658,25 @@
                      consts
                      names      ('functions', 'ownerOf')
                      varnames   ('.0', 'token_id')
                      freevars   ('self',)
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                      name       '<listcomp>'
-                     firstlineno 68
+                     firstlineno 66
                      lnotab 0x
                   'result'
                   ('token_id', 'owner')
                names      ('chain', 'batch_request', 'contract_request', 'zip', 'to_checksum_address')
                varnames   ('self', 'token_ids', 'block_identifier', 'kwargs', 'owners', 'token_id', 'owner_data')
                freevars   ()
                cellvars   ('self',)
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                name       'get_owners'
-               firstlineno 58
+               firstlineno 56
                lnotab 0x08060401040222011a0102fe040302fd06052a0136ff
             code
                argcount  : 3
                nlocals   : 7
                stacksize : 5
                flags     : 43
                code
@@ -695,90 +684,90 @@
                   006a0100000000000000006a02000000000000000088006601640184087c
                   014400a6000000ab000000000000000000660164027c0269017c03a4018e
                   017d047407000000000000000000007c017c04a6020000ab020000000000
                   00000044005d125c0200007d057d067c057c066403190000000000000000
                   0064049c025600970101008c1364005300
                              0 MAKE_CELL                0 (self)
                
-                75           2 RETURN_GENERATOR
+                73           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                81           8 LOAD_FAST                1 (token_ids)
+                79           8 LOAD_FAST                1 (token_ids)
                             10 POP_JUMP_FORWARD_IF_TRUE     2 (to 16)
                
-                82          12 BUILD_LIST               0
+                80          12 BUILD_LIST               0
                             14 RETURN_VALUE
                
-                84     >>   16 PUSH_NULL
+                82     >>   16 PUSH_NULL
                             18 LOAD_DEREF               0 (self)
                             20 LOAD_ATTR                0 (chain)
                             30 LOAD_ATTR                1 (batch_request)
                             40 LOAD_ATTR                2 (contract_request)
                
-                85          50 LOAD_CLOSURE             0 (self)
+                83          50 LOAD_CLOSURE             0 (self)
                             52 BUILD_TUPLE              1
-                            54 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 85>)
+                            54 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\erc721.py", line 83>)
                             56 MAKE_FUNCTION            8 (closure)
                             58 LOAD_FAST                1 (token_ids)
                             60 GET_ITER
                             62 PRECALL                  0
                             66 CALL                     0
                
-                84          76 BUILD_TUPLE              1
+                82          76 BUILD_TUPLE              1
                             78 LOAD_CONST               2 ('block_identifier')
                
-                86          80 LOAD_FAST                2 (block_identifier)
+                84          80 LOAD_FAST                2 (block_identifier)
                
-                84          82 BUILD_MAP                1
+                82          82 BUILD_MAP                1
                
-                87          84 LOAD_FAST                3 (kwargs)
+                85          84 LOAD_FAST                3 (kwargs)
                
-                84          86 DICT_MERGE               1
+                82          86 DICT_MERGE               1
                             88 CALL_FUNCTION_EX         1
                             90 STORE_FAST               4 (token_uris)
                
-                89          92 LOAD_GLOBAL              7 (NULL + zip)
+                87          92 LOAD_GLOBAL              7 (NULL + zip)
                            104 LOAD_FAST                1 (token_ids)
                            106 LOAD_FAST                4 (token_uris)
                            108 PRECALL                  2
                            112 CALL                     2
                            122 GET_ITER
                        >>  124 FOR_ITER                18 (to 162)
                            126 UNPACK_SEQUENCE          2
                            130 STORE_FAST               5 (token_id)
                            132 STORE_FAST               6 (uri_data)
                
-                90         134 LOAD_FAST                5 (token_id)
+                88         134 LOAD_FAST                5 (token_id)
                            136 LOAD_FAST                6 (uri_data)
                            138 LOAD_CONST               3 ('result')
                            140 BINARY_SUBSCR
                            150 LOAD_CONST               4 (('token_id', 'uri'))
                            152 BUILD_CONST_KEY_MAP      2
                            154 YIELD_VALUE
                            156 RESUME                   1
                            158 POP_TOP
                            160 JUMP_BACKWARD           19 (to 124)
                
-                89     >>  162 LOAD_CONST               0 (None)
+                87     >>  162 LOAD_CONST               0 (None)
                            164 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d1c7d0189026a000000000000000000a001000000
                         00000000000000000000000000000000007c01a6010000ab010000000000
                         00000091028c1d5300
                                    0 COPY_FREE_VARS           1
                      
-                      85           2 RESUME                   0
+                      83           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                28 (to 66)
                                   10 STORE_FAST               1 (token_id)
                                   12 LOAD_DEREF               2 (self)
                                   14 LOAD_ATTR                0 (functions)
                                   24 LOAD_METHOD              1 (tokenURI)
@@ -791,44 +780,44 @@
                      consts
                      names      ('functions', 'tokenURI')
                      varnames   ('.0', 'token_id')
                      freevars   ('self',)
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                      name       '<listcomp>'
-                     firstlineno 85
+                     firstlineno 83
                      lnotab 0x
                   'block_identifier'
                   'result'
                   ('token_id', 'uri')
                names      ('chain', 'batch_request', 'contract_request', 'zip')
                varnames   ('self', 'token_ids', 'block_identifier', 'kwargs', 'token_uris', 'token_id', 'uri_data')
                freevars   ()
                cellvars   ('self',)
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
                name       'get_token_uris'
-               firstlineno 75
+               firstlineno 73
                lnotab 0x08060401040222011aff040202fe020302fd06052a011cff
             (None,)
             ('latest',)
-         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'property', 'cache', 'name', 'symbol', 'BlockIdentifier', 'int', 'get_balance', 'Iterable', 'dict', 'get_balances', 'get_owners', 'get_token_uris', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'cached_property', 'name', 'symbol', 'BlockIdentifier', 'int', 'get_balance', 'Iterable', 'dict', 'get_balances', 'get_owners', 'get_token_uris', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
          name       'ERC721'
          firstlineno 14
          lnotab
-            0x0c0502fc040202fe020308fd0c09020102010aff0eff0e020203020102
-            010aff0eff0e02020602fd040202fe020302fd020402fc080a02fd04020e
-            fe020302fd020526fb081402fd04020efe020302fd020526fb081402fd04
-            020efe020302fd020526fb
+            0x0c0502fc040202fe020308fd0c0902010aff0e01020302010aff0e0102
+            0602fd040202fe020302fd020402fc080a02fd04020efe020302fd020526
+            fb081402fd04020efe020302fd020526fb081402fd04020efe020302fd02
+            0526fb
       'ERC721'
       None
-   names      ('typing', 'TYPE_CHECKING', 'Iterable', 'eth_typing', 'ChecksumAddress', 'BlockIdentifier', 'eth_utils', 'to_checksum_address', 'abi', 'ERC721_ABI', 'contract', 'Contract', 'utils', 'cache', 'chain', 'Chain', 'ERC721')
+   names      ('functools', 'cached_property', 'typing', 'TYPE_CHECKING', 'Iterable', 'eth_typing', 'ChecksumAddress', 'BlockIdentifier', 'eth_utils', 'to_checksum_address', '_abi', 'ERC721_ABI', 'contract', 'Contract', 'chain', 'Chain', 'ERC721')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\erc721.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201100210010c020c010c010c0204010c03
+   lnotab 0x00ff02010c01100210010c020c010c0204010c03
```

### Comparing `better_web3-1.3.1/better_web3/contract/__pycache__/multicall.cpython-311.pyc` & `better_web3-1.4.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x0a859464 (Thu Jun 22 17:29:46 2023 UTC)
-files sz: 6182
+moddate:  0xf6ffa764 (Fri Jul  7 12:07:18 2023 UTC)
+files sz: 6201
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a046d
@@ -96,15 +96,15 @@
                126 IMPORT_NAME             21 (web3.exceptions)
                128 IMPORT_FROM             22 (ContractLogicError)
                130 STORE_NAME              22 (ContractLogicError)
                132 POP_TOP
    
     15         134 LOAD_CONST              12 (1)
                136 LOAD_CONST              13 (('MULTICALL_V3_ABI',))
-               138 IMPORT_NAME             23 (abi)
+               138 IMPORT_NAME             23 (_abi)
                140 IMPORT_FROM             24 (MULTICALL_V3_ABI)
                142 STORE_NAME              24 (MULTICALL_V3_ABI)
                144 POP_TOP
    
     16         146 LOAD_CONST              12 (1)
                148 LOAD_CONST              14 (('Contract',))
                150 IMPORT_NAME             25 (contract)
@@ -126,15 +126,15 @@
                176 LOAD_CONST              17 (('Chain',))
                178 IMPORT_NAME             28 (chain)
                180 IMPORT_FROM             29 (Chain)
                182 STORE_NAME              29 (Chain)
                184 POP_TOP
    
     23     >>  186 LOAD_CONST              18 ('0xcA11bde05977b3631167028862bE2a173976CA11')
-               188 STORE_NAME              30 (MULTICALL_V3_ADDRESS)
+               188 STORE_NAME              30 (MULTICALL_V3_CONTRACT_ADDRESS)
    
     26         190 LOAD_NAME                2 (dataclass)
    
     27         192 PUSH_NULL
                194 LOAD_BUILD_CLASS
                196 LOAD_CONST              19 (<code object MulticallResult, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 26>)
                198 MAKE_FUNCTION            0
@@ -571,15 +571,15 @@
                   017c027c03a6030000ab030000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
                 43           2 RESUME                   0
                
                 49           4 LOAD_FAST                2 (address)
                              6 JUMP_IF_TRUE_OR_POP      6 (to 20)
-                             8 LOAD_GLOBAL              0 (MULTICALL_V3_ADDRESS)
+                             8 LOAD_GLOBAL              0 (MULTICALL_V3_CONTRACT_ADDRESS)
                        >>   20 STORE_FAST               2 (address)
                
                 50          22 LOAD_FAST                3 (abi)
                             24 JUMP_IF_TRUE_OR_POP      6 (to 38)
                             26 LOAD_GLOBAL              2 (MULTICALL_V3_ABI)
                        >>   38 STORE_FAST               3 (abi)
                
@@ -593,15 +593,15 @@
                             94 PRECALL                  3
                             98 CALL                     3
                            108 POP_TOP
                            110 LOAD_CONST               0 (None)
                            112 RETURN_VALUE
                consts
                   None
-               names      ('MULTICALL_V3_ADDRESS', 'MULTICALL_V3_ABI', 'super', '__init__')
+               names      ('MULTICALL_V3_CONTRACT_ADDRESS', 'MULTICALL_V3_ABI', 'super', '__init__')
                varnames   ('self', 'chain', 'address', 'abi')
                freevars   ('__class__',)
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                name       '__init__'
                firstlineno 43
                lnotab 0x040612011201
@@ -1389,15 +1389,15 @@
          firstlineno 42
          lnotab
             0x0c04020102fc040202fe020308fd0c0a020102010eff020246fe06ff0e
             010212020124ff0e01021b02fd04021efe020302fd020424fc081502fd04
             020efe020302fd020424fc0812020102fc04021efe020302fd020402fc02
             050efb081d020102fc04020efe020302fd020402fc02050efb
       'Multicall'
-   names      ('__doc__', 'dataclasses', 'dataclass', 'typing', 'Any', 'Sequence', 'eth_abi', 'eth_abi.exceptions', 'DecodingError', 'eth_typing', 'BlockIdentifier', 'BlockNumber', 'ChecksumAddress', 'hexbytes', 'HexBytes', 'web3._utils.abi', 'map_abi_data', 'web3._utils.normalizers', 'BASE_RETURN_NORMALIZERS', 'web3.contract.contract', 'ContractFunction', 'web3.exceptions', 'ContractLogicError', 'abi', 'MULTICALL_V3_ABI', 'contract', 'Contract', 'TYPE_CHECKING', 'chain', 'Chain', 'MULTICALL_V3_ADDRESS', 'MulticallResult', 'MulticallDecodedResult', 'Exception', 'MulticallFailed', 'Multicall')
+   names      ('__doc__', 'dataclasses', 'dataclass', 'typing', 'Any', 'Sequence', 'eth_abi', 'eth_abi.exceptions', 'DecodingError', 'eth_typing', 'BlockIdentifier', 'BlockNumber', 'ChecksumAddress', 'hexbytes', 'HexBytes', 'web3._utils.abi', 'map_abi_data', 'web3._utils.normalizers', 'BASE_RETURN_NORMALIZERS', 'web3.contract.contract', 'ContractFunction', 'web3.exceptions', 'ContractLogicError', '_abi', 'MULTICALL_V3_ABI', 'contract', 'Contract', 'TYPE_CHECKING', 'chain', 'Chain', 'MULTICALL_V3_CONTRACT_ADDRESS', 'MulticallResult', 'MulticallDecodedResult', 'Exception', 'MulticallFailed', 'Multicall')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
    name       '<module>'
    firstlineno 1
    lnotab
```

### Comparing `better_web3-1.3.1/better_web3/contract/abi/disperse.json` & `better_web3-1.4.0/better_web3/contract/abi/disperse.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/contract/abi/erc1155.json` & `better_web3-1.4.0/better_web3/contract/abi/erc1155.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/contract/abi/erc20.json` & `better_web3-1.4.0/better_web3/contract/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/contract/abi/erc721.json` & `better_web3-1.4.0/better_web3/contract/abi/erc721.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/contract/abi/multicall_v3.json` & `better_web3-1.4.0/better_web3/contract/abi/multicall_v3.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/contract/contract.py` & `better_web3-1.4.0/better_web3/contract/contract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import TYPE_CHECKING
 
 from eth_typing import ChecksumAddress
 from eth_utils import to_checksum_address
 from web3 import Web3
 from web3.contract.contract import Contract as Web3Contract
 from web3.contract.contract import ContractEvents, ContractFunctions
+from web3.types import ABI
 
 if TYPE_CHECKING:
     from ..chain import Chain
 
 
 class Contract:
     def __init__(self, chain: "Chain", address: ChecksumAddress | str, abi):
@@ -26,19 +27,19 @@
         return self._chain
 
     @property
     def contract(self) -> Web3Contract:
         return self._contract
 
     @property
-    def address(self) -> str:
+    def address(self) -> ChecksumAddress:
         return self._contract.address
 
     @property
-    def abi(self):
+    def abi(self) -> ABI:
         return self._contract.abi
 
     @property
     def functions(self) -> ContractFunctions:
         return self._contract.functions
 
     @property
```

### Comparing `better_web3-1.3.1/better_web3/contract/disperse.py` & `better_web3-1.4.0/better_web3/contract/disperse.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/contract/erc20.py` & `better_web3-1.4.0/better_web3/contract/erc20.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from functools import cached_property
 from typing import TYPE_CHECKING, Iterable
 
 from eth_typing import ChecksumAddress, BlockIdentifier
 from web3.types import Wei
 
 from ._abi import ERC20_ABI
 from .contract import Contract
-from ..utils import cache
 
 if TYPE_CHECKING:
     from ..chain import Chain
 
 
 class ERC20(Contract):
     def __init__(
@@ -17,26 +17,23 @@
             chain: "Chain",
             address: ChecksumAddress | str,
             abi=None,
     ):
         abi = abi or ERC20_ABI
         super().__init__(chain, address, abi)
 
-    @property
-    @cache
+    @cached_property
     def name(self) -> str:
         return self.functions.name().call()
 
-    @property
-    @cache
+    @cached_property
     def symbol(self) -> str:
         return self.functions.symbol().call()
 
-    @property
-    @cache
+    @cached_property
     def decimals(self) -> int:
         return self.functions.decimals().call()
 
     def get_balance(
             self,
             address: ChecksumAddress,
             block_identifier: BlockIdentifier = "latest",
```

### Comparing `better_web3-1.3.1/better_web3/contract/erc721.py` & `better_web3-1.4.0/better_web3/contract/erc721.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from functools import cached_property
 from typing import TYPE_CHECKING, Iterable
 
 from eth_typing import ChecksumAddress, BlockIdentifier
 from eth_utils import to_checksum_address
 
 from ._abi import ERC721_ABI
 from .contract import Contract
-from ..utils import cache
 
 if TYPE_CHECKING:
     from ..chain import Chain
 
 
 class ERC721(Contract):
     def __init__(
@@ -17,21 +17,19 @@
             chain: "Chain",
             address: ChecksumAddress | str,
             abi=None,
     ):
         abi = abi or ERC721_ABI
         super().__init__(chain, address, abi)
 
-    @property
-    @cache
+    @cached_property
     def name(self) -> str:
         return self.functions.name().call()
 
-    @property
-    @cache
+    @cached_property
     def symbol(self) -> str:
         return self.functions.symbol().call()
 
     def get_balance(
             self,
             address: ChecksumAddress,
             block_identifier: BlockIdentifier = "latest",
```

### Comparing `better_web3-1.3.1/better_web3/contract/multicall.py` & `better_web3-1.4.0/better_web3/contract/multicall.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-1.4.0/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,159 +1,191 @@
 magic:    0xa70d0d0a
-moddate:  0x97799064 (Mon Jun 19 15:51:51 2023 UTC)
-files sz: 1907
+moddate:  0xaafbb464 (Mon Jul 17 08:28:26 2023 UTC)
+files sz: 2131
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c045a04640064046c056d065a060100640064056c076d085a08010064
-      0064066c096d0a5a0a0100640064076c0b6d0c5a0c6d0d5a0d0100640064
-      086c0e6d0f5a0f6d105a106d115a11010064095a12640a6513640b650864
-      0c65136606640d84045a14640e6515640c65136604640f84045a16641065
-      01650c7001651319000000000000000000640c6517650d19000000000000
-      0000006604641184045a1864125a1964135a1a640e65156602641484045a
-      1b64156510640c6511650f7a0700006604641684045a1c64035300
+      036c046d055a050100640064046c065a06640064056c076d085a08010064
+      0064066c096d0a5a0a0100640064076c0b6d0c5a0c0100640064086c0d6d
+      0e5a0e6d0f5a0f0100640064096c106d115a116d125a126d135a13010064
+      0a640b6c146d155a150100640c5a16640d6517640e650a640f6517660664
+      1084045a1864116519640f65176604641284045a1a64136503650e700165
+      1719000000000000000000640f651b650f19000000000000000000660464
+      1484045a1c6415650165177a070000640f651b6416190000000000000000
+      006604641784045a1d64185a1e64195a1f641165196602641a84045a2064
+      1b6512640f651365117a0700006604641c84045a2164045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Iterable',))
-                 6 IMPORT_NAME              0 (typing)
-                 8 IMPORT_FROM              1 (Iterable)
-                10 STORE_NAME               1 (Iterable)
+                 4 LOAD_CONST               1 (('Path',))
+                 6 IMPORT_NAME              0 (pathlib)
+                 8 IMPORT_FROM              1 (Path)
+                10 STORE_NAME               1 (Path)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('HexBytes',))
-                18 IMPORT_NAME              2 (hexbytes)
-                20 IMPORT_FROM              3 (HexBytes)
-                22 STORE_NAME               3 (HexBytes)
+                16 LOAD_CONST               2 (('Iterable',))
+                18 IMPORT_NAME              2 (typing)
+                20 IMPORT_FROM              3 (Iterable)
+                22 STORE_NAME               3 (Iterable)
                 24 POP_TOP
    
-     4          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (None)
-                30 IMPORT_NAME              4 (eth_abi)
-                32 STORE_NAME               4 (eth_abi)
-   
-     5          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               4 (('encode_defunct',))
-                38 IMPORT_NAME              5 (eth_account.messages)
-                40 IMPORT_FROM              6 (encode_defunct)
-                42 STORE_NAME               6 (encode_defunct)
-                44 POP_TOP
+     3          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               3 (('HexBytes',))
+                30 IMPORT_NAME              4 (hexbytes)
+                32 IMPORT_FROM              5 (HexBytes)
+                34 STORE_NAME               5 (HexBytes)
+                36 POP_TOP
+   
+     5          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               4 (None)
+                42 IMPORT_NAME              6 (eth_abi)
+                44 STORE_NAME               6 (eth_abi)
    
      6          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               5 (('LocalAccount',))
-                50 IMPORT_NAME              7 (eth_account.account)
-                52 IMPORT_FROM              8 (LocalAccount)
-                54 STORE_NAME               8 (LocalAccount)
+                48 LOAD_CONST               5 (('encode_defunct',))
+                50 IMPORT_NAME              7 (eth_account.messages)
+                52 IMPORT_FROM              8 (encode_defunct)
+                54 STORE_NAME               8 (encode_defunct)
                 56 POP_TOP
    
      7          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               6 (('to_checksum_address',))
-                62 IMPORT_NAME              9 (eth_utils)
-                64 IMPORT_FROM             10 (to_checksum_address)
-                66 STORE_NAME              10 (to_checksum_address)
+                60 LOAD_CONST               6 (('LocalAccount',))
+                62 IMPORT_NAME              9 (eth_account.account)
+                64 IMPORT_FROM             10 (LocalAccount)
+                66 STORE_NAME              10 (LocalAccount)
                 68 POP_TOP
    
      8          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               7 (('AnyAddress', 'ChecksumAddress'))
-                74 IMPORT_NAME             11 (eth_typing)
-                76 IMPORT_FROM             12 (AnyAddress)
-                78 STORE_NAME              12 (AnyAddress)
-                80 IMPORT_FROM             13 (ChecksumAddress)
-                82 STORE_NAME              13 (ChecksumAddress)
-                84 POP_TOP
-   
-     9          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               8 (('BlockParams', 'BlockIdentifier', 'HexStr'))
-                90 IMPORT_NAME             14 (web3.types)
-                92 IMPORT_FROM             15 (BlockParams)
-                94 STORE_NAME              15 (BlockParams)
-                96 IMPORT_FROM             16 (BlockIdentifier)
-                98 STORE_NAME              16 (BlockIdentifier)
-               100 IMPORT_FROM             17 (HexStr)
-               102 STORE_NAME              17 (HexStr)
-               104 POP_TOP
-   
-    12         106 LOAD_CONST               9 (('latest', 'earliest', 'pending', 'safe', 'finalized'))
-               108 STORE_NAME              18 (BLOCK_PARAMS)
-   
-    15         110 LOAD_CONST              10 ('message')
-               112 LOAD_NAME               19 (str)
-               114 LOAD_CONST              11 ('account')
-               116 LOAD_NAME                8 (LocalAccount)
-               118 LOAD_CONST              12 ('return')
-               120 LOAD_NAME               19 (str)
-               122 BUILD_TUPLE              6
-               124 LOAD_CONST              13 (<code object sign_message, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 15>)
-               126 MAKE_FUNCTION            4 (annotations)
-               128 STORE_NAME              20 (sign_message)
-   
-    21         130 LOAD_CONST              14 ('data')
-               132 LOAD_NAME               21 (bytes)
-               134 LOAD_CONST              12 ('return')
-               136 LOAD_NAME               19 (str)
-               138 BUILD_TUPLE              4
-               140 LOAD_CONST              15 (<code object decode_string_or_bytes32, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 21>)
-               142 MAKE_FUNCTION            4 (annotations)
-               144 STORE_NAME              22 (decode_string_or_bytes32)
-   
-    33         146 LOAD_CONST              16 ('addresses')
-               148 LOAD_NAME                1 (Iterable)
-               150 LOAD_NAME               12 (AnyAddress)
-               152 JUMP_IF_TRUE_OR_POP      1 (to 156)
-               154 LOAD_NAME               19 (str)
-           >>  156 BINARY_SUBSCR
-               166 LOAD_CONST              12 ('return')
-               168 LOAD_NAME               23 (list)
-               170 LOAD_NAME               13 (ChecksumAddress)
-               172 BINARY_SUBSCR
-               182 BUILD_TUPLE              4
-               184 LOAD_CONST              17 (<code object to_checksum_addresses, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 33>)
-               186 MAKE_FUNCTION            4 (annotations)
-               188 STORE_NAME              24 (to_checksum_addresses)
-   
-    37         190 LOAD_CONST              18 (4)
-               192 STORE_NAME              25 (GAS_CALL_DATA_ZERO_BYTE)
-   
-    38         194 LOAD_CONST              19 (16)
-               196 STORE_NAME              26 (GAS_CALL_DATA_BYTE)
-   
-    41         198 LOAD_CONST              14 ('data')
-               200 LOAD_NAME               21 (bytes)
-               202 BUILD_TUPLE              2
-               204 LOAD_CONST              20 (<code object estimate_data_gas, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 41>)
-               206 MAKE_FUNCTION            4 (annotations)
-               208 STORE_NAME              27 (estimate_data_gas)
-   
-    54         210 LOAD_CONST              21 ('block_identifier')
-               212 LOAD_NAME               16 (BlockIdentifier)
-               214 LOAD_CONST              12 ('return')
-               216 LOAD_NAME               17 (HexStr)
-               218 LOAD_NAME               15 (BlockParams)
+                72 LOAD_CONST               7 (('to_checksum_address',))
+                74 IMPORT_NAME             11 (eth_utils)
+                76 IMPORT_FROM             12 (to_checksum_address)
+                78 STORE_NAME              12 (to_checksum_address)
+                80 POP_TOP
+   
+     9          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               8 (('AnyAddress', 'ChecksumAddress'))
+                86 IMPORT_NAME             13 (eth_typing)
+                88 IMPORT_FROM             14 (AnyAddress)
+                90 STORE_NAME              14 (AnyAddress)
+                92 IMPORT_FROM             15 (ChecksumAddress)
+                94 STORE_NAME              15 (ChecksumAddress)
+                96 POP_TOP
+   
+    10          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               9 (('BlockParams', 'BlockIdentifier', 'HexStr'))
+               102 IMPORT_NAME             16 (web3.types)
+               104 IMPORT_FROM             17 (BlockParams)
+               106 STORE_NAME              17 (BlockParams)
+               108 IMPORT_FROM             18 (BlockIdentifier)
+               110 STORE_NAME              18 (BlockIdentifier)
+               112 IMPORT_FROM             19 (HexStr)
+               114 STORE_NAME              19 (HexStr)
+               116 POP_TOP
+   
+    12         118 LOAD_CONST              10 (1)
+               120 LOAD_CONST              11 (('load_lines',))
+               122 IMPORT_NAME             20 (file)
+               124 IMPORT_FROM             21 (load_lines)
+               126 STORE_NAME              21 (load_lines)
+               128 POP_TOP
+   
+    14         130 LOAD_CONST              12 (('latest', 'earliest', 'pending', 'safe', 'finalized'))
+               132 STORE_NAME              22 (BLOCK_PARAMS)
+   
+    17         134 LOAD_CONST              13 ('message')
+               136 LOAD_NAME               23 (str)
+               138 LOAD_CONST              14 ('account')
+               140 LOAD_NAME               10 (LocalAccount)
+               142 LOAD_CONST              15 ('return')
+               144 LOAD_NAME               23 (str)
+               146 BUILD_TUPLE              6
+               148 LOAD_CONST              16 (<code object sign_message, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 17>)
+               150 MAKE_FUNCTION            4 (annotations)
+               152 STORE_NAME              24 (sign_message)
+   
+    23         154 LOAD_CONST              17 ('data')
+               156 LOAD_NAME               25 (bytes)
+               158 LOAD_CONST              15 ('return')
+               160 LOAD_NAME               23 (str)
+               162 BUILD_TUPLE              4
+               164 LOAD_CONST              18 (<code object decode_string_or_bytes32, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 23>)
+               166 MAKE_FUNCTION            4 (annotations)
+               168 STORE_NAME              26 (decode_string_or_bytes32)
+   
+    35         170 LOAD_CONST              19 ('addresses')
+               172 LOAD_NAME                3 (Iterable)
+               174 LOAD_NAME               14 (AnyAddress)
+               176 JUMP_IF_TRUE_OR_POP      1 (to 180)
+               178 LOAD_NAME               23 (str)
+           >>  180 BINARY_SUBSCR
+               190 LOAD_CONST              15 ('return')
+               192 LOAD_NAME               27 (list)
+               194 LOAD_NAME               15 (ChecksumAddress)
+               196 BINARY_SUBSCR
+               206 BUILD_TUPLE              4
+               208 LOAD_CONST              20 (<code object to_checksum_addresses, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 35>)
+               210 MAKE_FUNCTION            4 (annotations)
+               212 STORE_NAME              28 (to_checksum_addresses)
+   
+    39         214 LOAD_CONST              21 ('filepath')
+               216 LOAD_NAME                1 (Path)
+               218 LOAD_NAME               23 (str)
                220 BINARY_OP                7 (|)
-               224 BUILD_TUPLE              4
-               226 LOAD_CONST              22 (<code object hex_block_identifier, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 54>)
-               228 MAKE_FUNCTION            4 (annotations)
-               230 STORE_NAME              28 (hex_block_identifier)
-               232 LOAD_CONST               3 (None)
-               234 RETURN_VALUE
+               224 LOAD_CONST              15 ('return')
+               226 LOAD_NAME               27 (list)
+               228 LOAD_CONST              22 ('ChecksumAddress')
+               230 BINARY_SUBSCR
+               240 BUILD_TUPLE              4
+               242 LOAD_CONST              23 (<code object addresses_from_file, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 39>)
+               244 MAKE_FUNCTION            4 (annotations)
+               246 STORE_NAME              29 (addresses_from_file)
+   
+    43         248 LOAD_CONST              24 (4)
+               250 STORE_NAME              30 (GAS_CALL_DATA_ZERO_BYTE)
+   
+    44         252 LOAD_CONST              25 (16)
+               254 STORE_NAME              31 (GAS_CALL_DATA_BYTE)
+   
+    47         256 LOAD_CONST              17 ('data')
+               258 LOAD_NAME               25 (bytes)
+               260 BUILD_TUPLE              2
+               262 LOAD_CONST              26 (<code object estimate_data_gas, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 47>)
+               264 MAKE_FUNCTION            4 (annotations)
+               266 STORE_NAME              32 (estimate_data_gas)
+   
+    60         268 LOAD_CONST              27 ('block_identifier')
+               270 LOAD_NAME               18 (BlockIdentifier)
+               272 LOAD_CONST              15 ('return')
+               274 LOAD_NAME               19 (HexStr)
+               276 LOAD_NAME               17 (BlockParams)
+               278 BINARY_OP                7 (|)
+               282 BUILD_TUPLE              4
+               284 LOAD_CONST              28 (<code object hex_block_identifier, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 60>)
+               286 MAKE_FUNCTION            4 (annotations)
+               288 STORE_NAME              33 (hex_block_identifier)
+               290 LOAD_CONST               4 (None)
+               292 RETURN_VALUE
    consts
       0
+      ('Path',)
       ('Iterable',)
       ('HexBytes',)
       None
       ('encode_defunct',)
       ('LocalAccount',)
       ('to_checksum_address',)
       ('AnyAddress', 'ChecksumAddress')
       ('BlockParams', 'BlockIdentifier', 'HexStr')
+      1
+      ('load_lines',)
       ('latest', 'earliest', 'pending', 'safe', 'finalized')
       'message'
       'account'
       'return'
       code
          argcount  : 2
          nlocals   : 3
@@ -161,46 +193,46 @@
          flags     : 3
          code
             0x97007401000000000000000000007c00ac01a6010000ab010000000000
             0000007d007c01a00100000000000000000000000000000000000000007c
             00a6010000ab0100000000000000007d027c026a020000000000000000a0
             030000000000000000000000000000000000000000a6000000ab00000000
             00000000005300
-          15           0 RESUME                   0
+          17           0 RESUME                   0
          
-          16           2 LOAD_GLOBAL              1 (NULL + encode_defunct)
+          18           2 LOAD_GLOBAL              1 (NULL + encode_defunct)
                       14 LOAD_FAST                0 (message)
                       16 KW_NAMES                 1
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               0 (message)
          
-          17          34 LOAD_FAST                1 (account)
+          19          34 LOAD_FAST                1 (account)
                       36 LOAD_METHOD              1 (sign_message)
                       58 LOAD_FAST                0 (message)
                       60 PRECALL                  1
                       64 CALL                     1
                       74 STORE_FAST               2 (signed_message)
          
-          18          76 LOAD_FAST                2 (signed_message)
+          20          76 LOAD_FAST                2 (signed_message)
                       78 LOAD_ATTR                2 (signature)
                       88 LOAD_METHOD              3 (hex)
                      110 PRECALL                  0
                      114 CALL                     0
                      124 RETURN_VALUE
          consts
             None
             ('text',)
          names      ('encode_defunct', 'sign_message', 'signature', 'hex')
          varnames   ('message', 'account', 'signed_message')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'sign_message'
-         firstlineno 15
+         firstlineno 17
          lnotab 0x020120012a01
       'data'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
@@ -212,79 +244,79 @@
             0000006402190000000000000000007d017c01a003000000000000000000
             00000000000000000000006404a6010000ab0100000000000000007d027c
             0264056b020000000072167c01a001000000000000000000000000000000
             0000000000a6000000ab0000000000000000006302590053007c0164007c
             02850219000000000000000000a001000000000000000000000000000000
             0000000000a6000000ab0000000000000000006302590053007700780359
             007701
-          21           0 RESUME                   0
+          23           0 RESUME                   0
          
-          22           2 NOP
+          24           2 NOP
          
-          23           4 LOAD_GLOBAL              1 (NULL + eth_abi)
+          25           4 LOAD_GLOBAL              1 (NULL + eth_abi)
                       16 LOAD_ATTR                1 (decode)
                       26 LOAD_CONST               1 ('string')
                       28 BUILD_LIST               1
                       30 LOAD_FAST                0 (data)
                       32 PRECALL                  2
                       36 CALL                     2
                       46 LOAD_CONST               2 (0)
                       48 BINARY_SUBSCR
                       58 RETURN_VALUE
                  >>   60 PUSH_EXC_INFO
          
-          24          62 LOAD_GLOBAL              4 (OverflowError)
+          26          62 LOAD_GLOBAL              4 (OverflowError)
                       74 CHECK_EXC_MATCH
                       76 POP_JUMP_FORWARD_IF_FALSE   108 (to 294)
                       78 POP_TOP
          
-          25          80 LOAD_GLOBAL              1 (NULL + eth_abi)
+          27          80 LOAD_GLOBAL              1 (NULL + eth_abi)
                       92 LOAD_ATTR                1 (decode)
                      102 LOAD_CONST               3 ('bytes32')
                      104 BUILD_LIST               1
                      106 LOAD_FAST                0 (data)
                      108 PRECALL                  2
                      112 CALL                     2
                      122 LOAD_CONST               2 (0)
                      124 BINARY_SUBSCR
                      134 STORE_FAST               1 (name)
          
-          26         136 LOAD_FAST                1 (name)
+          28         136 LOAD_FAST                1 (name)
                      138 LOAD_METHOD              3 (find)
                      160 LOAD_CONST               4 (b'\x00')
                      162 PRECALL                  1
                      166 CALL                     1
                      176 STORE_FAST               2 (end_position)
          
-          27         178 LOAD_FAST                2 (end_position)
+          29         178 LOAD_FAST                2 (end_position)
                      180 LOAD_CONST               5 (-1)
                      182 COMPARE_OP               2 (==)
                      188 POP_JUMP_FORWARD_IF_FALSE    22 (to 234)
          
-          28         190 LOAD_FAST                1 (name)
+          30         190 LOAD_FAST                1 (name)
                      192 LOAD_METHOD              1 (decode)
                      214 PRECALL                  0
                      218 CALL                     0
                      228 SWAP                     2
                      230 POP_EXCEPT
                      232 RETURN_VALUE
          
-          30     >>  234 LOAD_FAST                1 (name)
+          32     >>  234 LOAD_FAST                1 (name)
                      236 LOAD_CONST               0 (None)
                      238 LOAD_FAST                2 (end_position)
                      240 BUILD_SLICE              2
                      242 BINARY_SUBSCR
                      252 LOAD_METHOD              1 (decode)
                      274 PRECALL                  0
                      278 CALL                     0
                      288 SWAP                     2
                      290 POP_EXCEPT
                      292 RETURN_VALUE
          
-          24     >>  294 RERAISE                  0
+          26     >>  294 RERAISE                  0
                  >>  296 COPY                     3
                      298 POP_EXCEPT
                      300 RERAISE                  1
          ExceptionTable:
            4 to 56 -> 60 [0]
            60 to 228 -> 296 [1] lasti
            234 to 288 -> 296 [1] lasti
@@ -298,26 +330,26 @@
             -1
          names      ('eth_abi', 'decode', 'OverflowError', 'find')
          varnames   ('data', 'name', 'end_position')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'decode_string_or_bytes32'
-         firstlineno 21
+         firstlineno 23
          lnotab 0x020102013a01120138012a010c012c023cfa
       'addresses'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x9700640184007c004400a6000000ab0000000000000000005300
-          33           0 RESUME                   0
+          35           0 RESUME                   0
          
-          34           2 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 34>)
+          36           2 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 36>)
                        4 MAKE_FUNCTION            0
                        6 LOAD_FAST                0 (addresses)
                        8 GET_ITER
                       10 PRECALL                  0
                       14 CALL                     0
                       24 RETURN_VALUE
          consts
@@ -326,15 +358,15 @@
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x970067007c005d117d017401000000000000000000007c01a6010000ab
                   01000000000000000091028c125300
-                34           0 RESUME                   0
+                36           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                17 (to 42)
                              8 STORE_FAST               1 (address)
                             10 LOAD_GLOBAL              1 (NULL + to_checksum_address)
                             22 LOAD_FAST                1 (address)
                             24 PRECALL                  1
@@ -345,87 +377,152 @@
                consts
                names      ('to_checksum_address',)
                varnames   ('.0', 'address')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
                name       '<listcomp>'
-               firstlineno 34
+               firstlineno 36
                lnotab 0x
          names      ()
          varnames   ('addresses',)
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'to_checksum_addresses'
-         firstlineno 33
+         firstlineno 35
+         lnotab 0x0201
+      'filepath'
+      'ChecksumAddress'
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 6
+         flags     : 3
+         code
+            0x9700740100000000000000000000640184007403000000000000000000
+            007c00a6010000ab0100000000000000004400a6000000ab000000000000
+            000000a6010000ab0100000000000000005300
+          39           0 RESUME                   0
+         
+          40           2 LOAD_GLOBAL              1 (NULL + to_checksum_addresses)
+                      14 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 40>)
+                      16 MAKE_FUNCTION            0
+                      18 LOAD_GLOBAL              3 (NULL + load_lines)
+                      30 LOAD_FAST                0 (filepath)
+                      32 PRECALL                  1
+                      36 CALL                     1
+                      46 GET_ITER
+                      48 PRECALL                  0
+                      52 CALL                     0
+                      62 PRECALL                  1
+                      66 CALL                     1
+                      76 RETURN_VALUE
+         consts
+            None
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 4
+               flags     : 19
+               code
+                  0x970067007c005d167d017c01a000000000000000000000000000000000
+                  0000000000a6000000ab00000000000000000091028c175300
+                40           0 RESUME                   0
+                             2 BUILD_LIST               0
+                             4 LOAD_FAST                0 (.0)
+                       >>    6 FOR_ITER                22 (to 52)
+                             8 STORE_FAST               1 (address)
+                            10 LOAD_FAST                1 (address)
+                            12 LOAD_METHOD              0 (strip)
+                            34 PRECALL                  0
+                            38 CALL                     0
+                            48 LIST_APPEND              2
+                            50 JUMP_BACKWARD           23 (to 6)
+                       >>   52 RETURN_VALUE
+               consts
+               names      ('strip',)
+               varnames   ('.0', 'address')
+               freevars   ()
+               cellvars   ()
+               filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
+               name       '<listcomp>'
+               firstlineno 40
+               lnotab 0x
+         names      ('to_checksum_addresses', 'load_lines')
+         varnames   ('filepath',)
+         freevars   ()
+         cellvars   ()
+         filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
+         name       'addresses_from_file'
+         firstlineno 39
          lnotab 0x0201
       4
       16
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c00740200000000000000000000a6
             020000ab020000000000000000720f7405000000000000000000007c00a6
             010000ab0100000000000000007d0064017d017c0044005d197d027c0273
             0b7c017406000000000000000000007a0d00007d018c0f7c017408000000
             000000000000007a0d00007d018c1a7c015300
-          41           0 RESUME                   0
+          47           0 RESUME                   0
          
-          42           2 LOAD_GLOBAL              1 (NULL + isinstance)
+          48           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (data)
                       16 LOAD_GLOBAL              2 (str)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_FALSE    15 (to 74)
          
-          43          44 LOAD_GLOBAL              5 (NULL + HexBytes)
+          49          44 LOAD_GLOBAL              5 (NULL + HexBytes)
                       56 LOAD_FAST                0 (data)
                       58 PRECALL                  1
                       62 CALL                     1
                       72 STORE_FAST               0 (data)
          
-          45     >>   74 LOAD_CONST               1 (0)
+          51     >>   74 LOAD_CONST               1 (0)
                       76 STORE_FAST               1 (gas)
          
-          46          78 LOAD_FAST                0 (data)
+          52          78 LOAD_FAST                0 (data)
                       80 GET_ITER
                  >>   82 FOR_ITER                25 (to 134)
                       84 STORE_FAST               2 (byte)
          
-          47          86 LOAD_FAST                2 (byte)
+          53          86 LOAD_FAST                2 (byte)
                       88 POP_JUMP_FORWARD_IF_TRUE    11 (to 112)
          
-          48          90 LOAD_FAST                1 (gas)
+          54          90 LOAD_FAST                1 (gas)
                       92 LOAD_GLOBAL              6 (GAS_CALL_DATA_ZERO_BYTE)
                      104 BINARY_OP               13 (+=)
                      108 STORE_FAST               1 (gas)
                      110 JUMP_BACKWARD           15 (to 82)
          
-          50     >>  112 LOAD_FAST                1 (gas)
+          56     >>  112 LOAD_FAST                1 (gas)
                      114 LOAD_GLOBAL              8 (GAS_CALL_DATA_BYTE)
                      126 BINARY_OP               13 (+=)
                      130 STORE_FAST               1 (gas)
                      132 JUMP_BACKWARD           26 (to 82)
          
-          51     >>  134 LOAD_FAST                1 (gas)
+          57     >>  134 LOAD_FAST                1 (gas)
                      136 RETURN_VALUE
          consts
             None
             0
          names      ('isinstance', 'str', 'HexBytes', 'GAS_CALL_DATA_ZERO_BYTE', 'GAS_CALL_DATA_BYTE')
          varnames   ('data', 'gas', 'byte')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'estimate_data_gas'
-         firstlineno 41
+         firstlineno 47
          lnotab 0x02012a011e0204010801040116021601
       'block_identifier'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
@@ -434,72 +531,72 @@
             000000000000007c00740400000000000000000000a6020000ab02000000
             000000000072107407000000000000000000007c00a6010000ab01000000
             00000000007d006e367403000000000000000000007c0074080000000000
             0000000000a6020000ab0200000000000000007221740b00000000000000
             0000007c00a6010000ab010000000000000000a003000000000000000000
             0000000000000000000000a6000000ab0000000000000000007d00740d00
             0000000000000000007c00a6010000ab0100000000000000005300
-          54           0 RESUME                   0
+          60           0 RESUME                   0
          
-          55           2 LOAD_FAST                0 (block_identifier)
+          61           2 LOAD_FAST                0 (block_identifier)
                        4 LOAD_GLOBAL              0 (BLOCK_PARAMS)
                       16 CONTAINS_OP              0
                       18 POP_JUMP_FORWARD_IF_FALSE     2 (to 24)
          
-          56          20 LOAD_FAST                0 (block_identifier)
+          62          20 LOAD_FAST                0 (block_identifier)
                       22 RETURN_VALUE
          
-          57     >>   24 LOAD_GLOBAL              3 (NULL + isinstance)
+          63     >>   24 LOAD_GLOBAL              3 (NULL + isinstance)
                       36 LOAD_FAST                0 (block_identifier)
                       38 LOAD_GLOBAL              4 (int)
                       50 PRECALL                  2
                       54 CALL                     2
                       64 POP_JUMP_FORWARD_IF_FALSE    16 (to 98)
          
-          58          66 LOAD_GLOBAL              7 (NULL + hex)
+          64          66 LOAD_GLOBAL              7 (NULL + hex)
                       78 LOAD_FAST                0 (block_identifier)
                       80 PRECALL                  1
                       84 CALL                     1
                       94 STORE_FAST               0 (block_identifier)
                       96 JUMP_FORWARD            54 (to 206)
          
-          59     >>   98 LOAD_GLOBAL              3 (NULL + isinstance)
+          65     >>   98 LOAD_GLOBAL              3 (NULL + isinstance)
                      110 LOAD_FAST                0 (block_identifier)
                      112 LOAD_GLOBAL              8 (bytes)
                      124 PRECALL                  2
                      128 CALL                     2
                      138 POP_JUMP_FORWARD_IF_FALSE    33 (to 206)
          
-          60         140 LOAD_GLOBAL             11 (NULL + HexBytes)
+          66         140 LOAD_GLOBAL             11 (NULL + HexBytes)
                      152 LOAD_FAST                0 (block_identifier)
                      154 PRECALL                  1
                      158 CALL                     1
                      168 LOAD_METHOD              3 (hex)
                      190 PRECALL                  0
                      194 CALL                     0
                      204 STORE_FAST               0 (block_identifier)
          
-          61     >>  206 LOAD_GLOBAL             13 (NULL + HexStr)
+          67     >>  206 LOAD_GLOBAL             13 (NULL + HexStr)
                      218 LOAD_FAST                0 (block_identifier)
                      220 PRECALL                  1
                      224 CALL                     1
                      234 RETURN_VALUE
          consts
             None
          names      ('BLOCK_PARAMS', 'isinstance', 'int', 'hex', 'bytes', 'HexBytes', 'HexStr')
          varnames   ('block_identifier',)
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'hex_block_identifier'
-         firstlineno 54
+         firstlineno 60
          lnotab 0x0201120104012a0120012a014201
-   names      ('typing', 'Iterable', 'hexbytes', 'HexBytes', 'eth_abi', 'eth_account.messages', 'encode_defunct', 'eth_account.account', 'LocalAccount', 'eth_utils', 'to_checksum_address', 'eth_typing', 'AnyAddress', 'ChecksumAddress', 'web3.types', 'BlockParams', 'BlockIdentifier', 'HexStr', 'BLOCK_PARAMS', 'str', 'sign_message', 'bytes', 'decode_string_or_bytes32', 'list', 'to_checksum_addresses', 'GAS_CALL_DATA_ZERO_BYTE', 'GAS_CALL_DATA_BYTE', 'estimate_data_gas', 'hex_block_identifier')
+   names      ('pathlib', 'Path', 'typing', 'Iterable', 'hexbytes', 'HexBytes', 'eth_abi', 'eth_account.messages', 'encode_defunct', 'eth_account.account', 'LocalAccount', 'eth_utils', 'to_checksum_address', 'eth_typing', 'AnyAddress', 'ChecksumAddress', 'web3.types', 'BlockParams', 'BlockIdentifier', 'HexStr', 'file', 'load_lines', 'BLOCK_PARAMS', 'str', 'sign_message', 'bytes', 'decode_string_or_bytes32', 'list', 'to_checksum_addresses', 'addresses_from_file', 'GAS_CALL_DATA_ZERO_BYTE', 'GAS_CALL_DATA_BYTE', 'estimate_data_gas', 'hex_block_identifier')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c0208010c010c010c011001140304031406100c2c0404
-      0104030c0d
+      0x00ff02010c010c010c0208010c010c010c01100114020c020403140610
+      0c2c042204040104030c0d
```

### Comparing `better_web3-1.3.1/better_web3/utils/__pycache__/file.cpython-311.pyc` & `better_web3-1.4.0/better_web3/utils/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-1.4.0/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x971c9c64 (Wed Jun 28 11:42:15 2023 UTC)
-files sz: 733
+moddate:  0xff6fa864 (Fri Jul  7 20:05:19 2023 UTC)
+files sz: 663
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
-      045a040100640064046c056d065a060100640064056c076d085a08010002
-      0065066401ac06a6010000ab0100000000000000005a0964076502640865
-      0a64096502650b190000000000000000006606640a84045a0c640b650d64
-      0c6508650d7a0700006604640d84045a0e6409650d6602640e84045a0f64
-      015300
+      045a040100640064046c056d065a06010064056502640665076407650265
+      08190000000000000000006606640884045a096409650a640a6506650a7a
+      0700006604640b84045a0b6407650a6602640c84045a0c64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (json)
                  8 STORE_NAME               0 (json)
    
@@ -30,146 +28,129 @@
      3          22 LOAD_CONST               0 (0)
                 24 LOAD_CONST               3 (('islice',))
                 26 IMPORT_NAME              3 (itertools)
                 28 IMPORT_FROM              4 (islice)
                 30 STORE_NAME               4 (islice)
                 32 POP_TOP
    
-     4          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               4 (('lru_cache',))
-                38 IMPORT_NAME              5 (functools)
-                40 IMPORT_FROM              6 (lru_cache)
-                42 STORE_NAME               6 (lru_cache)
+     5          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               4 (('HexStr',))
+                38 IMPORT_NAME              5 (eth_typing)
+                40 IMPORT_FROM              6 (HexStr)
+                42 STORE_NAME               6 (HexStr)
                 44 POP_TOP
    
-     6          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               5 (('HexStr',))
-                50 IMPORT_NAME              7 (eth_typing)
-                52 IMPORT_FROM              8 (HexStr)
-                54 STORE_NAME               8 (HexStr)
-                56 POP_TOP
-   
-     9          58 PUSH_NULL
-                60 LOAD_NAME                6 (lru_cache)
-                62 LOAD_CONST               1 (None)
-                64 KW_NAMES                 6
-                66 PRECALL                  1
-                70 CALL                     1
-                80 STORE_NAME               9 (cache)
-   
-    12          82 LOAD_CONST               7 ('elements')
-                84 LOAD_NAME                2 (Iterable)
-                86 LOAD_CONST               8 ('n')
-                88 LOAD_NAME               10 (int)
-                90 LOAD_CONST               9 ('return')
-                92 LOAD_NAME                2 (Iterable)
-                94 LOAD_NAME               11 (list)
-                96 BINARY_SUBSCR
-               106 BUILD_TUPLE              6
-               108 LOAD_CONST              10 (<code object chunks, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 12>)
-               110 MAKE_FUNCTION            4 (annotations)
-               112 STORE_NAME              12 (chunks)
-   
-    26         114 LOAD_CONST              11 ('explorer_url')
-               116 LOAD_NAME               13 (str)
-               118 LOAD_CONST              12 ('tx_hash')
-               120 LOAD_NAME                8 (HexStr)
-               122 LOAD_NAME               13 (str)
-               124 BINARY_OP                7 (|)
-               128 BUILD_TUPLE              4
-               130 LOAD_CONST              13 (<code object link_by_tx_hash, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 26>)
-               132 MAKE_FUNCTION            4 (annotations)
-               134 STORE_NAME              14 (link_by_tx_hash)
-   
-    30         136 LOAD_CONST               9 ('return')
-               138 LOAD_NAME               13 (str)
-               140 BUILD_TUPLE              2
-               142 LOAD_CONST              14 (<code object to_json, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 30>)
-               144 MAKE_FUNCTION            4 (annotations)
-               146 STORE_NAME              15 (to_json)
-               148 LOAD_CONST               1 (None)
-               150 RETURN_VALUE
+     8          46 LOAD_CONST               5 ('elements')
+                48 LOAD_NAME                2 (Iterable)
+                50 LOAD_CONST               6 ('n')
+                52 LOAD_NAME                7 (int)
+                54 LOAD_CONST               7 ('return')
+                56 LOAD_NAME                2 (Iterable)
+                58 LOAD_NAME                8 (list)
+                60 BINARY_SUBSCR
+                70 BUILD_TUPLE              6
+                72 LOAD_CONST               8 (<code object chunks, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 8>)
+                74 MAKE_FUNCTION            4 (annotations)
+                76 STORE_NAME               9 (chunks)
+   
+    22          78 LOAD_CONST               9 ('explorer_url')
+                80 LOAD_NAME               10 (str)
+                82 LOAD_CONST              10 ('tx_hash')
+                84 LOAD_NAME                6 (HexStr)
+                86 LOAD_NAME               10 (str)
+                88 BINARY_OP                7 (|)
+                92 BUILD_TUPLE              4
+                94 LOAD_CONST              11 (<code object link_by_tx_hash, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 22>)
+                96 MAKE_FUNCTION            4 (annotations)
+                98 STORE_NAME              11 (link_by_tx_hash)
+   
+    26         100 LOAD_CONST               7 ('return')
+               102 LOAD_NAME               10 (str)
+               104 BUILD_TUPLE              2
+               106 LOAD_CONST              12 (<code object to_json, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 26>)
+               108 MAKE_FUNCTION            4 (annotations)
+               110 STORE_NAME              12 (to_json)
+               112 LOAD_CONST               1 (None)
+               114 RETURN_VALUE
    consts
       0
       None
       ('Iterable',)
       ('islice',)
-      ('lru_cache',)
       ('HexStr',)
-      ('maxsize',)
       'elements'
       'n'
       'return'
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 6
          flags     : 35
          code
             0x4b00010097007401000000000000000000007c00a6010000ab01000000
             00000000007d020900740300000000000000000000740500000000000000
             0000007c027c01a6020000ab020000000000000000a6010000ab01000000
             00000000007d037c037302640253007c035600970101008c26
-          12           0 RETURN_GENERATOR
+           8           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-          18           6 LOAD_GLOBAL              1 (NULL + iter)
+          14           6 LOAD_GLOBAL              1 (NULL + iter)
                       18 LOAD_FAST                0 (elements)
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_FAST               2 (it)
          
-          19          36 NOP
+          15          36 NOP
          
-          20     >>   38 LOAD_GLOBAL              3 (NULL + list)
+          16     >>   38 LOAD_GLOBAL              3 (NULL + list)
                       50 LOAD_GLOBAL              5 (NULL + islice)
                       62 LOAD_FAST                2 (it)
                       64 LOAD_FAST                1 (n)
                       66 PRECALL                  2
                       70 CALL                     2
                       80 PRECALL                  1
                       84 CALL                     1
                       94 STORE_FAST               3 (chunk)
          
-          21          96 LOAD_FAST                3 (chunk)
+          17          96 LOAD_FAST                3 (chunk)
                       98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
          
-          22         100 LOAD_CONST               2 (None)
+          18         100 LOAD_CONST               2 (None)
                      102 RETURN_VALUE
          
-          23     >>  104 LOAD_FAST                3 (chunk)
+          19     >>  104 LOAD_FAST                3 (chunk)
                      106 YIELD_VALUE
                      108 RESUME                   1
                      110 POP_TOP
          
-          19         112 JUMP_BACKWARD           38 (to 38)
+          15         112 JUMP_BACKWARD           38 (to 38)
          consts
             '\n    :param elements: Iterable\n    :param n: Number per chunk\n    :return: Yield successive n-sized chunks from elements\n    '
             True
             None
          names      ('iter', 'list', 'islice')
          varnames   ('elements', 'n', 'it', 'chunk')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\other.py'
          name       'chunks'
-         firstlineno 12
+         firstlineno 8
          lnotab 0x06061e0102013a010401040108fc
       'explorer_url'
       'tx_hash'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code 0x97007c009b0064017c019b009d035300
-          26           0 RESUME                   0
+          22           0 RESUME                   0
          
-          27           2 LOAD_FAST                0 (explorer_url)
+          23           2 LOAD_FAST                0 (explorer_url)
                        4 FORMAT_VALUE             0
                        6 LOAD_CONST               1 ('/tx/')
                        8 LOAD_FAST                1 (tx_hash)
                       10 FORMAT_VALUE             0
                       12 BUILD_STRING             3
                       14 RETURN_VALUE
          consts
@@ -177,27 +158,27 @@
             '/tx/'
          names      ()
          varnames   ('explorer_url', 'tx_hash')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\other.py'
          name       'link_by_tx_hash'
-         firstlineno 26
+         firstlineno 22
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00640164
             02ac03a6030000ab0300000000000000005300
-          30           0 RESUME                   0
+          26           0 RESUME                   0
          
-          31           2 LOAD_GLOBAL              1 (NULL + json)
+          27           2 LOAD_GLOBAL              1 (NULL + json)
                       14 LOAD_ATTR                1 (dumps)
                       24 LOAD_FAST                0 (obj)
                       26 LOAD_CONST               1 ((',', ':'))
                       28 LOAD_CONST               2 (True)
                       30 KW_NAMES                 3
                       32 PRECALL                  3
                       36 CALL                     3
@@ -209,17 +190,17 @@
             ('separators', 'ensure_ascii')
          names      ('json', 'dumps')
          varnames   ('obj',)
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\other.py'
          name       'to_json'
-         firstlineno 30
+         firstlineno 26
          lnotab 0x0201
-   names      ('json', 'typing', 'Iterable', 'itertools', 'islice', 'functools', 'lru_cache', 'eth_typing', 'HexStr', 'cache', 'int', 'list', 'chunks', 'str', 'link_by_tx_hash', 'to_json')
+   names      ('json', 'typing', 'Iterable', 'itertools', 'islice', 'eth_typing', 'HexStr', 'int', 'list', 'chunks', 'str', 'link_by_tx_hash', 'to_json')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\other.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c010c010c020c031803200e1604
+   lnotab 0x00ff020108010c010c020c03200e1604
```

### Comparing `better_web3-1.3.1/better_web3/utils/eth.py` & `better_web3-1.4.0/better_web3/utils/eth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from pathlib import Path
 from typing import Iterable
 from hexbytes import HexBytes
 
 import eth_abi
 from eth_account.messages import encode_defunct
 from eth_account.account import LocalAccount
 from eth_utils import to_checksum_address
 from eth_typing import AnyAddress, ChecksumAddress
 from web3.types import BlockParams, BlockIdentifier, HexStr
 
+from .file import load_lines
 
 BLOCK_PARAMS = ("latest", "earliest", "pending", "safe", "finalized")
 
 
 def sign_message(message: str, account: LocalAccount) -> str:
     message = encode_defunct(text=message)
     signed_message = account.sign_message(message)
@@ -30,14 +32,18 @@
             return name[:end_position].decode()
 
 
 def to_checksum_addresses(addresses: Iterable[AnyAddress or str]) -> list[ChecksumAddress]:
     return [to_checksum_address(address) for address in addresses]
 
 
+def addresses_from_file(filepath: Path | str) -> list["ChecksumAddress"]:
+    return to_checksum_addresses([address.strip() for address in load_lines(filepath)])
+
+
 GAS_CALL_DATA_ZERO_BYTE = 4
 GAS_CALL_DATA_BYTE = 16  # 68 before Istanbul
 
 
 def estimate_data_gas(data: bytes):
     if isinstance(data, str):
         data = HexBytes(data)
```

### Comparing `better_web3-1.3.1/better_web3/utils/file.py` & `better_web3-1.4.0/better_web3/utils/file.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.3.1/better_web3/utils/other.py` & `better_web3-1.4.0/better_web3/utils/other.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import json
 from typing import Iterable
 from itertools import islice
-from functools import lru_cache
 
 from eth_typing import HexStr
 
 
-cache = lru_cache(maxsize=None)
-
-
 def chunks(elements: Iterable, n: int) -> Iterable[list]:
     """
     :param elements: Iterable
     :param n: Number per chunk
     :return: Yield successive n-sized chunks from elements
     """
     it = iter(elements)
```

### Comparing `better_web3-1.3.1/PKG-INFO` & `better_web3-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 1.3.1
+Version: 1.4.0
 Summary: Chains, Contracts(Multicall, Disperse, ERC20/ERC721), batch calls and other..
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: web3 (>=6.5.0,<7.0.0)
+Requires-Dist: web3 (>=6.6.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Better Web3.py
 [ [Telegram](https://t.me/cum_insider) ] [ [PyPi](https://pypi.org/project/better-web3) ]
 
 ```bash
 pip install better-web3
 ```
 
+- [Usage example](https://github.com/alenkimov/better_web3_scripts)
+
+
 ## Credits
 - [safe-global](https://github.com/safe-global) / [Safe-eth-py (previosly known as Gnosis-py)](https://github.com/safe-global/safe-eth-py)
 - [Whynot63](https://github.com/Whynot63) / [web3-premium](https://github.com/Whynot63/web3-premium)
```

