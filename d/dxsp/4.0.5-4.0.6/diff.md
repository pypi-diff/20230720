# Comparing `tmp/dxsp-4.0.5.tar.gz` & `tmp/dxsp-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.0.5.tar", max compression
+gzip compressed data, was "dxsp-4.0.6.tar", max compression
```

## Comparing `dxsp-4.0.5.tar` & `dxsp-4.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-16 21:17:16.566274 dxsp-4.0.5/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-16 21:17:16.566274 dxsp-4.0.5/README.md
--rw-r--r--   0        0        0      115 2023-07-16 21:17:17.282272 dxsp-4.0.5/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-16 21:17:16.566274 dxsp-4.0.5/dxsp/config.py
--rw-r--r--   0        0        0    10529 2023-07-16 21:17:16.566274 dxsp-4.0.5/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5622 2023-07-16 21:17:16.566274 dxsp-4.0.5/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-16 21:17:16.566274 dxsp-4.0.5/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-16 21:17:16.566274 dxsp-4.0.5/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1835 2023-07-16 21:17:16.566274 dxsp-4.0.5/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1036 2023-07-16 21:17:16.566274 dxsp-4.0.5/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-07-16 21:17:16.566274 dxsp-4.0.5/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4705 2023-07-16 21:17:16.570273 dxsp-4.0.5/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6590 2023-07-16 21:17:16.570273 dxsp-4.0.5/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1989 2023-07-16 21:17:16.570273 dxsp-4.0.5/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-07-16 21:17:16.570273 dxsp-4.0.5/dxsp/utils/utils.py
--rw-r--r--   0        0        0     2327 2023-07-16 21:17:17.282272 dxsp-4.0.5/pyproject.toml
--rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 dxsp-4.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-20 11:31:27.742168 dxsp-4.0.6/LICENSE
+-rw-r--r--   0        0        0     2857 2023-07-20 11:31:27.742168 dxsp-4.0.6/README.md
+-rw-r--r--   0        0        0      158 2023-07-20 11:31:28.842229 dxsp-4.0.6/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/config.py
+-rw-r--r--   0        0        0    10529 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5625 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4708 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     4100 2023-07-20 11:31:28.842229 dxsp-4.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 dxsp-4.0.6/PKG-INFO
```

### Comparing `dxsp-4.0.5/LICENSE` & `dxsp-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.5/README.md` & `dxsp-4.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,15 @@
    <a href="https://codebeat.co/projects/github-com-mraniki-dxsp-main"><img src="https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/dxsp"><img src="https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH"/> </a><br>
   <a href="https://codeclimate.com/github/mraniki/dxsp/maintainability"><img src="https://api.codeclimate.com/v1/badges/ec80e827d5878e60ba12/maintainability" /></a>
     </td>
     <td align="left"> 
 Swap made easy<br>
 Trade on any blockchains with uniswap based router or 0x protocol.
-    </td>
-     
+    </td> 
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
 <code>
    from dxsp import DexSwap
```

### Comparing `dxsp-4.0.5/dxsp/default_settings.toml` & `dxsp-4.0.6/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.5/dxsp/main.py` & `dxsp-4.0.6/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
  DEX SWAP Main
 """
 
+import decimal
 import logging
 from typing import Optional
-import decimal
+
 from web3 import Web3
 from web3.gas_strategies.time_based import medium_gas_price_strategy
+
 from dxsp.config import settings
-from dxsp.utils import ContractUtils, AccountUtils
+from dxsp.utils import AccountUtils, ContractUtils
+
 
 class DexSwap:
     """swap  class"""
     def __init__(self, w3: Optional[Web3] = None):
         self.logger = logging.getLogger(name="DexSwap")
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         if not self.w3.net.listening:
@@ -26,15 +29,15 @@
         self.dex_swap = None
         self.router = None
         self.quoter = None
         self.contract_utils = ContractUtils(w3=self.w3)
 
     async def get_protocol(self):
         """ protocol init """
-        from dxsp.protocols import DexSwapUniswap, DexSwapZeroX, DexSwapOneInch
+        from dxsp.protocols import DexSwapOneInch, DexSwapUniswap, DexSwapZeroX
         if self.protocol_type == "0x":
             self.dex_swap = DexSwapZeroX()
         elif self.protocol_type == "1inch":
             self.dex_swap = DexSwapOneInch()
         else:
             self.dex_swap = DexSwapUniswap()
```

### Comparing `dxsp-4.0.5/dxsp/protocols/oneinch.py` & `dxsp-4.0.6/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.5/dxsp/protocols/uniswap.py` & `dxsp-4.0.6/dxsp/protocols/uniswap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 uniswap  🦄
 """
-from dxsp.config import settings
-from dxsp.main import DexSwap
 from uniswap import Uniswap
 
+from dxsp.config import settings
+from dxsp.main import DexSwap
 
 
 class DexSwapUniswap(DexSwap):
     """
     A DEXSwap sub class using uniswap-python library
     """
     async def get_quote(
@@ -28,15 +28,16 @@
             amount_wei = amount * (10 ** (
                 await self.contract_utils.get_token_decimals(sell_address)))
             quote = uniswap.get_price_input(
                 sell_address, buy_address, amount_wei)
             return round(
                 float((quote /
                        (10 **
-                        (await self.contract_utils.get_token_decimals(buy_address))))), 5)
+                        (await self.contract_utils.get_token_decimals(
+                            buy_address))))), 5)
 
         except Exception as error:
             raise ValueError(f"Quote failed {error}") 
 
     async def get_swap(self, sell_address, buy_address, amount):
         try:
             uniswap = Uniswap(
```

### Comparing `dxsp-4.0.5/dxsp/protocols/zerox.py` & `dxsp-4.0.6/dxsp/protocols/zerox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 0️⃣x
 """
 from dxsp.config import settings
 from dxsp.main import DexSwap
 from dxsp.utils.utils import get
 
+
 class DexSwapZeroX(DexSwap):
 
     async def get_quote(self, buy_address, sell_address, amount=1):
         try:
             token_decimals = await self.contract_utils.get_token_decimals(sell_address)
             out_amount = amount * (10 ** token_decimals)
             url = (f"{settings.dex_0x_url}/swap/v1/quote"
```

### Comparing `dxsp-4.0.5/dxsp/utils/account_utils.py` & `dxsp-4.0.6/dxsp/utils/account_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
  DEX SWAP
 🔒 USER RELATED
 """
 import logging
 from typing import Optional
+
 from web3 import Web3
+
+from dxsp import __version__
 from dxsp.config import settings
-from dxsp.utils.explorer_utils import get_account_transactions
 from dxsp.utils.contract_utils import ContractUtils
-from dxsp import __version__
+from dxsp.utils.explorer_utils import get_account_transactions
+
 
 class AccountUtils:
 
     def __init__(self, w3: Optional[Web3] = None):
         self.logger = logging.getLogger(name="DexSwap")
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         self.wallet_address = self.w3.to_checksum_address(
```

### Comparing `dxsp-4.0.5/dxsp/utils/contract_utils.py` & `dxsp-4.0.6/dxsp/utils/contract_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
  DEX SWAP
 ✍️ CONTRACT
 """
 
+import decimal
 import logging
+from datetime import datetime
 from typing import Optional
-from web3 import Web3
+
 import requests
+from pycoingecko import CoinGeckoAPI
+from web3 import Web3
+
 from dxsp.config import settings
 from dxsp.utils.explorer_utils import get_explorer_abi
 from dxsp.utils.utils import get
-from pycoingecko import CoinGeckoAPI
-import decimal
-from datetime import datetime
 
 
 class ContractUtils:
 
     def __init__(self, w3: Optional[Web3] = None):
         self.logger = logging.getLogger(name="DexSwap")
         self.w3 = w3
@@ -113,15 +115,18 @@
         return contract.functions.symbol().call() 
 
     async def get_token_name(self, token_address: str):
         """Get token symbol"""
         contract = await self.get_token_contract(token_address)
         return contract.functions.name().call() 
 
-    async def get_token_balance(self, token_address: str,wallet_address: str) -> Optional[int]:
+    async def get_token_balance(
+        self, token_address: str,
+        wallet_address: str
+        ) -> Optional[int]:
         """Get token balance"""
         contract = await self.get_token_contract(token_address)
         if contract is None or contract.functions is None:
             raise ValueError("No Balance")
         balance = contract.functions.balanceOf(wallet_address).call()
         if balance is None:
             raise ValueError("No Balance")
```

### Comparing `dxsp-4.0.5/dxsp/utils/explorer_utils.py` & `dxsp-4.0.6/dxsp/utils/explorer_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
  DEX SWAP
 EXPLORER
 """
 
 from datetime import datetime, timedelta
+
 from dxsp.config import settings
 from dxsp.utils.utils import get
 
 
 async def get_explorer_abi(address):
     if not settings.dex_block_explorer_api:
         return None
```

### Comparing `dxsp-4.0.5/PKG-INFO` & `dxsp-4.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.0.5
+Version: 4.0.6
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -41,16 +41,15 @@
    <a href="https://codebeat.co/projects/github-com-mraniki-dxsp-main"><img src="https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/dxsp"><img src="https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH"/> </a><br>
   <a href="https://codeclimate.com/github/mraniki/dxsp/maintainability"><img src="https://api.codeclimate.com/v1/badges/ec80e827d5878e60ba12/maintainability" /></a>
     </td>
     <td align="left"> 
 Swap made easy<br>
 Trade on any blockchains with uniswap based router or 0x protocol.
-    </td>
-     
+    </td> 
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
 <code>
    from dxsp import DexSwap
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.0.5 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.0.6 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

