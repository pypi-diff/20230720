# Comparing `tmp/keyrock-model-2023.3.17.1651.tar.gz` & `tmp/keyrock-model-2023.7.20.2017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrock-model-2023.3.17.1651.tar", last modified: Fri Mar 17 16:51:52 2023, max compression
+gzip compressed data, was "keyrock-model-2023.7.20.2017.tar", last modified: Thu Jul 20 20:17:30 2023, max compression
```

## Comparing `keyrock-model-2023.3.17.1651.tar` & `keyrock-model-2023.7.20.2017.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 16:51:52.296938 keyrock-model-2023.3.17.1651/
--rw-r--r--   0 root         (0) root         (0)       66 2023-03-17 16:51:52.296938 keyrock-model-2023.3.17.1651/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 16:51:52.294187 keyrock-model-2023.3.17.1651/keyrock_model/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-03-17 16:51:36.000000 keyrock-model-2023.3.17.1651/keyrock_model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 16:51:52.296938 keyrock-model-2023.3.17.1651/keyrock_model/model/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-03-17 16:51:36.000000 keyrock-model-2023.3.17.1651/keyrock_model/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-03-17 16:51:36.000000 keyrock-model-2023.3.17.1651/keyrock_model/model/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-03-17 16:51:36.000000 keyrock-model-2023.3.17.1651/keyrock_model/model/factory.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-03-17 16:51:36.000000 keyrock-model-2023.3.17.1651/keyrock_model/model/test_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 16:51:52.296021 keyrock-model-2023.3.17.1651/keyrock_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)       66 2023-03-17 16:51:52.000000 keyrock-model-2023.3.17.1651/keyrock_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2023-03-17 16:51:52.000000 keyrock-model-2023.3.17.1651/keyrock_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 16:51:52.000000 keyrock-model-2023.3.17.1651/keyrock_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-17 16:51:52.000000 keyrock-model-2023.3.17.1651/keyrock_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-17 16:51:52.000000 keyrock-model-2023.3.17.1651/keyrock_model.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-03-17 16:51:36.000000 keyrock-model-2023.3.17.1651/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-03-17 16:51:52.297854 keyrock-model-2023.3.17.1651/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:30.884525 keyrock-model-2023.7.20.2017/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-20 20:17:30.884525 keyrock-model-2023.7.20.2017/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:30.882525 keyrock-model-2023.7.20.2017/keyrock_model/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-20 20:17:19.000000 keyrock-model-2023.7.20.2017/keyrock_model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:30.884525 keyrock-model-2023.7.20.2017/keyrock_model/model/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-20 20:17:19.000000 keyrock-model-2023.7.20.2017/keyrock_model/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-07-20 20:17:19.000000 keyrock-model-2023.7.20.2017/keyrock_model/model/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-07-20 20:17:19.000000 keyrock-model-2023.7.20.2017/keyrock_model/model/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2023-07-20 20:17:19.000000 keyrock-model-2023.7.20.2017/keyrock_model/model/test_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:30.883525 keyrock-model-2023.7.20.2017/keyrock_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-20 20:17:30.000000 keyrock-model-2023.7.20.2017/keyrock_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2023-07-20 20:17:30.000000 keyrock-model-2023.7.20.2017/keyrock_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 20:17:30.000000 keyrock-model-2023.7.20.2017/keyrock_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 20:17:30.000000 keyrock-model-2023.7.20.2017/keyrock_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 20:17:30.000000 keyrock-model-2023.7.20.2017/keyrock_model.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-20 20:17:19.000000 keyrock-model-2023.7.20.2017/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-20 20:17:30.884525 keyrock-model-2023.7.20.2017/setup.cfg
```

