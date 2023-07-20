# Comparing `tmp/kuksa_client-0.4.0a5.tar.gz` & `tmp/kuksa_client-0.4.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuksa_client-0.4.0a5.tar", last modified: Thu Jul 13 09:08:46 2023, max compression
+gzip compressed data, was "kuksa_client-0.4.0a6.tar", last modified: Mon Jul 17 09:12:42 2023, max compression
```

## Comparing `kuksa_client-0.4.0a5.tar` & `kuksa_client-0.4.0a6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.381458 kuksa_client-0.4.0a5/
--rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/MANIFEST.in
--rw-r--r--   0 erik      (1000) erik      (1000)    15872 2023-07-13 09:08:46.381458 kuksa_client-0.4.0a5/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)    15012 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/README.md
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.357469 kuksa_client-0.4.0a5/kuksa/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.357469 kuksa_client-0.4.0a5/kuksa/val/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa/val/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.357469 kuksa_client-0.4.0a5/kuksa/val/v1/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa/val/v1/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9993 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa/val/v1/types_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa/val/v1/types_pb2_grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4058 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa/val/v1/val_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa/val/v1/val_pb2_grpc.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.365465 kuksa_client-0.4.0a5/kuksa_certificates/
--rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a5/kuksa_certificates/CA.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_certificates/CA.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a5/kuksa_certificates/Client.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a5/kuksa_certificates/Client.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     3537 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a5/kuksa_certificates/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a5/kuksa_certificates/Server.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a5/kuksa_certificates/Server.pem
--rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_certificates/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     2023 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a5/kuksa_certificates/genCerts.sh
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.373462 kuksa_client-0.4.0a5/kuksa_certificates/jwt/
--rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/all-read-write.json
--rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/all-read-write.json.token
--rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/createToken.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/jwt.key
--rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/jwt.key.pub
--rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/recreateJWTkeyPair.sh
--rw-r--r--   0 erik      (1000) erik      (1000)       34 2023-05-10 08:02:45.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/requirements.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/single-read.json
--rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/single-read.json.token
--rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/super-admin.json
--rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/super-admin.json.token
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client/
--rw-r--r--   0 erik      (1000) erik      (1000)     3848 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)    26568 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/__main__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_client/_metadata.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client/cli_backend/
--rw-r--r--   0 erik      (1000) erik      (1000)     2259 2023-06-30 10:33:26.000000 kuksa_client-0.4.0a5/kuksa_client/cli_backend/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    11747 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/cli_backend/grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9903 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/cli_backend/ws.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client/grpc/
--rw-r--r--   0 erik      (1000) erik      (1000)    41063 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/grpc/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    16665 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/grpc/aio.py
--rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_client/logging.ini
--rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_client/logo
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client/ws/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_client/ws/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)    15872 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1558 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      212 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)     1370 2023-07-13 09:08:46.381458 kuksa_client-0.4.0a5/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1768 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.381458 kuksa_client-0.4.0a5/tests/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/tests/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-06-30 09:22:49.000000 kuksa_client-0.4.0a5/tests/conftest.py
--rw-r--r--   0 erik      (1000) erik      (1000)     5949 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/tests/test_datapoint.py
--rw-r--r--   0 erik      (1000) erik      (1000)    63305 2023-06-30 09:22:49.000000 kuksa_client-0.4.0a5/tests/test_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.301288 kuksa_client-0.4.0a6/
+-rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)    15798 2023-07-17 09:12:42.301288 kuksa_client-0.4.0a6/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)    15012 2023-07-17 08:35:58.000000 kuksa_client-0.4.0a6/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.293292 kuksa_client-0.4.0a6/kuksa/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.293292 kuksa_client-0.4.0a6/kuksa/val/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa/val/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.293292 kuksa_client-0.4.0a6/kuksa/val/v1/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa/val/v1/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9993 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa/val/v1/types_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa/val/v1/types_pb2_grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4058 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa/val/v1/val_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa/val/v1/val_pb2_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.297290 kuksa_client-0.4.0a6/kuksa_certificates/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a6/kuksa_certificates/CA.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa_certificates/CA.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a6/kuksa_certificates/Client.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a6/kuksa_certificates/Client.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     3537 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a6/kuksa_certificates/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a6/kuksa_certificates/Server.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a6/kuksa_certificates/Server.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa_certificates/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     2023 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a6/kuksa_certificates/genCerts.sh
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.297290 kuksa_client-0.4.0a6/kuksa_certificates/jwt/
+-rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/all-read-write.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/all-read-write.json.token
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/createToken.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/jwt.key
+-rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/jwt.key.pub
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/recreateJWTkeyPair.sh
+-rw-r--r--   0 erik      (1000) erik      (1000)       34 2023-05-10 08:02:45.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/requirements.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/single-read.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/single-read.json.token
+-rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/super-admin.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a6/kuksa_certificates/jwt/super-admin.json.token
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.297290 kuksa_client-0.4.0a6/kuksa_client/
+-rw-r--r--   0 erik      (1000) erik      (1000)     3848 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a6/kuksa_client/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    26568 2023-07-17 08:35:58.000000 kuksa_client-0.4.0a6/kuksa_client/__main__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa_client/_metadata.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.301288 kuksa_client-0.4.0a6/kuksa_client/cli_backend/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2259 2023-06-30 10:33:26.000000 kuksa_client-0.4.0a6/kuksa_client/cli_backend/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    11747 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a6/kuksa_client/cli_backend/grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9903 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a6/kuksa_client/cli_backend/ws.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.301288 kuksa_client-0.4.0a6/kuksa_client/grpc/
+-rw-r--r--   0 erik      (1000) erik      (1000)    41063 2023-07-17 08:35:58.000000 kuksa_client-0.4.0a6/kuksa_client/grpc/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    16665 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a6/kuksa_client/grpc/aio.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa_client/logging.ini
+-rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa_client/logo
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.301288 kuksa_client-0.4.0a6/kuksa_client/ws/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/kuksa_client/ws/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.297290 kuksa_client-0.4.0a6/kuksa_client.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)    15798 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa_client.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1558 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa_client.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      161 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa_client.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-07-17 09:12:42.000000 kuksa_client-0.4.0a6/kuksa_client.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)     1244 2023-07-17 09:12:42.301288 kuksa_client-0.4.0a6/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1768 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a6/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-17 09:12:42.301288 kuksa_client-0.4.0a6/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a6/tests/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-06-30 09:22:49.000000 kuksa_client-0.4.0a6/tests/conftest.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5949 2023-07-17 08:35:58.000000 kuksa_client-0.4.0a6/tests/test_datapoint.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    63305 2023-06-30 09:22:49.000000 kuksa_client-0.4.0a6/tests/test_grpc.py
```

### Comparing `kuksa_client-0.4.0a5/PKG-INFO` & `kuksa_client-0.4.0a6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kuksa_client
-Version: 0.4.0a5
-Summary: kuksa.val python clients and SDK
+Version: 0.4.0a6
+Summary: KUKSA.val Python Client and SDK
 Home-page: https://github.com/eclipse/kuksa.val
-Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
-Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
+Author: Eclipse KUKSA Project
+Author-email: kuksa-dev@eclipse.org
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `kuksa_client-0.4.0a5/README.md` & `kuksa_client-0.4.0a6/README.md`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa/val/v1/types_pb2.py` & `kuksa_client-0.4.0a6/kuksa/val/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa/val/v1/val_pb2.py` & `kuksa_client-0.4.0a6/kuksa/val/v1/val_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa/val/v1/val_pb2_grpc.py` & `kuksa_client-0.4.0a6/kuksa/val/v1/val_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/CA.key` & `kuksa_client-0.4.0a6/kuksa_certificates/CA.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/CA.pem` & `kuksa_client-0.4.0a6/kuksa_certificates/CA.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/Client.key` & `kuksa_client-0.4.0a6/kuksa_certificates/Client.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/Client.pem` & `kuksa_client-0.4.0a6/kuksa_certificates/Client.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/README.md` & `kuksa_client-0.4.0a6/kuksa_certificates/README.md`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/Server.key` & `kuksa_client-0.4.0a6/kuksa_certificates/Server.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/Server.pem` & `kuksa_client-0.4.0a6/kuksa_certificates/Server.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/genCerts.sh` & `kuksa_client-0.4.0a6/kuksa_certificates/genCerts.sh`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/jwt/all-read-write.json.token` & `kuksa_client-0.4.0a6/kuksa_certificates/jwt/all-read-write.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/jwt/createToken.py` & `kuksa_client-0.4.0a6/kuksa_certificates/jwt/createToken.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/jwt/jwt.key` & `kuksa_client-0.4.0a6/kuksa_certificates/jwt/jwt.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/jwt/jwt.key.pub` & `kuksa_client-0.4.0a6/kuksa_certificates/jwt/jwt.key.pub`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/jwt/recreateJWTkeyPair.sh` & `kuksa_client-0.4.0a6/kuksa_certificates/jwt/recreateJWTkeyPair.sh`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/jwt/single-read.json.token` & `kuksa_client-0.4.0a6/kuksa_certificates/jwt/single-read.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_certificates/jwt/super-admin.json.token` & `kuksa_client-0.4.0a6/kuksa_certificates/jwt/super-admin.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/__init__.py` & `kuksa_client-0.4.0a6/kuksa_client/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/__main__.py` & `kuksa_client-0.4.0a6/kuksa_client/__main__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/_metadata.py` & `kuksa_client-0.4.0a6/kuksa_client/_metadata.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/cli_backend/__init__.py` & `kuksa_client-0.4.0a6/kuksa_client/cli_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/cli_backend/grpc.py` & `kuksa_client-0.4.0a6/kuksa_client/cli_backend/grpc.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/cli_backend/ws.py` & `kuksa_client-0.4.0a6/kuksa_client/cli_backend/ws.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/grpc/__init__.py` & `kuksa_client-0.4.0a6/kuksa_client/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/grpc/aio.py` & `kuksa_client-0.4.0a6/kuksa_client/grpc/aio.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client/logo` & `kuksa_client-0.4.0a6/kuksa_client/logo`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/kuksa_client.egg-info/PKG-INFO` & `kuksa_client-0.4.0a6/kuksa_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kuksa-client
-Version: 0.4.0a5
-Summary: kuksa.val python clients and SDK
+Version: 0.4.0a6
+Summary: KUKSA.val Python Client and SDK
 Home-page: https://github.com/eclipse/kuksa.val
-Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
-Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
+Author: Eclipse KUKSA Project
+Author-email: kuksa-dev@eclipse.org
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `kuksa_client-0.4.0a5/kuksa_client.egg-info/SOURCES.txt` & `kuksa_client-0.4.0a6/kuksa_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/pyproject.toml` & `kuksa_client-0.4.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/setup.cfg` & `kuksa_client-0.4.0a6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [metadata]
 name = kuksa_client
-author = Sebastian Schildt, Naresh Nayak, Wenwen Chen
-author_email = sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
-description = kuksa.val python clients and SDK
+author = Eclipse KUKSA Project
+author_email = kuksa-dev@eclipse.org
+description = KUKSA.val Python Client and SDK
 long_description = file:./README.md
 long_description_content_type = text/markdown
 url = https://github.com/eclipse/kuksa.val
 project_urls = 
 	Source=https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 	Bug Tracker=https://github.com/eclipse/kuksa.val/issues
 classifiers = 
 	Intended Audience :: Developers
-	Development Status :: 3 - Alpha
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Topic :: Software Development
 license_files = 
 	LICENSE
 
 [options]
 python_requires = >=3.8
 install_requires = 
 	websockets >= 10.1
 	cmd2 >= 1.4, <2.0
 	pygments >= 2.5
-	importlib_metadata >= 3.6 ; python_version < "3.8"
 	grpcio-tools >= 1.54.2
 	jsonpath-ng >= 1.5.3
 packages = find:
 
 [options.extras_require]
 test = 
 	pylint
```

### Comparing `kuksa_client-0.4.0a5/setup.py` & `kuksa_client-0.4.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/tests/conftest.py` & `kuksa_client-0.4.0a6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/tests/test_datapoint.py` & `kuksa_client-0.4.0a6/tests/test_datapoint.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a5/tests/test_grpc.py` & `kuksa_client-0.4.0a6/tests/test_grpc.py`

 * *Files identical despite different names*

