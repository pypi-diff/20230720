# Comparing `tmp/adafri-0.0.40.tar.gz` & `tmp/adafri-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.40.tar", last modified: Thu Jul 20 07:39:07 2023, max compression
+gzip compressed data, was "adafri-0.0.41.tar", last modified: Thu Jul 20 08:02:07 2023, max compression
```

## Comparing `adafri-0.0.40.tar` & `adafri-0.0.41.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.598503 adafri-0.0.40/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-20 07:39:07.598089 adafri-0.0.40/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.538734 adafri-0.0.40/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-20 07:39:01.000000 adafri-0.0.40/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.545673 adafri-0.0.40/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.40/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.40/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16483 2023-07-20 06:24:00.000000 adafri-0.0.40/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.549153 adafri-0.0.40/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.40/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.555308 adafri-0.0.40/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.40/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.564902 adafri-0.0.40/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.40/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.40/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.40/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.565554 adafri-0.0.40/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.40/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.566911 adafri-0.0.40/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.40/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.40/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.567352 adafri-0.0.40/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.40/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.567791 adafri-0.0.40/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.40/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.578404 adafri-0.0.40/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.40/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6729 2023-07-20 06:02:29.000000 adafri-0.0.40/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.40/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16660 2023-07-20 07:26:41.000000 adafri-0.0.40/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.40/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9227 2023-07-20 07:38:44.000000 adafri-0.0.40/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:37:50.000000 adafri-0.0.40/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.583199 adafri-0.0.40/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.40/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.40/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.40/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.590999 adafri-0.0.40/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.40/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.40/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.592808 adafri-0.0.40/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.40/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.597114 adafri-0.0.40/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.40/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9309 2023-07-20 05:13:59.000000 adafri-0.0.40/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.40/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 07:39:07.542810 adafri-0.0.40/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-20 07:39:07.000000 adafri-0.0.40/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-20 07:39:07.000000 adafri-0.0.40/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-20 07:39:07.000000 adafri-0.0.40/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-20 07:39:07.000000 adafri-0.0.40/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-20 07:39:07.598652 adafri-0.0.40/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.40/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.991686 adafri-0.0.41/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-20 08:02:07.991283 adafri-0.0.41/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.937850 adafri-0.0.41/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-20 08:02:03.000000 adafri-0.0.41/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.942582 adafri-0.0.41/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.41/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.41/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16483 2023-07-20 06:24:00.000000 adafri-0.0.41/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.943652 adafri-0.0.41/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.41/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.944383 adafri-0.0.41/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.41/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.946481 adafri-0.0.41/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.41/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.41/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.41/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.947137 adafri-0.0.41/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.41/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.948454 adafri-0.0.41/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.41/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.41/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.949320 adafri-0.0.41/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.41/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.949774 adafri-0.0.41/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.41/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.966665 adafri-0.0.41/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.41/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6729 2023-07-20 06:02:29.000000 adafri-0.0.41/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.41/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16660 2023-07-20 07:26:41.000000 adafri-0.0.41/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.41/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9253 2023-07-20 08:01:44.000000 adafri-0.0.41/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:37:50.000000 adafri-0.0.41/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.970291 adafri-0.0.41/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.41/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.41/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.41/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.973967 adafri-0.0.41/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.41/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.41/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.974591 adafri-0.0.41/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.41/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.990130 adafri-0.0.41/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.41/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9309 2023-07-20 05:13:59.000000 adafri-0.0.41/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.41/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-20 08:02:07.940297 adafri-0.0.41/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-20 08:02:07.000000 adafri-0.0.41/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-20 08:02:07.000000 adafri-0.0.41/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-20 08:02:07.000000 adafri-0.0.41/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-20 08:02:07.000000 adafri-0.0.41/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-20 08:02:07.991832 adafri-0.0.41/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.41/setup.py
```

### Comparing `adafri-0.0.40/adafri/utils/response.py` & `adafri-0.0.41/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/utils/utils.py` & `adafri-0.0.41/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/account/models/account.py` & `adafri-0.0.41/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/account/models/account_fields.py` & `adafri-0.0.41/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.41/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.41/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.41/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.41/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.41/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.41/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.41/adafri/v1/auth/oauth/models/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,9 +191,9 @@
         expires_at = get_token_expire_at(expires_in).isoformat()
         token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": uid, 'scope': scope, 'scopes': scope_to_list(scope), 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at}
         access_token = Crypto().generate_token("access_token~"+json.dumps(token));
         token['access_token'] = access_token;
         if include_refresh_token:
             token['refresh_token'] = Crypto().generate_token("refresh_token~"+json.dumps(token));
         if grant_type == 'implicit':
-            return {"access_token": access_token}
+            return {"access_token": access_token, "expires_in": expires_in}
         return token
```

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.41/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.41/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.41/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/base/firebase_collection.py` & `adafri-0.0.41/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/user/models/user.py` & `adafri-0.0.41/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri/v1/user/models/user_fields.py` & `adafri-0.0.41/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/adafri.egg-info/SOURCES.txt` & `adafri-0.0.41/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.40/setup.py` & `adafri-0.0.41/setup.py`

 * *Files identical despite different names*

