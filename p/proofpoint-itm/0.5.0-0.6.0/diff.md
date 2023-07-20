# Comparing `tmp/proofpoint_itm-0.5.0.tar.gz` & `tmp/proofpoint_itm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proofpoint_itm-0.5.0.tar", last modified: Fri Jun  2 21:19:12 2023, max compression
+gzip compressed data, was "proofpoint_itm-0.6.0.tar", last modified: Thu Jul 20 21:40:24 2023, max compression
```

## Comparing `proofpoint_itm-0.5.0.tar` & `proofpoint_itm-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-06-02 21:19:12.657489 proofpoint_itm-0.5.0/
--rw-r--r--   0 molden     (501) staff       (20)    11357 2021-11-16 02:23:49.000000 proofpoint_itm-0.5.0/LICENSE
--rw-r--r--   0 molden     (501) staff       (20)     1432 2023-06-02 21:19:12.657547 proofpoint_itm-0.5.0/PKG-INFO
--rw-r--r--   0 molden     (501) staff       (20)      813 2023-05-17 16:06:21.000000 proofpoint_itm-0.5.0/README.md
--rw-r--r--   0 molden     (501) staff       (20)       74 2023-06-02 21:19:12.657761 proofpoint_itm-0.5.0/setup.cfg
--rw-r--r--   0 molden     (501) staff       (20)      925 2023-06-02 21:18:12.000000 proofpoint_itm-0.5.0/setup.py
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-06-02 21:19:12.654827 proofpoint_itm-0.5.0/src/
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-06-02 21:19:12.656834 proofpoint_itm-0.5.0/src/proofpoint_itm/
--rw-r--r--   0 molden     (501) staff       (20)       43 2022-10-14 21:09:35.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/__init__.py
--rw-r--r--   0 molden     (501) staff       (20)     1359 2022-11-23 17:14:39.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/auth.py
--rw-r--r--   0 molden     (501) staff       (20)    10810 2022-12-13 03:20:50.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/classes.py
--rw-r--r--   0 molden     (501) staff       (20)    49995 2023-06-02 21:15:31.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/client.py
--rw-r--r--   0 molden     (501) staff       (20)     2458 2023-06-02 21:10:35.000000 proofpoint_itm-0.5.0/src/proofpoint_itm/webclient.py
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-06-02 21:19:12.657376 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/
--rw-r--r--   0 molden     (501) staff       (20)     1432 2023-06-02 21:19:12.000000 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/PKG-INFO
--rw-r--r--   0 molden     (501) staff       (20)      353 2023-06-02 21:19:12.000000 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/SOURCES.txt
--rw-r--r--   0 molden     (501) staff       (20)        1 2023-06-02 21:19:12.000000 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/dependency_links.txt
--rw-r--r--   0 molden     (501) staff       (20)       15 2023-06-02 21:19:12.000000 proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/top_level.txt
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-07-20 21:40:24.883543 proofpoint_itm-0.6.0/
+-rw-r--r--   0 molden     (501) staff       (20)    11357 2021-11-16 02:23:49.000000 proofpoint_itm-0.6.0/LICENSE
+-rw-r--r--   0 molden     (501) staff       (20)     1432 2023-07-20 21:40:24.883600 proofpoint_itm-0.6.0/PKG-INFO
+-rw-r--r--   0 molden     (501) staff       (20)      813 2023-05-17 16:06:21.000000 proofpoint_itm-0.6.0/README.md
+-rw-r--r--   0 molden     (501) staff       (20)       74 2023-07-20 21:40:24.883807 proofpoint_itm-0.6.0/setup.cfg
+-rw-r--r--   0 molden     (501) staff       (20)      925 2023-07-20 21:39:08.000000 proofpoint_itm-0.6.0/setup.py
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-07-20 21:40:24.880452 proofpoint_itm-0.6.0/src/
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-07-20 21:40:24.882766 proofpoint_itm-0.6.0/src/proofpoint_itm/
+-rw-r--r--   0 molden     (501) staff       (20)       43 2022-10-14 21:09:35.000000 proofpoint_itm-0.6.0/src/proofpoint_itm/__init__.py
+-rw-r--r--   0 molden     (501) staff       (20)     1686 2023-07-12 23:28:29.000000 proofpoint_itm-0.6.0/src/proofpoint_itm/auth.py
+-rw-r--r--   0 molden     (501) staff       (20)    10810 2022-12-13 03:20:50.000000 proofpoint_itm-0.6.0/src/proofpoint_itm/classes.py
+-rw-r--r--   0 molden     (501) staff       (20)    58883 2023-07-20 21:18:26.000000 proofpoint_itm-0.6.0/src/proofpoint_itm/client.py
+-rw-r--r--   0 molden     (501) staff       (20)     2458 2023-06-02 21:10:35.000000 proofpoint_itm-0.6.0/src/proofpoint_itm/webclient.py
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-07-20 21:40:24.883436 proofpoint_itm-0.6.0/src/proofpoint_itm.egg-info/
+-rw-r--r--   0 molden     (501) staff       (20)     1432 2023-07-20 21:40:24.000000 proofpoint_itm-0.6.0/src/proofpoint_itm.egg-info/PKG-INFO
+-rw-r--r--   0 molden     (501) staff       (20)      353 2023-07-20 21:40:24.000000 proofpoint_itm-0.6.0/src/proofpoint_itm.egg-info/SOURCES.txt
+-rw-r--r--   0 molden     (501) staff       (20)        1 2023-07-20 21:40:24.000000 proofpoint_itm-0.6.0/src/proofpoint_itm.egg-info/dependency_links.txt
+-rw-r--r--   0 molden     (501) staff       (20)       15 2023-07-20 21:40:24.000000 proofpoint_itm-0.6.0/src/proofpoint_itm.egg-info/top_level.txt
```

### Comparing `proofpoint_itm-0.5.0/LICENSE` & `proofpoint_itm-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.5.0/PKG-INFO` & `proofpoint_itm-0.6.0/src/proofpoint_itm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: proofpoint_itm
-Version: 0.5.0
+Name: proofpoint-itm
+Version: 0.6.0
 Summary: Proofpoint ITM API client library
 Home-page: https://github.com/drizzo-tech/proofpoint_itm
 Author: Mike Olden
 Author-email: michael.olden@oldendigital.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/drizzo-tech/proofpoint_itm/issues
 Keywords: Proofpoint ITM,Proofpoint,ITM,ObserveIT
```

### Comparing `proofpoint_itm-0.5.0/README.md` & `proofpoint_itm-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.5.0/setup.py` & `proofpoint_itm-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(name='proofpoint_itm',
-    version='0.5.0',
+    version='0.6.0',
     description='Proofpoint ITM API client library',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Mike Olden',
     author_email='michael.olden@oldendigital.com',
     url = 'https://github.com/drizzo-tech/proofpoint_itm',
     project_urls={
```

### Comparing `proofpoint_itm-0.5.0/src/proofpoint_itm/auth.py` & `proofpoint_itm-0.6.0/src/proofpoint_itm/auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from proofpoint_itm import webclient
 
 class itm_auth:
     """
     Basic class to represent API Auth Info
     """
-    def __init__(self, config, verify=True, scope='*', grant_type='client_credentials'):
+    def __init__(self, config, verify=True, scope='*', grant_type='client_credentials', development=False):
         self.tenant_id = config['tenant_id']
         self.client_id = config['client_id']
         self.client_secret = config['client_secret']
+        self.development = development
         self.scope = scope
         self.grant_type = grant_type
         self.verify = verify
         self.token = self.get_token()
         self.access_token = self.token['access_token']
+        
 
     def get_token(self):
         endpoint = '/v2/apis/auth/oauth/token'
         base_url = f"https://{self.tenant_id}.explore.proofpoint.com"
         url = base_url + endpoint
 
         headers = {
@@ -26,14 +28,22 @@
         payload = {
             'client_id': self.client_id,
             'client_secret': self.client_secret,
             'grant_type': self.grant_type,
             'scope': self.scope
         }
 
+        if self.development:
+            return {
+                'access_token': 'access-token-testing123',
+                'token_type': 'Bearer',
+                'expires_in': 3599,
+                'refresh_token': 'refresh-token-testing123'
+            }
+
         resp = webclient.post_request(url, headers=headers, data=payload)
         token = {
             'access_token': resp['access_token'],
             'token_type': resp['token_type'],
             'expires_in': resp['expires_in'],
             'refresh_token': resp['refresh_token']
         }
```

### Comparing `proofpoint_itm-0.5.0/src/proofpoint_itm/classes.py` & `proofpoint_itm-0.6.0/src/proofpoint_itm/classes.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.5.0/src/proofpoint_itm/webclient.py` & `proofpoint_itm-0.6.0/src/proofpoint_itm/webclient.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.5.0/src/proofpoint_itm.egg-info/PKG-INFO` & `proofpoint_itm-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: proofpoint-itm
-Version: 0.5.0
+Name: proofpoint_itm
+Version: 0.6.0
 Summary: Proofpoint ITM API client library
 Home-page: https://github.com/drizzo-tech/proofpoint_itm
 Author: Mike Olden
 Author-email: michael.olden@oldendigital.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/drizzo-tech/proofpoint_itm/issues
 Keywords: Proofpoint ITM,Proofpoint,ITM,ObserveIT
```

