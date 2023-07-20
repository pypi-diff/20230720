# Comparing `tmp/llamaapi-0.1.2.tar.gz` & `tmp/llamaapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamaapi-0.1.2.tar", max compression
+gzip compressed data, was "llamaapi-0.1.3.tar", max compression
```

## Comparing `llamaapi-0.1.2.tar` & `llamaapi-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.2/LICENSE
--rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.2/README.md
--rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.2/llamaapi/__init__.py
--rw-r--r--   0        0        0     1523 2023-07-20 17:12:20.199684 llamaapi-0.1.2/llamaapi/llamaapi.py
--rw-r--r--   0        0        0      344 2023-07-20 17:15:21.597697 llamaapi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 llamaapi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.3/README.md
+-rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.3/llamaapi/__init__.py
+-rw-r--r--   0        0        0     1624 2023-07-20 17:36:40.114793 llamaapi-0.1.3/llamaapi/llamaapi.py
+-rw-r--r--   0        0        0      344 2023-07-20 17:36:44.344794 llamaapi-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 llamaapi-0.1.3/PKG-INFO
```

### Comparing `llamaapi-0.1.2/LICENSE` & `llamaapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.2/README.md` & `llamaapi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.2/llamaapi/llamaapi.py` & `llamaapi-0.1.3/llamaapi/llamaapi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 # LlamaAPI.py
 
 import aiohttp
 import asyncio
 import requests
-from concurrent.futures import ThreadPoolExecutor
+from threading import Thread
+from queue import Queue
 
 hostname = 'https://llama-api3.fly.dev'
 
 class LlamaAPI:
     def __init__(self, api_token):
         self.hostname = hostname
         self.api_token = api_token
         self.headers = {'Llama-API-Token': self.api_token}
 
-    async def _run_stream(self, api_request_json):
+    async def _run_stream(self, api_request_json, queue):
         async with aiohttp.ClientSession() as session:
             async with session.post(f"{self.hostname}/api/chat", headers=self.headers, json=api_request_json) as resp:
-                return [chunk.decode('utf-8') async for chunk in resp.content.iter_any()]
+                async for chunk in resp.content.iter_any():
+                    queue.put(chunk.decode('utf-8'))
+        queue.put(None)  # Signal the end of the iterator
 
     def run_stream(self, api_request_json):
-        with ThreadPoolExecutor() as executor:
+        queue = Queue()
+
+        def target():
             loop = asyncio.new_event_loop()
-            try:
-                asyncio.set_event_loop(loop)
-                return loop.run_until_complete(self._run_stream(api_request_json))
-            finally:
-                asyncio.set_event_loop(None)
+            asyncio.set_event_loop(loop)
+            loop.run_until_complete(self._run_stream(api_request_json, queue))
+            loop.close()
+
+        Thread(target=target).start()
+        return iter(queue.get, None)
 
     def run_simple(self, api_request_json):
         response = requests.post(f"{self.hostname}/api/chat", headers=self.headers, json=api_request_json)
         if response.status_code != 200:
             raise Exception(f"POST {response.status_code}")
         return response.json()  # assuming server responds with JSON
```

### Comparing `llamaapi-0.1.2/PKG-INFO` & `llamaapi-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamaapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Llama API python SDK
 License: MIT
 Author: Eduardo Reis
 Author-email: edu.pontes@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

