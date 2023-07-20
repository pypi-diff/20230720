# Comparing `tmp/minecraftstatus-0.0.8.tar.gz` & `tmp/minecraftstatus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraftstatus-0.0.8.tar", max compression
+gzip compressed data, was "minecraftstatus-0.0.9.tar", max compression
```

## Comparing `minecraftstatus-0.0.8.tar` & `minecraftstatus-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1087 2022-03-10 02:30:06.000000 minecraftstatus-0.0.8/LICENSE
--rw-r--r--   0        0        0      388 2022-03-10 02:30:06.000000 minecraftstatus-0.0.8/minecraftstatus/__init__.py
--rw-r--r--   0        0        0     3224 2023-07-05 13:58:33.599966 minecraftstatus-0.0.8/minecraftstatus/client.py
--rw-r--r--   0        0        0     1000 2022-03-15 12:48:24.000000 minecraftstatus-0.0.8/minecraftstatus/errors.py
--rw-r--r--   0        0        0      429 2022-03-10 02:30:06.000000 minecraftstatus-0.0.8/minecraftstatus/http.py
--rw-r--r--   0        0        0     3389 2023-07-05 14:21:25.086552 minecraftstatus-0.0.8/minecraftstatus/server_status.py
--rw-r--r--   0        0        0      534 2023-07-04 13:54:18.974850 minecraftstatus-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1279 2023-07-04 13:51:09.785431 minecraftstatus-0.0.8/README.md
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 minecraftstatus-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-05 14:31:32.387762 minecraftstatus-0.0.9/LICENSE
+-rw-r--r--   0        0        0      388 2023-07-20 12:55:17.685490 minecraftstatus-0.0.9/minecraftstatus/__init__.py
+-rw-r--r--   0        0        0     3386 2023-07-20 12:53:22.816904 minecraftstatus-0.0.9/minecraftstatus/client.py
+-rw-r--r--   0        0        0     1000 2022-03-15 12:48:24.000000 minecraftstatus-0.0.9/minecraftstatus/errors.py
+-rw-r--r--   0        0        0      640 2023-07-20 12:35:44.659013 minecraftstatus-0.0.9/minecraftstatus/http.py
+-rw-r--r--   0        0        0     3389 2023-07-05 14:21:25.086552 minecraftstatus-0.0.9/minecraftstatus/server_status.py
+-rw-r--r--   0        0        0      534 2023-07-20 12:54:29.654735 minecraftstatus-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1279 2023-07-04 13:51:09.785431 minecraftstatus-0.0.9/README.md
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 minecraftstatus-0.0.9/PKG-INFO
```

### Comparing `minecraftstatus-0.0.8/LICENSE` & `minecraftstatus-0.0.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Infernum1
+Copyright (c) 2023 Infernum1
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `minecraftstatus-0.0.8/minecraftstatus/client.py` & `minecraftstatus-0.0.9/minecraftstatus/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,36 +9,43 @@
 
 
 class MCStatus(HTTPClient):
     """
     The main MCStatus class.
     """
 
-    def __init__(self) -> None:
-        HTTPClient.__init__(self)
+    def __init__(self):
+        super().__init__()
+
+    async def __aenter__(self):
+        await self.open()
+        return self
+
+    async def __aexit__(self, *args, **kwargs):
+        await self.close()
 
     async def get_server(self, ip_address: str):
         """
         :param ip_address: IP address of the server
         :type ip_address: :class:`str`
         :raises ServerNotFound: server not found or is offline
         :return: a :class:`ServerStatus` class instance
         """
 
         resp = await self._request("GET", base_url.format(f"mc/server/status/{ip_address}"))
         data = await resp.json()
+
         if data["online"] is False:
-            await self._close()
             raise ServerNotFound(ip_address)
 
-        await self._close()
         return ServerStatus(data)
 
     async def get_server_card(self, ip_address: str, custom_server_name: str = ""):
         """
+        **This is a method of the MCStatus class**\n
         :param ip_address: IP address of the server
         :param custom_server_name: A custom server name to be displayed on the server card
         :type ip_address: :class:`str`
         :type custom_server_name: :class:`str`
         :raises `BadTextFormation`: text passed is not between 1-30 characters
         :return: an :class:`io.BytesIO` object co-relating the server card image.
         """
@@ -48,39 +55,40 @@
         if len(ip_address) > 30 and len(ip_address) < 1:
             raise BadTextFormation()
 
         res = await self._request(
             "GET", base_url.format(f"mc/server/status/{ip_address}/image?customName={custom_server_name}")
         )
         image = BytesIO(await res.read())
-        await self._close()
         return image
 
     async def achievement(self, achievement: str):
         """
+        **This is a method of the MCStatus class**
         :param achievement: name of the achievement to display.
         :type achievement: :class:`str`
         :raises BadTextFormation: text passed is not between 1-30 characters
         :return: an :class:`io.BytesIO` object co-relating the achievement image.
         """
         if len(achievement) > 30 and len(achievement) > 1:
             raise BadTextFormation()
 
         res = await self._request("GET", base_url.format(f"mc/image/achievement/{achievement}"))
         image = BytesIO(await res.read())
-        await self._close()
+
         return image
 
     async def splash_text(self, text: str):
         """
+        **This is a method of the MCStatus class**
         :param text: text to display in the splash.
         :type text: :class:`str`
         :raises BadTextFormation: text passed is not between 1-30 characters
         :return: an :class:`io.BytesIO` object co-relating the splash text image.
         """
         if len(text) > 30 and len(text) < 1:
             raise BadTextFormation()
 
         res = await self._request("GET", base_url.format(f"mc/image/splash/{text}"))
         image = BytesIO(await res.read())
-        await self._close()
+
         return image
```

### Comparing `minecraftstatus-0.0.8/minecraftstatus/errors.py` & `minecraftstatus-0.0.9/minecraftstatus/errors.py`

 * *Files identical despite different names*

### Comparing `minecraftstatus-0.0.8/minecraftstatus/server_status.py` & `minecraftstatus-0.0.9/minecraftstatus/server_status.py`

 * *Files identical despite different names*

### Comparing `minecraftstatus-0.0.8/pyproject.toml` & `minecraftstatus-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "minecraftstatus"
-version = "0.0.8"
+version = "0.0.9"
 description = "minecraftstatus is an asynchronous wrapper for https://api.iapetus11.me."
 authors = ["Infernum1"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Infernum1/minecraftstatus"
 
 [tool.poetry.dependencies]
```

### Comparing `minecraftstatus-0.0.8/README.md` & `minecraftstatus-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `minecraftstatus-0.0.8/PKG-INFO` & `minecraftstatus-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraftstatus
-Version: 0.0.8
+Version: 0.0.9
 Summary: minecraftstatus is an asynchronous wrapper for https://api.iapetus11.me.
 Home-page: https://github.com/Infernum1/minecraftstatus
 License: MIT
 Author: Infernum1
 Requires-Python: >3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

