# Comparing `tmp/muxa1l-sentry-auth-oidc-5.0.4.tar.gz` & `tmp/muxa1l-sentry-auth-oidc-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muxa1l-sentry-auth-oidc-5.0.4.tar", last modified: Thu Mar  2 12:11:42 2023, max compression
+gzip compressed data, was "muxa1l-sentry-auth-oidc-5.0.5.tar", last modified: Thu Jul 20 13:31:45 2023, max compression
```

## Comparing `muxa1l-sentry-auth-oidc-5.0.4.tar` & `muxa1l-sentry-auth-oidc-5.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10848 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/LICENSE
--rw-r--r--   0        0        0     2374 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/README.rst
--rw-r--r--   0        0        0        0 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/oidc/__init__.py
--rw-r--r--   0        0        0      222 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/oidc/apps.py
--rw-r--r--   0        0        0     1266 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/oidc/constants.py
--rw-r--r--   0        0        0     6815 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/oidc/provider.py
--rw-r--r--   0        0        0      146 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/oidc/templates/oidc/configure.html
--rw-r--r--   0        0        0     2234 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/oidc/views.py
--rw-r--r--   0        0        0      813 2023-03-02 12:11:21.241523 muxa1l-sentry-auth-oidc-5.0.4/pyproject.toml
--rw-r--r--   0        0        0     3122 2023-03-02 12:11:42.709143 muxa1l-sentry-auth-oidc-5.0.4/setup.py
--rw-r--r--   0        0        0     3009 2023-03-02 12:11:42.709454 muxa1l-sentry-auth-oidc-5.0.4/PKG-INFO
+-rw-r--r--   0        0        0    10848 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/LICENSE
+-rw-r--r--   0        0        0     2374 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/README.rst
+-rw-r--r--   0        0        0        0 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/oidc/__init__.py
+-rw-r--r--   0        0        0      222 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/oidc/apps.py
+-rw-r--r--   0        0        0     1266 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/oidc/constants.py
+-rw-r--r--   0        0        0     6815 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/oidc/provider.py
+-rw-r--r--   0        0        0      146 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/oidc/templates/oidc/configure.html
+-rw-r--r--   0        0        0     2241 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/oidc/views.py
+-rw-r--r--   0        0        0      813 2023-07-20 13:31:25.262228 muxa1l-sentry-auth-oidc-5.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3122 2023-07-20 13:31:45.757521 muxa1l-sentry-auth-oidc-5.0.5/setup.py
+-rw-r--r--   0        0        0     3009 2023-07-20 13:31:45.757870 muxa1l-sentry-auth-oidc-5.0.5/PKG-INFO
```

### Comparing `muxa1l-sentry-auth-oidc-5.0.4/LICENSE` & `muxa1l-sentry-auth-oidc-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `muxa1l-sentry-auth-oidc-5.0.4/README.rst` & `muxa1l-sentry-auth-oidc-5.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `muxa1l-sentry-auth-oidc-5.0.4/oidc/constants.py` & `muxa1l-sentry-auth-oidc-5.0.5/oidc/constants.py`

 * *Files identical despite different names*

### Comparing `muxa1l-sentry-auth-oidc-5.0.4/oidc/provider.py` & `muxa1l-sentry-auth-oidc-5.0.5/oidc/provider.py`

 * *Files identical despite different names*

### Comparing `muxa1l-sentry-auth-oidc-5.0.4/oidc/views.py` & `muxa1l-sentry-auth-oidc-5.0.5/oidc/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from sentry.auth.view import AuthView, ConfigureView
 from sentry.utils import json
-from sentry.utils.compat import map
+#from sentry.utils.compat import map
 from sentry.utils.signing import urlsafe_b64decode
 
 from .constants import ERR_INVALID_RESPONSE, ISSUER
 
 logger = logging.getLogger("sentry.auth.oidc")
 
 
@@ -22,15 +22,15 @@
         try:
             id_token = data["id_token"]
         except KeyError:
             logger.error("Missing id_token in OAuth response: %s" % data)
             return helper.error(ERR_INVALID_RESPONSE)
 
         try:
-            _, payload, _ = map(urlsafe_b64decode, id_token.split(".", 2))
+            _, payload, _ = list(map(urlsafe_b64decode, id_token.split(".", 2)))
         except Exception as exc:
             logger.error("Unable to decode id_token: %s" % exc, exc_info=True)
             return helper.error(ERR_INVALID_RESPONSE)
 
         try:
             payload = json.loads(payload)
         except Exception as exc:
```

### Comparing `muxa1l-sentry-auth-oidc-5.0.4/pyproject.toml` & `muxa1l-sentry-auth-oidc-5.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muxa1l-sentry-auth-oidc"
-version = "5.0.4"
+version = "5.0.5"
 description = "OpenID Connect authentication provider for Sentry"
 authors = ["Max Wittig <max.wittig@siemens.com>", "Mikhail Davydenko <mimih1990@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.rst"
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
```

### Comparing `muxa1l-sentry-auth-oidc-5.0.4/setup.py` & `muxa1l-sentry-auth-oidc-5.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'oidc': ['templates/oidc/*']}
 
 entry_points = \
 {'sentry.apps': ['oidc = oidc.apps.Config']}
 
 setup_kwargs = {
     'name': 'muxa1l-sentry-auth-oidc',
-    'version': '5.0.4',
+    'version': '5.0.5',
     'description': 'OpenID Connect authentication provider for Sentry',
     'long_description': 'OpenIDConnect Auth for Sentry\n=============================\n\nAn SSO provider for Sentry which enables `OpenID Connect <http://openid.net/connect/>`_ Apps authentication.\n\nThis is a fork of `sentry-auth-google <https://github.com/getsentry/sentry-auth-google/>`_.\n\nWhy fork, instead of adapting sentry-auth-google to work with every OpenID Connect provider?\n--------------------------------------------------------------------------------------------\nThe maintainer has different ideas with sentry-auth-google. See:\n\n* https://github.com/getsentry/sentry-auth-google/pull/29\n* https://github.com/getsentry/sentry/issues/5650\n\nInstall\n-------\n\n::\n\n    $ pip install sentry-auth-oidc\n\nExample Setup for Google\n------------------------\n\nStart by `creating a project in the Google Developers Console <https://console.developers.google.com>`_.\n\nIn the **Authorized redirect URIs** add the SSO endpoint for your installation::\n\n    https://sentry.example.com/auth/sso/\n\nNaturally other providers, that are supporting OpenID-Connect can also be used (like GitLab).\n\nFinally, obtain the API keys and the well-known account URL and plug them into your ``sentry.conf.py``:\n\n.. code-block:: python\n\n    OIDC_CLIENT_ID = ""\n\n    OIDC_CLIENT_SECRET = ""\n\n    OIDC_SCOPE = "openid email"\n\n    OIDC_DOMAIN = "https://accounts.google.com"  # e.g. for Google\n\nThe ``OIDC_DOMAIN`` defines where the OIDC configuration is going to be pulled from.\nBasically it specifies the OIDC server and adds the path ``.well-known/openid-configuration`` to it.\nThat\'s where different endpoint paths can be found.\n\nDetailed information can be found in the `ProviderConfig <https://openid.net/specs/openid-connect-discovery-1_0.html#ProviderConfig>`_ specification.\n\nYou can also define ``OIDC_ISSUER`` to change the default provider name in the UI, even when the ``OIDC_DOMAIN`` is set.\n\nIf your provider doesn\'t support the ``OIDC_DOMAIN``, then you have to set these\nrequired endpoints by yourself (autorization_endpoint, token_endpoint, userinfo_endpoint, issuer).\n\n.. code-block:: python\n\n    OIDC_AUTHORIZATION_ENDPOINT = "https://accounts.google.com/o/oauth2/v2/auth"  # e.g. for Google\n\n    OIDC_TOKEN_ENDPOINT = "https://www.googleapis.com/oauth2/v4/token"  # e.g. for Google\n\n    OIDC_USERINFO_ENDPOINT = "https://www.googleapis.com/oauth2/v3/userinfo" # e.g. for Google\n\n    OIDC_ISSUER = "Google"\n',
     'author': 'Max Wittig',
     'author_email': 'max.wittig@siemens.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `muxa1l-sentry-auth-oidc-5.0.4/PKG-INFO` & `muxa1l-sentry-auth-oidc-5.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxa1l-sentry-auth-oidc
-Version: 5.0.4
+Version: 5.0.5
 Summary: OpenID Connect authentication provider for Sentry
 Author: Max Wittig
 Author-email: max.wittig@siemens.com
 Requires-Python: >=3.6,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

