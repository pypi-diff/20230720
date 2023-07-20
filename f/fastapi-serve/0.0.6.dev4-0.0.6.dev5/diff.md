# Comparing `tmp/fastapi-serve-0.0.6.dev4.tar.gz` & `tmp/fastapi-serve-0.0.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.6.dev4.tar", last modified: Thu Jul 20 14:02:48 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.6.dev5.tar", last modified: Thu Jul 20 14:42:41 2023, max compression
```

## Comparing `fastapi-serve-0.0.6.dev4.tar` & `fastapi-serve-0.0.6.dev5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:02:48.532419 fastapi-serve-0.0.6.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-20 14:02:48.532419 fastapi-serve-0.0.6.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:02:48.528419 fastapi-serve-0.0.6.dev4/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 14:02:48.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:02:48.528419 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:02:48.528419 fastapi-serve-0.0.6.dev4/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:02:48.528419 fastapi-serve-0.0.6.dev4/fastapi_serve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/utils/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:02:48.532419 fastapi-serve-0.0.6.dev4/fastapi_serve/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/utils/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/utils/blob/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/fastapi_serve/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:02:48.528419 fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-20 14:02:48.000000 fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 14:02:48.000000 fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:02:48.000000 fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 14:02:48.000000 fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:02:48.000000 fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 14:02:48.000000 fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 14:02:48.000000 fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:02:48.532419 fastapi-serve-0.0.6.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-20 14:02:44.000000 fastapi-serve-0.0.6.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.985055 fastapi-serve-0.0.6.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-20 14:42:41.985055 fastapi-serve-0.0.6.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.985055 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:42:41.985055 fastapi-serve-0.0.6.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/setup.py
```

### Comparing `fastapi-serve-0.0.6.dev4/LICENSE` & `fastapi-serve-0.0.6.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/PKG-INFO` & `fastapi-serve-0.0.6.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.6.dev4
+Version: 0.0.6.dev5
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -44,15 +44,15 @@
 Designed with developers in mind, `fastapi-serve` simplifies the deployment process by packing robust functionality, ease-of-use, and automated procedures into one comprehensive package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI application development, allowing you to focus on what truly matters - writing great code!
 
 
 ## 😍 Features 
 
 - 🌎 **HTTPS**: Auto-provisioned DNS and TLS certificates for your app.
 - 🔗 **Protocols**: Full compatibility with HTTP, WebSocket, and GraphQL.
-- ↕️ **Scaling**: Scale your app manuallly or let it auto-scale based on RPS, CPU, and Memory.
+- ↕️ **Scaling**: Scale your app manually or let it auto-scale based on RPS, CPU, and Memory.
 - 🗝️ **Secrets**: Secure handling of secrets and environment variables.
 - 🎛️ **Hardware**: Choose the right compute resources for your app's needs with ease.
 - 🔒 **Authorization**: Built-in OAuth2.0 token-based security to secure your endpoints. 
 - 💾 **App Storage**: Persistent and secure network storage for your app data.
 - 🔄 **Blob Storage**: Built-in support for seamless user file uploads and downloads.
 - 🔎 **Observability**: Integrated access to logs, metrics, and traces. (Alerting coming soon!)
 - 📦 **Containerization**: Effortless containerization of your Python codebase with our integrated registry.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.6.dev4 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.6.dev5 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -27,16 +27,16 @@
 and scalable cloud platform. ð©ï¸ Designed with developers in mind,
 `fastapi-serve` simplifies the deployment process by packing robust
 functionality, ease-of-use, and automated procedures into one comprehensive
 package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI
 application development, allowing you to focus on what truly matters - writing
 great code! ## ð Features - ð **HTTPS**: Auto-provisioned DNS and TLS
 certificates for your app. - ð **Protocols**: Full compatibility with HTTP,
-WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manuallly or let
-it auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
+WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manually or let it
+auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
 handling of secrets and environment variables. - ðï¸ **Hardware**: Choose
 the right compute resources for your app's needs with ease. - ð
 **Authorization**: Built-in OAuth2.0 token-based security to secure your
 endpoints. - ð¾ **App Storage**: Persistent and secure network storage for
 your app data. - ð **Blob Storage**: Built-in support for seamless user file
 uploads and downloads. - ð **Observability**: Integrated access to logs,
 metrics, and traces. (Alerting coming soon!) - ð¦ **Containerization**:
```

### Comparing `fastapi-serve-0.0.6.dev4/README.md` & `fastapi-serve-0.0.6.dev5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Designed with developers in mind, `fastapi-serve` simplifies the deployment process by packing robust functionality, ease-of-use, and automated procedures into one comprehensive package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI application development, allowing you to focus on what truly matters - writing great code!
 
 
 ## 😍 Features 
 
 - 🌎 **HTTPS**: Auto-provisioned DNS and TLS certificates for your app.
 - 🔗 **Protocols**: Full compatibility with HTTP, WebSocket, and GraphQL.
-- ↕️ **Scaling**: Scale your app manuallly or let it auto-scale based on RPS, CPU, and Memory.
+- ↕️ **Scaling**: Scale your app manually or let it auto-scale based on RPS, CPU, and Memory.
 - 🗝️ **Secrets**: Secure handling of secrets and environment variables.
 - 🎛️ **Hardware**: Choose the right compute resources for your app's needs with ease.
 - 🔒 **Authorization**: Built-in OAuth2.0 token-based security to secure your endpoints. 
 - 💾 **App Storage**: Persistent and secure network storage for your app data.
 - 🔄 **Blob Storage**: Built-in support for seamless user file uploads and downloads.
 - 🔎 **Observability**: Integrated access to logs, metrics, and traces. (Alerting coming soon!)
 - 📦 **Containerization**: Effortless containerization of your Python codebase with our integrated registry.
```

#### html2text {}

```diff
@@ -10,16 +10,16 @@
 and scalable cloud platform. ð©ï¸ Designed with developers in mind,
 `fastapi-serve` simplifies the deployment process by packing robust
 functionality, ease-of-use, and automated procedures into one comprehensive
 package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI
 application development, allowing you to focus on what truly matters - writing
 great code! ## ð Features - ð **HTTPS**: Auto-provisioned DNS and TLS
 certificates for your app. - ð **Protocols**: Full compatibility with HTTP,
-WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manuallly or let
-it auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
+WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manually or let it
+auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
 handling of secrets and environment variables. - ðï¸ **Hardware**: Choose
 the right compute resources for your app's needs with ease. - ð
 **Authorization**: Built-in OAuth2.0 token-based security to secure your
 endpoints. - ð¾ **App Storage**: Persistent and secure network storage for
 your app data. - ð **Blob Storage**: Built-in support for seamless user file
 uploads and downloads. - ð **Observability**: Integrated access to logs,
 metrics, and traces. (Alerting coming soon!) - ð¦ **Containerization**:
```

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/__main__.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/export.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/export.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/options.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/helper.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/utils/auth.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/utils/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/utils/blob/storage.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/utils/blob/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve/utils/helper.py` & `fastapi-serve-0.0.6.dev5/fastapi_serve/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.6.dev4
+Version: 0.0.6.dev5
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -44,15 +44,15 @@
 Designed with developers in mind, `fastapi-serve` simplifies the deployment process by packing robust functionality, ease-of-use, and automated procedures into one comprehensive package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI application development, allowing you to focus on what truly matters - writing great code!
 
 
 ## 😍 Features 
 
 - 🌎 **HTTPS**: Auto-provisioned DNS and TLS certificates for your app.
 - 🔗 **Protocols**: Full compatibility with HTTP, WebSocket, and GraphQL.
-- ↕️ **Scaling**: Scale your app manuallly or let it auto-scale based on RPS, CPU, and Memory.
+- ↕️ **Scaling**: Scale your app manually or let it auto-scale based on RPS, CPU, and Memory.
 - 🗝️ **Secrets**: Secure handling of secrets and environment variables.
 - 🎛️ **Hardware**: Choose the right compute resources for your app's needs with ease.
 - 🔒 **Authorization**: Built-in OAuth2.0 token-based security to secure your endpoints. 
 - 💾 **App Storage**: Persistent and secure network storage for your app data.
 - 🔄 **Blob Storage**: Built-in support for seamless user file uploads and downloads.
 - 🔎 **Observability**: Integrated access to logs, metrics, and traces. (Alerting coming soon!)
 - 📦 **Containerization**: Effortless containerization of your Python codebase with our integrated registry.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.6.dev4 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.6.dev5 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -27,16 +27,16 @@
 and scalable cloud platform. ð©ï¸ Designed with developers in mind,
 `fastapi-serve` simplifies the deployment process by packing robust
 functionality, ease-of-use, and automated procedures into one comprehensive
 package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI
 application development, allowing you to focus on what truly matters - writing
 great code! ## ð Features - ð **HTTPS**: Auto-provisioned DNS and TLS
 certificates for your app. - ð **Protocols**: Full compatibility with HTTP,
-WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manuallly or let
-it auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
+WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manually or let it
+auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
 handling of secrets and environment variables. - ðï¸ **Hardware**: Choose
 the right compute resources for your app's needs with ease. - ð
 **Authorization**: Built-in OAuth2.0 token-based security to secure your
 endpoints. - ð¾ **App Storage**: Persistent and secure network storage for
 your app data. - ð **Blob Storage**: Built-in support for seamless user file
 uploads and downloads. - ð **Observability**: Integrated access to logs,
 metrics, and traces. (Alerting coming soon!) - ð¦ **Containerization**:
```

### Comparing `fastapi-serve-0.0.6.dev4/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev4/setup.py` & `fastapi-serve-0.0.6.dev5/setup.py`

 * *Files identical despite different names*

