# Comparing `tmp/openid_whisperer-0.1.5.tar.gz` & `tmp/openid_whisperer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openid_whisperer-0.1.5.tar", max compression
+gzip compressed data, was "openid_whisperer-0.1.6.tar", max compression
```

## Comparing `openid_whisperer-0.1.5.tar` & `openid_whisperer-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.5/LICENSE
--rw-r--r--   0        0        0     6961 2023-07-13 23:19:52.650318 openid_whisperer-0.1.5/README.md
--rw-r--r--   0        0        0     2144 2023-07-14 14:33:27.058333 openid_whisperer-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.5/src/openid_whisperer/__init__.py
--rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.5/src/openid_whisperer/__main__.py
--rw-r--r--   0        0        0     8708 2023-07-14 12:35:34.790984 openid_whisperer-0.1.5/src/openid_whisperer/config.py
--rw-r--r--   0        0        0     2539 2023-07-13 16:49:06.224941 openid_whisperer-0.1.5/src/openid_whisperer/demo_certs/ca_cert.pem
--rw-r--r--   0        0        0     2681 2023-07-13 16:49:06.225650 openid_whisperer-0.1.5/src/openid_whisperer/demo_certs/cert.pem
--rw-r--r--   0        0        0     1675 2023-07-13 16:49:06.226302 openid_whisperer-0.1.5/src/openid_whisperer/demo_certs/key.pem
--rw-r--r--   0        0        0     1119 2023-07-14 12:01:29.202109 openid_whisperer-0.1.5/src/openid_whisperer/main.py
--rw-r--r--   0        0        0    21289 2023-07-14 12:33:31.166614 openid_whisperer-0.1.5/src/openid_whisperer/openid_blueprint.py
--rw-r--r--   0        0        0    27497 2023-07-14 12:33:23.507724 openid_whisperer-0.1.5/src/openid_whisperer/openid_interface.py
--rw-r--r--   0        0        0      910 2023-07-14 12:33:04.149317 openid_whisperer-0.1.5/src/openid_whisperer/openid_types.py
--rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.5/src/openid_whisperer/py.typed
--rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.5/src/openid_whisperer/static/style.css
--rw-r--r--   0        0        0    29028 2023-07-13 16:49:06.234092 openid_whisperer-0.1.5/src/openid_whisperer/templates/authenticate.html
--rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.5/src/openid_whisperer/utils/__init__.py
--rw-r--r--   0        0        0     5082 2023-07-14 12:36:54.560754 openid_whisperer-0.1.5/src/openid_whisperer/utils/cert_utils.py
--rw-r--r--   0        0        0     4551 2023-07-14 12:51:22.117325 openid_whisperer-0.1.5/src/openid_whisperer/utils/common.py
--rw-r--r--   0        0        0     6144 2023-07-14 12:22:20.152374 openid_whisperer-0.1.5/src/openid_whisperer/utils/config_utils.py
--rw-r--r--   0        0        0     4812 2023-07-14 14:21:24.986862 openid_whisperer-0.1.5/src/openid_whisperer/utils/credential_store.py
--rw-r--r--   0        0        0    12332 2023-07-14 12:01:29.396179 openid_whisperer-0.1.5/src/openid_whisperer/utils/token_store.py
--rw-r--r--   0        0        0     3188 2023-07-14 12:43:25.019940 openid_whisperer-0.1.5/src/openid_whisperer/utils/token_utils.py
--rw-r--r--   0        0        0    10643 2023-07-14 14:21:25.060717 openid_whisperer-0.1.5/src/openid_whisperer/utils/user_info_ext.py
--rw-r--r--   0        0        0     8047 1970-01-01 00:00:00.000000 openid_whisperer-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6961 2023-07-13 23:19:52.650318 openid_whisperer-0.1.6/README.md
+-rw-r--r--   0        0        0     2144 2023-07-20 21:04:06.890418 openid_whisperer-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.6/src/openid_whisperer/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.6/src/openid_whisperer/__main__.py
+-rw-r--r--   0        0        0     8889 2023-07-19 16:17:02.507285 openid_whisperer-0.1.6/src/openid_whisperer/config.py
+-rw-r--r--   0        0        0     2539 2023-07-13 16:49:06.224941 openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/ca_cert.pem
+-rw-r--r--   0        0        0     2681 2023-07-13 16:49:06.225650 openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/cert.pem
+-rw-r--r--   0        0        0     1675 2023-07-13 16:49:06.226302 openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/key.pem
+-rw-r--r--   0        0        0     1135 2023-07-20 14:49:18.489462 openid_whisperer-0.1.6/src/openid_whisperer/main.py
+-rw-r--r--   0        0        0    22593 2023-07-20 20:58:33.784797 openid_whisperer-0.1.6/src/openid_whisperer/openid_blueprint.py
+-rw-r--r--   0        0        0    32983 2023-07-20 20:12:41.163231 openid_whisperer-0.1.6/src/openid_whisperer/openid_interface.py
+-rw-r--r--   0        0        0      910 2023-07-14 12:33:04.149317 openid_whisperer-0.1.6/src/openid_whisperer/openid_types.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.6/src/openid_whisperer/py.typed
+-rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.6/src/openid_whisperer/static/style.css
+-rw-r--r--   0        0        0    29021 2023-07-19 16:34:51.108344 openid_whisperer-0.1.6/src/openid_whisperer/templates/authenticate.html
+-rw-r--r--   0        0        0      451 2023-07-19 17:15:03.303758 openid_whisperer-0.1.6/src/openid_whisperer/templates/form_post_response.html
+-rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.6/src/openid_whisperer/utils/__init__.py
+-rw-r--r--   0        0        0     5082 2023-07-14 12:36:54.560754 openid_whisperer-0.1.6/src/openid_whisperer/utils/cert_utils.py
+-rw-r--r--   0        0        0     6840 2023-07-20 15:06:53.637647 openid_whisperer-0.1.6/src/openid_whisperer/utils/common.py
+-rw-r--r--   0        0        0     6144 2023-07-14 12:22:20.152374 openid_whisperer-0.1.6/src/openid_whisperer/utils/config_utils.py
+-rw-r--r--   0        0        0     4812 2023-07-14 14:21:24.986862 openid_whisperer-0.1.6/src/openid_whisperer/utils/credential_store.py
+-rw-r--r--   0        0        0     3637 2023-07-20 14:49:18.532645 openid_whisperer-0.1.6/src/openid_whisperer/utils/test_utils.py
+-rw-r--r--   0        0        0    19602 2023-07-20 16:34:57.398579 openid_whisperer-0.1.6/src/openid_whisperer/utils/token_store.py
+-rw-r--r--   0        0        0     3188 2023-07-14 12:43:25.019940 openid_whisperer-0.1.6/src/openid_whisperer/utils/token_utils.py
+-rw-r--r--   0        0        0    10641 2023-07-20 14:49:18.662763 openid_whisperer-0.1.6/src/openid_whisperer/utils/user_info_ext.py
+-rw-r--r--   0        0        0     8047 1970-01-01 00:00:00.000000 openid_whisperer-0.1.6/PKG-INFO
```

### Comparing `openid_whisperer-0.1.5/LICENSE` & `openid_whisperer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/README.md` & `openid_whisperer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/pyproject.toml` & `openid_whisperer-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openid-whisperer"
-version = "0.1.5"
+version = "0.1.6"
 description = "OpenID 1.0 Mock Identity Service"
 license = "MIT"
 authors = ["Robert Betts <betts_robert@yahoo.com>"]
 maintainers = ["Robert Betts <betts_robert@yahoo.com>"]
 readme = "README.md"
 homepage = "https://github.com/robertbetts/openid-whisperer"
 repository = "https://github.com/robertbetts/openid-whisperer"
```

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/config.py` & `openid_whisperer-0.1.6/src/openid_whisperer/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,21 @@
 
 class Config:
     default_config: default_config_type = {
         "instance_id": (str, uuid4().hex),
         "log_level": (str, "info"),
         "flask_debug": (boolify, False),
         "validate_certs": (boolify, False),
-        "id_service_prefix": (str, "/adfs"),
         "id_service_port": (int, 5005),
         "id_service_host": (str, "localhost"),
         "id_service_bind": (str, "0.0.0.0"),
         "id_service_port_gw": (int, 5005),
         "id_service_host_gw": (str, "localhost"),
         "validate_users": (boolify, False),
-        "json_user_file": (str, ""),
+        "json_users": (str, ""),
         "session_expiry_seconds": (int, 0),
         "maximum_login_attempts": (int, 0),
         "ca_cert_filename": (str, ""),
         "org_key_filename": (str, ""),
         "org_key_password": (str, ""),
         "org_cert_filename": (str, ""),
     }
@@ -53,27 +52,30 @@
     # General configuration parameters
     env_target: str | None
     log_level: str
     flask_debug: bool
     validate_certs: bool
 
     # Networking related configuration
-    id_service_prefix: str
     id_service_port: int
     id_service_host: str
     id_service_bind: str
     id_service_port_gw: str
     id_service_host_gw: str
 
     # Credential related configuration
     validate_users: bool
-    json_user_file: str
     session_expiry_seconds: int
     maximum_login_attempts: int
 
+    # this property is still under development and its type subject to change.
+    # Current thinking is that either it refers to a json text stream of user claim info,
+    # If the info is not valid json, then assume a file path containing json file content.
+    json_users: str
+
     # Credential and Web API related configuration. If not all the configuration entries
     # for these filenames are entered, then the demo certs in this package are used.
     ca_cert_filename: str  # this entry is not mandatory
     org_key_filename: str
     org_key_password: str
     org_cert_filename: str
```

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/demo_certs/ca_cert.pem` & `openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/ca_cert.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/demo_certs/cert.pem` & `openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/demo_certs/key.pem` & `openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/key.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/main.py` & `openid_whisperer-0.1.6/src/openid_whisperer/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ca_certs = [config.ca_cert] if config.ca_cert else None
     flask_app: "Flask" = app()
     flask_app.run(
         ssl_context=get_ssl_context(
             certificate=config.org_cert,
             private_key=config.org_key,
             issuer_certs=ca_certs,
-            verify=False,
+            verify=config.validate_certs,
         ),
         host=config.id_service_bind,
         port=config.id_service_port,
         debug=config.flask_debug,
     )
```

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/openid_blueprint.py` & `openid_whisperer-0.1.6/src/openid_whisperer/openid_blueprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 )
 from openid_whisperer.utils.common import boolify
 from openid_whisperer.utils.credential_store import UserCredentialStoreException
 from openid_whisperer.utils.token_store import (
     TokenIssuerCertificateStoreException,
 )
 from openid_whisperer.utils.common import package_get_logger
+from openid_whisperer.utils.user_info_ext import UserInfoExtensionTemplate
 
 logger = package_get_logger(__name__)
 
 
-class UserInfoExtensionTemplate:
-    pass
-
-
 def register_user_info_extension(
     openid_api: OpenidApiInterface,
     extension: str | UserInfoExtensionTemplate | None = None,
 ) -> None:
     """Register an extension with the credential store that returns user_information claims
     :param openid_api:
     :param extension:
@@ -69,23 +66,22 @@
 config = get_cached_config()
 openid_api_interface = OpenidApiInterface(
     ca_cert_filename=config.ca_cert_filename,
     org_key_filename=config.org_key_filename,
     org_key_password=config.org_key_password,
     org_cert_filename=config.org_cert_filename,
     validate_users=config.validate_users,
-    json_user_file=config.json_user_file,
+    json_users=config.json_users,
     session_expiry_seconds=config.session_expiry_seconds,
     maximum_login_attempts=config.maximum_login_attempts,
 )
 
 openid_blueprint: Blueprint = Blueprint(
     "openid",
     __name__,
-    url_prefix=config.id_service_prefix,
     template_folder="templates",
     static_folder="static",
 )
 
 
 def update_redirect_url_query(
     redirect_uri: str, data: Dict[str, Any]
@@ -94,18 +90,17 @@
         query_start: str = "&" if "?" in redirect_uri else "?"
         for key, value in data.items():
             redirect_uri += f"{query_start}{key}={value}"
             query_start = "&"
     return redirect_uri
 
 
-@openid_blueprint.route("/oauth2/authorize", methods=["GET"])  # type: ignore[misc]
-def authorize_get() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/oauth2/authorize", methods=["GET"])  # type: ignore[misc]
+def authorize_get(tenant: str) -> ResponseReturnValue:
     """Handles GET requests to the authorization endpoint"""
-    tenant: str = openid_blueprint.url_prefix
     # Mandatory query string arguments
     response_type: str = request.args.get("response_type", "")
     client_id: str = request.args.get("client_id", "")
     scope: str = request.args.get("scope", "")
 
     # Optional query string arguments
     response_mode: str = request.args.get("response_mode", "")
@@ -138,15 +133,15 @@
             prompt=prompt,
             rcode=rcode,
             code_challenge_method=code_challenge_method,
             code_challenge=code_challenge,
         )
         template_parameters.update(
             {
-                "tenant": openid_blueprint.url_prefix,
+                "tenant": tenant,
                 "resource": resource,
                 "state": state,
                 "scope": scope,
                 "nonce": nonce,
                 "redirect_uri": redirect_uri,
             }
         )
@@ -164,19 +159,19 @@
 
     except Exception as e:
         logger.exception(e)
         error = f"server_error: Error {request.method} {request.url} {e}"
         abort(500, error)
 
 
-@openid_blueprint.route("/oauth2/authorize", methods=["POST"])  # type: ignore[misc]
-def authorize_post() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/oauth2/authorize", methods=["POST"])  # type: ignore[misc]
+def authorize_post(tenant: str) -> ResponseReturnValue:
     """Handles an authorization POST request and returns an authorization response
 
-    Where an error arises relating to the processing this request, error_code and error_description are
+    Where an error arises relating to the processing this request, error and error_description are
     appended to the response.
     """
     response_type: str = request.form.get("response_type", "")
     response_mode: str = request.form.get("response_mode", "")
     client_id: str = request.form.get("client_id")
     client_secret: str = request.form.get("client_secret", "")
 
@@ -200,15 +195,15 @@
         request.cookies.get(f"openid-whisperer-token-{client_id}", "null")
     )
     if auth_cookie_token:
         logger.debug("kmsi: secure cookie token received.")  # pragma: no cover
 
     try:
         openid_response = openid_api_interface.post_authorize(
-            tenant=openid_blueprint.url_prefix,
+            tenant=tenant,
             response_type=response_type,
             response_mode=response_mode,
             client_id=client_id,
             client_secret=client_secret,
             scope=scope,
             redirect_uri=redirect_uri,
             nonce=nonce,
@@ -231,21 +226,21 @@
     ) as e:
         openid_response = e.to_dict()
         status_code = 403
 
     except Exception as e:
         logger.exception(e)
         openid_response = {
-            "error_code": "server_error",
+            "error": "server_error",
             "error_description": f"Error {request.method} {request.url} {e}",
         }
         status_code = 500
 
     if code_challenge_method != "" and redirect_uri == "":
-        if "error_code" in openid_response:
+        if "error" in openid_response:
             termination_reply = openid_response["error_description"]
         else:
             termination_reply = (
                 "Success, you have validated the user code provided to you."
             )
 
         template_parameters = {
@@ -265,26 +260,49 @@
         authorize_get_resp = make_response(
             render_template("authenticate.html", **template_parameters)
         )
         return authorize_get_resp, status_code
 
     if "code" in response_type:
         # TODO: Handling cases where redirect should be replaced by a form_post
-        if "error_code" in openid_response:
+        if "error" in openid_response:
             code_response = openid_response
         else:
             code_response = {
                 "code": openid_response["authorization_code"],
                 "state": state,
                 "nonce": nonce,
             }
-            #
-            ...
-        redirect_uri = update_redirect_url_query(redirect_uri, code_response)
-        authorize_get_resp = redirect(redirect_uri, code=302)
+
+        if response_mode == "form_post" and status_code == 200:
+            # TODO: for form_post render user friendly error to form if not 200
+            logger.debug("response_mode: form_post")
+            authorize_get_resp = make_response(
+                render_template(
+                    "form_post_response.html",
+                    action=redirect_uri,
+                    id_token=openid_response["access_token"],
+                    state=state,
+                    nonce=nonce,
+                )
+            )
+        elif response_mode == "form_post" and status_code != 200:  # pragma: no cover
+            abort(403, code_response)
+
+        else:
+            if response_mode == "fragment" and status_code == 200:
+                code_response = {
+                    "action": redirect_uri,
+                    "id_token": openid_response["access_token"],
+                    "state": state,
+                    "nonce": nonce,
+                }
+            redirect_uri = update_redirect_url_query(redirect_uri, code_response)
+            authorize_get_resp = redirect(redirect_uri, code=302)
+
         if kmsi:
             auth_cookie_token = json.dumps(
                 {
                     "username": username,
                     "client_id": client_id,
                     "scope": scope,
                     "resource": resource,
@@ -295,53 +313,63 @@
                 key=f"openid-whisperer-token-{client_id}",
                 value=auth_cookie_token,
                 secure=True,
                 httponly=True,
             )
         return authorize_get_resp
 
-    else:  # only other possible option is a response_type == "token":
-        if "error_code" in openid_response:
+    else:  # only other possible option is a response_type is "token" or "id_token":
+        if "error" in openid_response:
             response = openid_response
         else:
             response = openid_response["access_token"]
         return json.dumps(response), status_code
 
 
-@openid_blueprint.route("/oauth2/token", methods=["POST"])  # type: ignore[misc]
-def token() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/oauth2/token", methods=["POST"])  # type: ignore[misc]
+def token(tenant: str) -> ResponseReturnValue:
     """Returns a token response payload for the support grant_types"""
     grant_type: str = request.form.get("grant_type", "")
     device_code: str = request.form.get("device_code", "")
     access_token: str = request.form.get("access_token", "")
     refresh_token: str = request.form.get("refresh_token", "")
     token_type: str = request.form.get("token_type", "")
-    expires_in: int | str = request.form.get("token_type", "")
+    expires_in: int | str = request.form.get("expires_in", "")
+    requested_token_use: str = request.form.get("requested_token_use", "")
+
     client_id: str = request.form.get("client_id", "")
     client_secret: str = request.form.get("client_secret", "")
+    client_assertion: str = request.form.get("client_assertion", "")
+    client_assertion_type: str = request.form.get("client_assertion_type", "")
+    assertion: str = request.form.get("assertion", "")
+
     redirect_uri: str = request.args.get("redirect_uri", "")
 
     code: str = request.form.get("code", "")
     code_verifier: str = request.form.get("code_verifier", "")
 
     username: str = request.form.get("username", "")
     password: str = request.form.get("password", "")
     nonce: str = request.form.get("nonce", "")
     scope: str = request.form.get("scope", "")
     resource: str = request.form.get("resource", "")
 
     process_token_request_inputs = {
-        "tenant": openid_blueprint.url_prefix,
+        "tenant": tenant,
         "grant_type": grant_type,
         "client_id": client_id,
+        "client_secret": client_secret,
+        "client_assertion": client_assertion,
+        "client_assertion_type": client_assertion_type,
+        "assertion": assertion,
         "refresh_token": refresh_token,
         "token_type": token_type,
+        "requested_token_use": requested_token_use,
         "expires_in": expires_in,
         "access_token": access_token,
-        "client_secret": client_secret,
         "device_code": device_code,
         "code": code,
         "username": username,
         "password": password,
         "nonce": nonce,
         "scope": scope,
         "resource": resource,
@@ -354,30 +382,31 @@
         status_code = 200
     except (
         TokenIssuerCertificateStoreException,
         OpenidApiInterfaceException,
         UserCredentialStoreException,
     ) as e:
         response = e.to_dict()
+        logger.error(response)
+        logger.exception(e)
         status_code = 403
     except Exception as e:
         logger.exception(e)
         response = {
-            "error_code": "server_error",
+            "error": "server_error",
             "error_description": f"Error {request.method} {request.url} {e}",
         }
         status_code = 500
 
     return jsonify(response), status_code
 
 
-@openid_blueprint.route("/oauth2/userinfo", methods=["POST"])  # type: ignore[misc]
-def userinfo() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/oauth2/userinfo", methods=["POST"])  # type: ignore[misc]
+def userinfo(tenant: str) -> ResponseReturnValue:
     """Returns claims about the authenticated user"""
-    tenant: str = openid_blueprint.url_prefix
     client_id: str = request.form.get("client_id", "")
     client_secret: str = request.form.get("client_secret", "")
     username: str = request.form.get("username", "")
 
     status_code = 200
     try:
         response = openid_api_interface.post_userinfo(
@@ -392,24 +421,24 @@
         UserCredentialStoreException,
     ) as e:
         response = e.to_dict()
         status_code = 403
     except Exception as e:
         logger.exception(e)
         response = {
-            "error_code": "server_error",
+            "error": "server_error",
             "error_description": f"Error {request.method} {request.url} {e}",
         }
         status_code = 500
 
     return jsonify(response), status_code
 
 
-@openid_blueprint.route("/oauth2/devicecode", methods=["POST"])  # type: ignore[misc]
-def devicecode() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/oauth2/devicecode", methods=["POST"])  # type: ignore[misc]
+def devicecode(tenant: str) -> ResponseReturnValue:
     """Returns a response including a device code, uri for end user verification and user code for
     the end user to enter.
 
      Device Code Flow:
      1. An end user visits the client app
      2. Client app makes a device code request to the identity provider
      3. The identity provider returns information for the app to pass on to the end user, to independently
@@ -426,15 +455,14 @@
          "verification_uri":  quote(auth_link),
          "expires_in": int(expires_in_seconds),
          "interval": 5,  # The polling interval the client should respect when waiting for user approval
          "message": f"Enter the following code: {user_code} at this link, {auth_link}"
      }
     """
     try:
-        tenant: str = openid_blueprint.url_prefix
         client_id = request.form.get("client_id", "")
         client_secret = request.form.get("client_secret", "")
         scope = request.form.get("scope", "")
         resource = request.form.get("resource", "")
         response = openid_api_interface.get_devicecode_request(
             tenant=tenant,
             base_url=config.id_provider_base_url_external,
@@ -452,30 +480,29 @@
     ) as e:
         response = e.to_dict()
         status_code = 403
 
     except Exception as e:
         logger.exception(e)
         response = {
-            "error_code": "server_error",
+            "error": "server_error",
             "error_description": f"Error {request.method} {request.url} {e}",
         }
         status_code = 500
 
     return jsonify(response), status_code
 
 
-@openid_blueprint.route("/oauth2/v2.0/logout", methods=["GET"])  # type: ignore[misc]
-@openid_blueprint.route("/oauth2/logout", methods=["GET"])  # type: ignore[misc]
-def get_logout() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/oauth2/v2.0/logout", methods=["GET"])  # type: ignore[misc]
+@openid_blueprint.route("/<tenant>/oauth2/logout", methods=["GET"])  # type: ignore[misc]
+def get_logout(tenant: str) -> ResponseReturnValue:
     """logs out the end user, the client is also responsible for clearing out
     any cached authenticated session info held. The end uer is then redirected to the
     given post_logout_redirect_uri
     """
-    tenant: str = openid_blueprint.url_prefix
     client_id: str = request.args.get("client_id", "")
     username: str = request.args.get("username", "")
     post_logout_redirect_uri: str = request.args.get("post_logout_redirect_uri", "")
 
     try:
         response: Dict[str, Any] = openid_api_interface.logoff(
             tenant, client_id, username
@@ -492,30 +519,29 @@
     ) as e:
         response = e.to_dict()
         status_code = 403
 
     except Exception as e:
         logger.exception(e)
         response = {
-            "error_code": "server_error",
+            "error": "server_error",
             "error_description": f"Error {request.method} {request.url} {e}",
         }
         status_code = 500
 
     abort(status_code, response)
 
 
-@openid_blueprint.route("/oauth2/v2.0/logout", methods=["POST"])  # type: ignore[misc]
-@openid_blueprint.route("/oauth2/logout", methods=["POST"])  # type: ignore[misc]
-def post_logout() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/oauth2/v2.0/logout", methods=["POST"])  # type: ignore[misc]
+@openid_blueprint.route("/<tenant>/oauth2/logout", methods=["POST"])  # type: ignore[misc]
+def post_logout(tenant: str) -> ResponseReturnValue:
     """logs out the end user, the client is also responsible for clearing out
     any cached authenticated session info held. The end uer is then redirected to the
     given post_logout_redirect_uri
     """
-    tenant: str = openid_blueprint.url_prefix
     client_id: str = request.form.get("client_id", "")
     username: str = request.form.get("username", "")
     try:
         response = openid_api_interface.logoff(
             tenant=tenant, client_id=client_id, username=username
         )
         status_code = 200
@@ -526,70 +552,71 @@
     ) as e:
         response = e.to_dict()
         status_code = 403
 
     except Exception as e:
         logger.exception(e)
         response = {
-            "error_code": "server_error",
+            "error": "server_error",
             "error_description": f"Error {request.method} {request.url} {e}",
         }
         status_code = 500
 
     return jsonify(response), status_code
 
 
-@openid_blueprint.route("/discovery/keys", methods=["GET"])  # type: ignore[misc]
-def keys() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/discovery/keys", methods=["GET"])  # type: ignore[misc]
+def keys(tenant: str) -> ResponseReturnValue:
     """Returns the public keys used to sign tokens"""
+    _ = tenant
     status_code = 200
     try:
         response = openid_api_interface.token_store.get_keys()
     except (
         TokenIssuerCertificateStoreException,
         OpenidApiInterfaceException,
         UserCredentialStoreException,
     ) as e:  # pragma: no cover
         response = e.to_dict()
         status_code = 403
     except Exception as e:
         logger.exception(e)
         response = {
-            "error_code": "server_error",
+            "error": "server_error",
             "error_description": f"Error {request.method} {request.url} {e}",
         }
         status_code = 500
 
     return jsonify(response), status_code
 
 
-@openid_blueprint.route("/.well-known/openid-configuration", methods=["GET"])  # type: ignore[misc]
-def openid_configuration() -> ResponseReturnValue:
+@openid_blueprint.route("/<tenant>/.well-known/openid-configuration", methods=["GET"])  # type: ignore[misc]
+def openid_configuration(tenant: str) -> ResponseReturnValue:
     """returns OpenID Connect metadata"""
     # TODO: look at better way of determining this url, depending on the network location of
     #  the client_id and end user. i.e. if the endpoint is is accessible from different networks
     #  then there will have to be valid certificates in place for host ip of the listening
     #  endpoint and the url extracted from this send the usd user ot client app to the correct
     #  destination.
     try:
         id_provider_base_url = config.id_provider_base_url_external
         response = openid_api_interface.get_openid_configuration(
-            tenant=config.id_service_prefix,
+            tenant=tenant,
             base_url=id_provider_base_url,
         )
         status_code = 200
     except (
         TokenIssuerCertificateStoreException,
         OpenidApiInterfaceException,
         UserCredentialStoreException,
     ) as e:  # pragma: no cover
         response = e.to_dict()
         status_code = 403
     except Exception as e:  # pragma: no cover
         logger.exception(e)
         response = {
-            "error_code": "server_error",
+            "error": "server_error",
             "error_description": f"Error {request.method} {request.url} {e}",
         }
         status_code = 500
 
     return jsonify(response), status_code
```

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/openid_interface.py` & `openid_whisperer-0.1.6/src/openid_whisperer/openid_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import logging
 from typing import Dict, Any, Optional, List, Type
 import datetime
 import hashlib
 import secrets
 from urllib.parse import urljoin
 import string
+import jwt
 
 from openid_whisperer.utils.common import (
     RESPONSE_TYPES_SUPPORTED,
     RESPONSE_MODES_SUPPORTED,
-    GRANT_TYPES_SUPPORTED,
     stringify,
     get_audience,
-    boolify,
+    boolify, validate_grant_type,
 )
 from openid_whisperer.utils.common import GeneralPackageException, get_seconds_epoch
 from openid_whisperer.utils.credential_store import UserCredentialStore
 from openid_whisperer.utils.token_store import TokenIssuerCertificateStore
 from openid_whisperer.utils.user_info_ext import UserInfoExtensionTemplate
 from openid_whisperer.utils.common import package_get_logger
 
@@ -113,47 +114,14 @@
 
     if error_message:
         raise OpenidApiInterfaceException("api_validation_error", error_message)
 
     return response_mode
 
 
-def validate_grant_type(grant_type: str) -> str:
-    """Returns a tuple of (adjusted_grant_type, error_message)
-    Where the input grant_typ is in the forman of an urn e.g."urn:ietf:params:oauth:grant-type:jwt-bearer",
-    grant type is updated to only the grant_type reference.
-
-    OpenidException is raised for validation and processing errors
-
-    Parameters
-    ----------
-    grant_type:
-        required str
-    """
-    error_message: str | None = None
-    if grant_type is None or grant_type == "":
-        error_message = "An empty input for grant_type is not supported"
-    elif grant_type not in GRANT_TYPES_SUPPORTED:
-        error_message = f"The grant_type of '{grant_type}' is not supported"
-    elif grant_type.startswith("urn:ietf:params:oauth:grant-type:"):
-        grant_type = grant_type.split(":")[-1].strip()
-
-    if error_message is None and grant_type not in (
-        "device_code",
-        "authorization_code",
-        "password",
-    ):
-        error_message = f"The grant_type of '{grant_type}' not as yet implemented"
-
-    if error_message is not None:
-        raise OpenidApiInterfaceException("api_validation_error", error_message)
-
-    return grant_type
-
-
 class OpenidApiInterface:
     def __init__(self, **kwargs) -> None:
         self.issuer_reference: str | None = None
         self.devicecode_expires_in: int | None = None
 
         # Credential related configuration
         self.validate_users: bool | None = None
@@ -183,15 +151,15 @@
             self.issuer_reference = "urn:issuer:name:openid-whisperer"
         if self.devicecode_expires_in is None or self.devicecode_expires_in <= 0:
             self.devicecode_expires_in = 15 * 60
 
         self.credential_store = UserCredentialStore(
             validate_users=self.validate_users,
             json_users=self.json_users,
-            session_expiry_second=self.session_expiry_seconds,
+            session_expiry_seconds=self.session_expiry_seconds,
             maximum_login_attempts=self.maximum_login_attempts,
             user_info_extension=self.user_info_extension,
         )
         self.token_store = TokenIssuerCertificateStore(
             ca_cert_filename=self.ca_cert_filename,
             org_key_filename=self.org_key_filename,
             org_key_password=self.org_key_password,
@@ -204,24 +172,70 @@
         self.devicecode_user_codes: Dict[
             str, str
         ] = {}  # device_codes Indexed by user_code
         self.devicecode_authorization_codes: Dict[
             str, Any
         ] = {}  # authorization_codes Indexed by device_code
 
-    @classmethod
     def validate_client(
-        cls, client_id: str, client_secret: Optional[str] = None
+        self,
+        client_id: str,
+        client_secret: Optional[str] = None,
+        client_assertion: Optional[str] = None,
+        client_assertion_type: Optional[str] = None,
     ) -> bool:
         """Returns True or False depending on where client_id validated. Validation currently
         is a non-empty string for client_id
         """
         _ = client_secret
+        if client_assertion_type == 'urn:ietf:params:oauth:client-assertion-type:jwt-bearer':
+            return self.validate_client_assertion(
+                client_id=client_id,
+                client_assertion=client_assertion,
+                client_assertion_type=client_assertion_type
+            )
+        elif client_assertion_type:
+            raise OpenidApiInterfaceException("invalid_client_assertion", "Client assertion_type not supported")
+
+        """ for the purposes of this implementation the check below is not needed
+        if not (client_secret or client_assertion):
+            return False
+        """
+
         if isinstance(client_id, str) and client_id != "":
             return True
+
+        return False
+
+    @classmethod
+    def validate_client_assertion(
+        cls,
+        client_id: str,
+        client_assertion: str,
+        client_assertion_type: str,
+    ) -> bool:
+        """Returns True or False depending on whether the client assertion is validated."""
+        input_claims = jwt.decode(client_assertion, options={"verify_signature": False})
+        token_client_id = input_claims["sub"]
+        token_audience = input_claims["aud"]
+
+        # TODO: Audience check, is token_audience a valid token endpoint url
+
+        token_headers = jwt.get_unverified_header(client_assertion)
+        token_algorith = token_headers["alg"]
+        token_key_id = token_headers.get("kid")
+        token_key_x5t = token_headers.get("x5t")
+        key_id = token_key_x5t if token_key_x5t else token_key_id
+        try:
+            # validated_claims = self.token_store.decode_client_secret_token(client_assertion)
+            validated_claims = jwt.decode(client_assertion, options={"verify_signature": False})
+            if validated_claims:
+                return True
+        except Exception as e:
+            raise OpenidApiInterfaceException("invalid_client", str(e))
         return False
 
     def logoff(self, tenant: str, client_id: str, username: str) -> Dict[str, Any]:
         """Remove an authenticated_session if one exists for the user, if one does not exist then do nothing
 
         :param tenant:
         :param client_id:
@@ -301,15 +315,15 @@
             "prompt": prompt,
             "requires_mfa": False,
             "allows_kmsi": "False",
             "code_challenge_method": code_challenge_method,
             "code_challenge": code_challenge,
             "requires_user_code": requires_user_code,
             "requires_pkce": requires_pkce,
-            "submit_label": "Sing In",
+            "submit_label": "Sign In",
         }
 
     def post_authorize(
         self,
         tenant: str,
         response_type: str,
         response_mode: str,
@@ -319,26 +333,36 @@
         redirect_uri: str,
         nonce: str,
         username: str,
         **kwargs: Optional[Any],
     ) -> Dict[str, Any]:
         """Processes the information from a post submission to the authorize endpoint
 
+        Notes on the response_modes: query, form_post and fragment in the context of response_type code.
+        * query: After successful authorisation, the a redirect to the client / resource owner is made
+                 containing state and code to be used by the resource owner to fetch the end user's token.
+        * form_post: After successful authorisation, HTML is returned to the end user device where the
+                 end user has to accept the authorisation. The authentication token is embedded in the
+                 HTML form. the action is directed to the RO's redirect_uri.
+        * fragment: Similar to query, in that the the end user device receives the redirect response. However
+                 at this point it more similar with the form_post mode, where the use user device is responsible
+                 for unpacking the fragments from the url and then posting them to the RO.
+        * TODO: disable the token code lookup by the RO, as it is now redundant.
+
         TODO: Complete validation code_challenge s256 checks and originating redirect_uri
         """
         _ = (
             tenant,
-            client_secret,
             response_mode,
         )  # interface variables provided for future features
 
         # raises OpenidApiInterfaceException on failed validation
         response_type = validate_response_type(response_type)
 
-        if not self.validate_client(client_id):
+        if not self.validate_client(client_id, client_secret):
             raise OpenidApiInterfaceException(
                 "client_auth_error",
                 "Unable to validate the referring client application.",
             )
 
         scope = stringify(scope)
         password = stringify(kwargs.get("password"))
@@ -396,23 +420,24 @@
             """
             # TODO: if scope is blank default to "openid" and update scope with client_id and resource
             user_claims = self.credential_store.get_user_scope_claims(
                 username=username, scope=scope
             )
             logger.debug((client_id, resource, user_claims))
             audience = get_audience(client_id=client_id, scope=scope, resource=resource)
-            logger.debug(audience)
             authorization_code, token_response = self.token_store.create_new_token(
                 client_id=client_id,
                 issuer=self.issuer_reference,
                 sub=username,
                 user_claims=user_claims,
                 audience=audience,
                 nonce=nonce,
             )
+            logger.debug(f"aud: {audience}")
+            logger.debug(f"sub: {username}")
             logger.debug(f"token: {token_response['access_token']}")
 
             if device_code:
                 device_authorization = {
                     "expires_in": token_response["expires_in"],
                     "client_id": client_id,
                     "code_challenge": code_challenge,
@@ -420,14 +445,15 @@
                     "redirect_uri": redirect_uri,
                     "authorization_code": authorization_code,
                 }
                 self.devicecode_authorization_codes[device_code] = device_authorization
 
             return {
                 "authorization_code": authorization_code,
+                "access_token": token_response["access_token"],
             }
 
         else:  # if "token" in response_type:
             # Endpoint response for a response_type of "token" is JSON
 
             # TODO: if scope is blank default to "openid" and update scope with client_id and resource
             user_claims = self.credential_store.get_user_scope_claims(
@@ -479,15 +505,15 @@
         nonce = nonce if nonce else ""
         response_type = response_type if response_type else "code"
         code_challenge_method = (
             code_challenge_method if code_challenge_method else "plain"
         )
         prompt = prompt if prompt else "login"
 
-        auth_link = urljoin(base_url, f"{tenant}/oauth2/authorize")
+        auth_link = urljoin(base_url, f"/{tenant}/oauth2/authorize")
         auth_link = (
             f"{auth_link}?response_type={response_type}&client_id={client_id}&scope={scope}"
             f"&resource={resource}&prompt={prompt}&code_challenge_method={code_challenge_method}"
             f"&nonce={nonce}"
         )
         auth_link_complete = f"{auth_link}&user_code={user_code}"
         expires_in = datetime.datetime.utcnow() + datetime.timedelta(
@@ -509,19 +535,23 @@
         return device_code_request
 
     def get_token(
         self,
         tenant: str,
         grant_type: str,
         client_id: str,
+        client_secret: str,
+        client_assertion: str,
+        client_assertion_type: str,
         refresh_token: str,
         token_type: str,
+        requested_token_use: str,
+        assertion: str,
         expires_in: int | str,
         access_token: str,
-        client_secret: str,
         device_code: str,
         code: str,
         username: str,
         password: str,
         nonce: str,
         scope: str,
         resource: str,
@@ -530,33 +560,108 @@
     ) -> Dict[str, Any]:
         """Returns a token included within a dictionary containing details of the issued token. Other JSON error
         responses could also be returned e.g. pending, unsuccessful, error.
 
         OpenidException could also be raised for various validation and processing errors
         """
         _ = (
+            tenant,
             redirect_uri,
             code_verifier,
             refresh_token,
             token_type,
             expires_in,
             access_token,
         )  # interface variables provided for future features
 
-        if not self.validate_client(client_id, client_secret):
+        if grant_type != "client_credentials" and not self.validate_client(
+            client_id, client_secret
+        ):
             raise OpenidApiInterfaceException(
-                "auth_processing_error", "A valid client_id is required"
+                "auth_processing_error", "A valid client credentials are required"
             )
 
         # OpenidApiInterfaceException is raised below for an invalid grant_type
         grant_type = validate_grant_type(grant_type)
 
         token_response: Dict[str, Any] | None = None
 
-        if grant_type == "device_code":
+        logging.debug(client_assertion)
+        logging.debug(client_assertion_type)
+
+        if (
+            grant_type == "client_credentials"
+            and client_assertion_type
+            == "urn:ietf:params:oauth:client-assertion-type:jwt-bearer"
+        ):
+            logging.info(client_id)
+            logging.info(client_assertion)
+            logging.info(client_assertion_type)
+            logging.info(scope)
+            logging.info(resource)
+            try:
+                # validated_claims = self.token_store.decode_client_secret_token(client_assertion)
+                validated_claims = jwt.decode(client_assertion, options={"verify_signature": False})
+                if validated_claims:
+                    logging.info(validated_claims)
+                audience = get_audience(
+                    client_id=client_id, scope=scope, resource=resource
+                )
+                _, token_response = self.token_store.create_new_token(
+                    client_id=client_id,
+                    issuer=self.issuer_reference,
+                    sub=client_id,
+                    user_claims={},
+                    audience=audience,
+                    nonce=nonce,
+                )
+
+            except Exception as e:
+                raise OpenidApiInterfaceException("invalid_client", str(e))
+
+        elif (
+            grant_type in ("urn:ietf:params:oauth:grant-type:jwt-bearer",)
+            and requested_token_use == "on_behalf_of"
+        ):
+            """ During this step the following is required:
+            
+                Creates a token that will allow client_id(A) to access a different client_id(B)'s resource, using
+                the authorisation provided by an end-user token which is in the possession of client_id(A)
+                
+                For the purposes of the flow implemented here, it is assumed that the end-user has consented
+                to the on-behalf-of flow. 
+            """
+            logging.debug("on-behalf-of flow")
+            # TODO: A full implementation might implement the following:
+            # * validate the client_assertion
+            # * validate the assertion
+            # * authenticate the end user
+            logging.info(client_assertion)
+            # client_claims = self.token_store.decode_client_secret_token(client_assertion)
+            client_claims = jwt.decode(client_assertion, options={"verify_signature": False})
+            user_claims = jwt.decode(assertion, options={"verify_signature": False})
+            if not all([(client_id == client_claims["sub"]),
+                        (client_id in user_claims["aud"])]):
+                raise OpenidApiInterfaceException("client_validation_failed", "client_id not consistent across tokens")
+
+            # NOTE: Some claims inherited from client_claims will be overridden in create_new_token(...)
+            new_token_claims = {}
+            new_token_claims.update(client_claims)
+            audience = get_audience(client_id=client_id, scope=scope, resource=resource)
+
+            _, token_response = self.token_store.create_new_token(
+                client_id=client_id,
+                issuer=self.issuer_reference,
+                sub=username,
+                user_claims=new_token_claims,
+                audience=audience,
+                nonce=nonce,
+            )
+
+        elif grant_type in ("urn:ietf:params:oauth:grant-type:device_code", "device_code"):
             # TODO: check devicecode_request and handle additional unsuccessful
             #  error states, request expiry, authorization_declined etc.
             devicecode_request = self.devicecode_requests.get(device_code, None)
             _ = devicecode_request
 
             device_authorization = self.devicecode_authorization_codes.pop(
                 device_code, None
@@ -653,21 +758,21 @@
             )
 
     def get_openid_configuration(self, tenant: str, base_url: str) -> Dict[str, Any]:
         openid_configuration: Dict[str, Any] = {
             "access_token_issuer": self.issuer_reference,
             "as_access_token_token_binding_supported": False,
             "as_refresh_token_token_binding_supported": False,
-            "authorization_endpoint": urljoin(base_url, f"{tenant}/oauth2/authorize"),
+            "authorization_endpoint": urljoin(base_url, f"/{tenant}/oauth2/authorize"),
             "capabilities": ["kdf_ver2"],
             "CLAIMS_SUPPORTED": CLAIMS_SUPPORTED,
             "device_authorization_endpoint": urljoin(
-                base_url, f"{tenant}/oauth2/devicecode"
+                base_url, f"/{tenant}/oauth2/devicecode"
             ),
-            "end_session_endpoint": urljoin(base_url, f"{tenant}/oauth2/logout"),
+            "end_session_endpoint": urljoin(base_url, f"/{tenant}/oauth2/logout"),
             "frontchannel_logout_session_supported": True,
             "frontchannel_logout_supported": True,
             "grant_types_supported": [
                 "authorization_code",
                 "refresh_token",
                 "client_credentials",
                 "urn:ietf:params:oauth:grant-type:jwt-bearer",
@@ -676,16 +781,16 @@
                 "srv_challenge",
                 "urn:ietf:params:oauth:grant-type:device_code",
                 "device_code",
             ],
             "id_token_signing_alg_values_supported": [
                 self.token_store.token_issuer_algorithm
             ],
-            "issuer": urljoin(base_url, f"{tenant}"),
-            "jwks_uri": urljoin(base_url, f"{tenant}/discovery/keys"),
+            "issuer": urljoin(base_url, f"/{tenant}"),
+            "jwks_uri": urljoin(base_url, f"/{tenant}/discovery/keys"),
             "microsoft_multi_refresh_token": True,
             "op_id_token_token_binding_supported": False,
             "resource_access_token_token_binding_supported": False,
             "response_modes_supported": ["query", "fragment", "form_post"],
             "response_types_supported": [
                 "code",
                 "id_token",
@@ -693,20 +798,20 @@
                 "id_token token",
                 "code token",
                 "code id_token token",
             ],
             "rp_id_token_token_binding_supported": False,
             "SCOPES_SUPPORTED": SCOPES_SUPPORTED,
             "subject_types_supported": ["pairwise"],
-            "token_endpoint": urljoin(base_url, f"{tenant}/oauth2/token"),
+            "token_endpoint": urljoin(base_url, f"/{tenant}/oauth2/token"),
             "token_endpoint_auth_methods_supported": [
                 "client_secret_post",
                 "client_secret_basic",
                 "private_key_jwt",
                 "windows_client_authentication",
             ],
             "token_endpoint_auth_signing_alg_values_supported": [
                 self.token_store.token_issuer_algorithm
             ],
-            "userinfo_endpoint": urljoin(base_url, f"{tenant}/userinfo"),
+            "userinfo_endpoint": urljoin(base_url, f"/{tenant}/userinfo"),
         }
         return openid_configuration
```

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/openid_types.py` & `openid_whisperer-0.1.6/src/openid_whisperer/openid_types.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/static/style.css` & `openid_whisperer-0.1.6/src/openid_whisperer/static/style.css`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/templates/authenticate.html` & `openid_whisperer-0.1.6/src/openid_whisperer/templates/authenticate.html`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                         {% if termination_reply %}
                         <div id="TermMsg">{{ termination_reply }}</div>
                         {% else %}
                         <div id="loginArea">
                             <div id="loginMessage" class="groupMargin">Sign in</div>
                             <form method="post" id="loginForm" autocomplete="off" novalidate="novalidate" onKeyPress="if (event && event.keyCode == 13) Login.submitLoginRequest();" action="{{action}}">
                                 <div id="error" class="fieldMargin error smallText">
-                                    <span id="errorText" for="" aria-live="assertive" role="alert"></span>
+                                    <span id="errorText" aria-live="assertive" role="alert"></span>
                                 </div>
                                 <div id="formsAuthenticationArea">
                                     <div id="userNameArea">
                                         <label id="userNameInputLabel" for="userNameInput" class="hidden">User Account</label>
                                         <input id="userNameInput" name="UserName" type="email" value="" tabindex="1" class="text fullWidth"
                                                spellcheck="false" placeholder="someone@example.com" autocomplete="off"/>
                                     </div>
```

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/utils/cert_utils.py` & `openid_whisperer-0.1.6/src/openid_whisperer/utils/cert_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/utils/config_utils.py` & `openid_whisperer-0.1.6/src/openid_whisperer/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/utils/credential_store.py` & `openid_whisperer-0.1.6/src/openid_whisperer/utils/credential_store.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/utils/token_store.py` & `openid_whisperer-0.1.6/src/openid_whisperer/utils/token_store.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Module for Private Key and Certificate Management
 """
 import json
-from typing import List, Dict, Any, Literal, Optional, Tuple, TypedDict
+from typing import List, Dict, Any, Literal, Optional, TypedDict, Tuple
 import base64
 import datetime
 from uuid import uuid4
 
 from cryptography import x509
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.backends import default_backend
@@ -31,23 +31,25 @@
 
 
 class CertificatePairType(TypedDict):
     certificate: x509.Certificate
     private_key: Optional[CertificateIssuerPrivateKeyTypes]
 
 
+""" This code is not currently in use
 class TokenKeyType(TypedDict):
     kty: str
     use: str
     alg: str
     kid: str
     x5t: str
     n: str
     e: str
     x5c: List[str]
+"""
 
 
 class TokenIssuerCertificateStoreException(GeneralPackageException):
     """Exception raised when TokenIssueCertificateStore requirements are not met, other runtime
     exceptions are passed through.
     """
 
@@ -65,14 +67,15 @@
     """
 
     def __init__(self, **kwargs):
         """
         Parameters
         ----------
         """
+        self.token_issuer_key_id: str | None = None
         self.ca_cert_filename: str = ""
         self.org_key_filename: str = ""
         self.org_key_password: str = ""
         self.org_cert_filename: str = ""
         self.token_expiry_seconds: int | None = 600
         self.refresh_token_expiry_seconds: int | None = 3600
 
@@ -92,37 +95,39 @@
             self.token_expiry_seconds = 600  # 10 minutes
         if (
             self.refresh_token_expiry_seconds is None
             or self.refresh_token_expiry_seconds <= 0
         ):
             self.refresh_token_expiry_seconds = 3600  # 1 hour
 
-        self.ca_certificates: Dict[
-            str, x509.Certificate
-        ] = {}  # ca certificates Indexed on certificate serial number
-        self.token_certificates: Dict[
-            str, CertificatePairType
-        ] = {}  # org certificate/private key pairs Indexed on certificate serial number
-
-        self.token_issuer_key_id: str | None = (
-            None  # expected to be set during certificate initialisation
-        )
+        # This value is hardcoded to RS256 and should not be changed after class initialisation
         self.token_issuer_algorithm: str = "RS256"
 
-        # TODO: Track these
+        # ca certificates Indexed on certificate serial number
+        self.ca_certificates: Dict[str, x509.Certificate] = {}
+        # org certificate/private key pairs Indexed on certificate serial number
+        self.token_certificates: Dict[str, CertificatePairType] = {}
+
+        # Required to be set during certificate initialisation
+        self.token_issuer_key_id: str | None = None
+
+        # TODO: Track these in the background, processing expiry, revocation etc.
         self.tokens_issued: Dict[
             str, Tuple[Any, str]
         ] = {}  # (expires_in, authorization_code) indexed by jti
         self.refresh_tokens_issued: Dict[
             str, Tuple[int, str]
         ] = {}  # (expires_in, authorization_code) indexed by jti
         self.token_requests: Dict[
             str, Dict[str, Any]
         ] = {}  # token_request Dict indexed by authorisation_code
 
+        # Client secret keys, this is experimental, self.add_client_secret(client_id, algorithm, public_key)
+        self.client_secret_keys: Dict[str, List[Dict[str, Any]]] = {}
+
         self.init_certificate_store()
 
     @property
     def token_issuer_private_key(self):
         return self.token_certificates[self.token_issuer_key_id]["private_key"]
 
     @property
@@ -224,24 +229,210 @@
                     "n": pn_n,
                     "e": pn_e,
                     "x5c": [x5c],
                 }
             )
         return {"keys": key_list}
 
+    def add_client_secret(
+        self,
+        client_id: str,
+        key_id: str,
+        algorithm: str,
+        public_key: Any,
+        key_issuer: Optional[str] = None,
+    ) -> None:
+        """Returns None after storing the information regarding a client's secret. if key_issuer is None,
+        it is defaulted to client_id
+
+        If the below are True, a KeyError is raised:
+            * existing key id
+            * existing (algorithm, public_key) combination
+
+        :param client_id:
+        :param key_id:
+        :param algorithm:
+        :param public_key:
+        :param key_issuer:
+        :return: None
+        """
+        for key_info in self.client_secret_keys.setdefault(client_id, []):
+            if key_id == key_info["key_id"]:
+                raise KeyError("input key_id exists")
+            if (
+                algorithm == key_info["algorith"]
+                and public_key == key_info["public_key"]
+            ):
+                raise KeyError("input public_key exists")
+
+        self.client_secret_keys.setdefault(client_id, []).append(
+            {
+                "key_id": key_id,
+                "key_issuer": key_issuer if key_issuer else client_id,
+                "algorithm": algorithm,
+                "public_key": public_key,
+            }
+        )
+
+    def create_client_secret_token(
+        self,
+        client_id: str,
+        client_secret: str,
+        token_endpoint_url: str,
+        token_key_id: str,
+        token_expiry: int = 60,
+        token_algorithm: str = "RS256",
+        client_id_iss: Optional[str] = None,
+        token_claims: Optional[Dict[str, Any]] = None,
+        token_id: Optional[str] = None,
+    ) -> Dict[str, Any]:
+        """Returns a Dict that includes a JWT issued by the client to authenticate with an upstream identity provider.
+        This would typically be used by the implementation of this class when acting as a authentication relay.
+
+        The claims iss, sub, sud, exp, nbf, iat, jti are included in the token created.
+
+        https://datatracker.ietf.org/doc/html/rfc7523
+
+        :param client_id:
+            the valued for client_id in requests to the upstream identity provider
+        :param client_secret:
+            a secret shared only with the Identity provider
+        :param token_endpoint_url:
+            a value that identifies the authorization server as an intended audience. This is typically
+            the url of the token endpoint at the IP for inspection or verification of the token
+        :param token_key_id:
+            a reference to the public key required to validate the token signature.
+        :param token_expiry:
+            time in seconds after which the token expires, defaults to 60
+        :param token_algorithm:
+            cryptographic algorithm for signing, defaults to RS256
+        :param client_id_iss:
+            an alternative client identifier, defaults to client_id
+        :param token_claims:
+            optional additional claims to embed in the token
+        :param token_id:
+            a unique reference for identifying the token, defaulted to uuid4()
+        :return:
+            Dict that includes the JWT client_secret
+        """
+        client_id_iss = client_id_iss if client_id_iss else client_id
+        jti = token_id if token_id else uuid4().hex
+
+        auth_time = datetime.datetime.utcnow()
+        expires_in = auth_time + datetime.timedelta(seconds=token_expiry)
+        payload = token_claims if token_claims else {}
+
+        payload.update(
+            {
+                "sub": client_id,
+                "iss": client_id_iss,
+                "aud": token_endpoint_url,
+                "exp": get_seconds_epoch(expires_in),
+                "nbf": get_seconds_epoch(auth_time),
+                "iat": get_seconds_epoch(auth_time),
+                "jti": jti,
+            }
+        )
+        """ TODO: this may be upstream identity provider specific, however it should be assessed
+            what key identifier fields are required or optional for client secret JWTs.
+            
+            "kid": some_issuer_key_id
+        """
+        headers = {
+            "typ": "JWT",
+            "alg": token_algorithm,
+            "kid": token_key_id,
+            "x5t": token_key_id,
+        }
+        token = jwt.encode(
+            payload=payload,
+            key=client_secret,
+            algorithm=token_algorithm,
+            headers=headers,
+        )
+        token_response = {
+            "jti": jti,
+            "exp": get_seconds_epoch(expires_in),
+            "token": token,
+        }
+        return token_response
+
+    def get_client_keys(self, client_id: str) -> List[Dict[str, Any]]:
+        """Returns a list if dictionaries with the keys:
+                key_issuer, key_id, algorithm, public_key | hashed_secret
+
+        :param client_id:
+        :return:
+        """
+        client_keys = self.client_secret_keys.setdefault(client_id, [])
+        return client_keys
+
+    def decode_client_secret_token(self, token: str) -> Dict[str, Any]:
+        """Returns a dict of claims embedded in the token provided
+
+        exceptions raised are:
+            KeyError = Missing required JWT headers and claims
+            ValueError = unknown client or Missing client secret
+            jwt token validation exceptions
+
+        :param token:
+        :return:
+        """
+
+        input_claims = jwt.decode(token, options={"verify_signature": False})
+        token_client_id = input_claims["sub"]
+        token_audience = input_claims["aud"]
+
+        # TODO: Audience check, is token_audience a valid token endpoint url
+
+        token_headers = jwt.get_unverified_header(token)
+        token_algorith = token_headers["alg"]
+        _token_key_id = token_headers.get("kid")
+        _token_key_x5t = token_headers.get("x5t")
+        key_id = _token_key_x5t if _token_key_x5t else _token_key_id
+        if not key_id:
+            raise ValueError("Missing public key reference")
+
+        issuer = None
+        public_key = None
+        algorithm = None
+        for client_key in self.get_client_keys(token_client_id):
+            if (
+                key_id
+                and client_key["key_id"] != key_id
+                or token_algorith != client_key["algorithm"]
+            ):
+                continue
+            issuer = client_key["key_issuer"]
+            algorithm = client_key["algorithm"]
+            public_key = client_key["public_key"]
+
+        if issuer is None or algorithm is None or public_key is None:
+            raise ValueError("No valid key to validate the client secret JWT")
+
+        claims = jwt.decode(
+            jwt=token,
+            key=public_key,
+            algorithms=[algorithm],
+            issuer=issuer,
+            audience=token_audience,
+        )
+        logger.debug(claims)
+        return claims
+
     def create_new_token(
         self,
         client_id,
         issuer: str,
         sub: str,
         user_claims: Dict[str, Any],
         audience: List[str],
         nonce: str,
     ) -> Tuple[str, Dict[str, Any]]:
-        """Returns a new JWT response using the parameters given.
+        """Returns a response that include JWT.
 
         The claims iss, sun, exp, iat, auth_time, appid, ver are overriden by the TokenIssuerCertificateStore
 
         :param client_id:
         :param issuer:
         :param sub:
         :param user_claims:
@@ -266,14 +457,16 @@
                 "auth_time": auth_time.isoformat(sep=" "),
                 "appid": client_id,
                 "jti": jti,
                 "ver": "1.0",
             }
         )
         headers = {
+            "typ": "JWT",
+            "alg": self.token_issuer_algorithm,
             "kid": self.token_issuer_key_id,
             "x5t": self.token_issuer_key_id,
         }
         token = jwt.encode(
             payload=payload,
             key=self.token_issuer_private_key,
             algorithm=self.token_issuer_algorithm,
```

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/utils/token_utils.py` & `openid_whisperer-0.1.6/src/openid_whisperer/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.5/src/openid_whisperer/utils/user_info_ext.py` & `openid_whisperer-0.1.6/src/openid_whisperer/utils/user_info_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         :param username:
         """
         return username in self._user_info
 
     def get_user_claims(
         self, username: str, scope: str, include_empty: bool = False
     ) -> Dict[str, Dict[str, Any]]:
-        """ "Returns a set of compliant ida claims for the input username, if there are no claims for the
+        """Returns a set of compliant ida claims for the input username, if there are no claims for the
         input username, then a set is created, cached and returned.
 
         :param username:  username in format SID or SID@DOMAIN (0728000@EMEA)
         :param scope: Indicates set of claims returned in addition to the audience attached to a token request
         :param include_empty: when True include empty claim values
         :return: dictionary of claims
         """
```

### Comparing `openid_whisperer-0.1.5/PKG-INFO` & `openid_whisperer-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openid-whisperer
-Version: 0.1.5
+Version: 0.1.6
 Summary: OpenID 1.0 Mock Identity Service
 Home-page: https://github.com/robertbetts/openid-whisperer
 License: MIT
 Keywords: python,mock,api,oauth2,openid
 Author: Robert Betts
 Author-email: betts_robert@yahoo.com
 Maintainer: Robert Betts
```

