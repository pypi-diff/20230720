# Comparing `tmp/pydeezer_asy-1.2.1.tar.gz` & `tmp/pydeezer_asy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-1.2.1.tar", last modified: Wed Jul 12 12:56:22 2023, max compression
+gzip compressed data, was "pydeezer_asy-1.2.2.tar", last modified: Thu Jul 20 19:35:58 2023, max compression
```

## Comparing `pydeezer_asy-1.2.1.tar` & `pydeezer_asy-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:56:22.773484 pydeezer_asy-1.2.1/
--rw-rw-rw-   0        0        0     1662 2023-07-12 12:56:22.772487 pydeezer_asy-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1298 2023-07-12 12:53:05.000000 pydeezer_asy-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 12:56:22.625878 pydeezer_asy-1.2.1/deezer_asy/
--rw-rw-rw-   0        0        0    30354 2023-07-12 11:17:17.000000 pydeezer_asy-1.2.1/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.2.1/deezer_asy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:56:22.661784 pydeezer_asy-1.2.1/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.1/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.2.1/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:56:22.771531 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0     1662 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 12:56:22.000000 pydeezer_asy-1.2.1/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 12:56:22.775481 pydeezer_asy-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-07-12 12:56:15.000000 pydeezer_asy-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:35:58.542185 pydeezer_asy-1.2.2/
+-rw-rw-rw-   0        0        0     1662 2023-07-20 19:35:58.541195 pydeezer_asy-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1298 2023-07-12 12:53:05.000000 pydeezer_asy-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 19:35:58.464397 pydeezer_asy-1.2.2/deezer_asy/
+-rw-rw-rw-   0        0        0    32057 2023-07-20 19:35:28.000000 pydeezer_asy-1.2.2/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.2.2/deezer_asy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:35:58.486338 pydeezer_asy-1.2.2/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.2.2/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:35:58.539193 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0     1662 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 19:35:58.543183 pydeezer_asy-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-20 19:35:42.000000 pydeezer_asy-1.2.2/setup.py
```

### Comparing `pydeezer_asy-1.2.1/PKG-INFO` & `pydeezer_asy-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeezer_asy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pydeezer_asy-1.2.1/README.md` & `pydeezer_asy-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.1/deezer_asy/DeezerAsy.py` & `pydeezer_asy-1.2.2/deezer_asy/DeezerAsy.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,18 +48,68 @@
 
 
     """
         GENERAL
     """
     async def _generate_main_session(self):
         await self.get_user_data()
-
+    def _sync_generate_main_session(self):
+        self.sync_get_user_data()
     """
         API
     """
+    ####
+    def sync_get_user_data(self):
+        import requests
+        method = api_methods.GET_USER_DATA
+
+        l_session = requests.Session()
+        l_session.headers.update(networking_settings.HTTP_HEADERS)
+
+        
+
+        token = "null"
+        if method != api_methods.GET_USER_DATA:
+            token = self.token
+
+        req = l_session.post(api_urls.API_URL,json={}, params={
+            "api_version": "1.0",
+            "api_token": token,
+            "input": "3",
+            "method": method
+        }, cookies={'arl': self.arl})
+        if req.status_code:
+            data = req.json()
+            data = data['results']
+            self.token = data["checkForm"]
+
+            if not data["USER"]["USER_ID"]:
+                raise LoginError("Arl is invalid.")
+
+            raw_user = data["USER"]
+
+            _arl = self.arl
+            self.cookies = l_session.cookies
+            
+            if raw_user["USER_PICTURE"]:
+                self.user = {
+                    "id": raw_user["USER_ID"],
+                    "name": raw_user["BLOG_NAME"],
+                    "arl": _arl,
+                    "image": "https://e-cdns-images.dzcdn.net/images/user/{0}/250x250-000000-80-0-0.jpg".format(raw_user["USER_PICTURE"])
+                }
+            else:
+                self.user = {
+                    "id": raw_user["USER_ID"],
+                    "name": raw_user["BLOG_NAME"],
+                    "arl": _arl,
+                    "image": "https://e-cdns-images.dzcdn.net/images/user/250x250-000000-80-0-0.jpg"
+                }
+    ####
+
     async def get_user_data(self):
         """Gets the data of the user, this will only work arl is the cookie. Make sure you have run login_via_arl() before using this.
 
         Raises:
             LoginError: Will raise if the arl given is not identified by Deezer
         """
```

### Comparing `pydeezer_asy-1.2.1/deezer_asy/constants/api_methods.py` & `pydeezer_asy-1.2.2/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.1/deezer_asy/constants/track_formats.py` & `pydeezer_asy-1.2.2/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.1/deezer_asy/util.py` & `pydeezer_asy-1.2.2/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.1/pydeezer_asy.egg-info/PKG-INFO` & `pydeezer_asy-1.2.2/pydeezer_asy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeezer-asy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pydeezer_asy-1.2.1/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-1.2.2/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.1/setup.py` & `pydeezer_asy-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pydeezer_asy',
-    version='1.2.1',
+    version='1.2.2',
     description='Asynchronous version of the `py-deezer` module',
     author='drhspfn',
     author_email="drhspfn@gmail.com",
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/drhspfn/deezer-asy",
```

