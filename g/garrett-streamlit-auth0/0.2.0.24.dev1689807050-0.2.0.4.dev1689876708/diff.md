# Comparing `tmp/garrett-streamlit-auth0-0.2.0.24.dev1689807050.tar.gz` & `tmp/garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garrett-streamlit-auth0-0.2.0.24.dev1689807050.tar", last modified: Wed Jul 19 22:50:50 2023, max compression
+gzip compressed data, was "garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar", last modified: Thu Jul 20 18:11:48 2023, max compression
```

## Comparing `garrett-streamlit-auth0-0.2.0.24.dev1689807050.tar` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:50:50.369449 garrett-streamlit-auth0-0.2.0.24.dev1689807050/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-19 22:50:34.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 22:50:34.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-19 22:50:50.369449 garrett-streamlit-auth0-0.2.0.24.dev1689807050/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-19 22:50:34.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:50:50.361449 garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-19 22:50:34.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:50:50.357449 garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:50:50.361449 garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:50:50.365449 garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   337460 2023-07-19 22:50:49.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/frontend/dist/assets/index.13833558.js
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-19 22:50:49.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/frontend/dist/assets/index.1dbfa948.css
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-19 22:50:49.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:50:50.369449 garrett-streamlit-auth0-0.2.0.24.dev1689807050/garrett_streamlit_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-19 22:50:50.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/garrett_streamlit_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-19 22:50:50.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/garrett_streamlit_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:50:50.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/garrett_streamlit_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 22:50:50.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/garrett_streamlit_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 22:50:50.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/garrett_streamlit_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-19 22:50:34.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 22:50:50.369449 garrett-streamlit-auth0-0.2.0.24.dev1689807050/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-19 22:50:34.000000 garrett-streamlit-auth0-0.2.0.24.dev1689807050/setup.py
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

### Comparing `garrett-streamlit-auth0-0.2.0.24.dev1689807050/LICENSE` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/LICENSE`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.24.dev1689807050/README.md` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Welcome to Auth0-Streamlit
 
 **The fastest way to provide comprehensive login inside Streamlit**
 
 ![Example of Streamlit-Auth0|635x380](demo.gif?raw=true)
 
 ## Installation
-`pip install streamlit-auth0-component`
+`pip install garrett-streamlit-auth0`
 
 ## Setup
 
 - Register for Auth0
 - Create a Single Page Application and navigate to the "settings" tab 
 - set your callback url's to `http://localhost:8501/component/auth0_component.login_button/index.html` assuming you're running on localhost or `http://YOUR_DOMAIN/component/auth0_component.login_button/index.html` if you're deploying
 - Copy `client_id` and `domain` from this page
```

### Comparing `garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/__init__.py` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import streamlit.components.v1 as components
 
-_RELEASE = False
-# _RELEASE = True
+# _RELEASE = False
+_RELEASE = True
 
 
 if not _RELEASE:
     _login_button = components.declare_component(
         "login_button",
         url="http://localhost:3000",  # vite dev server port
     )
```

### Comparing `garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/frontend/dist/assets/index.13833558.js` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.13833558.js`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.24.dev1689807050/auth0_component/frontend/dist/assets/index.1dbfa948.css` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.1dbfa948.css`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.24.dev1689807050/setup.py` & `garrett-streamlit-auth0-0.2.0.4.dev1689876708/setup.py`

 * *Files identical despite different names*

