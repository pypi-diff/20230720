# Comparing `tmp/ninjakiwi_api-0.0.5.tar.gz` & `tmp/ninjakiwi_api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjakiwi_api-0.0.5.tar", max compression
+gzip compressed data, was "ninjakiwi_api-0.0.6.tar", max compression
```

## Comparing `ninjakiwi_api-0.0.5.tar` & `ninjakiwi_api-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.5/LICENSE
--rw-r--r--   0        0        0      276 2023-07-20 11:06:00.144748 ninjakiwi_api-0.0.5/README.md
--rw-r--r--   0        0        0       84 2023-07-20 11:13:18.959090 ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTD6/__init__.py
--rw-r--r--   0        0        0     3002 2023-07-20 11:13:18.975757 ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTD6/function.py
--rw-r--r--   0        0        0       85 2023-07-20 11:13:18.942423 ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTDB2/__init__.py
--rw-r--r--   0        0        0     1085 2023-07-20 11:13:18.939090 ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTDB2/function.py
--rw-r--r--   0        0        0      184 2023-07-20 11:13:18.949090 ninjakiwi_api-0.0.5/ninjakiwi_api/API/__init__.py
--rw-r--r--   0        0        0      116 2023-07-20 11:38:30.257333 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
--rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/ERROR/function.py
--rw-r--r--   0        0        0      108 2023-07-20 11:38:30.260666 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
--rw-r--r--   0        0        0      746 2023-07-20 11:43:09.057477 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/FETCH/function.py
--rw-r--r--   0        0        0     1004 2023-07-20 12:10:12.190776 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/FETCH/model.py
--rw-r--r--   0        0        0      157 2023-07-20 11:38:30.267333 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/__init__.py
--rw-r--r--   0        0        0      185 2023-07-20 11:13:18.952423 ninjakiwi_api-0.0.5/ninjakiwi_api/__init__.py
--rw-r--r--   0        0        0     2902 2023-07-20 11:43:09.044143 ninjakiwi_api-0.0.5/ninjakiwi_api/main.py
--rw-r--r--   0        0        0     2756 2023-07-20 11:14:22.317483 ninjakiwi_api-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      666 2023-07-20 11:56:58.995664 ninjakiwi_api-0.0.5/tests/test_main.py
--rw-r--r--   0        0        0     2431 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.6/LICENSE
+-rw-r--r--   0        0        0      820 2023-07-20 12:50:41.021503 ninjakiwi_api-0.0.6/README.md
+-rw-r--r--   0        0        0       84 2023-07-20 11:13:18.959090 ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTD6/__init__.py
+-rw-r--r--   0        0        0     3002 2023-07-20 11:13:18.975757 ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTD6/function.py
+-rw-r--r--   0        0        0       85 2023-07-20 11:13:18.942423 ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTDB2/__init__.py
+-rw-r--r--   0        0        0     1085 2023-07-20 11:13:18.939090 ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTDB2/function.py
+-rw-r--r--   0        0        0      184 2023-07-20 11:13:18.949090 ninjakiwi_api-0.0.6/ninjakiwi_api/API/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-20 11:38:30.257333 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/ERROR/function.py
+-rw-r--r--   0        0        0      108 2023-07-20 11:38:30.260666 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-20 11:43:09.057477 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/FETCH/function.py
+-rw-r--r--   0        0        0      869 2023-07-20 12:39:11.245148 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/FETCH/model.py
+-rw-r--r--   0        0        0      157 2023-07-20 11:38:30.267333 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-20 11:13:18.952423 ninjakiwi_api-0.0.6/ninjakiwi_api/__init__.py
+-rw-r--r--   0        0        0     3109 2023-07-20 12:43:41.544888 ninjakiwi_api-0.0.6/ninjakiwi_api/main.py
+-rw-r--r--   0        0        0     2756 2023-07-20 12:43:41.554888 ninjakiwi_api-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-20 12:39:33.825683 ninjakiwi_api-0.0.6/tests/test_main.py
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.6/PKG-INFO
```

### Comparing `ninjakiwi_api-0.0.5/LICENSE` & `ninjakiwi_api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTD6/function.py` & `ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTD6/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTDB2/function.py` & `ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTDB2/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/ERROR/function.py` & `ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/ERROR/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/FETCH/function.py` & `ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/FETCH/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.5/ninjakiwi_api/main.py` & `ninjakiwi_api-0.0.6/ninjakiwi_api/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,16 +64,20 @@
     - The `api_fetch` function is used to perform the actual HTTP request and fetch the data from the API.
     - The returned dictionary will vary depending on the specific data being fetched.
     - If the provided game or data is not recognized or supported, the function returns None.
 
     Examples
     --------
     >>> data = await fetch("BTD6", "races")
-    >>> if data:
-    >>>     print(f"Successfully fetched race data: {data}")
+    >>> if data is not None:
+    >>>     raw = await data.get_raw_data()
+    >>>     example = await data.get_data("id")
+    >>>     print(f"Successfully fetched race data: {raw}")
+    >>>     if example is not None:
+    >>>         print(f"Successfully fetched race data: {example}")
     >>> else:
     >>>     print("Failed to fetch race data.")
     """
     url = await _game_to_func(game, data)
     if url is not None:
         return await _api_fetch(url)
     else:
```

### Comparing `ninjakiwi_api-0.0.5/pyproject.toml` & `ninjakiwi_api-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "ninjakiwi_api"
-version = "0.0.5"
+version = "0.0.6"
 homepage = "https://github.com/GustavoSchip/ninjakiwi_api"
 description = "NinjaKiwi API (OpenDATA) for Python! (My first library)"
 authors = [
     "Gustavo Schip <gustavoschip@proton.me>",
 ]
 maintainers = [
     "Gustavo Schip <gustavoschip@proton.me>",
```

### Comparing `ninjakiwi_api-0.0.5/tests/test_main.py` & `ninjakiwi_api-0.0.6/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,20 +14,28 @@
 
     assert results is not None
 
     data = await results.get_raw_data()
 
     assert "success" in data
 
+    temp = await results.get_data("id")
+
+    assert temp is not None
+
 
 @pytest.mark.asyncio
 async def test_fetch_btdb2():
     """Sample pytest test function."""
     from ninjakiwi_api import fetch
 
     results = await fetch("BTDB2", "homs")
 
     assert results is not None
 
     data = await results.get_raw_data()
 
     assert "success" in data
+
+    temp = await results.get_data("id")
+
+    assert temp is not None
```

### Comparing `ninjakiwi_api-0.0.5/PKG-INFO` & `ninjakiwi_api-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e69 6e6a  : 2.1.Name: ninj
 00000020: 616b 6977 692d 6170 690a 5665 7273 696f  akiwi-api.Versio
-00000030: 6e3a 2030 2e30 2e35 0a53 756d 6d61 7279  n: 0.0.5.Summary
+00000030: 6e3a 2030 2e30 2e36 0a53 756d 6d61 7279  n: 0.0.6.Summary
 00000040: 3a20 4e69 6e6a 614b 6977 6920 4150 4920  : NinjaKiwi API 
 00000050: 284f 7065 6e44 4154 4129 2066 6f72 2050  (OpenDATA) for P
 00000060: 7974 686f 6e21 2028 4d79 2066 6972 7374  ython! (My first
 00000070: 206c 6962 7261 7279 290a 486f 6d65 2d70   library).Home-p
 00000080: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000090: 6875 622e 636f 6d2f 4775 7374 6176 6f53  hub.com/GustavoS
 000000a0: 6368 6970 2f6e 696e 6a61 6b69 7769 5f61  chip/ninjakiwi_a
@@ -144,9 +144,43 @@
 000008f0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
 00000900: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 00000910: 696f 2f70 7970 692f 762f 6e69 6e6a 616b  io/pypi/v/ninjak
 00000920: 6977 692d 6170 692e 7376 6722 0a20 2020  iwi-api.svg".   
 00000930: 2020 2020 2061 6c74 203d 2022 5265 6c65       alt = "Rele
 00000940: 6173 6520 5374 6174 7573 223e 0a3c 2f61  ase Status">.</a
 00000950: 3e0a 3c2f 703e 0a0a 3c62 723e 0a0a 2320  >.</p>..<br>..# 
-00000960: 436f 6d69 6e67 2073 6f6f 6e2e 2e0a 5374  Coming soon...St
-00000970: 6179 2074 756e 6564 2067 7579 730a 0a    ay tuned guys..
+00000960: 5573 6167 650a 0a2e 2e2e 0a0a 2320 4578  Usage.......# Ex
+00000970: 616d 706c 650a 0a60 6060 7079 7468 6f6e  ample..```python
+00000980: 0a69 6d70 6f72 7420 6173 796e 6369 6f0a  .import asyncio.
+00000990: 6672 6f6d 206e 696e 6a61 6b69 7769 5f61  from ninjakiwi_a
+000009a0: 7069 2069 6d70 6f72 7420 6665 7463 680a  pi import fetch.
+000009b0: 0a0a 6173 796e 6320 6465 6620 7374 6172  ..async def star
+000009c0: 7428 293a 0a20 2020 2064 6174 6120 3d20  t():.    data = 
+000009d0: 6177 6169 7420 6665 7463 6828 2242 5444  await fetch("BTD
+000009e0: 3622 2c20 2272 6163 6573 2229 0a20 2020  6", "races").   
+000009f0: 2069 6620 6461 7461 2069 7320 6e6f 7420   if data is not 
+00000a00: 4e6f 6e65 3a0a 2020 2020 2020 2020 7261  None:.        ra
+00000a10: 7720 3d20 6177 6169 7420 6461 7461 2e67  w = await data.g
+00000a20: 6574 5f72 6177 5f64 6174 6128 290a 2020  et_raw_data().  
+00000a30: 2020 2020 2020 6578 616d 706c 6520 3d20        example = 
+00000a40: 6177 6169 7420 6461 7461 2e67 6574 5f64  await data.get_d
+00000a50: 6174 6128 2269 6422 290a 2020 2020 2020  ata("id").      
+00000a60: 2020 7072 696e 7428 6622 5375 6363 6573    print(f"Succes
+00000a70: 7366 756c 6c79 2066 6574 6368 6564 2072  sfully fetched r
+00000a80: 6163 6520 6461 7461 3a20 7b72 6177 7d22  ace data: {raw}"
+00000a90: 290a 2020 2020 2020 2020 6966 2065 7861  ).        if exa
+00000aa0: 6d70 6c65 2069 7320 6e6f 7420 4e6f 6e65  mple is not None
+00000ab0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00000ac0: 696e 7428 6622 5375 6363 6573 7366 756c  int(f"Successful
+00000ad0: 6c79 2066 6574 6368 6564 2072 6163 6520  ly fetched race 
+00000ae0: 6461 7461 3a20 7b65 7861 6d70 6c65 7d22  data: {example}"
+00000af0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00000b00: 2020 2020 7072 696e 7428 2246 6169 6c65      print("Faile
+00000b10: 6420 746f 2066 6574 6368 2072 6163 6520  d to fetch race 
+00000b20: 6461 7461 2e22 290a 0a0a 6465 6620 6d61  data.")...def ma
+00000b30: 696e 2829 3a0a 2020 2020 6173 796e 6369  in():.    asynci
+00000b40: 6f2e 7275 6e28 7374 6172 7428 2929 0a0a  o.run(start())..
+00000b50: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+00000b60: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
+00000b70: 6d61 696e 2829 0a60 6060 0a0a 2320 436f  main().```..# Co
+00000b80: 6d69 6e67 2073 6f6f 6e2e 2e2e 0a0a 5374  ming soon.....St
+00000b90: 6179 2074 756e 6564 2067 7579 730a 0a    ay tuned guys..
```

