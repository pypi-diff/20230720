# Comparing `tmp/types-oauthlib-3.2.0.8.tar.gz` & `tmp/types-oauthlib-3.2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-oauthlib-3.2.0.8.tar", last modified: Wed May 10 15:22:01 2023, max compression
+gzip compressed data, was "types-oauthlib-3.2.0.9.tar", last modified: Thu Jul 20 15:19:38 2023, max compression
```

## Comparing `types-oauthlib-3.2.0.8.tar` & `types-oauthlib-3.2.0.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-10 15:22:00.000000 types-oauthlib-3.2.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:00.000000 types-oauthlib-3.2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.500296 types-oauthlib-3.2.0.8/oauthlib-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:22:00.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/common.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.500296 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.500296 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.500296 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/access_token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/authorization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/pre_configured.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/request_token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/signature_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/parameters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/request_validator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/signature.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.500296 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.500296 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.500296 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/backend_application.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/legacy_application.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/mobile_application.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/service_application.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/web_application.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/authorization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/introspect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/pre_configured.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/revocation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/authorization_code.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/client_credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/implicit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/refresh_token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/resource_owner_password_credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/parameters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/request_validator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/tokens.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/endpoints/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/endpoints/pre_configured.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/endpoints/userinfo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/authorization_code.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/dispatchers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/hybrid.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/implicit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/request_validator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/tokens.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-10 15:19:44.000000 types-oauthlib-3.2.0.8/oauthlib-stubs/uri_validate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-10 15:22:00.000000 types-oauthlib-3.2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:01.504296 types-oauthlib-3.2.0.8/types_oauthlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:22:01.000000 types-oauthlib-3.2.0.8/types_oauthlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-10 15:22:01.000000 types-oauthlib-3.2.0.8/types_oauthlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:01.000000 types-oauthlib-3.2.0.8/types_oauthlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:22:01.000000 types-oauthlib-3.2.0.8/types_oauthlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.839660 types-oauthlib-3.2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-20 15:19:37.000000 types-oauthlib-3.2.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:37.000000 types-oauthlib-3.2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:19:38.839660 types-oauthlib-3.2.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.827660 types-oauthlib-3.2.0.9/oauthlib-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 15:19:37.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/common.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.827660 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.831660 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.831660 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/access_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/authorization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/pre_configured.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/request_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/signature_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/parameters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/request_validator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/signature.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.831660 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.831660 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.835660 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/backend_application.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/legacy_application.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/mobile_application.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/service_application.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/web_application.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.835660 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/authorization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/introspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/pre_configured.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/revocation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.835660 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/authorization_code.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/client_credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/implicit.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/refresh_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/resource_owner_password_credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/parameters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/request_validator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/tokens.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.835660 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.835660 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.839660 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.839660 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/endpoints/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/endpoints/pre_configured.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/endpoints/userinfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.839660 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/authorization_code.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/dispatchers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/hybrid.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/implicit.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/request_validator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/tokens.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-20 15:15:13.000000 types-oauthlib-3.2.0.9/oauthlib-stubs/uri_validate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:38.839660 types-oauthlib-3.2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-20 15:19:37.000000 types-oauthlib-3.2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:38.839660 types-oauthlib-3.2.0.9/types_oauthlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:19:38.000000 types-oauthlib-3.2.0.9/types_oauthlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-20 15:19:38.000000 types-oauthlib-3.2.0.9/types_oauthlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:38.000000 types-oauthlib-3.2.0.9/types_oauthlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:19:38.000000 types-oauthlib-3.2.0.9/types_oauthlib.egg-info/top_level.txt
```

### Comparing `types-oauthlib-3.2.0.8/CHANGELOG.md` & `types-oauthlib-3.2.0.9/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.2.0.9 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 3.2.0.8 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 3.2.0.7 (2023-03-27)
 
 Add defaults for third-party stubs M-O (#9956)
```

### Comparing `types-oauthlib-3.2.0.8/PKG-INFO` & `types-oauthlib-3.2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-oauthlib
-Version: 3.2.0.8
+Version: 3.2.0.9
 Summary: Typing stubs for oauthlib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/oauthlib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `oauthlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/oauthlib. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/common.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/common.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/__init__.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/__init__.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/access_token.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/access_token.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/authorization.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/authorization.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/endpoints/request_token.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/endpoints/request_token.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/errors.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/request_validator.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/request_validator.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth1/rfc5849/signature.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth1/rfc5849/signature.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/__init__.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/__init__.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/base.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/base.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/service_application.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/service_application.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/clients/web_application.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/clients/web_application.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/__init__.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/authorization.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/authorization.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/base.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/base.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/introspect.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/introspect.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/metadata.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/metadata.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/pre_configured.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/pre_configured.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/resource.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/resource.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/revocation.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/revocation.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/endpoints/token.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/endpoints/token.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/errors.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/authorization_code.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/authorization_code.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/grant_types/base.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/grant_types/base.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/parameters.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/parameters.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/request_validator.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/request_validator.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/oauth2/rfc6749/tokens.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/oauth2/rfc6749/tokens.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/endpoints/pre_configured.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/endpoints/pre_configured.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/exceptions.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/dispatchers.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/dispatchers.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/grant_types/hybrid.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/grant_types/hybrid.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/request_validator.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/request_validator.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/openid/connect/core/tokens.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/openid/connect/core/tokens.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/oauthlib-stubs/uri_validate.pyi` & `types-oauthlib-3.2.0.9/oauthlib-stubs/uri_validate.pyi`

 * *Files identical despite different names*

### Comparing `types-oauthlib-3.2.0.8/setup.py` & `types-oauthlib-3.2.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `oauthlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/oauthlib. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="3.2.0.8",
+      version="3.2.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/oauthlib.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['oauthlib-stubs'],
-      package_data={'oauthlib-stubs': ['__init__.pyi', 'common.pyi', 'oauth1/__init__.pyi', 'oauth1/rfc5849/__init__.pyi', 'oauth1/rfc5849/endpoints/__init__.pyi', 'oauth1/rfc5849/endpoints/access_token.pyi', 'oauth1/rfc5849/endpoints/authorization.pyi', 'oauth1/rfc5849/endpoints/base.pyi', 'oauth1/rfc5849/endpoints/pre_configured.pyi', 'oauth1/rfc5849/endpoints/request_token.pyi', 'oauth1/rfc5849/endpoints/resource.pyi', 'oauth1/rfc5849/endpoints/signature_only.pyi', 'oauth1/rfc5849/errors.pyi', 'oauth1/rfc5849/parameters.pyi', 'oauth1/rfc5849/request_validator.pyi', 'oauth1/rfc5849/signature.pyi', 'oauth1/rfc5849/utils.pyi', 'oauth2/__init__.pyi', 'oauth2/rfc6749/__init__.pyi', 'oauth2/rfc6749/clients/__init__.pyi', 'oauth2/rfc6749/clients/backend_application.pyi', 'oauth2/rfc6749/clients/base.pyi', 'oauth2/rfc6749/clients/legacy_application.pyi', 'oauth2/rfc6749/clients/mobile_application.pyi', 'oauth2/rfc6749/clients/service_application.pyi', 'oauth2/rfc6749/clients/web_application.pyi', 'oauth2/rfc6749/endpoints/__init__.pyi', 'oauth2/rfc6749/endpoints/authorization.pyi', 'oauth2/rfc6749/endpoints/base.pyi', 'oauth2/rfc6749/endpoints/introspect.pyi', 'oauth2/rfc6749/endpoints/metadata.pyi', 'oauth2/rfc6749/endpoints/pre_configured.pyi', 'oauth2/rfc6749/endpoints/resource.pyi', 'oauth2/rfc6749/endpoints/revocation.pyi', 'oauth2/rfc6749/endpoints/token.pyi', 'oauth2/rfc6749/errors.pyi', 'oauth2/rfc6749/grant_types/__init__.pyi', 'oauth2/rfc6749/grant_types/authorization_code.pyi', 'oauth2/rfc6749/grant_types/base.pyi', 'oauth2/rfc6749/grant_types/client_credentials.pyi', 'oauth2/rfc6749/grant_types/implicit.pyi', 'oauth2/rfc6749/grant_types/refresh_token.pyi', 'oauth2/rfc6749/grant_types/resource_owner_password_credentials.pyi', 'oauth2/rfc6749/parameters.pyi', 'oauth2/rfc6749/request_validator.pyi', 'oauth2/rfc6749/tokens.pyi', 'oauth2/rfc6749/utils.pyi', 'openid/__init__.pyi', 'openid/connect/__init__.pyi', 'openid/connect/core/__init__.pyi', 'openid/connect/core/endpoints/__init__.pyi', 'openid/connect/core/endpoints/pre_configured.pyi', 'openid/connect/core/endpoints/userinfo.pyi', 'openid/connect/core/exceptions.pyi', 'openid/connect/core/grant_types/__init__.pyi', 'openid/connect/core/grant_types/authorization_code.pyi', 'openid/connect/core/grant_types/base.pyi', 'openid/connect/core/grant_types/dispatchers.pyi', 'openid/connect/core/grant_types/hybrid.pyi', 'openid/connect/core/grant_types/implicit.pyi', 'openid/connect/core/request_validator.pyi', 'openid/connect/core/tokens.pyi', 'signals.pyi', 'uri_validate.pyi', 'METADATA.toml']},
+      package_data={'oauthlib-stubs': ['__init__.pyi', 'common.pyi', 'oauth1/__init__.pyi', 'oauth1/rfc5849/__init__.pyi', 'oauth1/rfc5849/endpoints/__init__.pyi', 'oauth1/rfc5849/endpoints/access_token.pyi', 'oauth1/rfc5849/endpoints/authorization.pyi', 'oauth1/rfc5849/endpoints/base.pyi', 'oauth1/rfc5849/endpoints/pre_configured.pyi', 'oauth1/rfc5849/endpoints/request_token.pyi', 'oauth1/rfc5849/endpoints/resource.pyi', 'oauth1/rfc5849/endpoints/signature_only.pyi', 'oauth1/rfc5849/errors.pyi', 'oauth1/rfc5849/parameters.pyi', 'oauth1/rfc5849/request_validator.pyi', 'oauth1/rfc5849/signature.pyi', 'oauth1/rfc5849/utils.pyi', 'oauth2/__init__.pyi', 'oauth2/rfc6749/__init__.pyi', 'oauth2/rfc6749/clients/__init__.pyi', 'oauth2/rfc6749/clients/backend_application.pyi', 'oauth2/rfc6749/clients/base.pyi', 'oauth2/rfc6749/clients/legacy_application.pyi', 'oauth2/rfc6749/clients/mobile_application.pyi', 'oauth2/rfc6749/clients/service_application.pyi', 'oauth2/rfc6749/clients/web_application.pyi', 'oauth2/rfc6749/endpoints/__init__.pyi', 'oauth2/rfc6749/endpoints/authorization.pyi', 'oauth2/rfc6749/endpoints/base.pyi', 'oauth2/rfc6749/endpoints/introspect.pyi', 'oauth2/rfc6749/endpoints/metadata.pyi', 'oauth2/rfc6749/endpoints/pre_configured.pyi', 'oauth2/rfc6749/endpoints/resource.pyi', 'oauth2/rfc6749/endpoints/revocation.pyi', 'oauth2/rfc6749/endpoints/token.pyi', 'oauth2/rfc6749/errors.pyi', 'oauth2/rfc6749/grant_types/__init__.pyi', 'oauth2/rfc6749/grant_types/authorization_code.pyi', 'oauth2/rfc6749/grant_types/base.pyi', 'oauth2/rfc6749/grant_types/client_credentials.pyi', 'oauth2/rfc6749/grant_types/implicit.pyi', 'oauth2/rfc6749/grant_types/refresh_token.pyi', 'oauth2/rfc6749/grant_types/resource_owner_password_credentials.pyi', 'oauth2/rfc6749/parameters.pyi', 'oauth2/rfc6749/request_validator.pyi', 'oauth2/rfc6749/tokens.pyi', 'oauth2/rfc6749/utils.pyi', 'openid/__init__.pyi', 'openid/connect/__init__.pyi', 'openid/connect/core/__init__.pyi', 'openid/connect/core/endpoints/__init__.pyi', 'openid/connect/core/endpoints/pre_configured.pyi', 'openid/connect/core/endpoints/userinfo.pyi', 'openid/connect/core/exceptions.pyi', 'openid/connect/core/grant_types/__init__.pyi', 'openid/connect/core/grant_types/authorization_code.pyi', 'openid/connect/core/grant_types/base.pyi', 'openid/connect/core/grant_types/dispatchers.pyi', 'openid/connect/core/grant_types/hybrid.pyi', 'openid/connect/core/grant_types/implicit.pyi', 'openid/connect/core/request_validator.pyi', 'openid/connect/core/tokens.pyi', 'signals.pyi', 'uri_validate.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-oauthlib-3.2.0.8/types_oauthlib.egg-info/PKG-INFO` & `types-oauthlib-3.2.0.9/types_oauthlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-oauthlib
-Version: 3.2.0.8
+Version: 3.2.0.9
 Summary: Typing stubs for oauthlib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/oauthlib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `oauthlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/oauthlib. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-oauthlib-3.2.0.8/types_oauthlib.egg-info/SOURCES.txt` & `types-oauthlib-3.2.0.9/types_oauthlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

