# Comparing `tmp/gspot_django_auth-0.1.3.tar.gz` & `tmp/gspot_django_auth-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.1.3.tar", last modified: Tue Jul 18 14:04:43 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.1.4.tar", last modified: Thu Jul 20 19:31:27 2023, max compression
```

## Comparing `gspot_django_auth-0.1.3.tar` & `gspot_django_auth-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 14:04:43.035669 gspot_django_auth-0.1.3/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.1.3/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.1.3/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     4805 2023-07-18 14:04:43.035789 gspot_django_auth-0.1.3/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)     4209 2023-07-18 13:52:29.000000 gspot_django_auth-0.1.3/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 14:04:43.032043 gspot_django_auth-0.1.3/gspot_django_auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.1.3/gspot_django_auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-07-08 19:28:37.000000 gspot_django_auth-0.1.3/gspot_django_auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      176 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.3/gspot_django_auth/exceptions.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 14:04:43.033446 gspot_django_auth-0.1.3/gspot_django_auth/management/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:34:18.000000 gspot_django_auth-0.1.3/gspot_django_auth/management/__init__.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 14:04:43.033924 gspot_django_auth-0.1.3/gspot_django_auth/management/commands/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:45:15.000000 gspot_django_auth-0.1.3/gspot_django_auth/management/commands/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     4887 2023-07-18 14:04:28.000000 gspot_django_auth-0.1.3/gspot_django_auth/management/commands/load_test_tokens.py
--rw-r--r--   0 vitya      (501) staff       (20)     1244 2023-07-08 19:21:47.000000 gspot_django_auth-0.1.3/gspot_django_auth/models.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 14:04:43.035305 gspot_django_auth-0.1.3/gspot_django_auth/permissions/
--rw-r--r--   0 vitya      (501) staff       (20)      189 2023-07-08 19:43:37.000000 gspot_django_auth-0.1.3/gspot_django_auth/permissions/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1070 2023-07-08 19:08:49.000000 gspot_django_auth-0.1.3/gspot_django_auth/permissions/permissons.py
--rw-r--r--   0 vitya      (501) staff       (20)     1119 2023-07-03 13:21:53.000000 gspot_django_auth-0.1.3/gspot_django_auth/permissions/validators.py
--rw-r--r--   0 vitya      (501) staff       (20)     1683 2023-07-07 20:05:39.000000 gspot_django_auth-0.1.3/gspot_django_auth/permissions/verifiers.py
--rw-r--r--   0 vitya      (501) staff       (20)      781 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.3/gspot_django_auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      243 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.3/gspot_django_auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 14:04:43.033234 gspot_django_auth-0.1.3/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     4805 2023-07-18 14:04:43.000000 gspot_django_auth-0.1.3/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      776 2023-07-18 14:04:43.000000 gspot_django_auth-0.1.3/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-07-18 14:04:43.000000 gspot_django_auth-0.1.3/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-07-18 14:04:43.000000 gspot_django_auth-0.1.3/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-07-18 14:04:43.000000 gspot_django_auth-0.1.3/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      989 2023-07-18 14:04:40.000000 gspot_django_auth-0.1.3/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-07-18 14:04:43.036188 gspot_django_auth-0.1.3/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      168 2023-07-08 19:52:39.000000 gspot_django_auth-0.1.3/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.714051 gspot_django_auth-0.1.4/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.1.4/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.1.4/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     5063 2023-07-20 19:31:27.714212 gspot_django_auth-0.1.4/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)     4467 2023-07-20 19:26:21.000000 gspot_django_auth-0.1.4/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.709564 gspot_django_auth-0.1.4/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.1.4/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-07-08 19:28:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      176 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/exceptions.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.711855 gspot_django_auth-0.1.4/gspot_django_auth/management/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:34:18.000000 gspot_django_auth-0.1.4/gspot_django_auth/management/__init__.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.712194 gspot_django_auth-0.1.4/gspot_django_auth/management/commands/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:45:15.000000 gspot_django_auth-0.1.4/gspot_django_auth/management/commands/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     5152 2023-07-20 19:22:22.000000 gspot_django_auth-0.1.4/gspot_django_auth/management/commands/load_test_tokens.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1381 2023-07-20 17:42:19.000000 gspot_django_auth-0.1.4/gspot_django_auth/models.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.713714 gspot_django_auth-0.1.4/gspot_django_auth/permissions/
+-rw-r--r--   0 vitya      (501) staff       (20)      189 2023-07-08 19:43:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/permissions/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1070 2023-07-08 19:08:49.000000 gspot_django_auth-0.1.4/gspot_django_auth/permissions/permissons.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1119 2023-07-03 13:21:53.000000 gspot_django_auth-0.1.4/gspot_django_auth/permissions/validators.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1683 2023-07-07 20:05:39.000000 gspot_django_auth-0.1.4/gspot_django_auth/permissions/verifiers.py
+-rw-r--r--   0 vitya      (501) staff       (20)      781 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      243 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.711642 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     5063 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      776 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      989 2023-07-20 19:31:22.000000 gspot_django_auth-0.1.4/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-07-20 19:31:27.714651 gspot_django_auth-0.1.4/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      168 2023-07-08 19:52:39.000000 gspot_django_auth-0.1.4/setup.py
```

### Comparing `gspot_django_auth-0.1.3/LICENSE` & `gspot_django_auth-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.3/PKG-INFO` & `gspot_django_auth-0.1.4/gspot_django_auth.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gspot_django_auth
-Version: 0.1.3
+Name: gspot-django-auth
+Version: 0.1.4
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
@@ -61,80 +61,84 @@
 $ python manage.py load_test_tokens
 ```
 
 Token and data for Admin
 ```
 admin_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgyNzczLCJleHAiOjE2ODk2ODMwNzN9.Q-_Lz4GmjTJuprbsKv4jSW3OGZ-ixxCmRGHva8KLkoM"
 admin_data = {
-    "token_type": "access",
-    "iat": 1689682773,
-    "exp": 1689683073,
+    "username": "admin_username",
+    "first_name": "admin_first_name",
+    "last_name": "admin_last_name",
     "user_id": "7fff5488-a091-44a1-9a4e-cb9f535a7f34",
     "role": "administrator",
     "avatar": "",
     "permissions": [],
     "email": "admin@gmail.com",
     "phone": "88005553535",
     "country": None,
     "created_at": "2023-07-08 21:04:32.226941+00:00",
     "update_at": "2023-07-08 21:04:32.226953+00:00",
     "is_superuser": False,
+    "is_banned": False,
+    "is_active": True,
     "groups": [],
     "user_permissions": [],
     "developer_groups": [],
     "developer_permissions": []
 }
 ```
 Token and data for Developer
 ```
 dev_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzMTI3LCJleHAiOjE2ODk2ODM0Mjd9.h-pqm9eDO9yOs2FrHIW0nPTwT45kT9rHvieYfvJoUXc"
 dev_data = {
-    "token_type": "access",
-    "iat": 1689683127,
-    "exp": 1689683427,
+    "username": "dev_username",
+    "first_name": "dev_first_name",
+    "last_name": "dev_last_name",
     "user_id": "9c490b97-4423-4fae-8beb-7e0a128f469f",
     "role": "developer",
     "avatar": "",
     "permissions": [],
     "email": "developer@gmail.com",
     "phone": "88005553535",
     "country": {
         "id": 1,
         "name": "Russia"
     },
     "created_at": "2023-07-18 12:15:50.005936+00:00",
     "update_at": "2023-07-18 12:18:50.540200+00:00",
     "is_active": True,
+    "is_banned": False,
     "is_superuser": False,
     "groups": [],
     "user_permissions": [],
     "company": {}
 }
 ```
 Token and data for Company Owner
 ```
 owner_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzNTQwLCJleHAiOjE2ODk2ODM4NDB9.o8QLclmTxUOEUiVlvHyEghdjtKRbEYn9eAk_jXCswhQ"
 owner_data = {
-    "token_type": "access",
-    "iat": 1689683540,
-    "exp": 1689683840,
+    "username": "owner_username",
+    "first_name": "owner_first_name",
+    "last_name": "owner_last_name",
     "user_id": "36041f78-e46a-4c62-81a6-c0c9e7cce5a4",
     "role": "developer",
     "avatar": "",
     "permissions": [],
     "email": "company_owner@gmail.com",
     "phone": "88005553535",
     "country": {
         "id": 1,
         "name": "Russia"
     },
     "created_at": "2023-07-18 12:30:50.413011+00:00",
     "update_at": "2023-07-18 12:32:17.309680+00:00",
     "is_active": True,
     "is_superuser": False,
+    "is_banned": False,
     "groups": [],
     "user_permissions": [],
     "company": {
         "created_by": "9c490b97-4423-4fae-8beb-7e0a128f469f",
         "title": "Test Company",
         "description": "Test Company Description",
         "email": "test_company@gmail.com",
@@ -146,28 +150,29 @@
     }
 }
 ```
 Token and data for Customer
 ```
 customer_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5Njg0MDMxLCJleHAiOjE2ODk2ODQzMzF9.07kcY4cQWmw20PMf9NWrvxR7NbuVIoCmlN2Gi-hIi7A"
 customer_data = {
-    "token_type": "access",
-    "iat": 1689684031,
-    "exp": 1689684331,
+    "username": "customer_username",
+    "first_name": "customer_first_name",
+    "last_name": "customer_last_name",
     "user_id": "fd3e3c48-96fc-4863-9aa8-68d1e43a6750",
     "role": "customer",
     "avatar": "",
     "permissions": [],
     "age": 18,
     "email": "customer@gmail.com",
     "phone": "88005553535",
     "created_at": "2023-07-18 12:36:56.545791+00:00",
     "update_at": "2023-07-18 12:37:13.736690+00:00",
     "friends": ["dcada25f-b104-4b12-8ac1-9364252b9e7d"],
     "birthday": "2023-07-18",
+    "is_banned": False,
     "is_active": True,
     "country": {
         "id": 1,
         "name": "Russia"
     }
 }
 ```
```

### Comparing `gspot_django_auth-0.1.3/README.md` & `gspot_django_auth-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: gspot_django_auth
+Version: 0.1.4
+Summary: A Django app for auth.
+Home-page: https://github.com/DJWOMS/GSpot
+Author: Kosenko Viktor
+Author-email: oxpaoff <kosenkoviktor11@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
+Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Overview
 
 GSpot Auth is a Django app for GSpot project https://github.com/DJWOMS/GSpot
 
 Installation
 -----------
 ``$ pip install gspot-django-auth``
@@ -44,80 +61,84 @@
 $ python manage.py load_test_tokens
 ```
 
 Token and data for Admin
 ```
 admin_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgyNzczLCJleHAiOjE2ODk2ODMwNzN9.Q-_Lz4GmjTJuprbsKv4jSW3OGZ-ixxCmRGHva8KLkoM"
 admin_data = {
-    "token_type": "access",
-    "iat": 1689682773,
-    "exp": 1689683073,
+    "username": "admin_username",
+    "first_name": "admin_first_name",
+    "last_name": "admin_last_name",
     "user_id": "7fff5488-a091-44a1-9a4e-cb9f535a7f34",
     "role": "administrator",
     "avatar": "",
     "permissions": [],
     "email": "admin@gmail.com",
     "phone": "88005553535",
     "country": None,
     "created_at": "2023-07-08 21:04:32.226941+00:00",
     "update_at": "2023-07-08 21:04:32.226953+00:00",
     "is_superuser": False,
+    "is_banned": False,
+    "is_active": True,
     "groups": [],
     "user_permissions": [],
     "developer_groups": [],
     "developer_permissions": []
 }
 ```
 Token and data for Developer
 ```
 dev_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzMTI3LCJleHAiOjE2ODk2ODM0Mjd9.h-pqm9eDO9yOs2FrHIW0nPTwT45kT9rHvieYfvJoUXc"
 dev_data = {
-    "token_type": "access",
-    "iat": 1689683127,
-    "exp": 1689683427,
+    "username": "dev_username",
+    "first_name": "dev_first_name",
+    "last_name": "dev_last_name",
     "user_id": "9c490b97-4423-4fae-8beb-7e0a128f469f",
     "role": "developer",
     "avatar": "",
     "permissions": [],
     "email": "developer@gmail.com",
     "phone": "88005553535",
     "country": {
         "id": 1,
         "name": "Russia"
     },
     "created_at": "2023-07-18 12:15:50.005936+00:00",
     "update_at": "2023-07-18 12:18:50.540200+00:00",
     "is_active": True,
+    "is_banned": False,
     "is_superuser": False,
     "groups": [],
     "user_permissions": [],
     "company": {}
 }
 ```
 Token and data for Company Owner
 ```
 owner_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzNTQwLCJleHAiOjE2ODk2ODM4NDB9.o8QLclmTxUOEUiVlvHyEghdjtKRbEYn9eAk_jXCswhQ"
 owner_data = {
-    "token_type": "access",
-    "iat": 1689683540,
-    "exp": 1689683840,
+    "username": "owner_username",
+    "first_name": "owner_first_name",
+    "last_name": "owner_last_name",
     "user_id": "36041f78-e46a-4c62-81a6-c0c9e7cce5a4",
     "role": "developer",
     "avatar": "",
     "permissions": [],
     "email": "company_owner@gmail.com",
     "phone": "88005553535",
     "country": {
         "id": 1,
         "name": "Russia"
     },
     "created_at": "2023-07-18 12:30:50.413011+00:00",
     "update_at": "2023-07-18 12:32:17.309680+00:00",
     "is_active": True,
     "is_superuser": False,
+    "is_banned": False,
     "groups": [],
     "user_permissions": [],
     "company": {
         "created_by": "9c490b97-4423-4fae-8beb-7e0a128f469f",
         "title": "Test Company",
         "description": "Test Company Description",
         "email": "test_company@gmail.com",
@@ -129,28 +150,29 @@
     }
 }
 ```
 Token and data for Customer
 ```
 customer_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5Njg0MDMxLCJleHAiOjE2ODk2ODQzMzF9.07kcY4cQWmw20PMf9NWrvxR7NbuVIoCmlN2Gi-hIi7A"
 customer_data = {
-    "token_type": "access",
-    "iat": 1689684031,
-    "exp": 1689684331,
+    "username": "customer_username",
+    "first_name": "customer_first_name",
+    "last_name": "customer_last_name",
     "user_id": "fd3e3c48-96fc-4863-9aa8-68d1e43a6750",
     "role": "customer",
     "avatar": "",
     "permissions": [],
     "age": 18,
     "email": "customer@gmail.com",
     "phone": "88005553535",
     "created_at": "2023-07-18 12:36:56.545791+00:00",
     "update_at": "2023-07-18 12:37:13.736690+00:00",
     "friends": ["dcada25f-b104-4b12-8ac1-9364252b9e7d"],
     "birthday": "2023-07-18",
+    "is_banned": False,
     "is_active": True,
     "country": {
         "id": 1,
         "name": "Russia"
     }
 }
-```
+```
```

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth/authentication.py` & `gspot_django_auth-0.1.4/gspot_django_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth/management/commands/load_test_tokens.py` & `gspot_django_auth-0.1.4/gspot_django_auth/management/commands/load_test_tokens.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import json
 
 from django.core.management import BaseCommand
-from django.conf import settings
 
 from gspot_django_auth.redis_client import RedisAccessClient
 
 
 class Command(BaseCommand):
     def handle(self, *args, **options):
         tokens = self.get_tokens()
         self.add_to_redis(tokens)
 
     @staticmethod
     def get_tokens() -> dict:
         admin_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgyNzczLCJleHAiOjE2ODk2ODMwNzN9.Q-_Lz4GmjTJuprbsKv4jSW3OGZ-ixxCmRGHva8KLkoM"
         admin_data = {
-            "token_type": "access",
-            "iat": 1689682773,
-            "exp": 1689683073,
+            "username": "admin_username",
+            "first_name": "admin_first_name",
+            "last_name": "admin_last_name",
+            "is_banned": False,
+            "is_active": True,
             "user_id": "7fff5488-a091-44a1-9a4e-cb9f535a7f34",
             "role": "administrator",
             "avatar": "",
             "permissions": [],
             "email": "admin@gmail.com",
             "phone": "88005553535",
             "country": None,
@@ -32,17 +33,18 @@
             "user_permissions": [],
             "developer_groups": [],
             "developer_permissions": []
         }
 
         dev_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzMTI3LCJleHAiOjE2ODk2ODM0Mjd9.h-pqm9eDO9yOs2FrHIW0nPTwT45kT9rHvieYfvJoUXc"
         dev_data = {
-            "token_type": "access",
-            "iat": 1689683127,
-            "exp": 1689683427,
+            "username": "dev_username",
+            "first_name": "dev_first_name",
+            "last_name": "dev_last_name",
+            "is_banned": False,
             "user_id": "9c490b97-4423-4fae-8beb-7e0a128f469f",
             "role": "developer",
             "avatar": "",
             "permissions": [],
             "email": "developer@gmail.com",
             "phone": "88005553535",
             "country": {
@@ -55,17 +57,18 @@
             "is_superuser": False,
             "groups": [],
             "user_permissions": [],
             "company": {}
         }
         owner_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzNTQwLCJleHAiOjE2ODk2ODM4NDB9.o8QLclmTxUOEUiVlvHyEghdjtKRbEYn9eAk_jXCswhQ"
         owner_data = {
-            "token_type": "access",
-            "iat": 1689683540,
-            "exp": 1689683840,
+            "username": "owner_username",
+            "first_name": "owner_first_name",
+            "last_name": "owner_last_name",
+            "is_banned": False,
             "user_id": "36041f78-e46a-4c62-81a6-c0c9e7cce5a4",
             "role": "developer",
             "avatar": "",
             "permissions": [],
             "email": "company_owner@gmail.com",
             "phone": "88005553535",
             "country": {
@@ -88,17 +91,18 @@
                 "is_active": True,
                 "is_banned": False,
                 "contact": []
             }
         }
         customer_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5Njg0MDMxLCJleHAiOjE2ODk2ODQzMzF9.07kcY4cQWmw20PMf9NWrvxR7NbuVIoCmlN2Gi-hIi7A"
         customer_data = {
-            "token_type": "access",
-            "iat": 1689684031,
-            "exp": 1689684331,
+            "username": "customer_username",
+            "first_name": "customer_first_name",
+            "last_name": "customer_last_name",
+            "is_banned": False,
             "user_id": "fd3e3c48-96fc-4863-9aa8-68d1e43a6750",
             "role": "customer",
             "avatar": "",
             "permissions": [],
             "age": 18,
             "email": "customer@gmail.com",
             "phone": "88005553535",
```

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth/models.py` & `gspot_django_auth-0.1.4/gspot_django_auth/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 from typing import List
 from uuid import UUID
 
 
 @dataclass(frozen=True)
 class BaseUser:
     user_id: UUID
+    username: str
+    first_name: str
+    last_name: str
     email: str
     phone: str
     avatar: str
-    country: str
+    country: dict
     is_banned: bool
     is_active: bool
+    permissions: List[str]
     created_at: datetime
-    updated_at: datetime
+    update_at: datetime
 
     to_dict = asdict
 
 
 @dataclass(frozen=True)
 class AdminUser(BaseUser):
     is_superuser: bool
@@ -35,14 +39,15 @@
     groups: List[str] = field(default_factory=list)
     user_permissions: List[str] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
 class CustomerUser(BaseUser):
     birthday: datetime
+    friends: List[str] = field(default_factory=list)
 
 
 class UserFactory:
     users = {'administrator': AdminUser, 'developer': DeveloperUser, 'customer': CustomerUser}
 
     def get_user(self, role: str):
         return self.users.get(role)
```

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth/permissions/permissons.py` & `gspot_django_auth-0.1.4/gspot_django_auth/permissions/permissons.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth/permissions/validators.py` & `gspot_django_auth-0.1.4/gspot_django_auth/permissions/validators.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth/permissions/verifiers.py` & `gspot_django_auth-0.1.4/gspot_django_auth/permissions/verifiers.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth/redis_client.py` & `gspot_django_auth-0.1.4/gspot_django_auth/redis_client.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth.egg-info/PKG-INFO` & `gspot_django_auth-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: gspot-django-auth
-Version: 0.1.3
-Summary: A Django app for auth.
-Home-page: https://github.com/DJWOMS/GSpot
-Author: Kosenko Viktor
-Author-email: oxpaoff <kosenkoviktor11@gmail.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
-Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Overview
 
 GSpot Auth is a Django app for GSpot project https://github.com/DJWOMS/GSpot
 
 Installation
 -----------
 ``$ pip install gspot-django-auth``
@@ -61,80 +44,84 @@
 $ python manage.py load_test_tokens
 ```
 
 Token and data for Admin
 ```
 admin_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgyNzczLCJleHAiOjE2ODk2ODMwNzN9.Q-_Lz4GmjTJuprbsKv4jSW3OGZ-ixxCmRGHva8KLkoM"
 admin_data = {
-    "token_type": "access",
-    "iat": 1689682773,
-    "exp": 1689683073,
+    "username": "admin_username",
+    "first_name": "admin_first_name",
+    "last_name": "admin_last_name",
     "user_id": "7fff5488-a091-44a1-9a4e-cb9f535a7f34",
     "role": "administrator",
     "avatar": "",
     "permissions": [],
     "email": "admin@gmail.com",
     "phone": "88005553535",
     "country": None,
     "created_at": "2023-07-08 21:04:32.226941+00:00",
     "update_at": "2023-07-08 21:04:32.226953+00:00",
     "is_superuser": False,
+    "is_banned": False,
+    "is_active": True,
     "groups": [],
     "user_permissions": [],
     "developer_groups": [],
     "developer_permissions": []
 }
 ```
 Token and data for Developer
 ```
 dev_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzMTI3LCJleHAiOjE2ODk2ODM0Mjd9.h-pqm9eDO9yOs2FrHIW0nPTwT45kT9rHvieYfvJoUXc"
 dev_data = {
-    "token_type": "access",
-    "iat": 1689683127,
-    "exp": 1689683427,
+    "username": "dev_username",
+    "first_name": "dev_first_name",
+    "last_name": "dev_last_name",
     "user_id": "9c490b97-4423-4fae-8beb-7e0a128f469f",
     "role": "developer",
     "avatar": "",
     "permissions": [],
     "email": "developer@gmail.com",
     "phone": "88005553535",
     "country": {
         "id": 1,
         "name": "Russia"
     },
     "created_at": "2023-07-18 12:15:50.005936+00:00",
     "update_at": "2023-07-18 12:18:50.540200+00:00",
     "is_active": True,
+    "is_banned": False,
     "is_superuser": False,
     "groups": [],
     "user_permissions": [],
     "company": {}
 }
 ```
 Token and data for Company Owner
 ```
 owner_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzNTQwLCJleHAiOjE2ODk2ODM4NDB9.o8QLclmTxUOEUiVlvHyEghdjtKRbEYn9eAk_jXCswhQ"
 owner_data = {
-    "token_type": "access",
-    "iat": 1689683540,
-    "exp": 1689683840,
+    "username": "owner_username",
+    "first_name": "owner_first_name",
+    "last_name": "owner_last_name",
     "user_id": "36041f78-e46a-4c62-81a6-c0c9e7cce5a4",
     "role": "developer",
     "avatar": "",
     "permissions": [],
     "email": "company_owner@gmail.com",
     "phone": "88005553535",
     "country": {
         "id": 1,
         "name": "Russia"
     },
     "created_at": "2023-07-18 12:30:50.413011+00:00",
     "update_at": "2023-07-18 12:32:17.309680+00:00",
     "is_active": True,
     "is_superuser": False,
+    "is_banned": False,
     "groups": [],
     "user_permissions": [],
     "company": {
         "created_by": "9c490b97-4423-4fae-8beb-7e0a128f469f",
         "title": "Test Company",
         "description": "Test Company Description",
         "email": "test_company@gmail.com",
@@ -146,28 +133,29 @@
     }
 }
 ```
 Token and data for Customer
 ```
 customer_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5Njg0MDMxLCJleHAiOjE2ODk2ODQzMzF9.07kcY4cQWmw20PMf9NWrvxR7NbuVIoCmlN2Gi-hIi7A"
 customer_data = {
-    "token_type": "access",
-    "iat": 1689684031,
-    "exp": 1689684331,
+    "username": "customer_username",
+    "first_name": "customer_first_name",
+    "last_name": "customer_last_name",
     "user_id": "fd3e3c48-96fc-4863-9aa8-68d1e43a6750",
     "role": "customer",
     "avatar": "",
     "permissions": [],
     "age": 18,
     "email": "customer@gmail.com",
     "phone": "88005553535",
     "created_at": "2023-07-18 12:36:56.545791+00:00",
     "update_at": "2023-07-18 12:37:13.736690+00:00",
     "friends": ["dcada25f-b104-4b12-8ac1-9364252b9e7d"],
     "birthday": "2023-07-18",
+    "is_banned": False,
     "is_active": True,
     "country": {
         "id": 1,
         "name": "Russia"
     }
 }
-```
+```
```

### Comparing `gspot_django_auth-0.1.3/gspot_django_auth.egg-info/SOURCES.txt` & `gspot_django_auth-0.1.4/gspot_django_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.3/pyproject.toml` & `gspot_django_auth-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_django_auth-0.1.3/setup.cfg` & `gspot_django_auth-0.1.4/setup.cfg`

 * *Files identical despite different names*

