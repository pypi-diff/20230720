# Comparing `tmp/adafri-0.0.42.tar.gz` & `tmp/adafri-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.42.tar", last modified: Thu Jul 20 08:04:13 2023, max compression
+gzip compressed data, was "adafri-0.0.43.tar", last modified: Thu Jul 20 08:16:07 2023, max compression
```

## Comparing `adafri-0.0.42.tar` & `adafri-0.0.43.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.307788 adafri-0.0.42/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-20 08:04:13.307425 adafri-0.0.42/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.274742 adafri-0.0.42/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-20 08:04:09.000000 adafri-0.0.42/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.279286 adafri-0.0.42/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.42/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.42/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16483 2023-07-20 06:24:00.000000 adafri-0.0.42/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.280326 adafri-0.0.42/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.42/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.281306 adafri-0.0.42/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.42/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.283923 adafri-0.0.42/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.42/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.42/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.42/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.285005 adafri-0.0.42/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.42/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.286632 adafri-0.0.42/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.42/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.42/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.287501 adafri-0.0.42/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.42/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.287959 adafri-0.0.42/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.42/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.294739 adafri-0.0.42/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.42/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6729 2023-07-20 06:02:29.000000 adafri-0.0.42/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.42/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16660 2023-07-20 07:26:41.000000 adafri-0.0.42/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.42/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9269 2023-07-20 08:03:53.000000 adafri-0.0.42/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:37:50.000000 adafri-0.0.42/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.297151 adafri-0.0.42/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.42/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.42/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.42/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.299335 adafri-0.0.42/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.42/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.42/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.299961 adafri-0.0.42/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.42/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.306252 adafri-0.0.42/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.42/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9309 2023-07-20 05:13:59.000000 adafri-0.0.42/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.42/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:04:13.277070 adafri-0.0.42/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-20 08:04:13.000000 adafri-0.0.42/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-20 08:04:13.000000 adafri-0.0.42/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-20 08:04:13.000000 adafri-0.0.42/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-20 08:04:13.000000 adafri-0.0.42/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-20 08:04:13.307936 adafri-0.0.42/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.42/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.805829 adafri-0.0.43/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-20 08:16:07.805385 adafri-0.0.43/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.771708 adafri-0.0.43/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-20 08:15:32.000000 adafri-0.0.43/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.776147 adafri-0.0.43/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.43/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.43/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16483 2023-07-20 06:24:00.000000 adafri-0.0.43/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.777485 adafri-0.0.43/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.43/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.778651 adafri-0.0.43/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.43/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.785196 adafri-0.0.43/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.43/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.43/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.43/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.786022 adafri-0.0.43/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.43/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.787384 adafri-0.0.43/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.43/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.43/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.788423 adafri-0.0.43/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.43/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.788881 adafri-0.0.43/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.43/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.795666 adafri-0.0.43/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.43/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6729 2023-07-20 06:02:29.000000 adafri-0.0.43/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.43/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16019 2023-07-20 08:16:00.000000 adafri-0.0.43/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.43/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9269 2023-07-20 08:03:53.000000 adafri-0.0.43/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:37:50.000000 adafri-0.0.43/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.798657 adafri-0.0.43/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.43/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.43/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.43/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.800834 adafri-0.0.43/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.43/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.43/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.801408 adafri-0.0.43/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.43/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.804341 adafri-0.0.43/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.43/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9309 2023-07-20 05:13:59.000000 adafri-0.0.43/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.43/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:16:07.773939 adafri-0.0.43/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-20 08:16:07.000000 adafri-0.0.43/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-20 08:16:07.000000 adafri-0.0.43/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-20 08:16:07.000000 adafri-0.0.43/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-20 08:16:07.000000 adafri-0.0.43/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-20 08:16:07.811434 adafri-0.0.43/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.43/setup.py
```

### Comparing `adafri-0.0.42/adafri/utils/response.py` & `adafri-0.0.43/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/utils/utils.py` & `adafri-0.0.43/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/account/models/account.py` & `adafri-0.0.43/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/account/models/account_fields.py` & `adafri-0.0.43/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.43/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.43/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.43/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.43/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.43/adafri/v1/auth/oauth/models/grant.py`

 * *Files 4% similar despite different names*

```diff
@@ -330,14 +330,17 @@
         return exists_nonce(nonce, request)
 
     def get_jwt_config(self, grant):
         return DUMMY_JWT_CONFIG
 
     def generate_user_info(self, user, scope):
         return generate_user_info(user, scope)
+    
+    def authenticate_user(self, authorization_code):
+        return User({"uid": authorization_code.uid}).get()
 
 
 class OpenIDHybridGrant(_OpenIDHybridGrant):
     DEFAULT_RESPONSE_MODE = 'query'
     def create_authorization_code(self, client, grant_user, request):
         return create_authorization_code(client, grant_user, request)
     
@@ -376,28 +379,9 @@
 
     def generate_user_info(self, user, scope):
         return generate_user_info(user, scope)
     
     def create_authorization_response(self, redirect_uri, grant_user):
         return super().create_authorization_response(redirect_uri, grant_user)
 
-    def create_authorization_response(self, redirect_uri, grant_user):
-        state = self.request.state
-        if grant_user:
-            params = self.create_granted_params(grant_user)
-            if state:
-                params.append(('state', state))
-        else:
-            error = AccessDeniedError(state=state)
-            params = error.get_body()
-
-        # http://openid.net/specs/oauth-v2-multiple-response-types-1_0.html#ResponseModes
-        response_mode = self.request.data.get('response_mode', self.DEFAULT_RESPONSE_MODE)
-        print("creating autorization responnse")
-        print('ruri', redirect_uri)
-        print('params', params)
-        print('response mode', response_mode)
-        return create_response_mode_response(
-            redirect_uri=redirect_uri,
-            params=params,
-            response_mode=response_mode,
-        )
+    def authenticate_user(self, authorization_code):
+        return User({"uid": authorization_code.uid}).get()
```

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.43/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.43/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.43/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.43/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.43/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/base/firebase_collection.py` & `adafri-0.0.43/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/user/models/user.py` & `adafri-0.0.43/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri/v1/user/models/user_fields.py` & `adafri-0.0.43/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/adafri.egg-info/SOURCES.txt` & `adafri-0.0.43/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.42/setup.py` & `adafri-0.0.43/setup.py`

 * *Files identical despite different names*

