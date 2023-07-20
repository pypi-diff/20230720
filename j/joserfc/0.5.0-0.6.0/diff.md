# Comparing `tmp/joserfc-0.5.0.tar.gz` & `tmp/joserfc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joserfc-0.5.0.tar", last modified: Wed Jul 12 12:15:29 2023, max compression
+gzip compressed data, was "joserfc-0.6.0.tar", last modified: Thu Jul 20 12:44:50 2023, max compression
```

## Comparing `joserfc-0.5.0.tar` & `joserfc-0.6.0.tar`

### file list

```diff
@@ -1,79 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-12 12:15:20.000000 joserfc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-12 12:15:29.275596 joserfc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-12 12:15:20.000000 joserfc-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-12 12:15:20.000000 joserfc-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:15:29.275596 joserfc-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 12:15:20.000000 joserfc-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.267596 joserfc-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/drafts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/drafts/jwe_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/drafts/jwe_ecdh_1pu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/jwe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/jwk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/rfc7515/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7515/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/rfc7516/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7516/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc/rfc7517/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/keyset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7517/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc7518/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/derive_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/ec_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/jwe_algs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/jwe_encs.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/jwe_zips.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/jws_algs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/oct_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/rsa_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7518/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc7519/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7519/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7519/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7519/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc7638/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7638/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc7797/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7797/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7797/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7797/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc7797/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc8037/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc8037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc8037/jws_eddsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc8037/okp_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/src/joserfc/rfc8812/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/rfc8812/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-12 12:15:20.000000 joserfc-0.5.0/src/joserfc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.271596 joserfc-0.5.0/src/joserfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 12:15:29.000000 joserfc-0.5.0/src/joserfc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:15:29.275596 joserfc-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-12 12:15:20.000000 joserfc-0.5.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.256495 joserfc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-20 12:44:35.000000 joserfc-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 12:44:35.000000 joserfc-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-20 12:44:50.256495 joserfc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-20 12:44:35.000000 joserfc-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.216494 joserfc-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.216494 joserfc-0.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/_static/dark-logo.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17719 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/_static/light-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.220494 joserfc-0.6.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/api/jwe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/api/jwk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/api/jws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/api/jwt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.220494 joserfc-0.6.0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/contributing/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/contributing/sponsors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/contributing/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/contributing/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.220494 joserfc-0.6.0/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/guide/algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/guide/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/guide/jwe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/guide/jwk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/guide/jws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/guide/jwt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/guide/registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.208494 joserfc-0.6.0/docs/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.208494 joserfc-0.6.0/docs/locales/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.224494 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/api.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/changelog.po
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/contributing.po
+-rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/guide.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/install.po
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/migrations.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/recipes.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/security.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/locales/zh/LC_MESSAGES/stability.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.224494 joserfc-0.6.0/docs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/migrations/authlib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/migrations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/migrations/pyjwt.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.224494 joserfc-0.6.0/docs/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/recipes/azure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/recipes/openssl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/security.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-20 12:44:35.000000 joserfc-0.6.0/docs/stability.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-20 12:44:35.000000 joserfc-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:44:50.256495 joserfc-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:44:35.000000 joserfc-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.212494 joserfc-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.224494 joserfc-0.6.0/src/joserfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.228494 joserfc-0.6.0/src/joserfc/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/drafts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/drafts/jwe_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/drafts/jwe_ecdh_1pu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/jwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.228494 joserfc-0.6.0/src/joserfc/rfc7515/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7515/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7515/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7515/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7515/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7515/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7515/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.232494 joserfc-0.6.0/src/joserfc/rfc7516/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7516/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7516/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7516/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7516/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7516/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7516/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7516/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.232494 joserfc-0.6.0/src/joserfc/rfc7517/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7517/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7517/keyset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7517/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7517/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7517/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7517/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.236494 joserfc-0.6.0/src/joserfc/rfc7518/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/derive_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/ec_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/jwe_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/jwe_encs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/jwe_zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/jws_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/oct_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/rsa_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7518/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.240495 joserfc-0.6.0/src/joserfc/rfc7519/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7519/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7519/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7519/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.240495 joserfc-0.6.0/src/joserfc/rfc7638/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7638/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.240495 joserfc-0.6.0/src/joserfc/rfc7797/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7797/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7797/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7797/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc7797/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.240495 joserfc-0.6.0/src/joserfc/rfc8037/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc8037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc8037/jws_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc8037/okp_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.240495 joserfc-0.6.0/src/joserfc/rfc8812/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/rfc8812/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-20 12:44:35.000000 joserfc-0.6.0/src/joserfc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.228494 joserfc-0.6.0/src/joserfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-20 12:44:50.000000 joserfc-0.6.0/src/joserfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-20 12:44:50.000000 joserfc-0.6.0/src/joserfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:44:50.000000 joserfc-0.6.0/src/joserfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 12:44:50.000000 joserfc-0.6.0/src/joserfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 12:44:50.000000 joserfc-0.6.0/src/joserfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.240495 joserfc-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.244495 joserfc-0.6.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/fixtures/jwe_compact_ecdh_1pu.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/fixtures/jwe_compact_ecdh_es.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/fixtures/jwe_rfc7520.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/fixtures/jws_examples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/fixtures/jws_rfc7520.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/fixtures/jws_rfc7797.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/fixtures/jwt_use_jws.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.244495 joserfc-0.6.0/tests/jwe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwe/test_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwe/test_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwe/test_ecdh_1pu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwe/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwe/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwe/test_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.244495 joserfc-0.6.0/tests/jwk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwk/test_ec_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwk/test_jwk_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwk/test_key_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwk/test_oct_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwk/test_okp_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwk/test_rsa_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.248495 joserfc-0.6.0/tests/jws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jws/test_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jws/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jws/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jws/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jws/test_rfc7797.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.248495 joserfc-0.6.0/tests/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwt/test_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwt/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/jwt/test_jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.256495 joserfc-0.6.0/tests/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7516-A.1.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7516-A.2.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-EC-108.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-EC-120.json
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-EC-private.json
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-EC-public.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-RSA-73.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-RSA-84.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-RSA-private.json
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-RSA-public.json
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-oct-130.json
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-oct-enc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/RFC7520-oct-sig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-p256-alice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-p256-bob.json
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-p256-private.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-p256-public.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-p384-private.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-p384-public.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-p512-private.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-p512-public.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-secp256k1-private.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ec-secp256k1-public.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/okp-ed25519-private.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/okp-ed25519-public.json
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/okp-ed448-private.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/okp-ed448-public.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/okp-x25519-alice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/okp-x25519-bob.json
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/okp-x25519-charlie.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/rsa-openssl-private.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/rsa-openssl-public.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ssh-rsa-private.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/keys/ssh-rsa-public.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:50.256495 joserfc-0.6.0/tests/rfc7520/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/rfc7520/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/rfc7520/test_jwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/rfc7520/test_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-20 12:44:35.000000 joserfc-0.6.0/tests/test_util.py
```

### Comparing `joserfc-0.5.0/LICENSE` & `joserfc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joserfc-0.5.0/PKG-INFO` & `joserfc-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.5.0
+Version: 0.6.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
 Project-URL: Source, https://github.com/authlib/joserfc
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
@@ -20,20 +20,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: drafts
 License-File: LICENSE
 
 JOSE RFC
 ========
 
-``joserfc`` is a Python implementation of **JSON Object Signing and Encryption** (JOSE).
+`·joserfc·` is a Python library that provides a comprehensive implementation of several
+essential JSON Object Signing and Encryption (JOSE) standards.
 
 This package contains implementation of:
 
 - RFC7515: JSON Web Signature
 - RFC7516: JSON Web Encryption
 - RFC7517: JSON Web Key
 - RFC7518: JSON Web Algorithms
@@ -67,12 +69,11 @@
 
 Useful Links
 ------------
 
 1. GitHub: https://github.com/authlib/joserfc
 2. Docs: https://jose.authlib.org/
 
-
 License
 -------
 
 Licensed under BSD. Please see LICENSE for licensing details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `joserfc-0.5.0/README.rst` & `joserfc-0.6.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 JOSE RFC
 ========
 
-``joserfc`` is a Python implementation of **JSON Object Signing and Encryption** (JOSE).
+`·joserfc·` is a Python library that provides a comprehensive implementation of several
+essential JSON Object Signing and Encryption (JOSE) standards.
 
 This package contains implementation of:
 
 - RFC7515: JSON Web Signature
 - RFC7516: JSON Web Encryption
 - RFC7517: JSON Web Key
 - RFC7518: JSON Web Algorithms
@@ -39,12 +40,11 @@
 
 Useful Links
 ------------
 
 1. GitHub: https://github.com/authlib/joserfc
 2. Docs: https://jose.authlib.org/
 
-
 License
 -------
 
 Licensed under BSD. Please see LICENSE for licensing details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `joserfc-0.5.0/pyproject.toml` & `joserfc-0.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,17 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Security",
   "Topic :: Security :: Cryptography",
 ]
 
+[project.optional-dependencies]
+drafts = ["pycryptodome"]
+
 [project.urls]
 Documentation = "https://jose.authlib.org/"
 Source = "https://github.com/authlib/joserfc"
 Blog = "https://blog.authlib.org/"
 
 [build-system]
 requires = ["setuptools"]
@@ -38,14 +41,17 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "joserfc.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+joserfc = ["py.typed"]
+
 [tool.pytest.ini_options]
 pythonpath = ["src", "."]
 testpaths = ["tests"]
 filterwarnings = ["error"]
 
 [tool.coverage.run]
 branch = true
@@ -55,8 +61,15 @@
 source = ["src"]
 
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
   "raise NotImplementedError",
   "@(abc\\.)?abstractmethod",
+  "@overload",
 ]
+
+[tool.mypy]
+python_version = "3.8"
+files = ["src/joserfc"]
+show_error_codes = true
+pretty = true
```

### Comparing `joserfc-0.5.0/src/joserfc/drafts/jwe_chacha20.py` & `joserfc-0.6.0/src/joserfc/drafts/jwe_chacha20.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Tuple
 from Crypto.Cipher import ChaCha20_Poly1305
 from ..rfc7516.registry import JWERegistry
 from ..rfc7516.models import JWEEncModel
 
 __all__ = ["ChaCha20EncModel", "JWE_ENC_MODELS", "register_chaha20_poly1305"]
 
 
@@ -11,15 +12,15 @@
     recommended = False
 
     def __init__(self, name: str, description: str, iv_size: int):
         self.name = name
         self.description = description
         self.iv_size = iv_size
 
-    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> (bytes, bytes):
+    def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> Tuple[bytes, bytes]:
         """Key Encryption with AEAD_CHACHA20_POLY1305
         """
         chacha = ChaCha20_Poly1305.new(key=cek, nonce=iv)
         chacha.update(aad)
         ciphertext, tag = chacha.encrypt_and_digest(plaintext)
         return ciphertext, tag
```

### Comparing `joserfc-0.5.0/src/joserfc/drafts/jwe_ecdh_1pu.py` & `joserfc-0.6.0/src/joserfc/drafts/jwe_ecdh_1pu.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import typing as t
-from ..rfc7516.registry import JWERegistry
 from ..rfc7516.models import (
     Recipient,
     JWEKeyAgreement,
     JWEKeyWrapping,
     JWEEncModel
 )
 from ..rfc7517.models import CurveKey
@@ -30,16 +29,16 @@
     """
     more_header_registry = {
         "epk": HeaderParameter("Ephemeral Public Key", "jwk", True),
         "apu": HeaderParameter("Agreement PartyUInfo", "str"),
         "apv": HeaderParameter("Agreement PartyVInfo", "str"),
         "skid": HeaderParameter("Sender Key ID", "str"),
     }
+    key_types = ["EC", "OKP"]
     tag_aware = True
-    recommended: bool = False
 
     def __init__(self, key_wrapping: t.Optional[JWEKeyWrapping]):
         if key_wrapping is None:
             self.name = "ECDH-1PU"
             self.description = "ECDH-1PU using one-pass KDF and CEK in the Direct Key Agreement mode"
             self.key_size = None
         else:
@@ -67,38 +66,45 @@
     def decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient) -> bytes:
         return self.__decrypt_agreed_upon_key(enc, recipient, None)
 
     def decrypt_agreed_upon_key_with_tag(self, enc: JWEEncModel, recipient: Recipient, tag: bytes) -> bytes:
         return self.__decrypt_agreed_upon_key(enc, recipient, tag)
 
     def __encrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient, tag: t.Optional[bytes]) -> bytes:
-        sender_key: CurveKey = recipient.sender_key
-        sender_shared_key = sender_key.exchange_derive_key(recipient.recipient_key)
-        ephemeral_shared_key = recipient.ephemeral_key.exchange_derive_key(recipient.recipient_key)
+        sender_key: CurveKey = recipient.sender_key  # type: ignore
+        recipient_key: CurveKey = recipient.recipient_key  # type: ignore
+        ephemeral_key: CurveKey = recipient.ephemeral_key  # type: ignore
+        sender_shared_key = sender_key.exchange_derive_key(recipient_key)
+        ephemeral_shared_key = ephemeral_key.exchange_derive_key(recipient_key)
         shared_key = ephemeral_shared_key + sender_shared_key
         headers = recipient.headers()
         return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size, tag)
 
     def __decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient, tag: t.Optional[bytes]) -> bytes:
         self._check_enc(enc)
         headers = recipient.headers()
         assert "epk" in headers
 
-        recipient_key: CurveKey = recipient.recipient_key
-        ephemeral_key = recipient_key.import_key(headers["epk"])
-        sender_shared_key = recipient_key.exchange_derive_key(recipient.sender_key)
+        recipient_key: CurveKey = recipient.recipient_key  # type: ignore
+        ephemeral_key: CurveKey = recipient_key.import_key(headers["epk"])  # type: ignore
+        sender_key: CurveKey = recipient.sender_key  # type: ignore
+        sender_shared_key = recipient_key.exchange_derive_key(sender_key)
         ephemeral_shared_key = recipient_key.exchange_derive_key(ephemeral_key)
         shared_key = ephemeral_shared_key + sender_shared_key
         return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size, tag)
 
 
 JWE_ALG_MODELS = [
     ECDH1PUAlgModel(None),    # ECDH-1PU
     ECDH1PUAlgModel(A128KW),  # ECDH-1PU+A128KW
     ECDH1PUAlgModel(A192KW),  # ECDH-1PU+A192KW
     ECDH1PUAlgModel(A256KW),  # ECDH-1PU+A256KW
 ]
 
 
 def register_ecdh_1pu():
+    from ..jwe import JWERegistry
+    from ..jwk import KeySet
+
     for model in JWE_ALG_MODELS:
         JWERegistry.register(model)
+        KeySet.algorithm_keys[model.name] = model.key_types
```

### Comparing `joserfc-0.5.0/src/joserfc/errors.py` & `joserfc-0.6.0/src/joserfc/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,21 @@
     """Base Exception for all errors in joserfc."""
 
     #: short-string error code
     error = ""
     #: long-string to describe this error
     description = ""
 
-    def __init__(self, description: Optional[str] = None, error: Optional[str] = None):
-        if error is not None:
-            self.error = error
+    def __init__(self, description: Optional[str] = None):
         if description is not None:
             self.description = description
 
         message = "{}: {}".format(self.error, self.description)
         super(JoseError, self).__init__(message)
 
-    def __repr__(self):
-        return '<{} "{}">'.format(self.__class__.__name__, self.error)
-
 
 class DecodeError(JoseError):
     error = "decode_error"
 
 
 class UnsupportedKeyUseError(JoseError):
     error = "unsupported_key_use"
@@ -75,19 +70,14 @@
 class InvalidEncryptionAlgorithmError(JoseError):
     """This error is designed for JWE. It is raised when "enc" value
     does not work together with "alg" value.
     """
     error = 'invalid_encryption_algorithm'
 
 
-class UnwrapError(JoseError):
-    error = "unwrap_error"
-    description = "Unwrap AES key failed"
-
-
 class InvalidCEKLengthError(JoseError):
     error = "invalid_cek_length"
     description = 'Invalid "cek" length'
 
 
 class InvalidClaimError(JoseError):
     error = "invalid_claim"
```

### Comparing `joserfc-0.5.0/src/joserfc/jwe.py` & `joserfc-0.6.0/src/joserfc/jwe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 import typing as t
-from .rfc7516 import types
-from .rfc7516.types import JSONSerialization
+from typing import overload
+from .rfc7516.types import (
+    GeneralJSONSerialization,
+    FlattenedJSONSerialization,
+)
 from .rfc7516.models import (
     Recipient,
     CompactEncryption,
-    JSONEncryption,
+    GeneralJSONEncryption,
+    FlattenedJSONEncryption,
     JWEEncModel,
     JWEZipModel,
 )
 from .rfc7516.registry import (
     JWERegistry,
     default_registry,
 )
 from .rfc7516.message import perform_encrypt, perform_decrypt
 from .rfc7516.compact import represent_compact, extract_compact
-from .rfc7516.json import represent_json, extract_json
+from .rfc7516.json import (
+    represent_general_json,
+    represent_flattened_json,
+    extract_general_json,
+    extract_flattened_json,
+)
 from .rfc7518.jwe_algs import JWE_ALG_MODELS
 from .rfc7518.jwe_encs import JWE_ENC_MODELS
 from .rfc7518.jwe_zips import JWE_ZIP_MODELS
 from .jwk import KeySet, CurveKey, KeyFlexible, guess_key
 from .util import to_bytes
 from .registry import Header
 
 __all__ = [
-    "types",
     "JWERegistry",
     "JWEEncModel",
     "JWEZipModel",
     "Recipient",
     "CompactEncryption",
-    "JSONEncryption",
+    "GeneralJSONEncryption",
+    "FlattenedJSONEncryption",
     "encrypt_compact",
     "decrypt_compact",
     "encrypt_json",
     "decrypt_json",
     "default_registry",
 ]
 
 
 def __register():
     for _alg in JWE_ALG_MODELS:
         JWERegistry.register(_alg)
+        KeySet.algorithm_keys[_alg.name] = _alg.key_types
 
     for _enc in JWE_ENC_MODELS:
         JWERegistry.register(_enc)
 
     for _zip in JWE_ZIP_MODELS:
         JWERegistry.register(_zip)
 
@@ -124,47 +134,70 @@
     obj = extract_compact(to_bytes(value))
     if algorithms:
         registry = JWERegistry(algorithms=algorithms)
     elif registry is None:
         registry = default_registry
 
     recipient = obj.recipient
+    assert recipient is not None
     key = guess_key(private_key, recipient)
     key.check_use("enc")
     recipient.recipient_key = key
     if sender_key:
         recipient.sender_key = _guess_sender_key(recipient, sender_key)
-    return perform_decrypt(obj, registry)
+    perform_decrypt(obj, registry)
+    return obj
+
+
+@overload
+def encrypt_json(
+        obj: GeneralJSONEncryption,
+        public_key: t.Optional[KeyFlexible],
+        algorithms: t.Optional[t.List[str]] = None,
+        registry: t.Optional[JWERegistry] = None,
+        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None) -> GeneralJSONSerialization:
+    ...
+
+
+@overload
+def encrypt_json(
+        obj: FlattenedJSONEncryption,
+        public_key: t.Optional[KeyFlexible],
+        algorithms: t.Optional[t.List[str]] = None,
+        registry: t.Optional[JWERegistry] = None,
+        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None) -> FlattenedJSONSerialization:
+    ...
 
 
 def encrypt_json(
-        obj: JSONEncryption,
+        obj: t.Union[GeneralJSONEncryption, FlattenedJSONEncryption],
         public_key: t.Optional[KeyFlexible],
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWERegistry] = None,
-        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None) -> JSONSerialization:
+        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None):
     """Generate a JWE JSON Serialization (in dict). The JWE JSON Serialization
     represents encrypted content as a JSON object. This representation is neither
     optimized for compactness nor URL safe.
 
-    When calling this method, developers MUST construct an instance of a ``JSONEncryption``
-    object. Here is an example::
+    When calling this method, developers MUST construct an instance of a
+    ``GeneralJSONEncryption`` or ``FlattenedJSONEncryption`` object. Here
+    is an example::
 
-        from joserfc.jwe import JSONEncryption
+        from joserfc.jwe import GeneralJSONEncryption
 
         protected = {"enc": "A128CBC-HS256"}
         plaintext = b"hello world"
         header = {"jku": "https://server.example.com/keys.jwks"}  # optional shared header
-        obj = JSONEncryption(protected, plaintext, header)
+        obj = GeneralJSONEncryption(protected, plaintext, header)
         # add the recipients
         obj.add_recipient({"kid": "alice", "alg": "RSA1_5"})  # not configured a key
         bob_key = OctKey.import_key("bob secret")
         obj.add_recipient({"kid": "bob", "alg": "A128KW"}, bob_key)
 
-    :param obj: an instance of ``JSONEncryption``
+    :param obj: an instance of ``GeneralJSONEncryption`` or ``FlattenedJSONEncryption``
     :param public_key: a public key used to encrypt the CEK
     :param algorithms: a list of allowed algorithms
     :param registry: a JWERegistry to use
     :param sender_key: only required when using ECDH-1PU
     :return: JWE JSON Serialization in dict
     """
 
@@ -178,50 +211,69 @@
             recipient.sender_key = _guess_sender_key(recipient, sender_key)
         if not recipient.recipient_key:
             key = guess_key(public_key, recipient)
             key.check_use("enc")
             recipient.recipient_key = key
 
     perform_encrypt(obj, registry)
-    return represent_json(obj)
+    if isinstance(obj, GeneralJSONEncryption):
+        return represent_general_json(obj)
+    return represent_flattened_json(obj)
 
 
 def decrypt_json(
-        data: JSONSerialization,
+        data: t.Union[GeneralJSONSerialization, FlattenedJSONSerialization],
         private_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWERegistry] = None,
-        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None) -> JSONEncryption:
-    """Decrypt the JWE JSON Serialization (in dict) to a ``JSONEncryption`` object.
+        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None):
+    """Decrypt the JWE JSON Serialization (in dict) to a
+    ``GeneralJSONEncryption`` or ``FlattenedJSONEncryption`` object.
 
     :param data: JWE JSON Serialization in dict
     :param private_key: a flexible private key to decrypt the CEK
     :param algorithms: a list of allowed algorithms
     :param registry: a JWERegistry to use
     :param sender_key: only required when using ECDH-1PU
-    :return: an instance of ``JSONEncryption``
+    :return: an instance of ``GeneralJSONEncryption`` or ``FlattenedJSONEncryption``
     """
-    obj = extract_json(data)
-
     if algorithms:
         registry = JWERegistry(algorithms=algorithms)
     elif registry is None:
         registry = default_registry
 
-    for recipient in obj.recipients:
+    if "recipients" in data:
+        general_obj = extract_general_json(data)  # type: ignore
+        _attach_recipient_keys(general_obj.recipients, private_key, sender_key)
+        perform_decrypt(general_obj, registry)
+        return general_obj
+    else:
+        flattened_obj = extract_flattened_json(data)  # type: ignore
+        _attach_recipient_keys(flattened_obj.recipients, private_key, sender_key)
+        perform_decrypt(flattened_obj, registry)
+        return flattened_obj
+
+
+def _attach_recipient_keys(
+        recipients: t.List[Recipient],
+        private_key: KeyFlexible,
+        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None):
+    for recipient in recipients:
         key = guess_key(private_key, recipient)
         key.check_use("enc")
         recipient.recipient_key = key
         if sender_key:
             recipient.sender_key = _guess_sender_key(recipient, sender_key)
 
-    return perform_decrypt(obj, registry)
-
 
-def _guess_sender_key(recipient, key: t.Union[CurveKey, KeySet]):
+def _guess_sender_key(recipient: Recipient, key: t.Union[CurveKey, KeySet]):
     if isinstance(key, KeySet):
         headers = recipient.headers()
         skid = headers.get('skid')
         if skid:
             return key.get_by_kid(skid)
-        return None
+        skey = key.pick_random_key(headers["alg"])
+        if skey is not None:
+            recipient.add_header("skid", skey.kid)
+            return skey
+        raise ValueError("Invalid key")
     return key
```

### Comparing `joserfc-0.5.0/src/joserfc/jwk.py` & `joserfc-0.6.0/src/joserfc/jwk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,81 @@
-import random
-from typing import Callable, Union, Any, AnyStr, Protocol
+import typing as t
 from .rfc7517 import (
+    BaseKey,
     SymmetricKey,
     AsymmetricKey,
     CurveKey,
-    Key,
-    JWKRegistry,
-    KeySet,
+    JWKRegistry as _JWKRegistry,
+    KeySet as _KeySet,
 )
 from .rfc7517 import types
 from .rfc7518.oct_key import OctKey
 from .rfc7518.rsa_key import RSAKey
 from .rfc7518.ec_key import ECKey
 from .rfc8037.okp_key import OKPKey
 from .rfc8812 import register_secp256k1
 from .registry import Header
 
 
-KeyCallable = Callable[[Any, bool], Key]
-KeyFlexible = Union[AnyStr, Key, KeySet, KeyCallable]
-
 __all__ = [
     "types",
     "JWKRegistry",
+    "BaseKey",
     "SymmetricKey",
     "AsymmetricKey",
     "CurveKey",
     "Key",
     "KeyCallable",
     "KeyFlexible",
     "OctKey",
     "RSAKey",
     "ECKey",
     "OKPKey",
     "KeySet",
     "guess_key",
 ]
 
+register_secp256k1()
+
+
+class JWKRegistry(_JWKRegistry):
+    """A registry for JWK to record ``joserfc`` supported key types.
+    Normally, you would use explicit key types like ``OctKey``, ``RSAKey``;
+    This registry provides a way to dynamically import and generate keys.
+    For instance:
+
+    .. code-block:: python
+
+        from joserfc.jwk import JWKRegistry
+
+        # instead of choosing which key type to use yourself,
+        # JWKRegistry can import it automatically
+        data = {"kty": "oct", "k": "..."}
+        key = JWKRegistry.import_key(data)
+    """
+    key_types = {
+        OctKey.key_type: OctKey,
+        RSAKey.key_type: RSAKey,
+        ECKey.key_type: ECKey,
+        OKPKey.key_type: OKPKey,
+    }
+
+
+Key = t.Union[OctKey, RSAKey, ECKey, OKPKey]
+KeyCallable = t.Callable[[t.Any], Key]
+
 
-def __register():
-    JWKRegistry.register(OctKey)
-    JWKRegistry.register(RSAKey)
-    JWKRegistry.register(ECKey)
-    JWKRegistry.register(OKPKey)
-    # add {"crv": "secp256k1"} for ECKey
-    register_secp256k1()
+class KeySet(_KeySet):
+    registry_cls = JWKRegistry
 
 
-# register all key types
-__register()
+KeyFlexible = t.Union[t.AnyStr, Key, KeySet, KeyCallable]
 
 
-class GuestProtocol(Protocol):  # pragma: no cover
+class GuestProtocol(t.Protocol):  # pragma: no cover
     def headers(self) -> Header:
         ...
 
     def set_kid(self, kid: str):
         ...
 
 
@@ -64,30 +84,31 @@
 
     :param key: a very flexible key
     :param obj: a protocol that has ``headers`` and ``set_kid`` methods
     """
     headers = obj.headers()
 
     if isinstance(key, (str, bytes)):
-        rv_key = OctKey.import_key(key)
+        rv_key = OctKey.import_key(key)  # type: ignore
 
-    elif isinstance(key, (SymmetricKey, AsymmetricKey)):
-        rv_key = key
+    elif isinstance(key, BaseKey):
+        rv_key: Key = key  # type: ignore
 
     elif isinstance(key, KeySet):
         kid = headers.get("kid")
         if not kid:
             # choose one key by random
-            key: Key = random.choice(key.keys)
+            rv_key: Key = key.pick_random_key(headers["alg"])  # type: ignore
+            if rv_key is None:
+                raise ValueError("Invalid key")
             # use side effect to add kid information
-            obj.set_kid(key.kid)
-            rv_key = key
+            obj.set_kid(rv_key.kid)
         else:
-            rv_key = key.get_by_kid(kid)
+            rv_key: Key = key.get_by_kid(kid)  # type: ignore
 
     elif callable(key):
-        rv_key = key(obj)
+        rv_key = key(obj)  # type: ignore
 
     else:
         raise ValueError("Invalid key")
 
-    return rv_key
+    return rv_key  # type: ignore
```

### Comparing `joserfc-0.5.0/src/joserfc/jws.py` & `joserfc-0.6.0/src/joserfc/jws.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,82 @@
 import typing as t
-from .rfc7515 import types
+from typing import overload
 from .rfc7515.model import (
     JWSAlgModel,
     HeaderMember,
     CompactSignature,
-    JSONSignature,
+    GeneralJSONSignature,
+    FlattenedJSONSignature,
 )
 from .rfc7515.registry import (
     JWSRegistry,
     construct_registry,
 )
 from .rfc7515.compact import (
     sign_compact,
     extract_compact,
     verify_compact,
     detach_compact_content,
 )
 from .rfc7515.json import (
-    construct_json_signature,
-    sign_json,
-    verify_json,
-    extract_json,
+    sign_general_json,
+    sign_flattened_json,
+    verify_general_json,
+    verify_flattened_json,
+    extract_general_json,
+    extract_flattened_json,
     detach_json_content,
 )
 from .rfc7515.types import (
     HeaderDict,
-    JSONSerialization,
+    GeneralJSONSerialization,
+    FlattenedJSONSerialization,
 )
 from .rfc7518.jws_algs import JWS_ALGORITHMS
 from .rfc8037.jws_eddsa import EdDSA
 from .rfc8812 import ES256K
 from .errors import BadSignatureError
-from .jwk import Key, KeyFlexible, guess_key
-from .util import to_bytes, urlsafe_b64encode
+from .jwk import Key, KeyFlexible, KeySet, guess_key
+from .util import to_bytes
 from .registry import Header
 
 __all__ = [
-    "types",
     "JWSAlgModel",
     "JWSRegistry",
+    "HeaderDict",
     "HeaderMember",
     "CompactSignature",
-    "JSONSignature",
+    "GeneralJSONSignature",
+    "FlattenedJSONSignature",
+    "GeneralJSONSerialization",
+    "FlattenedJSONSerialization",
     "serialize_compact",
     "deserialize_compact",
     "extract_compact",
     "validate_compact",
     "serialize_json",
     "deserialize_json",
-    "extract_json",
-    "validate_json",
     "detach_content",
 ]
 
 
 # register supported alg models
 def __register():
     # register alg in RFC7518
     for _alg in JWS_ALGORITHMS:
         JWSRegistry.register(_alg)
+        KeySet.algorithm_keys[_alg.name] = [_alg.key_type]
+
     # register alg in RFC8037
     JWSRegistry.register(EdDSA)
+    KeySet.algorithm_keys[EdDSA.name] = [EdDSA.key_type]
+
     # register alg in RFC8812
     JWSRegistry.register(ES256K)
+    KeySet.algorithm_keys[ES256K.name] = [ES256K.key_type]
 
 
 __register()
 
 
 def serialize_compact(
         protected: Header,
@@ -95,43 +105,43 @@
         registry = construct_registry(algorithms)
 
     registry.check_header(protected)
     obj = CompactSignature(protected, to_bytes(payload))
     alg: JWSAlgModel = registry.get_alg(protected["alg"])
     key: Key = guess_key(private_key, obj)
     key.check_use("sig")
+    alg.check_key_type(key)
     key.check_alg(protected["alg"])
     out = sign_compact(obj, alg, key)
     return out.decode("utf-8")
 
 
 def validate_compact(
         obj: CompactSignature,
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
-        registry: t.Optional[JWSRegistry] = None):
+        registry: t.Optional[JWSRegistry] = None) -> bool:
     """Validate the JWS Compact Serialization with the given key.
     This method is usually used together with ``extract_compact``.
 
     :param obj: object of the JWS Compact Serialization
     :param public_key: a flexible public key to verify the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
-    :raise: ValueError or BadSignatureError
     """
     if registry is None:
         registry = construct_registry(algorithms)
 
     headers = obj.headers()
     registry.check_header(headers)
     key: Key = guess_key(public_key, obj)
     key.check_use("sig")
     alg: JWSAlgModel = registry.get_alg(headers["alg"])
-    if not verify_compact(obj, alg, key):
-        raise BadSignatureError()
+    alg.check_key_type(key)
+    return verify_compact(obj, alg, key)
 
 
 def deserialize_compact(
         value: t.AnyStr,
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWSRegistry] = None) -> CompactSignature:
@@ -151,24 +161,43 @@
     :param value: a string (or bytes) of the JWS Compact Serialization
     :param public_key: a flexible public key to verify the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :return: object of the ``CompactSignature``
     """
     obj = extract_compact(to_bytes(value))
-    validate_compact(obj, public_key, algorithms, registry)
+    if not validate_compact(obj, public_key, algorithms, registry):
+        raise BadSignatureError()
     return obj
 
 
+@overload
+def serialize_json(
+        members: t.List[HeaderDict],
+        payload: t.AnyStr,
+        private_key: KeyFlexible,
+        algorithms: t.Optional[t.List[str]] = None,
+        registry: t.Optional[JWSRegistry] = None) -> GeneralJSONSerialization: ...
+
+
+@overload
+def serialize_json(
+        members: HeaderDict,
+        payload: t.AnyStr,
+        private_key: KeyFlexible,
+        algorithms: t.Optional[t.List[str]] = None,
+        registry: t.Optional[JWSRegistry] = None) -> FlattenedJSONSerialization: ...
+
+
 def serialize_json(
         members: t.Union[HeaderDict, t.List[HeaderDict]],
         payload: t.AnyStr,
         private_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
-        registry: t.Optional[JWSRegistry] = None) -> JSONSerialization:
+        registry: t.Optional[JWSRegistry] = None):
     """Generate a JWS JSON Serialization (in dict). The JWS JSON Serialization
     represents digitally signed or MACed content as a JSON object. This representation
     is neither optimized for compactness nor URL-safe.
 
     A general JWS JSON Serialization contains:
 
     payload
@@ -190,60 +219,72 @@
             "header":<non-integrity-protected header contents>,
             "signature":"<signature contents>"
         }
     """
     if registry is None:
         registry = construct_registry(algorithms)
 
-    obj = construct_json_signature(members, payload, registry)
-    obj.segments["payload"] = urlsafe_b64encode(obj.payload)
     find_key = lambda d: guess_key(private_key, d)
-    return sign_json(obj, registry, find_key)
+    _payload = to_bytes(payload)
+    if isinstance(members, list):
+        return sign_general_json(members, _payload, registry, find_key)
+    else:
+        return sign_flattened_json(members, _payload, registry, find_key)
 
 
-def validate_json(
-        obj: JSONSignature,
+@overload
+def deserialize_json(
+        value: GeneralJSONSerialization,
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
-        registry: t.Optional[JWSRegistry] = None):
-    """Validate the JWS JSON Serialization with the given key.
-    This method is usually used together with ``extract_json``.
+        registry: t.Optional[JWSRegistry] = None) -> GeneralJSONSignature: ...
 
-    :param obj: object of the JWS JSON Serialization
-    :param public_key: a flexible public key to verify the signature
-    :param algorithms: a list of allowed algorithms
-    :param registry: a JWSRegistry to use
-    :raise: ValueError or BadSignatureError
-    """
-    if registry is None:
-        registry = construct_registry(algorithms)
-    find_key = lambda d: guess_key(public_key, d)
-    if not verify_json(obj, registry, find_key):
-        raise BadSignatureError()
+
+@overload
+def deserialize_json(
+        value: FlattenedJSONSerialization,
+        public_key: KeyFlexible,
+        algorithms: t.Optional[t.List[str]] = None,
+        registry: t.Optional[JWSRegistry] = None) -> FlattenedJSONSignature: ...
 
 
 def deserialize_json(
-        value: JSONSerialization,
+        value: t.Union[GeneralJSONSerialization, FlattenedJSONSerialization],
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
-        registry: t.Optional[JWSRegistry] = None) -> JSONSignature:
+        registry: t.Optional[JWSRegistry] = None):
     """Extract and validate the JWS (in string) with the given key.
 
     :param value: a dict of the JSON signature
     :param public_key: a flexible public key to verify the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a JWSRegistry to use
     :return: object of the SignatureData
+    :raise: ValueError or BadSignatureError
     """
-    obj = extract_json(value)
-    validate_json(obj, public_key, algorithms, registry)
-    return obj
+    if registry is None:
+        registry = construct_registry(algorithms)
 
+    find_key = lambda d: guess_key(public_key, d)
+    if "signatures" in value:
+        general_obj = extract_general_json(value)
+        if not verify_general_json(general_obj, registry, find_key):
+            raise BadSignatureError()
+        return general_obj
+    else:
+        flattened_obj = extract_flattened_json(value)
+        if not verify_flattened_json(flattened_obj, registry, find_key):
+            raise BadSignatureError()
+        return flattened_obj
 
-def detach_content(value: t.Union[str, JSONSerialization]):
+
+DetachValue = t.TypeVar("DetachValue", str, t.Dict[str, t.Any])
+
+
+def detach_content(value: DetachValue) -> DetachValue:
     """In some contexts, it is useful to integrity-protect content that is
     not itself contained in a JWS. This method is an implementation of
     https://www.rfc-editor.org/rfc/rfc7515#appendix-F
 
     It is used to detach the content of the compact and JSON serialization.
 
     .. code-block:: python
@@ -255,12 +296,16 @@
 
     You can also detach the JSON serialization:
 
     .. code-block:: python
 
         >>> obj = jws.serialize_json({"protected": {"alg": "HS256"}}, b"hello", "secret")
         >>> jws.detach_content(obj)
-        {'payload': '', 'signature': 'UYmO_lPAY5V0Wf4KZsfhiYs1SxqXPhxvjuYqellDV5A', 'protected': 'eyJhbGciOiJIUzI1NiJ9'}
+        {
+            'payload': '',
+            'signature': 'UYmO_lPAY5V0Wf4KZsfhiYs1SxqXPhxvjuYqellDV5A',
+            'protected': 'eyJhbGciOiJIUzI1NiJ9'
+        }
     """
     if isinstance(value, str):
         return detach_compact_content(value)
     return detach_json_content(value)
```

### Comparing `joserfc-0.5.0/src/joserfc/jwt.py` & `joserfc-0.6.0/src/joserfc/jwt.py`

 * *Files 23% similar despite different names*

```diff
@@ -54,21 +54,24 @@
     :param header: A dict of the JWT header
     :param claims: A dict of the JWT claims to be encoded
     :param key: key used to sign the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a ``JWSRegistry`` or ``JWERegistry`` to use
     """
     # add ``typ`` in header
-    header["typ"] = "JWT"
+    _header = {"typ": "JWT", **header}
     payload = convert_claims(claims)
-    if "enc" in header:
-        result = encrypt_compact(header, payload, key, algorithms, registry)
+    if "enc" in _header:
+        if registry is not None:
+            assert isinstance(registry, JWERegistry)
+        return encrypt_compact(_header, payload, key, algorithms, registry)
     else:
-        result = serialize_compact(header, payload, key, algorithms, registry)
-    return result
+        if registry is not None:
+            assert isinstance(registry, JWSRegistry)
+        return serialize_compact(_header, payload, key, algorithms, registry)
 
 
 def decode(
         value: t.AnyStr,
         key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWTRegistry] = None) -> Token:
@@ -77,27 +80,34 @@
 
     :param value: text of the JWT
     :param key: key used to verify the signature
     :param algorithms: a list of allowed algorithms
     :param registry: a ``JWSRegistry`` or ``JWERegistry`` to use
     :raise: BadSignatureError
     """
-    value = to_bytes(value)
-    if value.count(b".") == 4:
-        obj = decrypt_compact(value, key, algorithms, registry)
-        payload = obj.plaintext
+    _value = to_bytes(value)
+    _header: Header
+    if _value.count(b".") == 4:
+        if registry is not None:
+            assert isinstance(registry, JWERegistry)
+        jwe_obj = decrypt_compact(_value, key, algorithms, registry)
+        _header = jwe_obj.headers()
+        payload: bytes = jwe_obj.plaintext  # type: ignore
     else:
-        obj = deserialize_compact(value, key, algorithms, registry)
-        payload = obj.payload
+        if registry is not None:
+            assert isinstance(registry, JWSRegistry)
+        jws_obj = deserialize_compact(_value, key, algorithms, registry)
+        _header = jws_obj.headers()
+        payload: bytes = jws_obj.payload  # type: ignore
 
     try:
         claims: Claims = json.loads(payload)
     except (TypeError, ValueError):
         raise InvalidPayloadError()
 
-    token = Token(obj.headers(), claims)
+    token = Token(_header, claims)
     typ = token.header.get("typ")
     # https://www.rfc-editor.org/rfc/rfc7519#section-5.1
     # If present, it is RECOMMENDED that its value be "JWT".
     if typ and typ != "JWT":
         raise InvalidTypeError()
     return token
```

### Comparing `joserfc-0.5.0/src/joserfc/registry.py` & `joserfc-0.6.0/src/joserfc/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import typing as t
-from collections import namedtuple
 
 Header = t.Dict[str, t.Any]
 
 
 def is_str(value: str):
     if not isinstance(value, str):
         raise ValueError("must be a str")
@@ -25,62 +24,58 @@
         raise ValueError("must be an bool")
 
 
 def is_list_str(values):
     if not isinstance(values, list):
         raise ValueError("must be a list[str]")
 
-    for value in values:
-        if not isinstance(value, str):
-            raise ValueError("must be a list[str]")
+    if not all(isinstance(value, str) for value in values):
+        raise ValueError("must be a list[str]")
 
 
 def is_jwk(value):
     if not isinstance(value, dict):
         raise ValueError("must be a JWK")
 
 
 def in_choices(choices: t.List[str]):
     def _is_one_of(value):
         if isinstance(value, list):
-            for v in value:
-                if v not in choices:
-                    raise ValueError(f"must be one of {choices}")
+            if not all(v in choices for v in value):
+                raise ValueError(f"must be one of {choices}")
 
         elif value not in choices:
             raise ValueError(f"must be one of {choices}")
 
     return _is_one_of
 
 
 def not_support(_):
     raise ValueError("is not supported")
 
 
-Validate = t.Callable[[t.Any], t.NoReturn]
-_value_validators = {
+Validate = t.Callable[[t.Any], None]
+_value_validators: t.Dict[str, Validate] = {
     "str": is_str,
     "list[str]": is_list_str,
     "int": is_int,
     "bool": is_bool,
     "url": is_url,
     "jwk": is_jwk,
     "none": not_support,
 }
 
 
 class HeaderParameter:
     """Define the header parameter for JWS and JWE."""
     def __init__(self, description: str, validate: t.Union[str, Validate], required: bool = False):
         #: a short description of the header parameter
-        self.description: str = description
-        if isinstance(validate, str):
-            validate: Validate = _value_validators[validate]
+        self.description = description
         #: a function for validating the header parameter's value
-        self.validate: Validate = validate
+        self.validate = _value_validators[validate] if isinstance(validate, str) else validate
         #: if this header parameter is required
         self.required = required
 
 
 #: Define header parameters for JWS and JWE
 HeaderRegistryDict = t.Dict[str, HeaderParameter]
 
@@ -91,27 +86,31 @@
             self,
             description: str,
             validate: t.Union[str, Validate],
             private: t.Optional[bool] = None,
             required: bool = False):
         #: a short description of the key parameter
         self.description: str = description
-        if isinstance(validate, str):
-            validate: Validate = _value_validators[validate]
         #: a function for validating the key parameter's value
-        self.validate: Validate = validate
+        self.validate = _value_validators[validate] if isinstance(validate, str) else validate
         #: if this key parameter for private key only
         self.private = private
         #: if this key parameter is required
         self.required = required
 
 
+class KeyOperation:
+    def __init__(self, description: str, use: str, private: t.Optional[bool]):
+        self.description = description
+        self.use = use
+        self.private = private
+
+
 #: Define parameters for JWK
 KeyParameterRegistryDict = t.Dict[str, KeyParameter]
-KeyOperation = namedtuple("KeyOperation", ["description", "use", "private"])
 KeyOperationRegistryDict = t.Dict[str, KeyOperation]
 
 #: Basic JWS header registry
 JWS_HEADER_REGISTRY: HeaderRegistryDict = {
     "alg": HeaderParameter("Algorithm", is_str, True),
     "jku": HeaderParameter("JWK Set URL", is_url),
     "jwk": HeaderParameter("JSON Web Key", is_jwk),
@@ -178,16 +177,15 @@
         raise ValueError(f'Unsupported {unsupported_keys} in header')
 
 
 def validate_registry_header(
         registry: HeaderRegistryDict,
         header: Header,
         check_required: bool = True):
-    for key in registry:
-        reg: HeaderParameter = registry[key]
+    for key, reg in registry.items():
         if check_required and reg.required and key not in header:
             raise ValueError(f'Required "{key}" is missing in header')
         if key in header:
             try:
                 reg.validate(header[key])
             except ValueError as error:
                 raise ValueError(f'"{key}" in header {error}')
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7515/compact.py` & `joserfc-0.6.0/src/joserfc/rfc7515/compact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import binascii
+import typing as t
 from .model import JWSAlgModel, CompactSignature
 from ..errors import DecodeError, MissingAlgorithmError
 from ..util import (
     json_b64encode,
     json_b64decode,
     urlsafe_b64encode,
     urlsafe_b64decode,
@@ -53,15 +54,15 @@
 def detach_compact_content(value: str) -> str:
     # https://www.rfc-editor.org/rfc/rfc7515#appendix-F
     parts = value.split(".")
     parts[1] = ""
     return ".".join(parts)
 
 
-def decode_header(header_segment: bytes):
+def decode_header(header_segment: bytes) -> t.Dict[str, t.Any]:
     try:
         protected = json_b64decode(header_segment)
         if "alg" not in protected:
             raise MissingAlgorithmError()
     except (TypeError, ValueError, binascii.Error):
         raise DecodeError("Invalid header")
     return protected
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7515/json.py` & `joserfc-0.6.0/src/joserfc/rfc7515/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,169 +1,173 @@
 import typing as t
 import binascii
-from .model import JWSAlgModel, HeaderMember, JSONSignature
+import copy
+from .model import (
+    HeaderMember,
+    GeneralJSONSignature,
+    FlattenedJSONSignature,
+)
 from .types import (
     HeaderDict,
     JSONSignatureDict,
-    JSONSerialization,
     GeneralJSONSerialization,
     FlattenedJSONSerialization,
 )
 from .registry import JWSRegistry
 from ..util import (
-    to_bytes,
     json_b64encode,
     json_b64decode,
     urlsafe_b64encode,
     urlsafe_b64decode,
 )
 from ..errors import DecodeError
+from ..rfc7517.models import BaseKey
 
 
-def construct_json_signature(
-        members: t.Union[HeaderDict, t.List[HeaderDict]],
-        payload: t.AnyStr,
-        registry: JWSRegistry) -> JSONSignature:
-    if isinstance(members, dict):
-        flattened = True
-        __check_member(registry, members)
-        members = [members]
-    else:
-        flattened = False
-        for member in members:
-            __check_member(registry, member)
-
-    members = [HeaderMember(**member) for member in members]
-    payload = to_bytes(payload)
-    obj = JSONSignature(members, payload)
-    obj.flattened = flattened
-    return obj
-
-
-def __check_member(registry: JWSRegistry, member: HeaderDict):
-    header = {}
-    if "protected" in member:
-        header.update(member["protected"])
-    if "header" in member:
-        header.update(member["header"])
-    registry.check_header(header)
-
+FindKey = t.Callable[[HeaderMember], BaseKey]
 
-def sign_json(obj: JSONSignature, registry: JWSRegistry, find_key) -> JSONSerialization:
-    signatures: t.List[JSONSignatureDict] = []
 
-    payload_segment = obj.segments["payload"]
-    for member in obj.members:
-        headers = member.headers()
-        registry.check_header(headers)
-        alg = registry.get_alg(headers["alg"])
-        key = find_key(member)
-        key.check_use("sig")
-        signature = __sign_member(payload_segment, member, alg, key)
-        signatures.append(signature)
-
-    rv = {"payload": payload_segment.decode("utf-8")}
-    if obj.flattened and len(signatures) == 1:
-        rv.update(dict(signatures[0]))
-    else:
-        rv["signatures"] = signatures
-
-    obj.signatures = signatures
-    return rv
-
-
-def __sign_member(payload_segment, member: HeaderMember, alg: JWSAlgModel, key) -> JSONSignatureDict:
+def sign_general_json(
+        members: t.List[HeaderDict],
+        payload: bytes,
+        registry: JWSRegistry,
+        find_key: FindKey) -> GeneralJSONSerialization:
+
+    payload_segment = urlsafe_b64encode(payload)
+    signatures: t.List[JSONSignatureDict] = [
+        __sign_member(payload_segment, HeaderMember(**member), registry, find_key)
+        for member in members
+    ]
+    return {
+        "payload": payload_segment.decode("utf-8"),
+        "signatures": signatures,
+    }
+
+
+def sign_flattened_json(
+        member: HeaderDict,
+        payload: bytes,
+        registry: JWSRegistry,
+        find_key: FindKey) -> FlattenedJSONSerialization:
+    payload_segment = urlsafe_b64encode(payload)
+    signature = __sign_member(payload_segment, HeaderMember(**member), registry, find_key)
+    return {"payload": payload_segment.decode("utf-8"), **signature}  # type: ignore
+
+
+def __sign_member(
+        payload_segment: bytes,
+        member: HeaderMember,
+        registry: JWSRegistry,
+        find_key: FindKey) -> JSONSignatureDict:
+    headers = member.headers()
+    registry.check_header(headers)
+    alg = registry.get_alg(headers["alg"])
+    key = find_key(member)
+    key.check_use("sig")
+    alg.check_key_type(key)
     if member.protected:
         protected_segment = json_b64encode(member.protected)
     else:
         protected_segment = b""
     signing_input = b".".join([protected_segment, payload_segment])
     signature = urlsafe_b64encode(alg.sign(signing_input, key))
     rv: JSONSignatureDict = {"signature": signature.decode("utf-8")}
     if member.protected:
         rv["protected"] = protected_segment.decode("utf-8")
     if member.header:
         rv["header"] = member.header
     return rv
 
 
-def extract_json(value: JSONSerialization) -> JSONSignature:
-    """Extract the JWS JSON Serialization from dict to object.
-
-    :param value: JWS in dict
-    """
+def extract_general_json(value: GeneralJSONSerialization) -> GeneralJSONSignature:
     payload_segment: bytes = value["payload"].encode("utf-8")
-
     try:
         payload = urlsafe_b64decode(payload_segment)
     except (TypeError, ValueError, binascii.Error):
         raise DecodeError("Invalid payload")
 
-    if "signatures" in value:
-        flattened = False
-        value: GeneralJSONSerialization
-        signatures: t.List[JSONSignatureDict] = value["signatures"]
-    else:
-        flattened = True
-        value: FlattenedJSONSerialization
-        _sig: JSONSignatureDict = {
-            "protected": value["protected"],
-            "signature": value["signature"],
-        }
-        if "header" in value:
-            _sig["header"] = value["header"]
-        signatures = [_sig]
-
-    members = []
-    for sig in signatures:
-        member = HeaderMember()
-        if "protected" in sig:
-            protected_segment = sig["protected"]
-            member.protected = json_b64decode(protected_segment)
-        if "header" in sig:
-            member.header = sig["header"]
-        members.append(member)
-
-    obj = JSONSignature(members, payload)
-    obj.segments.update({"payload": payload_segment})
-    obj.flattened = flattened
+    signatures: t.List[JSONSignatureDict] = value["signatures"]
+    members = [__signature_to_member(sig) for sig in signatures]
+    obj = GeneralJSONSignature(members, payload)
     obj.signatures = signatures
+    obj.segments = {"payload": payload_segment}
     return obj
 
 
-def verify_json(obj: JSONSignature, registry: JWSRegistry, find_key) -> bool:
-    """Verify the signature of this JSON serialization with the given
-    algorithm and key.
-
-    :param obj: instance of the SignatureData
-    :param find_alg: a function to return "alg" model
-    :param find_key: a function to return public key
-    """
+def extract_flattened_json(value: FlattenedJSONSerialization) -> FlattenedJSONSignature:
+    payload_segment: bytes = value["payload"].encode("utf-8")
+    try:
+        payload = urlsafe_b64decode(payload_segment)
+    except (TypeError, ValueError, binascii.Error):
+        raise DecodeError("Invalid payload")
+
+    _sig: JSONSignatureDict = {"signature": value["signature"]}
+    if "protected" in value:
+        _sig["protected"] = value["protected"]
+    if "header" in value:
+        _sig["header"] = value["header"]
+
+    member = __signature_to_member(_sig)
+    obj = FlattenedJSONSignature(member, payload)
+    obj.signature = _sig
+    obj.segments = {"payload": payload_segment}
+    return obj
+
+
+def __signature_to_member(sig: JSONSignatureDict) -> HeaderMember:
+    member = HeaderMember()
+    if "protected" in sig:
+        protected_segment = sig["protected"]
+        member.protected = json_b64decode(protected_segment)
+    if "header" in sig:
+        member.header = sig["header"]
+    return member
+
+
+def verify_general_json(
+        obj: GeneralJSONSignature,
+        registry: JWSRegistry,
+        find_key: FindKey) -> bool:
     payload_segment = obj.segments["payload"]
     for index, signature in enumerate(obj.signatures):
         member = obj.members[index]
-        headers = member.headers()
-        registry.check_header(headers)
-        alg = registry.get_alg(headers["alg"])
-        key = find_key(member)
-        key.check_use("sig")
-        if not _verify_signature(signature, payload_segment, alg, key):
+        if not verify_signature(member, signature, payload_segment, registry, find_key):
             return False
     return True
 
 
-def _verify_signature(signature: JSONSignatureDict, payload_segment, alg: JWSAlgModel, key) -> bool:
+def verify_flattened_json(
+        obj: FlattenedJSONSignature,
+        registry: JWSRegistry,
+        find_key: FindKey) -> bool:
+    payload_segment = obj.segments["payload"]
+    assert obj.signature is not None
+    return verify_signature(obj.member, obj.signature, payload_segment, registry, find_key)
+
+
+def verify_signature(
+        member: HeaderMember,
+        signature: JSONSignatureDict,
+        payload_segment: bytes,
+        registry: JWSRegistry,
+        find_key: FindKey) -> bool:
+    headers = member.headers()
+    registry.check_header(headers)
+    alg = registry.get_alg(headers["alg"])
+    key = find_key(member)
+    key.check_use("sig")
+    alg.check_key_type(key)
     if "protected" in signature:
         protected_segment = signature["protected"].encode("utf-8")
     else:
         protected_segment = b""
     sig = urlsafe_b64decode(signature["signature"].encode("utf-8"))
     signing_input = b".".join([protected_segment, payload_segment])
     return alg.verify(signing_input, sig, key)
 
 
-def detach_json_content(value: JSONSerialization) -> JSONSerialization:
+def detach_json_content(value: t.Dict[str, t.Any]) -> t.Dict[str, t.Any]:
     # https://www.rfc-editor.org/rfc/rfc7515#appendix-F
-    rv = value.copy()  # don't alter original value
+    rv = copy.deepcopy(value)  # don't alter original value
     if "payload" in rv:
         del rv["payload"]
     return rv
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7515/model.py` & `joserfc-0.6.0/src/joserfc/rfc7515/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import typing as t
 from abc import ABCMeta, abstractmethod
 from .types import SegmentsDict, JSONSignatureDict
+from ..errors import InvalidKeyTypeError
 from ..registry import Header
+from ..rfc7517.models import BaseKey
 
 
 class HeaderMember:
+    """A header member of the JSON signature. It is combined with protected header,
+    and unprotected header.
+    """
     def __init__(self, protected: t.Optional[Header] = None, header: t.Optional[Header] = None):
+        #: protected header
         self.protected = protected
+        #: unprotected header
         self.header = header
 
     def headers(self) -> Header:
         rv: Header = {}
         if self.protected:
             rv.update(self.protected)
         if self.header:
@@ -35,55 +42,78 @@
     def headers(self) -> Header:
         return self.protected
 
     def set_kid(self, kid: str):
         self.protected["kid"] = kid
 
 
-class JSONSignature:
-    """JSON Web Signature object for JSON mode. This object is used to
-    represent the JWS instance.
-    """
+class FlattenedJSONSignature:
+    """"JSON Signature object that represents a flattened JSON serialization."""
+
+    #: mark it as flattened
+    flattened: t.ClassVar[bool] = True
+
+    def __init__(self, member: HeaderMember, payload: bytes):
+        #: the only header member
+        self.member = member
+        #: payload content
+        self.payload = payload
+        self.signature: t.Optional[JSONSignatureDict] = None
+        self.segments: SegmentsDict = {}
+
+    @property
+    def members(self) -> t.List[HeaderMember]:
+        return [self.member]
+
+    def headers(self) -> Header:
+        return self.member.headers()
+
+
+class GeneralJSONSignature:
+    """"JSON Signature object that represents a general JSON serialization."""
+
+    #: mark it as not flattened (general)
+    flattened: t.ClassVar[bool] = False
+
     def __init__(self, members: t.List[HeaderMember], payload: bytes):
+        #: a list of header members
         self.members = members
+        #: payload content
         self.payload = payload
         self.signatures: t.List[JSONSignatureDict] = []
-        self.flattened: bool = False
         self.segments: SegmentsDict = {}
 
-    def headers(self) -> Header:
-        if self.flattened and len(self.members) == 1:
-            return self.members[0].headers()
-        raise ValueError("Only flattened JSON Serialization has .headers() method.")
-
 
 class JWSAlgModel(object, metaclass=ABCMeta):
     """Interface for JWS algorithm. JWA specification (RFC7518) SHOULD
     implement the algorithms for JWS with this base implementation.
     """
 
     name: str
     description: str
     recommended: bool = False
+    key_type = "oct"
     algorithm_type = "JWS"
     algorithm_location = "sig"
 
+    def check_key_type(self, key: BaseKey):
+        if key.key_type != self.key_type:
+            raise InvalidKeyTypeError(f'Algorithm "{self.name}" requires "{self.key_type}" key')
+
     @abstractmethod
-    def sign(self, msg: bytes, key) -> bytes:
+    def sign(self, msg: bytes, key: t.Any) -> bytes:
         """Sign the text msg with a private/sign key.
 
         :param msg: message bytes to be signed
         :param key: private key to sign the message
         :return: bytes
         """
-        pass
 
     @abstractmethod
-    def verify(self, msg: bytes, sig: bytes, key) -> bool:
+    def verify(self, msg: bytes, sig: bytes, key: t.Any) -> bool:
         """Verify the signature of text msg with a public/verify key.
 
         :param msg: message bytes to be signed
         :param sig: result signature to be compared
         :param key: public key to verify the signature
         :return: boolean
         """
-        pass
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7515/registry.py` & `joserfc-0.6.0/src/joserfc/rfc7515/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     HeaderRegistryDict,
     validate_registry_header,
     check_crit_header,
     check_supported_header,
 )
 
 
-class JWSRegistry(object):
+class JWSRegistry:
     """A registry for JSON Web Signature to keep all the supported algorithms.
     An instance of ``JWSRegistry`` is usually used together with methods in
     ``joserfc.jws``.
 
     :param header_registry: extra header parameters registry
     :param algorithms: allowed algorithms to be used
     :param strict_check_header: only allow header key in the registry to be used
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7515/types.py` & `joserfc-0.6.0/src/joserfc/rfc7515/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,42 +3,39 @@
 
 __all__ = [
     "SegmentsDict",
     "HeaderDict",
     "JSONSignatureDict",
     "GeneralJSONSerialization",
     "FlattenedJSONSerialization",
-    "JSONSerialization",
 ]
 
-SegmentsDict = t.TypedDict("SegmentsDict", {
-    "header": bytes,
-    "payload": bytes,
-    "signature": bytes,
-}, total=False)
-
-HeaderDict = t.TypedDict("HeaderDict", {
-    "protected": Header,
-    "header": Header,
-}, total=False)
-
-
-JSONSignatureDict = t.TypedDict("JSONSignatureDict", {
-    "protected": str,
-    "header": Header,
-    "signature": str,
-}, total=False)
-
-
-GeneralJSONSerialization = t.TypedDict("GeneralJSONSerialization", {
-    "payload": str,
-    "signatures": t.List[JSONSignatureDict],
-})
-
-FlattenedJSONSerialization = t.TypedDict("FlattenedJSONSerialization", {
-    "payload": str,
-    "protected": str,
-    "header": Header,
-    "signature": str,
-}, total=False)
 
-JSONSerialization = t.Union[GeneralJSONSerialization, FlattenedJSONSerialization]
+class SegmentsDict(t.TypedDict, total=False):
+    header: bytes
+    payload: bytes
+    signature: bytes
+
+
+class HeaderDict(t.TypedDict, total=False):
+    protected: Header
+    header: Header
+
+
+class JSONSignatureDict(t.TypedDict, total=False):
+    protected: str
+    header: Header
+    signature: str
+
+
+@t.final
+class GeneralJSONSerialization(t.TypedDict):
+    payload: str
+    signatures: t.List[JSONSignatureDict]
+
+
+@t.final
+class FlattenedJSONSerialization(t.TypedDict, total=False):
+    payload: str
+    protected: str
+    header: Header
+    signature: str
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7516/compact.py` & `joserfc-0.6.0/src/joserfc/rfc7516/compact.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,17 +9,20 @@
     json_b64decode,
     urlsafe_b64encode,
     urlsafe_b64decode,
 )
 
 
 def represent_compact(obj: CompactEncryption) -> bytes:
+    assert obj.recipient is not None
+    encrypted_key = obj.recipient.encrypted_key
+    assert encrypted_key is not None
     return b".".join([
         obj.base64_segments["aad"],
-        urlsafe_b64encode(obj.recipient.encrypted_key),
+        urlsafe_b64encode(encrypted_key),
         obj.base64_segments["iv"],
         obj.base64_segments["ciphertext"],
         obj.base64_segments["tag"],
     ])
 
 
 def extract_compact(value: bytes) -> CompactEncryption:
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7516/json.py` & `joserfc-0.6.0/src/joserfc/rfc7516/json.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,109 @@
-from .models import JSONEncryption, Recipient
-from .types import JSONSerialization
+import typing as t
+from .models import (
+    BaseJSONEncryption,
+    GeneralJSONEncryption,
+    FlattenedJSONEncryption,
+    Recipient,
+)
+from .types import (
+    JSONRecipientDict,
+    GeneralJSONSerialization,
+    FlattenedJSONSerialization,
+)
+from ..registry import Header
 from ..util import (
     to_bytes,
-    to_unicode,
+    to_str,
     json_b64encode,
     json_b64decode,
     urlsafe_b64encode,
     urlsafe_b64decode,
 )
 
 
-def represent_json(obj: JSONEncryption) -> JSONSerialization:
-    data: JSONSerialization = {
-        "protected": to_unicode(json_b64encode(obj.protected)),
-        "iv": to_unicode(obj.base64_segments["iv"]),
-        "ciphertext": to_unicode(obj.base64_segments["ciphertext"]),
-        "tag": to_unicode(obj.base64_segments["tag"]),
-    }
-    if obj.aad:
-        data["aad"] = to_unicode(urlsafe_b64encode(obj.aad))
-
-    if obj.unprotected:
-        data["unprotected"] = obj.unprotected
-
+def represent_general_json(obj: GeneralJSONEncryption) -> GeneralJSONSerialization:
+    data = __represent_json_serialization(obj)
     recipients = []
     for recipient in obj.recipients:
-        item = {}
+        item: JSONRecipientDict = {}
         if recipient.header:
             item["header"] = recipient.header
         if recipient.encrypted_key:
-            item["encrypted_key"] = to_unicode(urlsafe_b64encode(recipient.encrypted_key))
-        if data:
-            recipients.append(item)
+            item["encrypted_key"] = to_str(urlsafe_b64encode(recipient.encrypted_key))
+        recipients.append(item)
+    data["recipients"] = recipients
+    return data  # type: ignore
+
+
+def represent_flattened_json(obj: FlattenedJSONEncryption) -> FlattenedJSONSerialization:
+    data = __represent_json_serialization(obj)
+    recipient = obj.recipients[0]
+    assert recipient is not None
+    if recipient.header:
+        data["header"] = recipient.header
+    if recipient.encrypted_key:
+        data["encrypted_key"] = to_str(urlsafe_b64encode(recipient.encrypted_key))
+    return data  # type: ignore
+
+
+def __represent_json_serialization(obj: BaseJSONEncryption):
+    data: t.Dict[str, t.Union[str, Header]] = {
+        "protected": to_str(json_b64encode(obj.protected)),
+        "iv": to_str(obj.base64_segments["iv"]),
+        "ciphertext": to_str(obj.base64_segments["ciphertext"]),
+        "tag": to_str(obj.base64_segments["tag"]),
+    }
+    if obj.aad:
+        data["aad"] = to_str(urlsafe_b64encode(obj.aad))
 
-    if obj.flattened and len(recipients) == 1:
-        data.update(recipients[0])
-    else:
-        data["recipients"] = recipients
+    if obj.unprotected:
+        data["unprotected"] = obj.unprotected
     return data
 
 
-def extract_json(data: JSONSerialization) -> JSONEncryption:
+def extract_general_json(data: GeneralJSONSerialization) -> GeneralJSONEncryption:
     protected = json_b64decode(data["protected"])
     unprotected = data.get("unprotected")
-    obj = JSONEncryption(protected, None, unprotected)
-    obj.base64_segments["iv"] = to_bytes(data["iv"])
-    obj.base64_segments["ciphertext"] = to_bytes(data["ciphertext"])
-    obj.base64_segments["tag"] = to_bytes(data["tag"])
-
-    # save decoded segments
-    obj.bytes_segments["iv"] = urlsafe_b64decode(obj.base64_segments["iv"])
-    obj.bytes_segments["ciphertext"] = urlsafe_b64decode(obj.base64_segments["ciphertext"])
-    obj.bytes_segments["tag"] = urlsafe_b64decode(obj.base64_segments["tag"])
+    base64_segments, bytes_segments, aad = __extract_segments(data)
+    obj = GeneralJSONEncryption(protected, None, unprotected, aad)
+    obj.base64_segments = base64_segments
+    obj.bytes_segments = bytes_segments
+    for item in data["recipients"]:
+        recipient = Recipient(obj, item.get("header"))
+        if "encrypted_key" in item:
+            recipient.encrypted_key = urlsafe_b64decode(to_bytes(item["encrypted_key"]))
+        obj.recipients.append(recipient)
+    return obj
 
-    if "aad" in data:
-        obj.aad = urlsafe_b64decode(to_bytes(data["aad"]))
 
-    if "recipients" in data:
-        obj.flattened = False
-        for item in data["recipients"]:
-            recipient = Recipient(obj, item.get("header"))
-            if "encrypted_key" in item:
-                recipient.encrypted_key = urlsafe_b64decode(to_bytes(item["encrypted_key"]))
-            obj.recipients.append(recipient)
-    else:
-        obj.flattened = True
-        recipient = Recipient(obj, data.get("header"))
-        if "encrypted_key" in data:
-            recipient.encrypted_key = urlsafe_b64decode(to_bytes(data["encrypted_key"]))
-        obj.recipients.append(recipient)
+def extract_flattened_json(data: FlattenedJSONSerialization) -> FlattenedJSONEncryption:
+    protected = json_b64decode(data["protected"])
+    unprotected = data.get("unprotected")
+    base64_segments, bytes_segments, aad = __extract_segments(data)
+    obj = FlattenedJSONEncryption(protected, None, unprotected, aad)
+    obj.base64_segments = base64_segments
+    obj.bytes_segments = bytes_segments
+
+    recipient = Recipient(obj, data.get("header"))
+    if "encrypted_key" in data:
+        recipient.encrypted_key = urlsafe_b64decode(to_bytes(data["encrypted_key"]))
+    obj.recipients.append(recipient)
     return obj
+
+
+def __extract_segments(data: t.Union[GeneralJSONSerialization, FlattenedJSONSerialization]):
+    base64_segments: t.Dict[str, bytes] = {
+        "iv": to_bytes(data["iv"]),
+        "ciphertext": to_bytes(data["ciphertext"]),
+        "tag": to_bytes(data["tag"]),
+    }
+    bytes_segments: t.Dict[str, bytes] = {
+        "iv": urlsafe_b64decode(base64_segments["iv"]),
+        "ciphertext": urlsafe_b64decode(base64_segments["ciphertext"]),
+        "tag": urlsafe_b64decode(base64_segments["tag"]),
+    }
+    if "aad" in data:
+        aad = urlsafe_b64decode(to_bytes(data["aad"]))
+    else:
+        aad = None
+    return base64_segments, bytes_segments, aad
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7516/message.py` & `joserfc-0.6.0/src/joserfc/rfc7516/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 import typing as t
 from .models import (
     CompactEncryption,
-    JSONEncryption,
+    BaseJSONEncryption,
+    GeneralJSONEncryption,
+    FlattenedJSONEncryption,
     Recipient,
     JWEAlgModel,
     JWEEncModel,
+    JWEKeyAgreement,
+    JWEDirectEncryption,
+    JWEKeyEncryption,
+    JWEKeyWrapping,
 )
 from .registry import JWERegistry
 from ..errors import (
     DecodeError,
     InvalidCEKLengthError,
     InvalidEncryptedKeyError,
     ConflictAlgorithmError,
 )
 from ..util import (
     json_b64encode,
     urlsafe_b64encode,
 )
 
-EncryptionData = t.Union[CompactEncryption, JSONEncryption]
+EncryptionData = t.Union[CompactEncryption, GeneralJSONEncryption, FlattenedJSONEncryption]
 
 
-def perform_encrypt(obj: EncryptionData, registry: JWERegistry) -> EncryptionData:
+def perform_encrypt(obj: EncryptionData, registry: JWERegistry):
     enc = registry.get_enc(obj.protected["enc"])
     cek, delayed_tasks = pre_encrypt_recipients(enc, obj.recipients, registry)
 
     # Step 9, Generate a random JWE Initialization Vector of the correct size
     # for the content encryption algorithm (if required for the algorithm);
     # otherwise, let the JWE Initialization Vector be the empty octet sequence.
     iv = enc.generate_iv()
@@ -34,44 +40,44 @@
     # BASE64URL(JWE Initialization Vector).
     obj.base64_segments["iv"] = urlsafe_b64encode(iv)
 
     # Step 11, If a "zip" parameter was included, compress the plaintext using
     # the specified compression algorithm and let M be the octet sequence
     # representing the compressed plaintext; otherwise, let M be the octet
     # sequence representing the plaintext.
+    assert obj.plaintext is not None
     if "zip" in obj.protected:
         zip_ = registry.get_zip(obj.protected["zip"])
-        plaintext = zip_.compress(obj.plaintext)
+        plaintext: bytes = zip_.compress(obj.plaintext)  # type: ignore
     else:
-        plaintext = obj.plaintext
+        plaintext: bytes = obj.plaintext  # type: ignore
 
     # Step 13, Compute the Encoded Protected Header value BASE64URL(UTF8(JWE Protected Header)).
     aad = json_b64encode(obj.protected, "ascii")
 
     # Step 14, Let the Additional Authenticated Data encryption parameter be
     # ASCII(Encoded Protected Header).  However, if a JWE AAD value is
     # present (which can only be the case when using the JWE JSON Serialization),
     # instead let the Additional Authenticated Data encryption parameter be
     # ASCII(Encoded Protected Header || '.' || BASE64URL(JWE AAD)).
-    if isinstance(obj, JSONEncryption) and obj.aad:
+    if isinstance(obj, BaseJSONEncryption) and obj.aad:
         aad = aad + b"." + urlsafe_b64encode(obj.aad)
     obj.base64_segments["aad"] = aad
 
     # encrypting plaintext
     ciphertext, tag = enc.encrypt(plaintext, cek, iv, aad)
 
     # delay encrypting every recipient
     post_encrypt_recipients(enc, delayed_tasks, cek, tag)
 
     obj.base64_segments["ciphertext"] = urlsafe_b64encode(ciphertext)
     obj.base64_segments["tag"] = urlsafe_b64encode(tag)
-    return obj
 
 
-def perform_decrypt(obj: EncryptionData, registry: JWERegistry) -> EncryptionData:
+def perform_decrypt(obj: EncryptionData, registry: JWERegistry):
     enc = registry.get_enc(obj.protected["enc"])
 
     iv = obj.bytes_segments["iv"]
     enc.check_iv(iv)
 
     tag = obj.bytes_segments["tag"]
     ciphertext = obj.bytes_segments["ciphertext"]
@@ -90,121 +96,128 @@
         raise DecodeError('Multiple "cek" found')
 
     cek = cek_set.pop()
     if len(cek) * 8 != enc.cek_size:
         raise InvalidCEKLengthError(f"A key of size {enc.cek_size} bits MUST be used")
 
     aad = json_b64encode(obj.protected, "ascii")
-    if isinstance(obj, JSONEncryption) and obj.aad:
+    if isinstance(obj, BaseJSONEncryption) and obj.aad:
         aad = aad + b"." + urlsafe_b64encode(obj.aad)
 
     msg = enc.decrypt(ciphertext, tag, cek, iv, aad)
     if "zip" in obj.protected:
         zip_ = registry.get_zip(obj.protected["zip"])
         obj.plaintext = zip_.decompress(msg)
     else:
         obj.plaintext = msg
-    return obj
 
 
 def pre_encrypt_recipients(enc: JWEEncModel, recipients: t.List[Recipient], registry: JWERegistry):
-    cek = b""
-    delayed_tasks = []
+    cek: bytes = b""
+    delayed_tasks: t.List[t.Tuple[JWEKeyAgreement, Recipient]] = []
     for recipient in recipients:
         # https://www.rfc-editor.org/rfc/rfc7516#section-5
         headers = recipient.headers()
         registry.check_header(headers)
         # 1. Determine the Key Management Mode employed by the algorithm used
         # to determine the Content Encryption Key value.  (This is the
         # algorithm recorded in the "alg" (algorithm) Header Parameter of
         # the resulting JWE.)
         alg = registry.get_alg(headers["alg"])
 
-        if alg.key_agreement:
+        if isinstance(alg, JWEKeyAgreement):
             alg.prepare_ephemeral_key(recipient)
 
         if alg.direct_mode:
             if len(recipients) > 1:
                 raise ConflictAlgorithmError(f"Algorithm {alg.name} SHOULD have 1 recipient only")
 
-            if alg.key_agreement:
+            if isinstance(alg, JWEKeyAgreement):
                 # 3. When Direct Key Agreement is employed,
                 # let the CEK be the agreed upon key.
-                cek: bytes = alg.encrypt_agreed_upon_key(enc, recipient)
+                cek = alg.encrypt_agreed_upon_key(enc, recipient)
                 if len(cek) * 8 != enc.cek_size:
                     raise InvalidCEKLengthError(f"A key of size {enc.cek_size} bits MUST be used")
             else:
                 # 6. When Direct Encryption is employed, let the CEK be the shared
                 # symmetric key.
-                cek: bytes = alg.compute_cek(enc.cek_size, recipient)
+                assert isinstance(alg, JWEDirectEncryption)
+                cek = alg.compute_cek(enc.cek_size, recipient)
 
             # 5. When Direct Key Agreement or Direct Encryption are employed, let
             # the JWE Encrypted Key be the empty octet sequence.
             recipient.encrypted_key = b""
         else:
             if not cek:
                 # 2. When Key Wrapping, Key Encryption, or Key Agreement with Key
                 # Wrapping are employed, generate a random CEK value.  See RFC
                 # 4086 [RFC4086] for considerations on generating random values.
                 # The CEK MUST have a length equal to that required for the
                 # content encryption algorithm.
                 cek = enc.generate_cek()
 
-            if alg.key_agreement:
+            if isinstance(alg, JWEKeyAgreement):
                 delayed_tasks.append((alg, recipient))
             else:
                 # 4. When Key Wrapping, or Key Encryption are employed, encrypt the CEK
                 # to the recipient and let the result be the JWE Encrypted Key.
+                assert isinstance(alg, (JWEKeyWrapping, JWEKeyEncryption))
                 recipient.encrypted_key = alg.encrypt_cek(cek, recipient)
     return cek, delayed_tasks
 
 
 def post_encrypt_recipients(
         enc: JWEEncModel,
-        tasks: t.List[t.Tuple[JWEAlgModel, Recipient]],
+        tasks: t.List[t.Tuple[JWEKeyAgreement, Recipient]],
         cek: bytes,
         tag: bytes):
     for alg, recipient in tasks:
         if alg.tag_aware:
             agreed_upon_key = alg.encrypt_agreed_upon_key_with_tag(enc, recipient, tag)
         else:
             agreed_upon_key = alg.encrypt_agreed_upon_key(enc, recipient)
         # 4. When Key Agreement with Key Wrapping is employed, encrypt the CEK
         # to the recipient and let the result be the JWE Encrypted Key.
         recipient.encrypted_key = alg.wrap_cek_with_auk(cek, agreed_upon_key)
 
 
 def decrypt_recipient(alg: JWEAlgModel, enc: JWEEncModel, recipient: Recipient, tag: bytes):
+    cek: bytes
     if alg.direct_mode:
         # 10.  When Direct Key Agreement or Direct Encryption are employed,
         # verify that the JWE Encrypted Key value is an empty octet
         # sequence.
         if recipient.encrypted_key:
             raise InvalidEncryptedKeyError()
-        if alg.key_agreement:
+
+        if isinstance(alg, JWEKeyAgreement):
             # 8. When Direct Key Agreement is employed, let the CEK be the agreed upon key.
             cek = alg.decrypt_agreed_upon_key(enc, recipient)
         else:
             # 11. When Direct Encryption is employed, let the CEK be the shared
             # symmetric key.
+            assert isinstance(alg, JWEDirectEncryption)
             cek = alg.compute_cek(enc.cek_size, recipient)
-    elif alg.key_agreement:
+    elif isinstance(alg, JWEKeyAgreement):
+        agreed_upon_key: bytes
         if alg.tag_aware:
             agreed_upon_key = alg.decrypt_agreed_upon_key_with_tag(enc, recipient, tag)
         else:
             agreed_upon_key = alg.decrypt_agreed_upon_key(enc, recipient)
 
         # 8. When Key Agreement with Key Wrapping is employed, the agreed upon key
         # will be used to decrypt the JWE Encrypted Key.
+        assert recipient.encrypted_key is not None
         cek = alg.unwrap_cek_with_auk(recipient.encrypted_key, agreed_upon_key)
     else:
         # 9. When Key Wrapping, Key Encryption, or Key Agreement with Key
         # Wrapping are employed, decrypt the JWE Encrypted Key to produce
         # the CEK.  The CEK MUST have a length equal to that required for
         # the content encryption algorithm.  Note that when there are
         # multiple recipients, each recipient will only be able to decrypt
         # JWE Encrypted Key values that were encrypted to a key in that
         # recipient's possession.  It is therefore normal to only be able
         # to decrypt one of the per-recipient JWE Encrypted Key values to
         # obtain the CEK value.
+        assert isinstance(alg, (JWEKeyWrapping, JWEKeyEncryption))
         cek = alg.decrypt_cek(recipient)
     return cek
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7516/models.py` & `joserfc-0.6.0/src/joserfc/rfc7516/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import os
 import typing as t
 from abc import ABCMeta, abstractmethod
-from ..rfc7517.models import Key, CurveKey
-from ..rfc7518.oct_key import OctKey
+from ..rfc7517.models import BaseKey, CurveKey
 from ..registry import Header, HeaderRegistryDict
 from ..errors import InvalidKeyTypeError, InvalidKeyLengthError
 
 
 class Recipient:
     def __init__(
             self,
-            parent: t.Union["CompactEncryption", "JSONEncryption"],
+            parent: t.Union["CompactEncryption", "GeneralJSONEncryption", "FlattenedJSONEncryption"],
             header: t.Optional[Header] = None,
-            recipient_key: t.Optional[Key] = None):
+            recipient_key: t.Optional[BaseKey] = None):
         self.__parent = parent
         self.header = header
         self.recipient_key = recipient_key
-        self.sender_key: t.Optional[Key] = None
+        self.sender_key: t.Optional[BaseKey] = None
         self.encrypted_key: t.Optional[bytes] = None
         self.ephemeral_key: t.Optional[CurveKey] = None
-        self.segments = {}  # store temporary segments
 
     def headers(self) -> Header:
-        rv = {}
+        rv: Header = {}
         rv.update(self.__parent.protected)
-        if isinstance(self.__parent, JSONEncryption) and self.__parent.unprotected:
+        if isinstance(self.__parent, BaseJSONEncryption) and self.__parent.unprotected:
             rv.update(self.__parent.unprotected)
         if self.header:
             rv.update(self.header)
         return rv
 
     def add_header(self, k: str, v: t.Any):
         if isinstance(self.__parent, CompactEncryption):
@@ -54,85 +52,118 @@
         self.recipient: t.Optional[Recipient] = None
         self.bytes_segments: t.Dict[str, bytes] = {}  # store the decoded segments
         self.base64_segments: t.Dict[str, bytes] = {}  # store the encoded segments
 
     def headers(self):
         return self.protected
 
-    def attach_recipient(self, key: Key, header: t.Optional[Header] = None):
+    def attach_recipient(self, key: BaseKey, header: t.Optional[Header] = None):
         """Add a recipient to the JWE Compact Serialization. Please add a key that
         comply with the given "alg" value.
 
         :param key: an instance of a key, e.g. (OctKey, RSAKey, ECKey, and etc)
         :param header: extra header in dict
         """
         recipient = Recipient(self, None, key)
         if header:
             self.protected.update(header)
         self.recipient = recipient
 
     @property
     def recipients(self) -> t.List[Recipient]:
-        return [self.recipient]
+        if self.recipient is not None:
+            return [self.recipient]
+        return []
+
+
+class BaseJSONEncryption(metaclass=ABCMeta):
+    #: represents if the object is in flatten syntax
+    flattened: t.ClassVar[bool]
+    #: protected header in dict
+    protected: Header
+    #: the plaintext in bytes
+    plaintext: t.Optional[bytes]
+    #: unprotected header in dict
+    unprotected: t.Optional[Header]
+    #: an optional additional authenticated data
+    aad: t.Optional[bytes]
+    #: a list of recipients
+    recipients: t.List[Recipient]
 
-
-class JSONEncryption:
-    """An object to represent the JWE JSON Serialization. It is used by
-    ``encrypt_json``, and it is usually returned by ``decrypt_json`` method.
-
-    To construct an object of ``JSONEncryption``:
-
-    .. code-block:: python
-
-        protected = {"enc": "A128CBC-HS256"}
-        plaintext = b"hello world"
-        obj = JSONEncryption(protected, plaintext)
-        # then add each recipient
-        obj.add_recipient({"alg": "A128KW"})
-    """
     def __init__(
             self,
             protected: Header,
             plaintext: t.Optional[bytes] = None,
             unprotected: t.Optional[Header] = None,
-            aad: t.Optional[bytes] = None,
-            flattened: bool = False):
-        #: protected header in dict
-        self.protected: Header = protected
-        #: the plaintext in bytes
-        self.plaintext: bytes = plaintext
-        #: unprotected header in dict
-        self.unprotected: t.Optional[Header] = unprotected
-        #: an optional additional authenticated data
-        self.aad: t.Optional[bytes] = aad
-        #: represents if the object is in flatten syntax
-        self.flattened: bool = flattened
-        #: a list of recipients
-        self.recipients: t.List[Recipient] = []
-
+            aad: t.Optional[bytes] = None):
+        self.protected = protected
+        self.plaintext = plaintext
+        self.unprotected = unprotected
+        self.aad = aad
+        self.recipients = []
         self.bytes_segments: t.Dict[str, bytes] = {}  # store the decoded segments
         self.base64_segments: t.Dict[str, bytes] = {}  # store the encoded segments
 
-    def add_recipient(self, header: t.Optional[Header] = None, key: t.Optional[Key] = None):
+    @abstractmethod
+    def add_recipient(self, header: t.Optional[Header] = None, key: t.Optional[BaseKey] = None):
         """Add a recipient to the JWE JSON Serialization. Please add a key that
         comply with the "alg" to this recipient.
 
         :param header: recipient's own (unprotected) header
         :param key: an instance of a key, e.g. (OctKey, RSAKey, ECKey, and etc)
         """
+
+
+class GeneralJSONEncryption(BaseJSONEncryption):
+    """An object to represent the JWE General JSON Serialization. It is used by
+    ``encrypt_json``, and it is usually returned by ``decrypt_json`` method.
+
+    To construct an object of ``GeneralJSONEncryption``:
+
+    .. code-block:: python
+
+        protected = {"enc": "A128CBC-HS256"}
+        plaintext = b"hello world"
+        obj = GeneralJSONEncryption(protected, plaintext)
+        # then add each recipient
+        obj.add_recipient({"alg": "A128KW"})
+    """
+    flattened = False
+
+    def add_recipient(self, header: t.Optional[Header] = None, key: t.Optional[BaseKey] = None):
         recipient = Recipient(self, header, key)
         self.recipients.append(recipient)
 
 
+class FlattenedJSONEncryption(BaseJSONEncryption):
+    """An object to represent the JWE Flattened JSON Serialization. It is used by
+    ``encrypt_json``, and it is usually returned by ``decrypt_json`` method.
+
+    To construct an object of ``FlattenedJSONEncryption``:
+
+    .. code-block:: python
+
+        protected = {"enc": "A128CBC-HS256"}
+        plaintext = b"hello world"
+        obj = FlattenedJSONEncryption(protected, plaintext)
+        # then add each recipient
+        obj.add_recipient({"alg": "A128KW"})
+    """
+    flattened = True
+
+    def add_recipient(self, header: t.Optional[Header] = None, key: t.Optional[BaseKey] = None):
+        self.recipients = [Recipient(self, header, key)]
+
+
 class JWEEncModel(object, metaclass=ABCMeta):
     name: str
     description: str
     recommended: bool = False
-    algorithm_type = "JWE"
-    algorithm_location = "enc"
+    algorithm_type: t.Literal["JWE"] = "JWE"
+    algorithm_location: t.Literal["enc"] = "enc"
 
     iv_size: int
     cek_size: int
 
     def generate_cek(self) -> bytes:
         return os.urandom(self.cek_size // 8)
 
@@ -153,16 +184,16 @@
         pass
 
 
 class JWEZipModel(object, metaclass=ABCMeta):
     name: str
     description: str
     recommended: bool = True
-    algorithm_type = "JWE"
-    algorithm_location = "zip"
+    algorithm_type: t.Literal["JWE"] = "JWE"
+    algorithm_location: t.Literal["zip"] = "zip"
 
     @abstractmethod
     def compress(self, s: bytes) -> bytes:
         pass
 
     @abstractmethod
     def decompress(self, s: bytes) -> bytes:
@@ -170,32 +201,34 @@
 
 
 class KeyManagement:
     name: str
     description: str
     recommended: bool = False
     key_size: t.Optional[int] = None
-    algorithm_type = "JWE"
-    algorithm_location = "alg"
+    key_types: t.List[str]
+    algorithm_type: t.Literal["JWE"] = "JWE"
+    algorithm_location: t.Literal["alg"] = "alg"
     more_header_registry: HeaderRegistryDict = {}
-    key_agreement: bool = False
 
     @property
     def direct_mode(self) -> bool:
         return self.key_size is None
 
-    @staticmethod
-    def check_recipient_key(key) -> Key:
-        raise NotImplementedError()
+    def check_key_type(self, key: BaseKey):
+        if key.key_type not in self.key_types:
+            raise InvalidKeyTypeError()
 
     def prepare_recipient_header(self, recipient: Recipient):
         raise NotImplementedError()
 
 
 class JWEDirectEncryption(KeyManagement, metaclass=ABCMeta):
+    key_types = ["oct"]
+
     @abstractmethod
     def compute_cek(self, size: int, recipient: Recipient) -> bytes:
         pass
 
 
 class JWEKeyEncryption(KeyManagement, metaclass=ABCMeta):
     @property
@@ -208,24 +241,21 @@
 
     @abstractmethod
     def decrypt_cek(self, recipient: Recipient) -> bytes:
         pass
 
 
 class JWEKeyWrapping(KeyManagement, metaclass=ABCMeta):
+    key_size: int
+    key_types = ["oct"]
+
     @property
     def direct_mode(self) -> bool:
         return False
 
-    @staticmethod
-    def check_recipient_key(key) -> OctKey:
-        if isinstance(key, OctKey):
-            return key
-        raise InvalidKeyTypeError()
-
     def check_op_key(self, op_key: bytes):
         if len(op_key) * 8 != self.key_size:
             raise InvalidKeyLengthError(f"A key of size {self.key_size} bits MUST be used")
 
     @abstractmethod
     def wrap_cek(self, cek: bytes, key: bytes) -> bytes:
         pass
@@ -240,42 +270,41 @@
 
     @abstractmethod
     def decrypt_cek(self, recipient: Recipient) -> bytes:
         pass
 
 
 class JWEKeyAgreement(KeyManagement, metaclass=ABCMeta):
-    tag_aware = False
-    key_agreement = True
-    key_wrapping: JWEKeyWrapping
-
-    @staticmethod
-    def check_recipient_key(key) -> CurveKey:
-        if isinstance(key, CurveKey):
-            return key
-        raise InvalidKeyTypeError()
+    key_types = ["EC", "OKP"]
+    tag_aware: bool = False
+    key_wrapping: t.Optional[JWEKeyWrapping]
 
     def prepare_ephemeral_key(self, recipient: Recipient):
-        recipient_key = self.check_recipient_key(recipient.recipient_key)
+        recipient_key: CurveKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(recipient_key)
         if recipient.ephemeral_key is None:
-            recipient.ephemeral_key = recipient_key.generate_key(recipient_key.curve_name, private=True)
+            ephemeral_key: CurveKey = recipient_key.generate_key(
+                recipient_key.curve_name, private=True)  # type: ignore
+            recipient.ephemeral_key = ephemeral_key
         recipient.add_header("epk", recipient.ephemeral_key.as_dict(private=False))
 
     @abstractmethod
     def encrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient) -> bytes:
         pass
 
     @abstractmethod
     def decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient) -> bytes:
         pass
 
     def wrap_cek_with_auk(self, cek: bytes, key: bytes) -> bytes:
+        assert self.key_wrapping is not None
         return self.key_wrapping.wrap_cek(cek, key)
 
     def unwrap_cek_with_auk(self, ek: bytes, key: bytes) -> bytes:
+        assert self.key_wrapping is not None
         return self.key_wrapping.unwrap_cek(ek, key)
 
     def encrypt_agreed_upon_key_with_tag(self, enc: JWEEncModel, recipient: Recipient, tag: bytes) -> bytes:
         raise NotImplementedError()
 
     def decrypt_agreed_upon_key_with_tag(self, enc: JWEEncModel, recipient: Recipient, tag: bytes) -> bytes:
         raise NotImplementedError()
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7516/registry.py` & `joserfc-0.6.0/src/joserfc/rfc7516/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,36 +12,31 @@
 JWEAlgorithm = t.Union[JWEAlgModel, JWEEncModel, JWEZipModel]
 
 AlgorithmsDict = t.TypedDict("AlgorithmsDict", {
     "alg": t.Dict[str, JWEAlgModel],
     "enc": t.Dict[str, JWEEncModel],
     "zip": t.Dict[str, JWEZipModel],
 })
-AlgorithmNamesDict = t.TypedDict("AlgorithmNamesDict", {
-    "alg": t.List[str],
-    "enc": t.List[str],
-    "zip": t.List[str],
-}, total=False)
 
 
 class JWERegistry:
     """A registry for JSON Web Encryption to keep all the supported algorithms.
     An instance of ``JWERegistry`` is usually used together with methods in
     ``joserfc.jwe``.
 
     :param header_registry: extra header parameters registry
     :param algorithms: allowed algorithms to be used
     :param strict_check_header: only allow header key in the registry to be used
     """
-    algorithms: AlgorithmsDict = {
+    algorithms: t.ClassVar[AlgorithmsDict] = {
         "alg": {},
         "enc": {},
         "zip": {},
     }
-    recommended: t.List[str] = []
+    recommended: t.ClassVar[t.List[str]] = []
 
     def __init__(
             self,
             header_registry: t.Optional[HeaderRegistryDict] = None,
             algorithms: t.Optional[t.List[str]] = None,
             strict_check_header: bool = True):
         self.header_registry: HeaderRegistryDict = {}
@@ -49,16 +44,15 @@
         if header_registry is not None:
             self.header_registry.update(header_registry)
         self.allowed = algorithms
         self.strict_check_header = strict_check_header
 
     @classmethod
     def register(cls, model: JWEAlgorithm):
-        location: t.Literal["alg", "enc", "zip"] = model.algorithm_location
-        cls.algorithms[location][model.name] = model
+        cls.algorithms[model.algorithm_location][model.name] = model  # type: ignore
         if model.recommended:
             cls.recommended.append(model.name)
 
     def check_header(self, header: Header, check_more=False):
         """Check and validate the fields in header part of a JWS object."""
         check_crit_header(header)
         validate_registry_header(self.header_registry, header)
@@ -92,15 +86,15 @@
         """Get the allowed ("zip") algorithm instance of the given name.
 
         :param name: value of the ``zip``, e.g. ``DEF``
         """
         return self._get_algorithm("zip", name)
 
     def _get_algorithm(self, location: t.Literal["alg", "enc", "zip"], name: str):
-        registry: t.Dict[str, JWEAlgorithm] = self.algorithms[location]
+        registry: t.Dict[str, JWEAlgorithm] = self.algorithms[location]  # type: ignore
         if name not in registry:
             raise ValueError(f'Algorithm of "{name}" is not supported')
 
         if self.allowed:
             allowed = self.allowed
         else:
             allowed = self.recommended
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7517/keyset.py` & `joserfc-0.6.0/src/joserfc/rfc7517/keyset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 import typing as t
-from .models import Key, SymmetricKey
-from .types import KeySetDict, KeyParameters
+import random
+from .models import BaseKey as Key, SymmetricKey
+from .types import KeyDict, KeySetDict, KeyParameters
 from .registry import JWKRegistry
 
 
 class KeySet:
+    #: keys in the key set
+    keys: t.List[Key]
+
+    registry_cls: t.ClassVar[t.Type[JWKRegistry]]
+    algorithm_keys: t.ClassVar[t.Dict[str, t.List[str]]] = {}
+
     def __init__(self, keys: t.List[Key]):
         self.keys = keys
 
-    def as_dict(self, private=None, **params):
-        keys = []
+    def __iter__(self) -> t.Iterator[Key]:
+        return iter(self.keys)
+
+    def as_dict(self, private: t.Optional[bool] = None, **params: t.Any) -> KeySetDict:
+        keys: t.List[KeyDict] = []
 
         for key in self.keys:
             # trigger key to generate kid via thumbprint
             assert key.kid is not None
             if isinstance(key, SymmetricKey):
                 keys.append(key.as_dict(**params))
             else:
@@ -25,31 +35,44 @@
             return self.keys[0]
 
         for key in self.keys:
             if key.kid == kid:
                 return key
         raise ValueError(f'No key for kid: "{kid}"')
 
+    def pick_random_key(self, algorithm: str) -> t.Optional[Key]:
+        key_types = self.algorithm_keys.get(algorithm)
+        if key_types:
+            keys = [k for k in self.keys if k.key_type in key_types]
+        else:
+            keys = self.keys
+        if keys:
+            return random.choice(keys)
+        return None
+
     @classmethod
-    def import_key_set(cls, value: KeySetDict, parameters: KeyParameters = None) -> "KeySet":
+    def import_key_set(
+            cls,
+            value: KeySetDict,
+            parameters: t.Optional[KeyParameters] = None) -> "KeySet":
         keys = []
 
         for data in value["keys"]:
-            keys.append(JWKRegistry.import_key(data, parameters=parameters))
+            keys.append(cls.registry_cls.import_key(data, parameters=parameters))
 
         return cls(keys)
 
     @classmethod
     def generate_key_set(
             cls,
             key_type: str,
             crv_or_size: t.Union[str, int],
-            parameters: KeyParameters = None,
+            parameters: t.Optional[KeyParameters] = None,
             private: bool = True,
             count: int = 4) -> "KeySet":
 
         keys = []
-        for i in range(count):
-            key = JWKRegistry.generate_key(key_type, crv_or_size, parameters, private)
+        for _ in range(count):
+            key = cls.registry_cls.generate_key(key_type, crv_or_size, parameters, private)
             keys.append(key)
 
         return cls(keys)
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7517/models.py` & `joserfc-0.6.0/src/joserfc/rfc7517/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing as t
+from typing import overload
 from abc import ABCMeta, abstractmethod
 from .types import KeyDict, KeyAny, KeyParameters
 from ..registry import (
     KeyParameterRegistryDict,
     JWK_PARAMETER_REGISTRY,
     KeyOperationRegistryDict,
     JWK_OPERATION_REGISTRY,
@@ -12,37 +13,37 @@
 from ..errors import (
     UnsupportedKeyUseError,
     UnsupportedKeyAlgorithmError,
     UnsupportedKeyOperationError,
 )
 
 
-NativePublicKey = t.TypeVar("NativePublicKey")
 NativePrivateKey = t.TypeVar("NativePrivateKey")
+NativePublicKey = t.TypeVar("NativePublicKey")
 
 
-class NativeKeyBinding(object, metaclass=ABCMeta):
-    use_key_ops_registry = {
+class NativeKeyBinding(metaclass=ABCMeta):
+    use_key_ops_registry: t.ClassVar[t.Dict[str, t.List[str]]] = {
         "sig": ["sign", "verify"],
         "enc": ["encrypt", "decrypt", "wrapKey", "unwrapKey", "deriveKey", "deriveBits"],
     }
 
     @classmethod
     @abstractmethod
-    def convert_raw_key_to_dict(cls, raw_key, private: bool) -> KeyDict:
+    def convert_raw_key_to_dict(cls, raw_key: t.Any, private: bool) -> KeyDict:
         pass
 
     @classmethod
     @abstractmethod
     def import_from_dict(cls, value: KeyDict):
         pass
 
     @classmethod
     @abstractmethod
-    def import_from_bytes(cls, value: bytes, password=None):
+    def import_from_bytes(cls, value: bytes, password: t.Optional[t.Any] = None):
         pass
 
     @staticmethod
     def as_bytes(key: "BaseKey", encoding=None, private=None, password=None) -> bytes:  # pragma: no cover
         return key.raw_value
 
     @classmethod
@@ -56,41 +57,44 @@
                     registry[k].validate(dict_key[k])
                 except ValueError as error:
                     raise ValueError(f'"{k}" {error}')
 
     @classmethod
     def validate_dict_key_use_operations(cls, dict_key: KeyDict):
         if "use" in dict_key and "key_ops" in dict_key:
-            operations = cls.use_key_ops_registry[dict_key["use"]]
+            _use: str = dict_key["use"]  # type: ignore
+            operations = cls.use_key_ops_registry[_use]
             for op in dict_key["key_ops"]:
                 if op not in operations:
                     raise ValueError('"use" and "key_ops" does not match')
 
 
-class BaseKey(t.Generic[NativePublicKey, NativePrivateKey]):
-    key_type: str
-    value_registry: KeyParameterRegistryDict
-    param_registry: KeyParameterRegistryDict = JWK_PARAMETER_REGISTRY
-    operation_registry: KeyOperationRegistryDict = JWK_OPERATION_REGISTRY
-    binding = NativeKeyBinding
+class BaseKey(t.Generic[NativePrivateKey, NativePublicKey]):
+    key_type: t.ClassVar[str]
+    binding: t.ClassVar[t.Type[NativeKeyBinding]]
+    value_registry: t.ClassVar[KeyParameterRegistryDict]
+    param_registry: t.ClassVar[KeyParameterRegistryDict] = JWK_PARAMETER_REGISTRY
+    operation_registry: t.ClassVar[KeyOperationRegistryDict] = JWK_OPERATION_REGISTRY
 
-    def __init__(self, raw_value, original_value, parameters: KeyParameters = None):
+    def __init__(
+            self,
+            raw_value: t.Union[NativePrivateKey, NativePublicKey],
+            original_value: t.Any,
+            parameters: t.Optional[KeyParameters] = None):
         self._raw_value = raw_value
         self.original_value = original_value
         self.extra_parameters = parameters
+        self._dict_value: KeyDict = {}
         if isinstance(original_value, dict):
-            data = original_value.copy()
-            data["kty"] = self.key_type
-            if parameters:
-                data.update(dict(parameters))
-
+            if parameters is not None:
+                data = {**original_value, **parameters, "kty": self.key_type}
+            else:
+                data = {**original_value, "kty": self.key_type}
             self.validate_dict_key(data)
             self._dict_value = data
-        else:
-            self._dict_value = None
 
     def keys(self):
         return self.dict_value.keys()
 
     def __getitem__(self, k: str):
         return self.dict_value[k]
 
@@ -116,16 +120,16 @@
     @property
     def dict_value(self) -> KeyDict:
         """Property of the Key in Dict (JSON)."""
         if self._dict_value:
             return self._dict_value
 
         data = self.binding.convert_raw_key_to_dict(self.raw_value, self.is_private)
-        if self.extra_parameters:
-            data.update(dict(self.extra_parameters))
+        if self.extra_parameters is not None:
+            data.update(self.extra_parameters)  # type: ignore
         data["kty"] = self.key_type
         self.validate_dict_key(data)
         self._dict_value = data
         return data
 
     @property
     def public_key(self) -> NativePublicKey:
@@ -138,17 +142,17 @@
     def thumbprint(self) -> str:
         """Call this method will generate the thumbprint with algorithm
         defined in RFC7638."""
         fields = [k for k in self.value_registry if self.value_registry[k].required]
         fields.append("kty")
         return thumbprint(self.dict_value, fields)
 
-    def as_dict(self, private: t.Optional[bool] = None, **params) -> KeyDict:
+    def as_dict(self, private: t.Optional[bool] = None, **params: t.Any) -> KeyDict:
         """Output this key to a JWK format (in dict). By default, it will return
-        the :property:`dict_value` of this key.
+        the ``dict_value`` of this key.
 
         :param private: determine whether this method should output private key or not
         :param params: other parameters added into this key
         :raise: ValueError
         """
         # check private conflicts
         if private and not self.is_private:
@@ -198,43 +202,58 @@
             raise UnsupportedKeyOperationError(f'Unsupported key_op "{operation}"')
 
         assert operation in self.operation_registry
         reg = self.operation_registry[operation]
         if reg.private and not self.is_private:
             raise UnsupportedKeyOperationError(f'Invalid key_op "{operation}" for public key')
 
+    @overload
+    def get_op_key(self, operation: t.Literal["verify", "encrypt", "wrapKey", "deriveKey"]) -> NativePublicKey: ...
+
+    @overload
+    def get_op_key(self, operation: t.Literal["sign", "decrypt", "unwrapKey"]) -> NativePrivateKey: ...
+
     def get_op_key(self, operation: str) -> t.Union[NativePublicKey, NativePrivateKey]:
         self.check_key_op(operation)
         reg = self.operation_registry[operation]
         if reg.private:
+            assert self.private_key is not None
             return self.private_key
         return self.public_key
 
     @classmethod
     def validate_dict_key(cls, data: KeyDict):
         cls.binding.validate_dict_key_registry(data, cls.param_registry)
         cls.binding.validate_dict_key_registry(data, cls.value_registry)
         cls.binding.validate_dict_key_use_operations(data)
 
     @classmethod
-    def import_key(cls, value: KeyAny, parameters: KeyParameters = None, password=None) -> "BaseKey":
+    def import_key(
+            cls,
+            value: KeyAny,
+            parameters: t.Optional[KeyParameters] = None,
+            password: t.Optional[t.Any] = None) -> "BaseKey":
         if isinstance(value, dict):
             cls.validate_dict_key(value)
             raw_key = cls.binding.import_from_dict(value)
             return cls(raw_key, value, parameters)
 
         raw_key = cls.binding.import_from_bytes(to_bytes(value), password)
         return cls(raw_key, value, parameters)
 
     @classmethod
-    def generate_key(cls, size_or_crv, parameters: KeyParameters = None, private: bool = True) -> "BaseKey":
+    def generate_key(
+            cls,
+            size_or_crv,
+            parameters: t.Optional[KeyParameters] = None,
+            private: bool = True) -> "BaseKey":
         raise NotImplementedError()
 
 
-class SymmetricKey(BaseKey[NativePublicKey, NativePrivateKey], metaclass=ABCMeta):
+class SymmetricKey(BaseKey[bytes, bytes], metaclass=ABCMeta):
     @property
     def raw_value(self) -> bytes:
         """The raw key in bytes."""
         return self._raw_value
 
     @property
     def is_private(self) -> bool:
@@ -248,15 +267,15 @@
 
     @property
     def private_key(self) -> bytes:
         """Returns the ``raw_value`` as the private key."""
         return self.raw_value
 
 
-class AsymmetricKey(BaseKey[NativePublicKey, NativePrivateKey], metaclass=ABCMeta):
+class AsymmetricKey(BaseKey[NativePrivateKey, NativePublicKey], metaclass=ABCMeta):
     @property
     def raw_value(self) -> t.Union[NativePublicKey, NativePrivateKey]:
         return self._raw_value
 
     def as_bytes(
             self,
             encoding: t.Optional[str] = None,
@@ -267,19 +286,16 @@
     def as_pem(self, private=None, password=None) -> bytes:
         return self.as_bytes(private=private, password=password)
 
     def as_der(self, private=None, password=None) -> bytes:
         return self.as_bytes(encoding="DER", private=private, password=password)
 
 
-class CurveKey(AsymmetricKey[NativePublicKey, NativePrivateKey]):
+class CurveKey(AsymmetricKey[NativePrivateKey, NativePublicKey]):
     @property
     @abstractmethod
     def curve_name(self) -> str:
         pass
 
     @abstractmethod
-    def exchange_derive_key(self, key: "CurveKey") -> bytes:
+    def exchange_derive_key(self, key) -> bytes:
         pass
-
-
-Key = t.Union[SymmetricKey, AsymmetricKey, CurveKey]
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7517/pem.py` & `joserfc-0.6.0/src/joserfc/rfc7517/pem.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,73 +6,79 @@
     load_ssh_public_key,
     load_ssh_private_key,
     load_der_private_key,
     load_der_public_key,
     Encoding,
     PrivateFormat,
     PublicFormat,
+    KeySerializationEncryption,
     BestAvailableEncryption,
     NoEncryption,
 )
 from cryptography.hazmat.backends import default_backend
-from .models import NativeKeyBinding
+from .models import NativeKeyBinding, BaseKey
 from .types import KeyDict
 from ..util import to_bytes
 
 
 def load_pem_key(raw: bytes, ssh_type: t.Optional[bytes] = None, password: t.Optional[bytes] = None):
     if ssh_type and raw.startswith(ssh_type):
-        key = load_ssh_public_key(raw, backend=default_backend())
+        key = load_ssh_public_key(raw, backend=default_backend())  # type: ignore
 
     elif b"OPENSSH PRIVATE" in raw:
-        key = load_ssh_private_key(raw, password=password, backend=default_backend())
+        key = load_ssh_private_key(raw, password=password, backend=default_backend())  # type: ignore
 
     elif b"PUBLIC" in raw:
-        key = load_pem_public_key(raw, backend=default_backend())
+        key = load_pem_public_key(raw, backend=default_backend())  # type: ignore
 
     elif b"PRIVATE" in raw:
-        key = load_pem_private_key(raw, password=password, backend=default_backend())
+        key = load_pem_private_key(raw, password=password, backend=default_backend())  # type: ignore
 
     else:
         try:
-            key = load_der_private_key(raw, password=password, backend=default_backend())
+            key = load_der_private_key(raw, password=password, backend=default_backend())  # type: ignore
         except ValueError:
-            key = load_der_public_key(raw, backend=default_backend())
+            key = load_der_public_key(raw, backend=default_backend())  # type: ignore
     return key
 
 
-def dump_pem_key(key, encoding=None, private=False, password=None) -> bytes:
+def dump_pem_key(
+        key: t.Any,
+        encoding: t.Optional[t.Literal["PEM", "DER"]] = None,
+        private: t.Optional[bool] = False,
+        password: t.Optional[t.Any] = None) -> bytes:
     """Export key into PEM/DER format bytes.
 
     :param key: native cryptography key
     :param encoding: "PEM" or "DER"
     :param private: export private key or public key
     :param password: encrypt private key with password
     :return: bytes
     """
 
     if encoding is None or encoding == "PEM":
-        encoding = Encoding.PEM
+        encoding_enum = Encoding.PEM
     elif encoding == "DER":
-        encoding = Encoding.DER
+        encoding_enum = Encoding.DER
     else:  # pragma: no cover
         raise ValueError("Invalid encoding: {!r}".format(encoding))
 
     if private:
+        encryption_algorithm: KeySerializationEncryption
         if password is None:
             encryption_algorithm = NoEncryption()
         else:
             encryption_algorithm = BestAvailableEncryption(to_bytes(password))
         return key.private_bytes(
-            encoding=encoding,
+            encoding=encoding_enum,
             format=PrivateFormat.PKCS8,
             encryption_algorithm=encryption_algorithm,
         )
     return key.public_bytes(
-        encoding=encoding,
+        encoding=encoding_enum,
         format=PublicFormat.SubjectPublicKeyInfo,
     )
 
 
 class CryptographyBinding(NativeKeyBinding, metaclass=ABCMeta):
     ssh_type: bytes
 
@@ -85,21 +91,25 @@
     @classmethod
     def import_from_dict(cls, value: KeyDict):
         if "d" in value:
             return cls.import_private_key(value)
         return cls.import_public_key(value)
 
     @classmethod
-    def import_from_bytes(cls, value: bytes, password=None):
+    def import_from_bytes(cls, value: bytes, password: t.Optional[t.Any] = None):
         if password is not None:
             password = to_bytes(password)
         return load_pem_key(value, cls.ssh_type, password)
 
     @staticmethod
-    def as_bytes(key, encoding=None, private=None, password=None) -> bytes:
+    def as_bytes(
+            key: BaseKey,
+            encoding: t.Optional[t.Literal["PEM", "DER"]] = None,
+            private: t.Optional[bool] = False,
+            password: t.Optional[t.Any] = None) -> bytes:
         if private is True:
             return dump_pem_key(key.private_key, encoding, private, password)
         elif private is False:
             return dump_pem_key(key.public_key, encoding, private, password)
         return dump_pem_key(key.raw_value, encoding, key.is_private, password)
 
     @staticmethod
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7517/registry.py` & `joserfc-0.6.0/src/joserfc/rfc7517/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 import typing as t
-from .models import Key
+from .models import BaseKey as Key
 from .types import KeyAny, KeyParameters
 from ..util import to_bytes
 
 
 class JWKRegistry:
-    """A registry for JWK to record ``joserfc`` supported key types.
-    Normally, you would use explicit key types like ``OctKey``, ``RSAKey``;
-    This registry provides a way to dynamically import and generate keys.
-    For instance:
-
-    .. code-block:: python
-
-        # instead of choosing which key type to use yourself,
-        # JWKRegistry can import it automatically
-        data = {"kty": "oct", "k": "..."}
-        key = JWKRegistry.import_key(data)
-    """
     key_types: t.Dict[str, t.Type[Key]] = {}
 
     @classmethod
-    def register(cls, model: t.Type[Key]):
-        cls.key_types[model.key_type] = model
-
-    @classmethod
-    def import_key(cls, data: KeyAny, key_type: t.Optional[str] = None, parameters: KeyParameters = None) -> Key:
+    def import_key(
+            cls,
+            data: KeyAny,
+            key_type: t.Optional[str] = None,
+            parameters: t.Optional[KeyParameters] = None) -> Key:
         """A class method for importing a key from bytes, string, and dict.
         When ``value`` is a dict, this method can tell the key type automatically,
         otherwise, developers SHOULD pass the ``key_type`` themselves.
 
         :param data: the key data in bytes, string, or dict.
         :param key_type: an optional key type in string.
         :param parameters: extra key parameters
         :return: OctKey, RSAKey, ECKey, or OKPKey
         """
         if isinstance(data, dict) and key_type is None:
-            if "kty" not in data:
+            if "kty" in data:
+                key_type = data["kty"]  # type: ignore
+            else:
                 raise ValueError("Missing key type")
-            key_type = data["kty"]
 
         if key_type not in cls.key_types:
             raise ValueError(f'Invalid key type: "{key_type}"')
 
         if isinstance(data, str):
             data = to_bytes(data)
 
@@ -49,15 +38,15 @@
         return key_cls.import_key(data, parameters)  # type: ignore
 
     @classmethod
     def generate_key(
             cls,
             key_type: str,
             crv_or_size: t.Union[str, int],
-            parameters: KeyParameters = None,
+            parameters: t.Optional[KeyParameters] = None,
             private: bool = True) -> Key:
         """A class method for generating key according to the given key type.
         When ``key_type`` is "oct" and "RSA", the second parameter SHOULD be
         a key size in bits. When ``key_type`` is "EC" and "OKP", the second
         parameter SHOULD be a "crv" string.
 
         .. code-block:: python
@@ -65,8 +54,8 @@
             JWKRegistry.generate_key("RSA", 2048)
             JWKRegistry.generate_key("EC", "P-256")
         """
         if key_type not in cls.key_types:
             raise ValueError(f'Invalid key type: "{key_type}"')
 
         key_cls = cls.key_types[key_type]
-        return key_cls.generate_key(crv_or_size, parameters, private)  # type: ignore
+        return key_cls.generate_key(crv_or_size, parameters, private)
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7517/types.py` & `joserfc-0.6.0/src/joserfc/rfc7517/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     "kid": str,
     "x5u": str,
     "x5c": t.List[str],
     "x5t": str,
     "x5t#S256": str,
 }, total=False)
 
+
 #: JWKs in dict
-KeySetDict = t.TypedDict("KeySetDict", {
-    "keys": t.List[KeyDict],
-})
+class KeySetDict(t.TypedDict):
+    keys: t.List[KeyDict]
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7518/derive_key.py` & `joserfc-0.6.0/src/joserfc/rfc7518/derive_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.5.0/src/joserfc/rfc7518/ec_key.py` & `joserfc-0.6.0/src/joserfc/rfc7518/ec_key.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Dict
+import typing as t
 from functools import cached_property
 from cryptography.hazmat.primitives.asymmetric.ec import (
     generate_private_key,
     ECDH,
     EllipticCurvePublicKey,
     EllipticCurvePrivateKey,
     EllipticCurvePrivateNumbers,
@@ -10,18 +10,24 @@
     SECP256R1,
     SECP384R1,
     SECP521R1,
 )
 from cryptography.hazmat.backends import default_backend
 from ..rfc7517.models import CurveKey
 from ..rfc7517.pem import CryptographyBinding
-from ..rfc7517.types import KeyDict, KeyParameters
+from ..rfc7517.types import KeyParameters
 from ..util import base64_to_int, int_to_base64
 from ..registry import KeyParameter
 
+KeyDict = t.TypedDict("KeyDict", {
+    "crv": str,
+    "x": str,
+    "y": str,
+    "d": str,  # optional
+}, total=False)
 
 DSS_CURVES = {
     "P-256": SECP256R1,
     "P-384": SECP384R1,
     "P-521": SECP521R1,
 }
 CURVES_DSS = {
@@ -32,103 +38,105 @@
 
 
 class ECBinding(CryptographyBinding):
     ssh_type = b"ecdsa-sha2-"
 
     @staticmethod
     def import_private_key(obj: KeyDict) -> EllipticCurvePrivateKey:
-        curve = DSS_CURVES[obj["crv"]]()
+        curve = DSS_CURVES[obj["crv"]]()  # type: ignore
         public_numbers = EllipticCurvePublicNumbers(
             base64_to_int(obj["x"]),
             base64_to_int(obj["y"]),
             curve,
         )
-        private_numbers = EllipticCurvePrivateNumbers(base64_to_int(obj["d"]), public_numbers)
+        d = base64_to_int(obj["d"])
+        private_numbers = EllipticCurvePrivateNumbers(d, public_numbers)
         return private_numbers.private_key(default_backend())
 
     @staticmethod
-    def export_private_key(key: EllipticCurvePrivateKey) -> Dict[str, str]:
+    def export_private_key(key: EllipticCurvePrivateKey) -> t.Dict[str, str]:
         numbers = key.private_numbers()
         return {
-            "crv": CURVES_DSS[key.curve.name],
+            "crv": CURVES_DSS[key.curve.name],  # type: ignore
             "x": int_to_base64(numbers.public_numbers.x),
             "y": int_to_base64(numbers.public_numbers.y),
             "d": int_to_base64(numbers.private_value),
         }
 
     @staticmethod
     def import_public_key(obj: KeyDict) -> EllipticCurvePublicKey:
-        curve = DSS_CURVES[obj["crv"]]()
+        curve = DSS_CURVES[obj["crv"]]()  # type: ignore
         public_numbers = EllipticCurvePublicNumbers(
             base64_to_int(obj["x"]),
             base64_to_int(obj["y"]),
             curve,
         )
         return public_numbers.public_key(default_backend())
 
     @staticmethod
-    def export_public_key(key: EllipticCurvePublicKey) -> Dict[str, str]:
+    def export_public_key(key: EllipticCurvePublicKey) -> t.Dict[str, str]:
         numbers = key.public_numbers()
         return {
-            "crv": CURVES_DSS[numbers.curve.name],
+            "crv": CURVES_DSS[numbers.curve.name],  # type: ignore
             "x": int_to_base64(numbers.x),
             "y": int_to_base64(numbers.y),
         }
 
 
-class ECKey(CurveKey[EllipticCurvePublicKey, EllipticCurvePrivateKey]):
-    key_type: str = "EC"
+class ECKey(CurveKey[EllipticCurvePrivateKey, EllipticCurvePublicKey]):
+    key_type = "EC"
     #: Registry definition for EC Key
     #: https://www.rfc-editor.org/rfc/rfc7518#section-6.2
     value_registry = {
         "crv": KeyParameter("Curve", "str", private=False, required=True),
         "x": KeyParameter("X Coordinate", "str", private=False, required=True),
         "y": KeyParameter("Y Coordinate", "str", private=False, required=True),
         "d": KeyParameter("EC Private Key", "str", private=True, required=False),
     }
     binding = ECBinding
 
-    def exchange_derive_key(self, key: "ECKey") -> bytes:
-        pubkey = key.get_op_key("deriveKey")
-        if self.private_key and self.curve_name == key.curve_name:
-            return self.private_key.exchange(ECDH(), pubkey)
-        raise ValueError("Invalid key for exchanging shared key")
-
     @property
     def is_private(self) -> bool:
         return isinstance(self.raw_value, EllipticCurvePrivateKey)
 
     @cached_property
     def public_key(self) -> EllipticCurvePublicKey:
         if isinstance(self.raw_value, EllipticCurvePrivateKey):
             return self.raw_value.public_key()
         return self.raw_value
 
     @property
-    def private_key(self) -> Optional[EllipticCurvePrivateKey]:
-        if self.is_private:
+    def private_key(self) -> t.Optional[EllipticCurvePrivateKey]:
+        if isinstance(self.raw_value, EllipticCurvePrivateKey):
             return self.raw_value
         return None
 
+    def exchange_derive_key(self, key: "ECKey") -> bytes:
+        pubkey = key.get_op_key("deriveKey")
+        if self.private_key and self.curve_name == key.curve_name:
+            return self.private_key.exchange(ECDH(), pubkey)
+        raise ValueError("Invalid key for exchanging shared key")
+
     @property
     def curve_name(self) -> str:
-        return CURVES_DSS[self.raw_value.curve.name]
+        return CURVES_DSS[self.raw_value.curve.name]  # type: ignore
 
     @property
     def curve_key_size(self) -> int:
         return self.raw_value.curve.key_size
 
     @classmethod
     def generate_key(
             cls,
             crv: str = "P-256",
-            parameters: KeyParameters = None,
+            parameters: t.Optional[KeyParameters] = None,
             private: bool = True) -> "ECKey":
         if crv not in DSS_CURVES:
             raise ValueError('Invalid crv value: "{}"'.format(crv))
         raw_key = generate_private_key(
-            curve=DSS_CURVES[crv](),
+            curve=DSS_CURVES[crv](),  # type: ignore
             backend=default_backend(),
         )
-        if not private:
-            raw_key = raw_key.public_key()
-        return cls(raw_key, raw_key, parameters)
+        if private:
+            return cls(raw_key, raw_key, parameters)
+        pub_key = raw_key.public_key()
+        return cls(pub_key, pub_key, parameters)
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7518/jwe_algs.py` & `joserfc-0.6.0/src/joserfc/rfc7518/jwe_algs.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,87 +8,84 @@
     aes_key_unwrap,
     InvalidUnwrap,
 )
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import GCM
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
-from .rsa_key import RSAKey
-from .oct_key import OctKey
+from cryptography.exceptions import InvalidTag
 from .derive_key import derive_key_for_concat_kdf
+from .oct_key import OctKey
+from .rsa_key import RSAKey
 from ..rfc7517.models import CurveKey
 from ..rfc7516.models import (
+    JWEAlgModel,
     JWEDirectEncryption,
     JWEKeyEncryption,
     JWEKeyWrapping,
     JWEKeyAgreement,
     JWEEncModel,
     Recipient,
 )
 from ..util import to_bytes, urlsafe_b64encode, urlsafe_b64decode
 from ..registry import HeaderParameter
 from ..errors import (
     InvalidKeyLengthError,
-    InvalidKeyTypeError,
-    UnwrapError,
+    DecodeError,
 )
 
 
 class DirectAlgModel(JWEDirectEncryption):
     name = "dir"
     description = "Direct use of a shared symmetric key"
     recommended = True
 
-    @staticmethod
-    def check_recipient_key(key) -> OctKey:
-        if isinstance(key, OctKey):
-            return key
-        raise InvalidKeyTypeError()
-
     def compute_cek(self, size: int, recipient: Recipient):
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: OctKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         cek = key.raw_value
         if len(cek) * 8 != size:
             raise InvalidKeyLengthError(f"A key of size {size} bits MUST be used")
         return cek
 
 
 class RSAAlgModel(JWEKeyEncryption):
     #: A key of size 2048 bits or larger MUST be used with these algorithms
     #: RSA1_5, RSA-OAEP, RSA-OAEP-256
     key_size = 2048
+    key_types = ["RSA"]
 
     def __init__(
             self,
             name: str,
             description: str,
             pad_fn: padding.AsymmetricPadding,
             recommended: bool = False):
         self.name = name
         self.description = description
         self.padding = pad_fn
         self.recommended = recommended
 
-    @staticmethod
-    def check_recipient_key(key) -> RSAKey:
-        if isinstance(key, RSAKey):
-            return key
-        raise InvalidKeyTypeError()
-
     def encrypt_cek(self, cek: bytes, recipient: Recipient):
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: RSAKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         op_key = key.get_op_key("encrypt")
         if op_key.key_size < self.key_size:
             raise InvalidKeyLengthError(f"A key of size {self.key_size} bits or larger MUST be used")
         return op_key.encrypt(cek, self.padding)
 
     def decrypt_cek(self, recipient: Recipient) -> bytes:
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: RSAKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         op_key = key.get_op_key("decrypt")
-        cek = op_key.decrypt(recipient.encrypted_key, self.padding)
+        try:
+            assert recipient.encrypted_key is not None
+            cek = op_key.decrypt(recipient.encrypted_key, self.padding)
+        except ValueError as error:
+            raise DecodeError(str(error))
         return cek
 
 
 class AESAlgModel(JWEKeyWrapping):
     def __init__(self, key_size: int, recommended: bool = False):
         self.name = f"A{key_size}KW"
         self.description = f"AES Key Wrap using {key_size}-bit key"
@@ -100,25 +97,28 @@
         return aes_key_wrap(key, cek, default_backend())
 
     def unwrap_cek(self, ek: bytes, key: bytes):
         self.check_op_key(key)
         try:
             cek = aes_key_unwrap(key, ek, default_backend())
         except InvalidUnwrap:
-            raise UnwrapError()
+            raise DecodeError("Unwrap AES key failed")
         return cek
 
     def encrypt_cek(self, cek: bytes, recipient: Recipient) -> bytes:
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: OctKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         op_key = key.get_op_key("wrapKey")
         return self.wrap_cek(cek, op_key)
 
     def decrypt_cek(self, recipient: Recipient) -> bytes:
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: OctKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         op_key = key.get_op_key("unwrapKey")
+        assert recipient.encrypted_key is not None
         return self.unwrap_cek(recipient.encrypted_key, op_key)
 
 
 class AESGCMAlgModel(JWEKeyWrapping):
     more_header_registry = {
         "iv": HeaderParameter("Initialization vector", "str", True),
         "tag": HeaderParameter("Authentication tag", "str", True),
@@ -132,15 +132,16 @@
     def wrap_cek(self, cek: bytes, key: bytes) -> bytes:  # pragma: no cover
         raise RuntimeError(f"{self.name} can not be used together with Key Agreement")
 
     def unwrap_cek(self, ek: bytes, key: bytes):  # pragma: no cover
         raise RuntimeError(f"{self.name} can not be used together with Key Agreement")
 
     def encrypt_cek(self, cek: bytes, recipient: Recipient) -> bytes:
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: OctKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         op_key = key.get_op_key("wrapKey")
         self.check_op_key(op_key)
 
         #: https://tools.ietf.org/html/rfc7518#section-4.7.1.1
         #: The "iv" (initialization vector) Header Parameter value is the
         #: base64url-encoded representation of the 96-bit IV value
         iv_size = 96
@@ -151,31 +152,37 @@
 
         encrypted_key = enc.update(cek) + enc.finalize()
         recipient.add_header("iv", urlsafe_b64encode(iv).decode("ascii"))
         recipient.add_header("tag", urlsafe_b64encode(enc.tag).decode("ascii"))
         return encrypted_key
 
     def decrypt_cek(self, recipient: Recipient) -> bytes:
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: OctKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         op_key = key.get_op_key("unwrapKey")
         self.check_op_key(op_key)
 
         headers = recipient.headers()
         assert "iv" in headers
         assert "tag" in headers
         iv = urlsafe_b64decode(to_bytes(headers["iv"]))
         tag = urlsafe_b64decode(to_bytes(headers["tag"]))
 
         cipher = Cipher(AES(op_key), GCM(iv, tag), backend=default_backend())
         d = cipher.decryptor()
-        cek = d.update(recipient.encrypted_key) + d.finalize()
+        try:
+            assert recipient.encrypted_key is not None
+            cek = d.update(recipient.encrypted_key) + d.finalize()
+        except InvalidTag as error:
+            raise DecodeError(str(error))
         return cek
 
 
 class ECDHESAlgModel(JWEKeyAgreement):
+    key_types = ["EC", "OKP"]
     more_header_registry = {
         "epk": HeaderParameter("Ephemeral Public Key", "jwk", True),
         "apu": HeaderParameter("Agreement PartyUInfo", "str"),
         "apv": HeaderParameter("Agreement PartyVInfo", "str"),
     }
 
     # https://tools.ietf.org/html/rfc7518#section-4.6
@@ -189,53 +196,50 @@
             self.name = f"ECDH-ES+{key_wrapping.name}"
             self.description = f"ECDH-ES using Concat KDF and CEK wrapped with {key_wrapping.name}"
             self.key_size = key_wrapping.key_size
             self.recommended = key_wrapping.recommended
         self.key_wrapping = key_wrapping
 
     def encrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient):
-        recipient_key: CurveKey = recipient.recipient_key
-        ephemeral_key: CurveKey = recipient.ephemeral_key
+        recipient_key: CurveKey = recipient.recipient_key  # type: ignore
+        ephemeral_key: CurveKey = recipient.ephemeral_key  # type: ignore
         shared_key = ephemeral_key.exchange_derive_key(recipient_key)
         headers = recipient.headers()
         return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size)
 
     def decrypt_agreed_upon_key(self, enc: JWEEncModel, recipient: Recipient) -> bytes:
         headers = recipient.headers()
         assert "epk" in headers
 
-        recipient_key: CurveKey = self.check_recipient_key(recipient.recipient_key)
+        recipient_key: CurveKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(recipient_key)
         ephemeral_key = recipient_key.import_key(headers["epk"])
         shared_key = recipient_key.exchange_derive_key(ephemeral_key)
         return derive_key_for_concat_kdf(shared_key, headers, enc.cek_size, self.key_size)
 
 
 class PBES2HSAlgModel(JWEKeyEncryption):
     # https://www.rfc-editor.org/rfc/rfc7518#section-4.8
+    key_size: int
     more_header_registry = {
         "p2s": HeaderParameter("PBES2 Salt Input", "str", True),
         "p2c": HeaderParameter("PBES2 Count", "int", True),
     }
+    key_types = ["oct"]
 
     # A minimum iteration count of 1000 is RECOMMENDED.
     DEFAULT_P2C = 2048
 
     def __init__(self, hash_size: int, key_wrapping: JWEKeyWrapping):
         self.name = f"PBES2-HS{hash_size}+{key_wrapping.name}"
         self.description = f"PBES2 with HMAC SHA-{hash_size} and {key_wrapping.name} wrapping"
         self.key_size = key_wrapping.key_size
         self.key_wrapping = key_wrapping
         self.hash_alg = getattr(hashes, f"SHA{hash_size}")()
 
-    @staticmethod
-    def check_recipient_key(key) -> OctKey:
-        if isinstance(key, OctKey):
-            return key
-        raise InvalidKeyTypeError()
-
     def compute_derived_key(self, key: bytes, p2s: bytes, p2c: int) -> bytes:
         # The salt value used is (UTF8(Alg) || 0x00 || Salt Input)
         salt = to_bytes(self.name) + b"\x00" + p2s
         kdf = PBKDF2HMAC(
             algorithm=self.hash_alg,
             length=self.key_size // 8,
             salt=salt,
@@ -255,36 +259,39 @@
         if "p2c" not in headers:
             # A minimum iteration count of 1000 is RECOMMENDED.
             p2c = self.DEFAULT_P2C
             recipient.add_header("p2c", p2c)
         else:
             p2c = headers["p2c"]
 
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: OctKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         kek = self.compute_derived_key(key.get_op_key("deriveKey"), p2s, p2c)
         return self.key_wrapping.wrap_cek(cek, kek)
 
     def decrypt_cek(self, recipient: Recipient) -> bytes:
         headers = recipient.headers()
         assert "p2s" in headers
         assert "p2c" in headers
         p2s = urlsafe_b64decode(to_bytes(headers["p2s"]))
         p2c = headers["p2c"]
-        key = self.check_recipient_key(recipient.recipient_key)
+        key: OctKey = recipient.recipient_key  # type: ignore
+        self.check_key_type(key)
         kek = self.compute_derived_key(key.get_op_key("deriveKey"), p2s, p2c)
+        assert recipient.encrypted_key is not None
         return self.key_wrapping.unwrap_cek(recipient.encrypted_key, kek)
 
 
 A128KW = AESAlgModel(128, True)  # A128KW, Recommended
 A192KW = AESAlgModel(192)  # A192KW
 A256KW = AESAlgModel(256, True)  # A256KW, Recommended
 
 
 #: https://www.rfc-editor.org/rfc/rfc7518#section-4.1
-JWE_ALG_MODELS = [
+JWE_ALG_MODELS: t.List[JWEAlgModel] = [
     # Avoid all RSA-PKCS1 v1.5 encryption algorithms ([RFC8017], Section 7.2),
     # preferring RSAES-OAEP ([RFC8017], Section 7.1).
     # https://www.rfc-editor.org/rfc/rfc8725#section-3.2
     RSAAlgModel("RSA1_5", "RSAES-PKCS1-v1_5", padding.PKCS1v15()),
     RSAAlgModel(
         "RSA-OAEP",
         "RSAES OAEP using default parameters",
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7518/jwe_encs.py` & `joserfc-0.6.0/src/joserfc/rfc7518/jwe_encs.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 import hmac
 import hashlib
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import GCM, CBC
 from cryptography.hazmat.primitives.padding import PKCS7
+from cryptography.exceptions import InvalidTag
 from ..rfc7516.models import JWEEncModel
+from ..errors import DecodeError
 from .util import encode_int
 
 
 class CBCHS2EncModel(JWEEncModel):
     # The IV used is a 128-bit value generated randomly or
     # pseudo-randomly for use in the cipher.
     iv_size = 128
@@ -62,15 +64,15 @@
     def decrypt(self, ciphertext: bytes, tag: bytes, cek: bytes, iv: bytes, aad: bytes) -> bytes:
         """Key Decryption with AES AES_CBC_HMAC_SHA2."""
         hkey = cek[:self.key_len]
         dkey = cek[self.key_len:]
 
         ctag = self._hmac(ciphertext, aad, iv, hkey)
         if not hmac.compare_digest(ctag, tag):
-            raise ValueError("tag does not match")
+            raise DecodeError("tag does not match")
 
         cipher = Cipher(AES(dkey), CBC(iv), backend=default_backend())
         d = cipher.decryptor()
         data = d.update(ciphertext) + d.finalize()
         unpad = PKCS7(AES.block_size).unpadder()
         return unpad.update(data) + unpad.finalize()
 
@@ -96,18 +98,21 @@
         return ciphertext, enc.tag
 
     def decrypt(self, ciphertext: bytes, tag: bytes, cek: bytes, iv: bytes, aad: bytes) -> bytes:
         """Key Decryption with AES GCM"""
         cipher = Cipher(AES(cek), GCM(iv, tag), backend=default_backend())
         d = cipher.decryptor()
         d.authenticate_additional_data(aad)
-        return d.update(ciphertext) + d.finalize()
+        try:
+            return d.update(ciphertext) + d.finalize()
+        except InvalidTag as error:
+            raise DecodeError(str(error))
 
 
-JWE_ENC_MODELS = [
+JWE_ENC_MODELS: t.List[JWEEncModel] = [
     CBCHS2EncModel(128, 256),  # A128CBC-HS256
     CBCHS2EncModel(192, 384),  # A192CBC-HS384
     CBCHS2EncModel(256, 512),  # A256CBC-HS512
     GCMEncModel(128),  # A128GCM
     GCMEncModel(192),  # A192GCM
     GCMEncModel(256),  # A256GCM
 ]
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7518/jwe_zips.py` & `joserfc-0.6.0/src/joserfc/rfc7518/jwe_zips.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import zlib
+from typing import List
 from ..rfc7516.models import JWEZipModel
 
 
 class DeflateZipModel(JWEZipModel):
     name = "DEF"
     description = "DEFLATE"
 
@@ -13,8 +14,8 @@
         return data[2:-4]
 
     def decompress(self, s: bytes) -> bytes:
         """Decompress DEFLATE bytes data."""
         return zlib.decompress(s, -zlib.MAX_WBITS)
 
 
-JWE_ZIP_MODELS = [DeflateZipModel()]
+JWE_ZIP_MODELS: List[JWEZipModel] = [DeflateZipModel()]
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7518/jws_algs.py` & `joserfc-0.6.0/src/joserfc/rfc7518/jws_algs.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,37 +7,39 @@
     "alg" (Algorithm) Header Parameter Values for JWS per `Section 3`_.
 
     .. _`Section 3`: https://tools.ietf.org/html/rfc7518#section-3
 """
 
 import hmac
 import hashlib
+import typing as t
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric.utils import (
     decode_dss_signature,
     encode_dss_signature,
 )
 from cryptography.hazmat.primitives.asymmetric.ec import ECDSA
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.exceptions import InvalidSignature
 from ..rfc7515.model import JWSAlgModel
+from ..rfc7517.models import BaseKey
 from .oct_key import OctKey
 from .rsa_key import RSAKey
 from .ec_key import ECKey
 from .util import encode_int, decode_int
 
 
 class NoneAlgModel(JWSAlgModel):
     name = "none"
     description = "No digital signature or MAC performed"
 
-    def sign(self, msg, key):
+    def sign(self, msg: bytes, key: BaseKey):
         return b""
 
-    def verify(self, msg, sig, key):
+    def verify(self, msg: bytes, sig: bytes, key: BaseKey):
         return False
 
 
 class HMACAlgModel(JWSAlgModel):
     """HMAC using SHA algorithms for JWS. Available algorithms:
 
     - HS256: HMAC using SHA-256
@@ -45,15 +47,15 @@
     - HS512: HMAC using SHA-512
     """
 
     SHA256 = hashlib.sha256
     SHA384 = hashlib.sha384
     SHA512 = hashlib.sha512
 
-    def __init__(self, sha_type: int, recommended: bool = False):
+    def __init__(self, sha_type: t.Literal[256, 384, 512], recommended: bool = False):
         self.name = f"HS{sha_type}"
         self.description = f"HMAC using SHA-{sha_type}"
         self.recommended = recommended
         self.hash_alg = getattr(self, f"SHA{sha_type}")
 
     def sign(self, msg: bytes, key: OctKey) -> bytes:
         # it is faster than the one in cryptography
@@ -69,21 +71,22 @@
 class RSAAlgModel(JWSAlgModel):
     """RSA using SHA algorithms for JWS. Available algorithms:
 
     - RS256: RSASSA-PKCS1-v1_5 using SHA-256
     - RS384: RSASSA-PKCS1-v1_5 using SHA-384
     - RS512: RSASSA-PKCS1-v1_5 using SHA-512
     """
+    key_type = "RSA"
 
     SHA256 = hashes.SHA256
     SHA384 = hashes.SHA384
     SHA512 = hashes.SHA512
     padding = padding.PKCS1v15()
 
-    def __init__(self, sha_type: int, recommended: bool = False):
+    def __init__(self, sha_type: t.Literal[256, 384, 512], recommended: bool = False):
         self.name = f"RS{sha_type}"
         self.description = f"RSASSA-PKCS1-v1_5 using SHA-{sha_type}"
         self.recommended = recommended
         self.hash_alg = getattr(self, f"SHA{sha_type}")
 
     def sign(self, msg: bytes, key: RSAKey) -> bytes:
         op_key = key.get_op_key("sign")
@@ -101,27 +104,28 @@
 class ECAlgModel(JWSAlgModel):
     """ECDSA using SHA algorithms for JWS. Available algorithms:
 
     - ES256: ECDSA using P-256 and SHA-256
     - ES384: ECDSA using P-384 and SHA-384
     - ES512: ECDSA using P-521 and SHA-512
     """
+    key_type = "EC"
 
     SHA256 = hashes.SHA256
     SHA384 = hashes.SHA384
     SHA512 = hashes.SHA512
 
-    def __init__(self, name: str, curve: str, sha_type: int, recommended: bool = False):
+    def __init__(self, name: str, curve: str, sha_type: t.Literal[256, 384, 512], recommended: bool = False):
         self.name = name
         self.curve = curve
         self.description = f"ECDSA using {self.curve} and SHA-{sha_type}"
         self.recommended = recommended
         self.hash_alg = getattr(self, f"SHA{sha_type}")
 
-    def _check_key(self, key: ECKey):
+    def _check_key(self, key: ECKey) -> ECKey:
         if key.curve_name != self.curve:
             raise ValueError(f'Key for "{self.name}" not supported, only "{self.curve}" allowed')
         return key
 
     def sign(self, msg: bytes, key: ECKey) -> bytes:
         self._check_key(key)
         op_key = key.get_op_key("sign")
@@ -153,20 +157,21 @@
 class RSAPSSAlgModel(JWSAlgModel):
     """RSASSA-PSS using SHA algorithms for JWS. Available algorithms:
 
     - PS256: RSASSA-PSS using SHA-256 and MGF1 with SHA-256
     - PS384: RSASSA-PSS using SHA-384 and MGF1 with SHA-384
     - PS512: RSASSA-PSS using SHA-512 and MGF1 with SHA-512
     """
+    key_type = "RSA"
 
     SHA256 = hashes.SHA256
     SHA384 = hashes.SHA384
     SHA512 = hashes.SHA512
 
-    def __init__(self, sha_type: int):
+    def __init__(self, sha_type: t.Literal[256, 384, 512]):
         self.name = f"PS{sha_type}"
         self.description = f"RSASSA-PSS using SHA-{sha_type} and MGF1 with SHA-{sha_type}"
         self.hash_alg = getattr(self, f"SHA{sha_type}")
         self.padding = padding.PSS(mgf=padding.MGF1(self.hash_alg()), salt_length=self.hash_alg.digest_size)
 
     def sign(self, msg: bytes, key: RSAKey) -> bytes:
         op_key = key.get_op_key("sign")
@@ -177,15 +182,15 @@
         try:
             op_key.verify(sig, msg, self.padding, self.hash_alg())
             return True
         except InvalidSignature:
             return False
 
 
-JWS_ALGORITHMS = [
+JWS_ALGORITHMS: t.List[JWSAlgModel] = [
     NoneAlgModel(),  # none
     HMACAlgModel(256, True),  # HS256
     HMACAlgModel(384),  # HS384
     HMACAlgModel(512),  # HS512
     RSAAlgModel(256, True),  # RS256
     RSAAlgModel(384),  # RS384
     RSAAlgModel(512),  # RS512
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7518/oct_key.py` & `joserfc-0.6.0/src/joserfc/rfc7518/oct_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 import string
+from typing import Optional
 from ..util import (
     to_bytes,
     urlsafe_b64decode,
     urlsafe_b64encode,
 )
 from ..registry import KeyParameter
 from ..rfc7517.models import SymmetricKey, NativeKeyBinding
@@ -32,25 +33,29 @@
     def import_from_bytes(cls, value: bytes, password=None):
         # security check
         if value.startswith(POSSIBLE_UNSAFE_KEYS):
             raise ValueError("This key may not be safe to import")
         return value
 
 
-class OctKey(SymmetricKey[bytes, bytes]):
+class OctKey(SymmetricKey):
     """OctKey is a symmetric key, defined by RFC7518 Section 6.4.
     """
-    key_type: str = "oct"
+    key_type = "oct"
     binding = OctBinding
 
     #: https://www.rfc-editor.org/rfc/rfc7518#section-6.4
     value_registry = {"k": KeyParameter("Key Value", "str", True, True)}
 
     @classmethod
-    def generate_key(cls, key_size=256, parameters: KeyParameters = None, private: bool = True) -> "OctKey":
+    def generate_key(
+            cls,
+            key_size=256,
+            parameters: Optional[KeyParameters] = None,
+            private: bool = True) -> "OctKey":
         """Generate a ``OctKey`` with the given bit size (not bytes).
 
         :param key_size: size in bit
         :param parameters: extra parameter in JWK
         :param private: must be True
         """
         if not private:
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7518/rsa_key.py` & `joserfc-0.6.0/src/joserfc/rfc7518/rsa_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Dict
+import typing as t
 from functools import cached_property
 from cryptography.hazmat.primitives.asymmetric.rsa import (
     generate_private_key,
     RSAPublicKey,
     RSAPrivateKey,
     RSAPrivateNumbers,
     RSAPublicNumbers,
@@ -11,18 +11,30 @@
     rsa_crt_dmq1,
     rsa_crt_iqmp,
 )
 from cryptography.hazmat.backends import default_backend
 from ..registry import KeyParameter
 from ..rfc7517.models import AsymmetricKey
 from ..rfc7517.pem import CryptographyBinding
-from ..rfc7517.types import KeyDict, KeyParameters
+from ..rfc7517.types import KeyParameters
 from ..util import int_to_base64, base64_to_int
 
 
+KeyDict = t.TypedDict("KeyDict", {
+    "n": str,
+    "e": str,
+    "d": str,
+    "p": str,
+    "q": str,
+    "dp": str,
+    "dq": str,
+    "qi": str,
+}, total=False)
+
+
 class RSABinding(CryptographyBinding):
     ssh_type = b"ssh-rsa"
 
     @staticmethod
     def import_private_key(obj: KeyDict) -> RSAPrivateKey:
         if "oth" in obj:  # pragma: no cover
             # https://tools.ietf.org/html/rfc7518#section-6.3.2.7
@@ -52,15 +64,15 @@
                 iqmp=rsa_crt_iqmp(p, q),
                 public_numbers=public_numbers,
             )
 
         return numbers.private_key(default_backend())
 
     @staticmethod
-    def export_private_key(key: RSAPrivateKey) -> Dict[str, str]:
+    def export_private_key(key: RSAPrivateKey) -> KeyDict:
         numbers = key.private_numbers()
         return {
             "n": int_to_base64(numbers.public_numbers.n),
             "e": int_to_base64(numbers.public_numbers.e),
             "d": int_to_base64(numbers.d),
             "p": int_to_base64(numbers.p),
             "q": int_to_base64(numbers.q),
@@ -71,21 +83,21 @@
 
     @staticmethod
     def import_public_key(obj: KeyDict) -> RSAPublicKey:
         numbers = RSAPublicNumbers(base64_to_int(obj["e"]), base64_to_int(obj["n"]))
         return numbers.public_key(default_backend())
 
     @staticmethod
-    def export_public_key(key: RSAPublicKey) -> Dict[str, str]:
+    def export_public_key(key: RSAPublicKey) -> t.Dict[str, str]:
         numbers = key.public_numbers()
         return {"n": int_to_base64(numbers.n), "e": int_to_base64(numbers.e)}
 
 
-class RSAKey(AsymmetricKey[RSAPublicKey, RSAPrivateKey]):
-    key_type: str = "RSA"
+class RSAKey(AsymmetricKey[RSAPrivateKey, RSAPublicKey]):
+    key_type = "RSA"
     #: Registry definition for RSA Key
     #: https://www.rfc-editor.org/rfc/rfc7518#section-6.3
     value_registry = {
         "n": KeyParameter("Modulus", "str", private=False, required=True),
         "e": KeyParameter("Exponent", "str", private=False, required=True),
         "d": KeyParameter("Private Exponent", "str", private=True, required=False),
         "p": KeyParameter("First Prime Factor", "str", private=True, required=False),
@@ -104,37 +116,38 @@
     @cached_property
     def public_key(self) -> RSAPublicKey:
         if isinstance(self.raw_value, RSAPrivateKey):
             return self.raw_value.public_key()
         return self.raw_value
 
     @property
-    def private_key(self) -> Optional[RSAPrivateKey]:
-        if self.is_private:
+    def private_key(self) -> t.Optional[RSAPrivateKey]:
+        if isinstance(self.raw_value, RSAPrivateKey):
             return self.raw_value
         return None
 
     @classmethod
     def generate_key(
             cls,
             key_size: int = 2048,
-            parameters: KeyParameters = None,
+            parameters: t.Optional[KeyParameters] = None,
             private: bool = True) -> "RSAKey":
         if key_size < 512:
             raise ValueError("key_size must not be less than 512")
         if key_size % 8 != 0:
             raise ValueError("Invalid key_size for RSAKey")
         raw_key = generate_private_key(
             public_exponent=65537,
             key_size=key_size,
             backend=default_backend(),
         )
-        if not private:
-            raw_key = raw_key.public_key()
-        return cls(raw_key, raw_key, parameters)
+        if private:
+            return cls(raw_key, raw_key, parameters)
+        pub_key = raw_key.public_key()
+        return cls(pub_key, pub_key, parameters)
 
 
 def has_all_prime_factors(obj) -> bool:
     props = ["p", "q", "dp", "dq", "qi"]
     props_found = [prop in obj for prop in props]
     if all(props_found):
         return True
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7519/claims.py` & `joserfc-0.6.0/src/joserfc/rfc7519/claims.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.5.0/src/joserfc/rfc7519/registry.py` & `joserfc-0.6.0/src/joserfc/rfc7519/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,29 @@
     InvalidClaimError,
     ExpiredTokenError,
     InvalidTokenError,
 )
 
 
 #: http://openid.net/specs/openid-connect-core-1_0.html#IndividualClaimsRequests
-ClaimsOption = TypedDict("ClaimsOption", {
-    "essential": bool,
-    "value": Union[str, int],
-    "values": List[Union[str, int]],
-}, total=False)
+class ClaimsOption(TypedDict, total=False):
+    essential: bool
+    value: Union[str, int]
+    values: List[Union[str, int]]
 
 
 class ClaimsRegistry:
     """Requesting "claims" for JWT with the given conditions."""
 
     def __init__(self, **kwargs: ClaimsOption):
         self.options = kwargs
         self.essential_keys = {key for key in kwargs if kwargs[key].get("essential")}
 
     def check_value(self, claim_name: str, value: Any):
-        option: ClaimsOption = self.options.get(claim_name)
+        option = self.options.get(claim_name)
         if option:
             option_value = option.get("value")
             if option_value and value != option_value:
                 raise InvalidClaimError(claim_name)
 
             option_values = option.get("values")
             if option_values and value not in option_values:
@@ -52,37 +51,37 @@
     def __init__(self, now: Optional[int] = None, leeway=0, **kwargs: ClaimsOption):
         if now is None:
             now = int(time.time())
         self.now = now
         self.leeway = leeway
         super().__init__(**kwargs)
 
-    def validate_aud(self, value):
+    def validate_aud(self, value: Any):
         """The "aud" (audience) claim identifies the recipients that the JWT is
         intended for.  Each principal intended to process the JWT MUST
         identify itself with a value in the audience claim.  If the principal
         processing the claim does not identify itself with a value in the
         "aud" claim when this claim is present, then the JWT MUST be
         rejected.  In the general case, the "aud" value is an array of
         case-sensitive strings, each containing a StringOrURI value.  In the
         special case when the JWT has one audience, the "aud" value MAY be a
         single case-sensitive string containing a StringOrURI value.  The
         interpretation of audience values is generally application specific.
         Use of this claim is OPTIONAL.
         """
-        option: ClaimsOption = self.options.get("aud")
+        option = self.options.get("aud")
         if not option:
             return
 
         option_values = option.get("values")
 
-        if not option_values:
+        if option_values is None:
             option_value = option.get("value")
             if option_value:
-                option_values = option_value
+                option_values = [option_value]
 
         if not option_values:
             return
 
         if isinstance(value, list):
             aud_list = value
         else:
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7797/compact.py` & `joserfc-0.6.0/src/joserfc/rfc7797/compact.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     CompactSignature,
     JWSRegistry as _JWSRegistry,
     serialize_compact as _serialize_compact,
     deserialize_compact as _deserialize_compact,
 )
 from ..util import (
     to_bytes,
-    to_unicode,
+    to_str,
     json_b64encode,
     urlsafe_b64encode,
     urlsafe_b64decode,
 )
 from ..rfc7515.compact import decode_header
 from ..errors import BadSignatureError
 from .registry import JWSRegistry
@@ -87,15 +87,15 @@
 # the application MUST ensure that the payload contains only the URL-safe
 # characters 'a'-'z', 'A'-'Z', '0'-'9', dash ('-'), underscore ('_'),
 # and tilde ('~')
 _re_urlsafe = re.compile("^[a-zA-Z0-9-_~]+$")
 
 
 def __is_urlsafe_characters(s: t.AnyStr) -> bool:
-    return bool(_re_urlsafe.match(to_unicode(s)))
+    return bool(_re_urlsafe.match(to_str(s)))
 
 
 def _extract_compact(value: bytes, payload: t.Optional[t.AnyStr] = None):
     parts = value.split(b".")
     if len(parts) != 3:
         raise ValueError("Invalid JSON Web Signature")
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7797/json.py` & `joserfc-0.6.0/src/joserfc/rfc7797/json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import typing as t
+from ..rfc7515.json import verify_signature
+from ..rfc7515.types import JSONSignatureDict
 from ..jws import (
     HeaderDict,
     HeaderMember,
-    JSONSignature,
-    JSONSerialization,
+    FlattenedJSONSignature,
+    FlattenedJSONSerialization,
     JWSRegistry as _JWSRegistry,
     serialize_json as _serialize_json,
     deserialize_json as _deserialize_json,
 )
 from ..jwk import KeyFlexible, guess_key
 from ..util import (
     to_bytes,
-    to_unicode,
+    to_str,
     json_b64encode,
     json_b64decode,
     urlsafe_b64encode,
-    urlsafe_b64decode,
 )
 from ..errors import BadSignatureError
 from .registry import JWSRegistry
 
 
 def serialize_json(
         member: HeaderDict,
         payload: t.AnyStr,
         private_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
-        registry: t.Optional[_JWSRegistry] = None) -> JSONSerialization:
+        registry: t.Optional[_JWSRegistry] = None) -> FlattenedJSONSerialization:
 
     _member = HeaderMember(**member)
     headers = _member.headers()
     if "b64" not in headers:
         return _serialize_json(member, payload, private_key, algorithms, registry)
 
     if registry is None:
@@ -49,53 +50,50 @@
         protected_segment = json_b64encode(_member.protected)
     else:
         protected_segment = b""
 
     signing_input = b".".join([protected_segment, to_bytes(payload)])
     signature = urlsafe_b64encode(alg.sign(signing_input, key))
 
-    rv = {
-        "payload": to_unicode(payload),
-        "signature": to_unicode(signature),
+    rv: FlattenedJSONSerialization = {
+        "payload": to_str(payload),
+        "signature": to_str(signature),
     }
     if protected_segment:
-        rv["protected"] = to_unicode(protected_segment)
+        rv["protected"] = to_str(protected_segment)
     if _member.header:
         rv["header"] = _member.header
     return rv
 
 
 def deserialize_json(
-        value: JSONSerialization,
+        value: FlattenedJSONSerialization,
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
-        registry: t.Optional[_JWSRegistry] = None) -> JSONSignature:
+        registry: t.Optional[_JWSRegistry] = None) -> FlattenedJSONSignature:
     obj = _extract_json(value)
     if obj is None:
         return _deserialize_json(value, public_key, algorithms, registry)
 
     if registry is None:
         registry = JWSRegistry(algorithms=algorithms)
 
-    member = obj.members[0]
-    headers = member.headers()
+    headers = obj.headers()
     if headers["b64"] is True:
         return _deserialize_json(value, public_key, registry=registry)
 
-    registry.check_header(headers)
-    key = guess_key(public_key, member)
-    alg = registry.get_alg(headers["alg"])
-    signing_input = b".".join([obj.segments["header"], obj.payload])
-    sig = urlsafe_b64decode(obj.segments["signature"])
-    if not alg.verify(signing_input, sig, key):
+    payload_segment = obj.segments["payload"]
+    find_key = lambda d: guess_key(public_key, d)
+    assert obj.signature is not None
+    if not verify_signature(obj.member, obj.signature, payload_segment, registry, find_key):
         raise BadSignatureError()
     return obj
 
 
-def _extract_json(value: JSONSerialization):
+def _extract_json(value: FlattenedJSONSerialization):
     if "signatures" in value:
         return None
 
     if "protected" in value:
         protected_segment = to_bytes(value["protected"])
         protected = json_b64decode(protected_segment)
     else:
@@ -105,14 +103,16 @@
     header = value.get("header")
     member = HeaderMember(protected, header)
     headers = member.headers()
     if "b64" not in headers:
         return None
 
     payload = to_bytes(value["payload"])
-    obj = JSONSignature([member], payload)
-    obj.segments = {
-        "header": protected_segment,
-        "signature": to_bytes(value["signature"]),
-    }
-    obj.flattened = True
+    obj = FlattenedJSONSignature(member, payload)
+    _sig: JSONSignatureDict = {"signature": value["signature"]}
+    if "protected" in value:
+        _sig["protected"] = value["protected"]
+    if "header" in value:
+        _sig["header"] = value["header"]
+    obj.signature = _sig
+    obj.segments = {"payload": payload}
     return obj
```

### Comparing `joserfc-0.5.0/src/joserfc/rfc7797/registry.py` & `joserfc-0.6.0/src/joserfc/rfc7797/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.5.0/src/joserfc/rfc8037/okp_key.py` & `joserfc-0.6.0/src/joserfc/rfc8037/okp_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,132 +1,140 @@
-from typing import Optional, Union, Dict
+import typing as t
 from functools import cached_property
 from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PublicKey, Ed25519PrivateKey
 from cryptography.hazmat.primitives.asymmetric.ed448 import Ed448PublicKey, Ed448PrivateKey
 from cryptography.hazmat.primitives.asymmetric.x25519 import X25519PublicKey, X25519PrivateKey
 from cryptography.hazmat.primitives.asymmetric.x448 import X448PublicKey, X448PrivateKey
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
     PublicFormat,
     PrivateFormat,
     NoEncryption,
 )
 from ..rfc7517.models import CurveKey
-from ..rfc7517.types import KeyDict, KeyParameters
+from ..rfc7517.types import KeyParameters
 from ..rfc7517.pem import CryptographyBinding
 from ..util import to_bytes, urlsafe_b64decode, urlsafe_b64encode
 from ..registry import KeyParameter
 
-PUBLIC_KEYS_MAP = {
+PublicOKPKey = t.Union[Ed25519PublicKey, Ed448PublicKey, X25519PublicKey, X448PublicKey]
+PrivateOKPKey = t.Union[Ed25519PrivateKey, Ed448PrivateKey, X25519PrivateKey, X448PrivateKey]
+KeyDict = t.TypedDict("KeyDict", {
+    "crv": t.Literal["Ed25519", "Ed448", "X25519", "X448"],
+    "x": str,
+    "d": str,
+}, total=False)
+PUBLIC_KEYS_MAP: t.Dict[str, t.Type[PublicOKPKey]] = {
     "Ed25519": Ed25519PublicKey,
     "Ed448": Ed448PublicKey,
     "X25519": X25519PublicKey,
     "X448": X448PublicKey,
 }
-PRIVATE_KEYS_MAP = {
+PRIVATE_KEYS_MAP: t.Dict[str, t.Type[PrivateOKPKey]] = {
     "Ed25519": Ed25519PrivateKey,
     "Ed448": Ed448PrivateKey,
     "X25519": X25519PrivateKey,
     "X448": X448PrivateKey,
 }
-PrivateKeyTypes = tuple(PRIVATE_KEYS_MAP.values())
-PublicOKPKey = Union[Ed25519PublicKey, Ed448PublicKey, X25519PublicKey, X448PublicKey]
-PrivateOKPKey = Union[Ed25519PrivateKey, Ed448PrivateKey, X25519PrivateKey, X448PrivateKey]
+PrivateKeyTypes = (Ed25519PrivateKey, Ed448PrivateKey, X25519PrivateKey, X448PrivateKey)
 
 
 class OKPBinding(CryptographyBinding):
     ssh_type = b"ssh-ed25519"
 
     @staticmethod
     def import_private_key(obj: KeyDict) -> PrivateOKPKey:
-        crv_key = PRIVATE_KEYS_MAP[obj["crv"]]
-        d_bytes = urlsafe_b64decode(to_bytes(obj["d"]))
-        return crv_key.from_private_bytes(d_bytes)
+        crv_key: t.Type[PrivateOKPKey] = PRIVATE_KEYS_MAP[obj["crv"]]
+        d = urlsafe_b64decode(to_bytes(obj["d"]))
+        return crv_key.from_private_bytes(d)
 
     @staticmethod
     def import_public_key(obj: KeyDict) -> PublicOKPKey:
-        crv_key = PUBLIC_KEYS_MAP[obj["crv"]]
+        crv_key: t.Type[PublicOKPKey] = PUBLIC_KEYS_MAP[obj["crv"]]
         x_bytes = urlsafe_b64decode(to_bytes(obj["x"]))
         return crv_key.from_public_bytes(x_bytes)
 
     @staticmethod
-    def export_private_key(key: PrivateOKPKey) -> Dict[str, str]:
+    def export_private_key(key: PrivateOKPKey) -> t.Dict[str, str]:
         obj = OKPBinding.export_public_key(key.public_key())
         d_bytes = key.private_bytes(Encoding.Raw, PrivateFormat.Raw, NoEncryption())
         obj["d"] = urlsafe_b64encode(d_bytes).decode("utf-8")
         return obj
 
     @staticmethod
-    def export_public_key(key: PublicOKPKey) -> Dict[str, str]:
+    def export_public_key(key: PublicOKPKey) -> t.Dict[str, str]:
         x_bytes = key.public_bytes(Encoding.Raw, PublicFormat.Raw)
         return {
             "crv": get_key_curve(key),
             "x": urlsafe_b64encode(x_bytes).decode("utf-8"),
         }
 
 
-class OKPKey(CurveKey[PublicOKPKey, PrivateOKPKey]):
+class OKPKey(CurveKey[PrivateOKPKey, PublicOKPKey]):
     """Key class of the ``OKP`` key type."""
 
-    key_type: str = "OKP"
+    key_type = "OKP"
     #: Registry definition for OKP Key
     #: https://www.rfc-editor.org/rfc/rfc8037#section-2
     value_registry = {
         "crv": KeyParameter("Curve", "str", private=False, required=True),
         "x": KeyParameter("X Coordinate", "str", private=False, required=True),
         "d": KeyParameter("OKP Private Key", "str", private=True, required=False),
     }
     binding = OKPBinding
     required_fields = frozenset(["crv", "x"])
     private_only_fields = frozenset(["d"])
 
     def exchange_derive_key(self, key: "OKPKey") -> bytes:
         # used in ECDHESAlgorithm
-        pubkey = key.get_op_key("deriveKey")
-        if self.private_key and self.curve_name in ("X25519", "X448") and self.curve_name == key.curve_name:
+        pubkey: t.Union[X25519PublicKey, X448PublicKey] = key.get_op_key("deriveKey")  # type: ignore
+        if isinstance(self.private_key, X25519PrivateKey) and isinstance(pubkey, X25519PublicKey):
+            return self.private_key.exchange(pubkey)
+        elif isinstance(self.private_key, X448PrivateKey) and isinstance(pubkey, X448PublicKey):
             return self.private_key.exchange(pubkey)
         raise ValueError("Invalid key for exchanging shared key")
 
     @property
     def is_private(self) -> bool:
         return isinstance(self.raw_value, PrivateKeyTypes)
 
     @cached_property
     def public_key(self) -> PublicOKPKey:
-        if self.is_private:
+        if isinstance(self.raw_value, PrivateKeyTypes):
             return self.raw_value.public_key()
         return self.raw_value
 
     @property
-    def private_key(self) -> Optional[PrivateOKPKey]:
-        if self.is_private:
+    def private_key(self) -> t.Optional[PrivateOKPKey]:
+        if isinstance(self.raw_value, PrivateKeyTypes):
             return self.raw_value
         return None
 
     @property
     def curve_name(self) -> str:
         return get_key_curve(self.raw_value)
 
     @classmethod
     def generate_key(
             cls,
             crv: str = "Ed25519",
-            parameters: KeyParameters = None,
+            parameters: t.Optional[KeyParameters] = None,
             private: bool = True) -> "OKPKey":
         if crv not in PRIVATE_KEYS_MAP:
             raise ValueError('Invalid crv value: "{}"'.format(crv))
 
-        private_key_cls = PRIVATE_KEYS_MAP[crv]
+        private_key_cls: t.Type[PrivateOKPKey] = PRIVATE_KEYS_MAP[crv]
         raw_key = private_key_cls.generate()
-        if not private:
-            raw_key = raw_key.public_key()
-        return cls(raw_key, raw_key, parameters)
+        if private:
+            return cls(raw_key, raw_key, parameters)
+        pub_key = raw_key.public_key()
+        return cls(pub_key, pub_key, parameters)
 
 
-def get_key_curve(key: Union[PublicOKPKey, PrivateOKPKey]):
+def get_key_curve(key: t.Union[PublicOKPKey, PrivateOKPKey]):
     if isinstance(key, (Ed25519PublicKey, Ed25519PrivateKey)):
         return "Ed25519"
     elif isinstance(key, (Ed448PublicKey, Ed448PrivateKey)):
         return "Ed448"
     elif isinstance(key, (X25519PublicKey, X25519PrivateKey)):
         return "X25519"
     elif isinstance(key, (X448PublicKey, X448PrivateKey)):
```

### Comparing `joserfc-0.5.0/src/joserfc/util.py` & `joserfc-0.6.0/src/joserfc/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+import typing as t
 import base64
 import struct
 import json
 
 
-def to_bytes(x, charset="utf-8", errors="strict"):
+def to_bytes(x: t.Any, charset: str = "utf-8", errors: str = "strict") -> bytes:
     if isinstance(x, bytes):
         return x
     if isinstance(x, str):
         return x.encode(charset, errors)
     if isinstance(x, (int, float)):
         return str(x).encode(charset, errors)
     return bytes(x)
 
 
-def to_unicode(x, charset="utf-8") -> str:
+def to_str(x: t.Union[bytes, str], charset: str = "utf-8") -> str:
     if isinstance(x, bytes):
         return x.decode(charset)
     return x
 
 
-def json_dumps(data: dict, ensure_ascii=False):
+def json_dumps(data: t.Any, ensure_ascii: bool = False) -> str:
     return json.dumps(data, ensure_ascii=ensure_ascii, separators=(",", ":"))
 
 
 def urlsafe_b64decode(s: bytes) -> bytes:
     s += b"=" * (-len(s) % 4)
     return base64.urlsafe_b64decode(s)
 
@@ -42,15 +43,15 @@
     if num < 0:
         raise ValueError("Must be a positive integer")
 
     s = num.to_bytes((num.bit_length() + 7) // 8, "big", signed=False)
     return urlsafe_b64encode(s).decode("utf-8", "strict")
 
 
-def json_b64encode(text, charset="utf-8") -> bytes:
+def json_b64encode(text: t.Any, charset: str = "utf-8") -> bytes:
     if isinstance(text, dict):
         text = json_dumps(text)
     return urlsafe_b64encode(to_bytes(text, charset))
 
 
-def json_b64decode(text, charset="utf-8") -> dict:
+def json_b64decode(text: t.Any, charset="utf-8") -> t.Dict[str, t.Any]:
     return json.loads(urlsafe_b64decode(to_bytes(text, charset)))
```

### Comparing `joserfc-0.5.0/src/joserfc.egg-info/PKG-INFO` & `joserfc-0.6.0/src/joserfc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.5.0
+Version: 0.6.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
 Project-URL: Source, https://github.com/authlib/joserfc
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
@@ -20,20 +20,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: drafts
 License-File: LICENSE
 
 JOSE RFC
 ========
 
-``joserfc`` is a Python implementation of **JSON Object Signing and Encryption** (JOSE).
+`·joserfc·` is a Python library that provides a comprehensive implementation of several
+essential JSON Object Signing and Encryption (JOSE) standards.
 
 This package contains implementation of:
 
 - RFC7515: JSON Web Signature
 - RFC7516: JSON Web Encryption
 - RFC7517: JSON Web Key
 - RFC7518: JSON Web Algorithms
@@ -67,12 +69,11 @@
 
 Useful Links
 ------------
 
 1. GitHub: https://github.com/authlib/joserfc
 2. Docs: https://jose.authlib.org/
 
-
 License
 -------
 
 Licensed under BSD. Please see LICENSE for licensing details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `joserfc-0.5.0/tests/test_util.py` & `joserfc-0.6.0/tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     def test_to_bytes(self):
         self.assertEqual(util.to_bytes(b'foo'), b'foo')
         self.assertEqual(util.to_bytes('foo'), b'foo')
         self.assertEqual(util.to_bytes(123), b'123')
         self.assertEqual(util.to_bytes([102, 111, 111]), b'foo')
 
     def test_to_unicode(self):
-        self.assertEqual(util.to_unicode(b'foo'), 'foo')
-        self.assertEqual(util.to_unicode('foo'), 'foo')
+        self.assertEqual(util.to_str(b'foo'), 'foo')
+        self.assertEqual(util.to_str('foo'), 'foo')
 
     def test_int_to_base64(self):
         self.assertRaises(
             ValueError,
             util.int_to_base64,
             -1
         )
```

