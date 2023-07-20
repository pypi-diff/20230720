# Comparing `tmp/rubpy-6.3.0.tar.gz` & `tmp/rubpy-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.3.0.tar", last modified: Thu Jul 20 00:56:17 2023, max compression
+gzip compressed data, was "rubpy-6.3.1.tar", last modified: Thu Jul 20 09:51:42 2023, max compression
```

## Comparing `rubpy-6.3.0.tar` & `rubpy-6.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 00:56:17.894381 rubpy-6.3.0/
--rw-rw-rw-   0        0        0     3378 2023-07-20 00:56:17.894381 rubpy-6.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 00:56:17.847102 rubpy-6.3.0/rubpy/
--rw-rw-rw-   0        0        0      240 2023-07-20 00:55:46.000000 rubpy-6.3.0/rubpy/__init__.py
--rw-rw-rw-   0        0        0    44693 2023-07-19 15:51:55.000000 rubpy-6.3.0/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:56:17.863122 rubpy-6.3.0/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     3288 2023-07-19 15:43:06.000000 rubpy-6.3.0/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:56:17.863122 rubpy-6.3.0/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.3.0/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.3.0/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.3.0/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.3.0/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     6772 2023-06-29 12:36:38.000000 rubpy-6.3.0/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:56:17.878760 rubpy-6.3.0/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    12281 2023-07-20 00:22:22.000000 rubpy-6.3.0/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:56:17.878760 rubpy-6.3.0/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.3.0/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:56:17.878760 rubpy-6.3.0/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.3.0/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.3.0/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:56:17.863122 rubpy-6.3.0/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-07-20 00:56:17.000000 rubpy-6.3.0/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-07-20 00:56:17.000000 rubpy-6.3.0/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 00:56:17.000000 rubpy-6.3.0/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-20 00:56:17.000000 rubpy-6.3.0/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-20 00:56:17.000000 rubpy-6.3.0/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 00:56:17.894381 rubpy-6.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-07-20 00:55:32.000000 rubpy-6.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:51:42.118984 rubpy-6.3.1/
+-rw-rw-rw-   0        0        0     3378 2023-07-20 09:51:42.118984 rubpy-6.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 09:51:42.024793 rubpy-6.3.1/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-07-20 09:50:59.000000 rubpy-6.3.1/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    44693 2023-07-19 15:51:55.000000 rubpy-6.3.1/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:51:42.056162 rubpy-6.3.1/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3288 2023-07-19 15:43:06.000000 rubpy-6.3.1/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:51:42.084547 rubpy-6.3.1/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.3.1/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.3.1/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.3.1/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.3.1/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     6772 2023-06-29 12:36:38.000000 rubpy-6.3.1/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:51:42.094680 rubpy-6.3.1/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    12184 2023-07-20 09:50:47.000000 rubpy-6.3.1/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:51:42.104908 rubpy-6.3.1/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.3.1/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:51:42.114796 rubpy-6.3.1/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.3.1/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.3.1/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:51:42.056162 rubpy-6.3.1/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-07-20 09:51:41.000000 rubpy-6.3.1/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-20 09:51:41.000000 rubpy-6.3.1/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 09:51:41.000000 rubpy-6.3.1/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-20 09:51:41.000000 rubpy-6.3.1/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 09:51:41.000000 rubpy-6.3.1/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 09:51:42.118984 rubpy-6.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-07-20 09:51:21.000000 rubpy-6.3.1/setup.py
```

### Comparing `rubpy-6.3.0/PKG-INFO` & `rubpy-6.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.3.0
+Version: 6.3.1
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.3.0 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.3.1 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.3.0/README.md` & `rubpy-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/client.py` & `rubpy-6.3.1/rubpy/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/crypto/crypto.py` & `rubpy-6.3.1/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/gadgets/classino.py` & `rubpy-6.3.1/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/gadgets/exceptions.py` & `rubpy-6.3.1/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/gadgets/grouping.py` & `rubpy-6.3.1/rubpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/gadgets/methods.py` & `rubpy-6.3.1/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/gadgets/thumbnail.py` & `rubpy-6.3.1/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/network/connection.py` & `rubpy-6.3.1/rubpy/network/connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -279,40 +279,39 @@
 
         self._client._logger.debug('upload failed', extra={'data': result})
         raise exceptions(status_det)(result, request=result)
 
     async def download(self, dc_id: int, file_id: int, access_hash: str, size: int, chunk=131072, callback=None):
         url = f'https://messenger{dc_id}.iranlms.ir/GetFile.ashx'
         start_index = 0
-        last_index = int(size) if int(size) <= chunk else chunk
-        result: bytes = b''
+        result = b''
 
         headers = {
             'auth': self._client._auth,
             'access-hash-rec': access_hash,
             'file-id': str(file_id),
-            'start-index': str(start_index),
-            'last-index': str(last_index)
+            'user-agent': self._client._user_agent
         }
 
         async with aiohttp.ClientSession() as session:
             while True:
-                async with session.post(url, headers=headers) as response:
-                    data = await response.read()
-                    result += data
+                last_index = start_index + chunk - 1 if start_index + chunk < size else size - 1
+
+                headers['start-index'] = str(start_index)
+                headers['last-index'] = str(last_index)
 
-                    if callback:
-                        await callback(size, len(result))
+                async with session.post(url, headers=headers) as response:
+                    if response.status == 200:
+                        data = await response.read()
+                        if data:
+                            result += data
+                            if callback:
+                                await callback(size, len(result))
+
+                # بررسی پایان فایل
+                if len(result) >= size:
+                    break
 
-                    # بروزرسانی مقادیر start_index و last_index برای دریافت بخش بعدی فایل
-                    start_index += len(data)
-                    last_index = start_index + chunk - 1
-
-                    # بررسی پایان فایل
-                    if len(data) < chunk:
-                        break
-
-                    # بروزرسانی هدرها برای دریافت بخش بعدی فایل
-                    headers['start-index'] = str(start_index)
-                    headers['last-index'] = str(last_index)
+                # بروزرسانی مقدار start_index برای دریافت بخش بعدی فایل
+                start_index = last_index + 1
 
         return result
```

### Comparing `rubpy-6.3.0/rubpy/network/proxies.py` & `rubpy-6.3.1/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/sessions/sqliteSession.py` & `rubpy-6.3.1/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/sessions/stringSession.py` & `rubpy-6.3.1/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/structs/handlers.py` & `rubpy-6.3.1/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/structs/models.py` & `rubpy-6.3.1/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/structs/results.py` & `rubpy-6.3.1/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy/structs/struct.py` & `rubpy-6.3.1/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/rubpy.egg-info/PKG-INFO` & `rubpy-6.3.1/rubpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.3.0
+Version: 6.3.1
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.3.0 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.3.1 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.3.0/rubpy.egg-info/SOURCES.txt` & `rubpy-6.3.1/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.3.0/setup.py` & `rubpy-6.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.3.0',
+    version = '6.3.1',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

