# Comparing `tmp/sumatra-client-1.3.1.tar.gz` & `tmp/sumatra-client-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumatra-client-1.3.1.tar", last modified: Thu Jun 22 16:40:28 2023, max compression
+gzip compressed data, was "sumatra-client-1.3.2.tar", last modified: Thu Jul 20 20:30:21 2023, max compression
```

## Comparing `sumatra-client-1.3.1.tar` & `sumatra-client-1.3.2.tar`

### file list

```diff
@@ -1,30 +1,25 @@
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.741750 sumatra-client-1.3.1/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.3.1/LICENSE
--rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-06-22 16:40:28.741972 sumatra-client-1.3.1/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.3.1/README.md
--rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.3.1/pyproject.toml
--rw-r--r--   0 kuhlmann   (501) staff       (20)      824 2023-06-22 16:40:28.743060 sumatra-client-1.3.1/setup.cfg
--rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.3.1/setup.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.732729 sumatra-client-1.3.1/sumatra_client/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      373 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/__init__.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     5568 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/admin.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     9612 2023-06-09 15:42:09.000000 sumatra-client-1.3.1/sumatra_client/auth.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.740563 sumatra-client-1.3.1/sumatra_client/certs/
--rw-r--r--   0 kuhlmann   (501) staff       (20)     1574 2023-06-22 16:35:16.000000 sumatra-client-1.3.1/sumatra_client/certs/cert1.pem
--rw-r--r--   0 kuhlmann   (501) staff       (20)     3749 2023-06-09 15:42:09.000000 sumatra-client-1.3.1/sumatra_client/certs/chain1.pem
--rw-r--r--   0 kuhlmann   (501) staff       (20)     5323 2023-06-22 16:35:16.000000 sumatra-client-1.3.1/sumatra_client/certs/fullchain1.pem
--rw-r--r--   0 kuhlmann   (501) staff       (20)      241 2023-06-22 16:35:16.000000 sumatra-client-1.3.1/sumatra_client/certs/privkey1.pem
--rw-r--r--   0 kuhlmann   (501) staff       (20)    23855 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/cli.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)    99304 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/client.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     8677 2023-06-09 15:42:09.000000 sumatra-client-1.3.1/sumatra_client/config.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     4367 2023-06-06 20:19:27.000000 sumatra-client-1.3.1/sumatra_client/workspace.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.737386 sumatra-client-1.3.1/sumatra_client.egg-info/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)      646 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/SOURCES.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/dependency_links.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/entry_points.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.3.1/sumatra_client.egg-info/not-zip-safe
--rw-r--r--   0 kuhlmann   (501) staff       (20)       99 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/requires.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-06-22 16:40:28.000000 sumatra-client-1.3.1/sumatra_client.egg-info/top_level.txt
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-06-22 16:40:28.741243 sumatra-client-1.3.1/tests/
--rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.3.1/tests/test_config.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-07-20 20:30:21.242565 sumatra-client-1.3.2/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.3.2/LICENSE
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-07-20 20:30:21.242743 sumatra-client-1.3.2/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.3.2/README.md
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.3.2/pyproject.toml
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      771 2023-07-20 20:30:21.243748 sumatra-client-1.3.2/setup.cfg
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.3.2/setup.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-07-20 20:30:21.237627 sumatra-client-1.3.2/sumatra_client/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      373 2023-07-19 18:49:40.000000 sumatra-client-1.3.2/sumatra_client/__init__.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     5568 2023-07-19 18:49:40.000000 sumatra-client-1.3.2/sumatra_client/admin.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    10193 2023-07-19 18:49:40.000000 sumatra-client-1.3.2/sumatra_client/auth.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    23855 2023-07-19 18:49:40.000000 sumatra-client-1.3.2/sumatra_client/cli.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    99304 2023-07-20 20:25:07.000000 sumatra-client-1.3.2/sumatra_client/client.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     8918 2023-07-19 18:49:40.000000 sumatra-client-1.3.2/sumatra_client/config.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     4367 2023-07-19 18:49:40.000000 sumatra-client-1.3.2/sumatra_client/workspace.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-07-20 20:30:21.241665 sumatra-client-1.3.2/sumatra_client.egg-info/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-07-20 20:30:21.000000 sumatra-client-1.3.2/sumatra_client.egg-info/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      513 2023-07-20 20:30:21.000000 sumatra-client-1.3.2/sumatra_client.egg-info/SOURCES.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-07-20 20:30:21.000000 sumatra-client-1.3.2/sumatra_client.egg-info/dependency_links.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-07-20 20:30:21.000000 sumatra-client-1.3.2/sumatra_client.egg-info/entry_points.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.3.2/sumatra_client.egg-info/not-zip-safe
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       99 2023-07-20 20:30:21.000000 sumatra-client-1.3.2/sumatra_client.egg-info/requires.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-07-20 20:30:21.000000 sumatra-client-1.3.2/sumatra_client.egg-info/top_level.txt
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-07-20 20:30:21.242160 sumatra-client-1.3.2/tests/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.3.2/tests/test_config.py
```

### Comparing `sumatra-client-1.3.1/PKG-INFO` & `sumatra-client-1.3.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.3.1
+Version: 1.3.2
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.3.1/setup.cfg` & `sumatra-client-1.3.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumatra-client
-version = 1.3.1
+version = 1.3.2
 author = Sumatra
 author_email = support@sumatra.ai
 url = https://sumatra.ai
 description = Sumatra Python Client and CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Sumatra Proprietary
@@ -27,17 +27,14 @@
 	python_graphql_client
 	pendulum
 	requests
 	click
 	tqdm
 	sumatra-sdk
 
-[options.package_data]
-sumatra_client = certs/*.pem
-
 [options.entry_points]
 console_scripts = 
 	sumatra = sumatra_client.cli:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sumatra-client-1.3.1/sumatra_client/admin.py` & `sumatra-client-1.3.2/sumatra_client/admin.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.1/sumatra_client/auth.py` & `sumatra-client-1.3.2/sumatra_client/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from logging import getLogger
 
 from configparser import ConfigParser
 from requests.auth import AuthBase
 from http.server import BaseHTTPRequestHandler, HTTPServer
 import ssl
 
-from sumatra_client.config import CONFIG
+from sumatra_client.config import CONFIG, _CONFIG_PATH, urljoin
 
 logger = getLogger("sumatra.auth")
 
 AUTH_REDIRECT_PORTS = [20005, 20015, 20025]
 
 
 class TokenNotFoundException(Exception):
@@ -182,14 +182,15 @@
     # open browser and allow user to authenticate using selected cognito flow
     # and store returned auth code
     def _fetch_authorization_tokens(self):
         logger.info("Launching browser-based authentication.")
         if CONFIG.server_version.startswith("v1.2"):
             self._start_callback_listener_compat()
         else:
+            self._download_certs()
             self._start_callback_listener()
 
         auth_url = self._build_auth_url()
         try:
             click.launch(auth_url)
             self._httpd.serve_forever(poll_interval=1)
         except:
@@ -201,14 +202,24 @@
                 "access_token": self._httpd.access_token,
                 "expires_at": self._httpd.expires_at,
             }
             self._httpd.server_close()
             if not (self._httpd.refresh_token and self._httpd.id_token and self._httpd.access_token):
                 raise RuntimeError("Callback server failed to receive access tokens")
 
+    def _download_certs(self):
+        logger.debug("Downloading local certificates")
+        os.makedirs(os.path.join(_CONFIG_PATH, "certs"), exist_ok=True)
+        response = requests.get(urljoin(CONFIG.lrd_certs_url, "privkey.pem"))
+        with open(os.path.join(_CONFIG_PATH, "certs", "privkey.pem"), "w") as f:
+            f.write(response.text)
+        response = requests.get(urljoin(CONFIG.lrd_certs_url, "fullchain.pem"))
+        with open(os.path.join(_CONFIG_PATH, "certs", "fullchain.pem"), "w") as f:
+            f.write(response.text)
+
     def _build_auth_url(self):
         return f"{CONFIG.instance_url}/log-in-ext/{self._redirect_port}"
 
     def _start_callback_listener_compat(self):
         logger.debug("Using 1.2.0 compatible request handler")
         for port in AUTH_REDIRECT_PORTS:
             try:
@@ -228,18 +239,18 @@
             raise
 
     def _start_callback_listener(self):
         for port in AUTH_REDIRECT_PORTS:
             try:
                 context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
                 certfile = os.path.join(
-                    os.path.dirname(__file__), "certs", "fullchain1.pem"
+                    _CONFIG_PATH, "certs", "fullchain.pem"
                 )
                 keyfile = os.path.join(
-                    os.path.dirname(__file__), "certs", "privkey1.pem"
+                    _CONFIG_PATH, "certs", "privkey.pem"
                 )
                 context.load_cert_chain(certfile, keyfile)
                 self._httpd = CallbackServer(
                     ("l0.lrd.sumatra.ai", int(port)), CallbackServerHandler,
                     origin=CONFIG.instance_url
                 )
                 self._redirect_uri = f"http://l0.lrd.sumatra.ai:{port}"
```

### Comparing `sumatra-client-1.3.1/sumatra_client/cli.py` & `sumatra-client-1.3.2/sumatra_client/cli.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.1/sumatra_client/client.py` & `sumatra-client-1.3.2/sumatra_client/client.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.1/sumatra_client/config.py` & `sumatra-client-1.3.2/sumatra_client/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,22 @@
     def sdk_endpoint(self) -> str:
         return _strip_suffix(self._get_or_stack("sdk_endpoint"), "/graphql")
 
     @property
     def sdk_graphql_url(self) -> str:
         return urljoin(self.sdk_endpoint, "graphql")
 
+    @property
+    def certs_url(self) -> str:
+        return self._get("certs_url") or "https://resources.sumatra.ai/certs/"
+    
+    @property
+    def lrd_certs_url(self) -> str:
+        return urljoin(self.certs_url, "l0.lrd.sumatra.ai")
+
     def save(self, update_default_instance: bool = True) -> None:
         logger.info(f"Saving config to '{self._fname}'")
         if update_default_instance:
             self._config["DEFAULT"]["instance"] = self.instance
         os.makedirs(os.path.dirname(self._fname), exist_ok=True)
         with open(self._fname, "w") as f:
             self._config.write(f)
```

### Comparing `sumatra-client-1.3.1/sumatra_client/workspace.py` & `sumatra-client-1.3.2/sumatra_client/workspace.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.3.1/sumatra_client.egg-info/PKG-INFO` & `sumatra-client-1.3.2/sumatra_client.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.3.1
+Version: 1.3.2
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.3.1/tests/test_config.py` & `sumatra-client-1.3.2/tests/test_config.py`

 * *Files identical despite different names*

