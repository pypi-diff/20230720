# Comparing `tmp/garrett-streamlit-auth0-0.2.0.3.tar.gz` & `tmp/garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garrett-streamlit-auth0-0.2.0.3.tar", last modified: Thu Jul 20 18:21:35 2023, max compression
+gzip compressed data, was "garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar", last modified: Thu Jul 20 18:11:48 2023, max compression
```

## Comparing `garrett-streamlit-auth0-0.2.0.3.tar` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:21:35.560865 garrett-streamlit-auth0-0.2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-20 18:21:20.000000 garrett-streamlit-auth0-0.2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 18:21:20.000000 garrett-streamlit-auth0-0.2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 18:21:35.560865 garrett-streamlit-auth0-0.2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-20 18:21:20.000000 garrett-streamlit-auth0-0.2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:21:35.560865 garrett-streamlit-auth0-0.2.0.3/auth0_component/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 18:21:20.000000 garrett-streamlit-auth0-0.2.0.3/auth0_component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:21:35.556865 garrett-streamlit-auth0-0.2.0.3/auth0_component/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:21:35.560865 garrett-streamlit-auth0-0.2.0.3/auth0_component/frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:21:35.560865 garrett-streamlit-auth0-0.2.0.3/auth0_component/frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   337460 2023-07-20 18:21:35.000000 garrett-streamlit-auth0-0.2.0.3/auth0_component/frontend/dist/assets/index.13833558.js
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-20 18:21:35.000000 garrett-streamlit-auth0-0.2.0.3/auth0_component/frontend/dist/assets/index.1dbfa948.css
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 18:21:35.000000 garrett-streamlit-auth0-0.2.0.3/auth0_component/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:21:35.560865 garrett-streamlit-auth0-0.2.0.3/garrett_streamlit_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 18:21:35.000000 garrett-streamlit-auth0-0.2.0.3/garrett_streamlit_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:21:35.000000 garrett-streamlit-auth0-0.2.0.3/garrett_streamlit_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:21:35.000000 garrett-streamlit-auth0-0.2.0.3/garrett_streamlit_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 18:21:35.000000 garrett-streamlit-auth0-0.2.0.3/garrett_streamlit_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:21:35.000000 garrett-streamlit-auth0-0.2.0.3/garrett_streamlit_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 18:21:20.000000 garrett-streamlit-auth0-0.2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:21:35.560865 garrett-streamlit-auth0-0.2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 18:21:20.000000 garrett-streamlit-auth0-0.2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   337460 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.13833558.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.1dbfa948.css
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/setup.py
```

### Comparing `garrett-streamlit-auth0-0.2.0.3/LICENSE` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/LICENSE`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.3/README.md` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/README.md`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.3/auth0_component/__init__.py` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/__init__.py`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.3/auth0_component/frontend/dist/assets/index.13833558.js` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.13833558.js`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.3/auth0_component/frontend/dist/assets/index.1dbfa948.css` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.1dbfa948.css`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.3/setup.py` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/setup.py`

 * *Files identical despite different names*

