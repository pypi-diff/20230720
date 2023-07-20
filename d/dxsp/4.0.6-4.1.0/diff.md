# Comparing `tmp/dxsp-4.0.6.tar.gz` & `tmp/dxsp-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.0.6.tar", max compression
+gzip compressed data, was "dxsp-4.1.0.tar", max compression
```

## Comparing `dxsp-4.0.6.tar` & `dxsp-4.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-20 11:31:27.742168 dxsp-4.0.6/LICENSE
--rw-r--r--   0        0        0     2857 2023-07-20 11:31:27.742168 dxsp-4.0.6/README.md
--rw-r--r--   0        0        0      158 2023-07-20 11:31:28.842229 dxsp-4.0.6/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/config.py
--rw-r--r--   0        0        0    10529 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5625 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/main.py
--rw-r--r--   0        0        0      104 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1864 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1037 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4708 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6619 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1990 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-07-20 11:31:27.742168 dxsp-4.0.6/dxsp/utils/utils.py
--rw-r--r--   0        0        0     4100 2023-07-20 11:31:28.842229 dxsp-4.0.6/pyproject.toml
--rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 dxsp-4.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-20 14:52:07.399715 dxsp-4.1.0/LICENSE
+-rw-r--r--   0        0        0     2857 2023-07-20 14:52:07.399715 dxsp-4.1.0/README.md
+-rw-r--r--   0        0        0      158 2023-07-20 14:52:08.227724 dxsp-4.1.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/config.py
+-rw-r--r--   0        0        0    12100 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5701 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4834 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-07-20 14:52:07.399715 dxsp-4.1.0/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     4100 2023-07-20 14:52:08.227724 dxsp-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 dxsp-4.1.0/PKG-INFO
```

### Comparing `dxsp-4.0.6/LICENSE` & `dxsp-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.6/README.md` & `dxsp-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.6/dxsp/default_settings.toml` & `dxsp-4.1.0/dxsp/default_settings.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+########################################
+###          DEFAULT SETTINGS        ###
+########################################
+
+# Any of those settings can be changed
+# by the user. To overwrite a setting, 
+# create a settings.toml or load the 
+# settings from .env file or vars.
+# As an example, to disable the 
+# dxsp object:
+# settings.toml
+# [default]
+# dxsp_enabled = false
+
 [default]
 VALUE = "On default"
 dxsp_enabled = true
+dxsp_commands = "🎯 BUY WBTC\n🎯 /q WBTC\n 🏦 /bal\n 🏦 /pos\n"
 loglevel = "INFO"
 dex_wallet_address = "0x1234567890123456789012345678901234567890"
 dex_private_key = "0xdeadbeef45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_0x_url = "https://api.0x.org/mainnet"
@@ -23,24 +38,48 @@
 trading_risk_amount = 10 # 10% of the position
 dex_trading_slippage = 2 # 2% slippage
 dex_notify_invalid_token = true
 
 
 
 
+########################################
+###     END OF DEFAULT SETTINGS      ###
+########################################
+
+
+
+
+                                        
+# _   _                           _   ___  
+#| | | |                         | | |__ \ 
+#| |_| |__   ___    ___ _ __   __| |    )|
+#| __| '_ \ / _ \  / _ \ '_ \ / _` |   / / 
+#| |_| | | |  __/ |  __/ | | | (_| |  |_|  
+# \__|_| |_|\___|  \___|_| |_|\__,_|  (_)  
+########################################                                                                                      
+
+
+
 
 
 
+########################################
+###         TESTING SETTINGS         ###
+########################################
+
+
 ##############
 ## SETTINGS ##
 ## FOR TEST ##
 ##############
 [uniswap]
 VALUE = "On Testing"
 dxsp_enabled = true
+dxsp_commands = "🎯 BUY WBTC\n🎯 /q WBTC\n 🏦 /bal\n 🏦 /pos\n"
 loglevel = "DEBUG"
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
@@ -56,14 +95,15 @@
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 [zerox]
 VALUE = "test_zerox"
 loglevel = "DEBUG"
 dxsp_enabled = true
+dxsp_commands = "🎯 BUY WBTC\n🎯 /q WBTC\n 🏦 /bal\n 🏦 /pos\n"
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "0x"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_0x_url = "https://api.0x.org/"
 dex_router_contract_addr = "0xdef1c0ded9bec7f1a1670819833240f027b25eff"
@@ -75,18 +115,20 @@
 dex_trading_slippage = 2
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
+
 [testnet]
 VALUE = "On Testnet"
 loglevel = "DEBUG"
 dxsp_enabled = true
+dxsp_commands = "🎯 BUY WBTC\n🎯 /q WBTC\n 🏦 /bal\n 🏦 /pos\n"
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth_goerli"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
@@ -97,17 +139,19 @@
 dex_trading_slippage = 2
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
+
 [bsc]
 VALUE = "chain_56"
 dxsp_enabled = true
+dxsp_commands = "🎯 BUY WBTC\n🎯 /q WBTC\n 🏦 /bal\n 🏦 /pos\n"
 dex_wallet_address = "0xf977814e90da44bfa03b6295a0616a897441acec"
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/bsc"
 dex_router_contract_addr = "0x10ED43C718714eb63d5aA57B78B54704E256024E"
 dex_factory_contract_addr = "0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73"
@@ -116,17 +160,19 @@
 dex_trading_slippage = 2
 dex_notify_invalid_token = false
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
+
 [uniswapv3]
 VALUE = "On uniswap3"
 dxsp_enabled = true
+dxsp_commands = "🎯 BUY WBTC\n🎯 /q WBTC\n 🏦 /bal\n 🏦 /pos\n"
 loglevel = "DEBUG"
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap"
 dex_protocol_version = 3
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_router_contract_addr = "0x1F98431c8aD98523631AE4a59f267346ea31F984"
@@ -138,17 +184,19 @@
 dex_trading_slippage = 2
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
+
 [pancake3]
 VALUE = "On pancake3"
 dxsp_enabled = true
+dxsp_commands = "🎯 BUY WBTC\n🎯 /q WBTC\n 🏦 /bal\n 🏦 /pos\n"
 loglevel = "DEBUG"
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap"
 dex_protocol_version = 3
 dex_rpc = "https://rpc.ankr.com/bsc"
 dex_router_contract_addr = "0x1F98431c8aD98523631AE4a59f267346ea31F984"
@@ -161,15 +209,15 @@
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 
-
+ 
 # [oneinch]
 # VALUE = "1inchtesting"
 # loglevel = "DEBUG"
 # dxsp_enabled = true
 # headers = {User-Agent= 'Mozilla/5.0'}
 # token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 # token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dxsp-4.0.6/dxsp/main.py` & `dxsp-4.1.0/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,17 @@
         except Exception as error:
             return f"⚠️: {error}"
 
 # 🔒 USER RELATED
     async def get_info(self):
         return await self.account.get_info()
 
+    async def get_help(self):
+        return await self.account.get_help()
+
     async def get_name(self):
         return await self.account.get_name()
 
     async def get_account_balance(self):
         return await self.account.get_account_balance()
 
     async def get_trading_asset_balance(self):
```

### Comparing `dxsp-4.0.6/dxsp/protocols/oneinch.py` & `dxsp-4.1.0/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.6/dxsp/protocols/uniswap.py` & `dxsp-4.1.0/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.6/dxsp/protocols/zerox.py` & `dxsp-4.1.0/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.6/dxsp/utils/account_utils.py` & `dxsp-4.1.0/dxsp/utils/account_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,28 @@
             settings.dex_wallet_address)
         self.account_number = (f"{str(self.w3.net.version)} - "
                         f"{str(self.wallet_address)[-8:]}")
         self.private_key = settings.dex_private_key
         self.trading_asset_address = self.w3.to_checksum_address(
         settings.trading_asset_address)
         self.contract_utils = ContractUtils(w3=self.w3)
+        self.commands = settings.dxsp_commands
 
     async def get_info(self):
         try:
-            return (f"ℹ️ {__version__}\n"
+            return (f"ℹ️ DexSwap v{__version__}\n"
                     f"💱 {await self.get_name()}\n"
                     f"🪪 {self.account_number}")
         except Exception as error:
             return error
 
+    async def get_help(self):
+        return (f"{self.commands}\n")
+
+
     async def get_name(self):
         if settings.dex_router_contract_addr:
             return str(settings.dex_router_contract_addr)[-8:]
 
     async def get_account_balance(self):
         account_balance = self.w3.eth.get_balance(
             self.w3.to_checksum_address(self.wallet_address))
```

### Comparing `dxsp-4.0.6/dxsp/utils/contract_utils.py` & `dxsp-4.1.0/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.6/dxsp/utils/explorer_utils.py` & `dxsp-4.1.0/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.0.6/pyproject.toml` & `dxsp-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.0.6"
+version = "4.1.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-4.0.6/PKG-INFO` & `dxsp-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.0.6
+Version: 4.1.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.0.6 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.1.0 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

