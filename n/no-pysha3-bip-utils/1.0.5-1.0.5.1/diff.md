# Comparing `tmp/no_pysha3_bip_utils-1.0.5.tar.gz` & `tmp/no_pysha3_bip_utils-1.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no_pysha3_bip_utils-1.0.5.tar", last modified: Thu Jul 20 09:40:22 2023, max compression
+gzip compressed data, was "no_pysha3_bip_utils-1.0.5.1.tar", last modified: Thu Jul 20 09:50:37 2023, max compression
```

## Comparing `no_pysha3_bip_utils-1.0.5.tar` & `no_pysha3_bip_utils-1.0.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 09:40:22.088566 no_pysha3_bip_utils-1.0.5/
--rw-r--r--   0 rollo      (501) staff       (20)     1076 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/LICENSE
--rw-r--r--   0 rollo      (501) staff       (20)    19169 2023-07-20 09:40:22.088832 no_pysha3_bip_utils-1.0.5/PKG-INFO
--rw-r--r--   0 rollo      (501) staff       (20)    18274 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/README.md
-drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 09:40:22.086966 no_pysha3_bip_utils-1.0.5/bip_utils/
--rw-r--r--   0 rollo      (501) staff       (20)     2217 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/P2PKH.py
--rw-r--r--   0 rollo      (501) staff       (20)     2530 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/P2SH.py
--rw-r--r--   0 rollo      (501) staff       (20)     2355 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/P2WPKH.py
--rw-r--r--   0 rollo      (501) staff       (20)     1304 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/__init__.py
--rw-r--r--   0 rollo      (501) staff       (20)       22 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/_version.py
--rw-r--r--   0 rollo      (501) staff       (20)     6429 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/base58.py
--rw-r--r--   0 rollo      (501) staff       (20)     1196 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/base58_ex.py
--rw-r--r--   0 rollo      (501) staff       (20)     7836 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bech32.py
--rw-r--r--   0 rollo      (501) staff       (20)     1545 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bech32_ex.py
--rw-r--r--   0 rollo      (501) staff       (20)    15853 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip32.py
--rw-r--r--   0 rollo      (501) staff       (20)     1292 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip32_ex.py
--rw-r--r--   0 rollo      (501) staff       (20)     4861 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip32_key_ser.py
--rw-r--r--   0 rollo      (501) staff       (20)     3858 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip32_path.py
--rw-r--r--   0 rollo      (501) staff       (20)     1902 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip32_utils.py
--rw-r--r--   0 rollo      (501) staff       (20)    13801 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip39.py
--rw-r--r--   0 rollo      (501) staff       (20)     1304 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip39_ex.py
--rw-r--r--   0 rollo      (501) staff       (20)    13117 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip39_wordslist_en.txt
--rw-r--r--   0 rollo      (501) staff       (20)     6829 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip44.py
--rw-r--r--   0 rollo      (501) staff       (20)    16349 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip44_base.py
--rw-r--r--   0 rollo      (501) staff       (20)     1321 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip44_base_ex.py
--rw-r--r--   0 rollo      (501) staff       (20)     4436 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip44_coins.py
--rw-r--r--   0 rollo      (501) staff       (20)     6653 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip49.py
--rw-r--r--   0 rollo      (501) staff       (20)     4605 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip49_coins.py
--rw-r--r--   0 rollo      (501) staff       (20)     6284 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip84.py
--rw-r--r--   0 rollo      (501) staff       (20)     2466 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip84_coins.py
--rw-r--r--   0 rollo      (501) staff       (20)     4535 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip_coin_base.py
--rw-r--r--   0 rollo      (501) staff       (20)     6865 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip_coin_conf.py
--rw-r--r--   0 rollo      (501) staff       (20)     3181 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip_coin_conf_helper.py
--rw-r--r--   0 rollo      (501) staff       (20)     4908 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/bip_keys.py
--rw-r--r--   0 rollo      (501) staff       (20)     2595 2023-07-20 09:38:54.000000 no_pysha3_bip_utils-1.0.5/bip_utils/eth_addr.py
--rw-r--r--   0 rollo      (501) staff       (20)     3015 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/key_helper.py
--rw-r--r--   0 rollo      (501) staff       (20)     5345 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/utils.py
--rw-r--r--   0 rollo      (501) staff       (20)     3937 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/wif.py
--rw-r--r--   0 rollo      (501) staff       (20)     1755 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5/bip_utils/xrp_addr.py
-drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 09:40:22.088420 no_pysha3_bip_utils-1.0.5/no_pysha3_bip_utils.egg-info/
--rw-r--r--   0 rollo      (501) staff       (20)    19169 2023-07-20 09:40:22.000000 no_pysha3_bip_utils-1.0.5/no_pysha3_bip_utils.egg-info/PKG-INFO
--rw-r--r--   0 rollo      (501) staff       (20)     1025 2023-07-20 09:40:22.000000 no_pysha3_bip_utils-1.0.5/no_pysha3_bip_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rollo      (501) staff       (20)        1 2023-07-20 09:40:22.000000 no_pysha3_bip_utils-1.0.5/no_pysha3_bip_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rollo      (501) staff       (20)       15 2023-07-20 09:40:22.000000 no_pysha3_bip_utils-1.0.5/no_pysha3_bip_utils.egg-info/requires.txt
--rw-r--r--   0 rollo      (501) staff       (20)       10 2023-07-20 09:40:22.000000 no_pysha3_bip_utils-1.0.5/no_pysha3_bip_utils.egg-info/top_level.txt
--rw-r--r--   0 rollo      (501) staff       (20)      102 2023-07-20 09:40:22.089382 no_pysha3_bip_utils-1.0.5/setup.cfg
--rw-r--r--   0 rollo      (501) staff       (20)     1675 2023-07-20 09:37:05.000000 no_pysha3_bip_utils-1.0.5/setup.py
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 09:50:37.232568 no_pysha3_bip_utils-1.0.5.1/
+-rw-r--r--   0 rollo      (501) staff       (20)     1076 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/LICENSE
+-rw-r--r--   0 rollo      (501) staff       (20)    19173 2023-07-20 09:50:37.232688 no_pysha3_bip_utils-1.0.5.1/PKG-INFO
+-rw-r--r--   0 rollo      (501) staff       (20)    18274 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/README.md
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 09:50:37.231549 no_pysha3_bip_utils-1.0.5.1/bip_utils/
+-rw-r--r--   0 rollo      (501) staff       (20)     2217 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/P2PKH.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2530 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/P2SH.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2355 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/P2WPKH.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1304 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/__init__.py
+-rw-r--r--   0 rollo      (501) staff       (20)       24 2023-07-20 09:50:23.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/_version.py
+-rw-r--r--   0 rollo      (501) staff       (20)     6429 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/base58.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1196 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/base58_ex.py
+-rw-r--r--   0 rollo      (501) staff       (20)     7836 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bech32.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1545 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bech32_ex.py
+-rw-r--r--   0 rollo      (501) staff       (20)    15853 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1292 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32_ex.py
+-rw-r--r--   0 rollo      (501) staff       (20)     4861 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32_key_ser.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3858 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32_path.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1902 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32_utils.py
+-rw-r--r--   0 rollo      (501) staff       (20)    13801 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip39.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1304 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip39_ex.py
+-rw-r--r--   0 rollo      (501) staff       (20)    13117 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip39_wordslist_en.txt
+-rw-r--r--   0 rollo      (501) staff       (20)     6829 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip44.py
+-rw-r--r--   0 rollo      (501) staff       (20)    16349 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip44_base.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1321 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip44_base_ex.py
+-rw-r--r--   0 rollo      (501) staff       (20)     4436 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip44_coins.py
+-rw-r--r--   0 rollo      (501) staff       (20)     6653 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip49.py
+-rw-r--r--   0 rollo      (501) staff       (20)     4605 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip49_coins.py
+-rw-r--r--   0 rollo      (501) staff       (20)     6284 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip84.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2466 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip84_coins.py
+-rw-r--r--   0 rollo      (501) staff       (20)     4535 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip_coin_base.py
+-rw-r--r--   0 rollo      (501) staff       (20)     6865 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip_coin_conf.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3181 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip_coin_conf_helper.py
+-rw-r--r--   0 rollo      (501) staff       (20)     4908 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/bip_keys.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2601 2023-07-20 09:49:58.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/eth_addr.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3015 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/key_helper.py
+-rw-r--r--   0 rollo      (501) staff       (20)     5345 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/utils.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3937 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/wif.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1755 2023-07-20 09:31:12.000000 no_pysha3_bip_utils-1.0.5.1/bip_utils/xrp_addr.py
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 09:50:37.232438 no_pysha3_bip_utils-1.0.5.1/no_pysha3_bip_utils.egg-info/
+-rw-r--r--   0 rollo      (501) staff       (20)    19173 2023-07-20 09:50:37.000000 no_pysha3_bip_utils-1.0.5.1/no_pysha3_bip_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rollo      (501) staff       (20)     1025 2023-07-20 09:50:37.000000 no_pysha3_bip_utils-1.0.5.1/no_pysha3_bip_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rollo      (501) staff       (20)        1 2023-07-20 09:50:37.000000 no_pysha3_bip_utils-1.0.5.1/no_pysha3_bip_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rollo      (501) staff       (20)       15 2023-07-20 09:50:37.000000 no_pysha3_bip_utils-1.0.5.1/no_pysha3_bip_utils.egg-info/requires.txt
+-rw-r--r--   0 rollo      (501) staff       (20)       10 2023-07-20 09:50:37.000000 no_pysha3_bip_utils-1.0.5.1/no_pysha3_bip_utils.egg-info/top_level.txt
+-rw-r--r--   0 rollo      (501) staff       (20)      102 2023-07-20 09:50:37.233078 no_pysha3_bip_utils-1.0.5.1/setup.cfg
+-rw-r--r--   0 rollo      (501) staff       (20)     1675 2023-07-20 09:37:05.000000 no_pysha3_bip_utils-1.0.5.1/setup.py
```

### Comparing `no_pysha3_bip_utils-1.0.5/LICENSE` & `no_pysha3_bip_utils-1.0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/PKG-INFO` & `no_pysha3_bip_utils-1.0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: no_pysha3_bip_utils
-Version: 1.0.5
+Version: 1.0.5.1
 Summary: Implementation of BIP39, BIP32, BIP44, BIP49 and BIP84 for wallet seeds, keys and addresses generation. Supported coins: Bitcoin, Litecoin, Dogecoin, Ethereum.
 Home-page: https://github.com/ebellocchia/bip_utils
 Author: A Byte Ahead
 Author-email: laalaguer@gmail.com
 Maintainer: A Byte Ahead
 Maintainer-email: laalaguer@gmail.com
 License: MIT
-Download-URL: https://github.com/ebellocchia/bip_utils/archive/v1.0.5.tar.gz
+Download-URL: https://github.com/ebellocchia/bip_utils/archive/v1.0.5.1.tar.gz
 Keywords: bitcoin,litecoin,dogecoin,dash,ethereum,ripple,wallet,hd-wallet,bip39,bip32,bip44,bip49,bip84,python
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
```

### Comparing `no_pysha3_bip_utils-1.0.5/README.md` & `no_pysha3_bip_utils-1.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/P2PKH.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/P2PKH.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/P2SH.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/P2SH.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/P2WPKH.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/P2WPKH.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/__init__.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/base58.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/base58.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/base58_ex.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/base58_ex.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bech32.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bech32.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bech32_ex.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bech32_ex.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip32.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip32_ex.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32_ex.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip32_key_ser.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32_key_ser.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip32_path.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32_path.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip32_utils.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip32_utils.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip39.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip39.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip39_ex.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip39_ex.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip39_wordslist_en.txt` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip39_wordslist_en.txt`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip44.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip44.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip44_base.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip44_base.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip44_base_ex.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip44_base_ex.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip44_coins.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip44_coins.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip49.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip49.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip49_coins.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip49_coins.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip84.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip84.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip84_coins.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip84_coins.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip_coin_base.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip_coin_base.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip_coin_conf.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip_coin_conf.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip_coin_conf_helper.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip_coin_conf_helper.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/bip_keys.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/bip_keys.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/eth_addr.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/eth_addr.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             addr (str): Address string
 
         Returns:
             str: Checksum encoded address
         """
 
         # Compute address digest
-        addr_digest = keccak.new(addr.encode()).hexdigest()
+        addr_digest = keccak.new(addr.encode()).digest().hex()
         # Encode it
         enc_addr = [c.upper() if (int(addr_digest[i], 16) >= 8) else c.lower() for i, c in enumerate(addr)]
 
         return "".join(enc_addr)
 
 
 class EthAddr:
@@ -69,9 +69,9 @@
 
         Raised:
             ValueError: If the key is not a public uncompressed key
         """
         if not KeyHelper.IsPublicUncompressed(pub_key_bytes):
             raise ValueError("Public uncompressed key is required for Ethereum address")
 
-        addr = keccak.new(pub_key_bytes).hexdigest()[EthAddrConst.START_BYTE:]
+        addr = keccak.new(pub_key_bytes).digest().hex()[EthAddrConst.START_BYTE:]
         return EthAddrConst.PREFIX + EthAddrUtils.ChecksumEncode(addr)
```

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/key_helper.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/key_helper.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/utils.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/utils.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/wif.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/wif.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/bip_utils/xrp_addr.py` & `no_pysha3_bip_utils-1.0.5.1/bip_utils/xrp_addr.py`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/no_pysha3_bip_utils.egg-info/PKG-INFO` & `no_pysha3_bip_utils-1.0.5.1/no_pysha3_bip_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: no-pysha3-bip-utils
-Version: 1.0.5
+Version: 1.0.5.1
 Summary: Implementation of BIP39, BIP32, BIP44, BIP49 and BIP84 for wallet seeds, keys and addresses generation. Supported coins: Bitcoin, Litecoin, Dogecoin, Ethereum.
 Home-page: https://github.com/ebellocchia/bip_utils
 Author: A Byte Ahead
 Author-email: laalaguer@gmail.com
 Maintainer: A Byte Ahead
 Maintainer-email: laalaguer@gmail.com
 License: MIT
-Download-URL: https://github.com/ebellocchia/bip_utils/archive/v1.0.5.tar.gz
+Download-URL: https://github.com/ebellocchia/bip_utils/archive/v1.0.5.1.tar.gz
 Keywords: bitcoin,litecoin,dogecoin,dash,ethereum,ripple,wallet,hd-wallet,bip39,bip32,bip44,bip49,bip84,python
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
```

### Comparing `no_pysha3_bip_utils-1.0.5/no_pysha3_bip_utils.egg-info/SOURCES.txt` & `no_pysha3_bip_utils-1.0.5.1/no_pysha3_bip_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `no_pysha3_bip_utils-1.0.5/setup.py` & `no_pysha3_bip_utils-1.0.5.1/setup.py`

 * *Files identical despite different names*

