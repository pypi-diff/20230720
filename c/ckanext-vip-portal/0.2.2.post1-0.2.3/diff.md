# Comparing `tmp/ckanext-vip-portal-0.2.2.post1.tar.gz` & `tmp/ckanext-vip-portal-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-vip-portal-0.2.2.post1.tar", last modified: Thu Jun 22 18:24:00 2023, max compression
+gzip compressed data, was "ckanext-vip-portal-0.2.3.tar", last modified: Thu Jul 20 20:30:47 2023, max compression
```

## Comparing `ckanext-vip-portal-0.2.2.post1.tar` & `ckanext-vip-portal-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-22 18:24:00.878874 ckanext-vip-portal-0.2.2.post1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2.post1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      212 2023-03-03 00:11:02.000000 ckanext-vip-portal-0.2.2.post1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3720 2023-06-22 18:24:00.878874 ckanext-vip-portal-0.2.2.post1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3066 2023-06-22 18:22:24.000000 ckanext-vip-portal-0.2.2.post1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-22 18:24:00.878874 ckanext-vip-portal-0.2.2.post1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-24 14:50:12.000000 ckanext-vip-portal-0.2.2.post1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-22 18:24:00.878874 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-22 18:24:00.878874 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3350 2023-06-13 11:36:51.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2332 2023-06-22 18:21:49.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      850 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/interfaces.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3695 2023-05-21 19:59:13.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-22 18:24:00.878874 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-10-24 17:18:21.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      958 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/utils.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-22 18:24:00.878874 ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3720 2023-06-22 18:24:00.000000 ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2023-06-22 18:24:00.000000 ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-22 18:24:00.000000 ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-06-22 18:24:00.000000 ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-22 18:24:00.000000 ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       19 2023-06-22 18:24:00.000000 ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-22 18:24:00.000000 ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2927 2023-03-02 17:22:47.000000 ckanext-vip-portal-0.2.2.post1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1671 2023-06-22 18:24:00.888874 ckanext-vip-portal-0.2.2.post1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-24 14:50:12.000000 ckanext-vip-portal-0.2.2.post1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 20:30:47.540268 ckanext-vip-portal-0.2.3/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.3/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      212 2023-03-03 00:11:02.000000 ckanext-vip-portal-0.2.3/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3975 2023-07-20 20:30:47.540268 ckanext-vip-portal-0.2.3/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3327 2023-07-20 20:29:41.000000 ckanext-vip-portal-0.2.3/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 20:30:47.530261 ckanext-vip-portal-0.2.3/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-24 14:50:12.000000 ckanext-vip-portal-0.2.3/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 20:30:47.530261 ckanext-vip-portal-0.2.3/ckanext/vip_portal/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 20:30:47.540268 ckanext-vip-portal-0.2.3/ckanext/vip_portal/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/assets/script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/assets/style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3350 2023-06-13 11:36:51.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2332 2023-06-22 18:21:49.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      850 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/interfaces.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4008 2023-07-20 20:29:41.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 20:30:47.540268 ckanext-vip-portal-0.2.3/ckanext/vip_portal/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-10-24 17:18:21.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      958 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.3/ckanext/vip_portal/utils.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-20 20:30:47.540268 ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3975 2023-07-20 20:30:47.000000 ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2023-07-20 20:30:47.000000 ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-20 20:30:47.000000 ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-07-20 20:30:47.000000 ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-20 20:30:47.000000 ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       19 2023-07-20 20:30:47.000000 ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-20 20:30:47.000000 ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2927 2023-03-02 17:22:47.000000 ckanext-vip-portal-0.2.3/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1665 2023-07-20 20:30:47.540268 ckanext-vip-portal-0.2.3/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-24 14:50:12.000000 ckanext-vip-portal-0.2.3/setup.py
```

### Comparing `ckanext-vip-portal-0.2.2.post1/LICENSE` & `ckanext-vip-portal-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.2.post1/PKG-INFO` & `ckanext-vip-portal-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-vip-portal
-Version: 0.2.2.post1
+Version: 0.2.3
 Home-page: https://github.com/DataShades/ckanext-vip-portal
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -101,14 +101,20 @@
 ckanext.vip_portal.extra_allowed_prefixes = /dataset /organization /group /static
 
 # Allow anonymous user to access any path that ends with the following
 # suffixes
 # (optional, default: )
 ckanext.vip_portal.extra_allowed_suffixes = .svg .html .css
 
+# Allows to customize the route that the user will get redirected to
+# after a successful login. Empty value allow user to be redirected to the page 
+# requested before displaying login page
+# (optional, default: )
+ckan.auth.route_after_login = dataset.search
+
 ```
 
 
 ## Developer installation
 
 To install `ckanext-vip-portal` for development, activate your CKAN virtualenv and
 do:
```

### Comparing `ckanext-vip-portal-0.2.2.post1/README.md` & `ckanext-vip-portal-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,20 @@
 ckanext.vip_portal.extra_allowed_prefixes = /dataset /organization /group /static
 
 # Allow anonymous user to access any path that ends with the following
 # suffixes
 # (optional, default: )
 ckanext.vip_portal.extra_allowed_suffixes = .svg .html .css
 
+# Allows to customize the route that the user will get redirected to
+# after a successful login. Empty value allow user to be redirected to the page 
+# requested before displaying login page
+# (optional, default: )
+ckan.auth.route_after_login = dataset.search
+
 ```
 
 
 ## Developer installation
 
 To install `ckanext-vip-portal` for development, activate your CKAN virtualenv and
 do:
```

### Comparing `ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/config.py` & `ckanext-vip-portal-0.2.3/ckanext/vip_portal/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/config_declaration.yaml` & `ckanext-vip-portal-0.2.3/ckanext/vip_portal/config_declaration.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/interfaces.py` & `ckanext-vip-portal-0.2.3/ckanext/vip_portal/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/plugin.py` & `ckanext-vip-portal-0.2.3/ckanext/vip_portal/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 from typing import Optional
 
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
+import ckan.lib.helpers as h
 
 from . import config, utils, interfaces
 
 try:
     config_declarations = tk.blanket.config_declarations
 except AttributeError:
     def config_declarations(cls):
@@ -75,15 +76,21 @@
             resp = plugin.make_vip_rejection_response(user)
             if resp:
                 break
         else:
             if user:
                 resp = tk.abort(403, tk._("Not authorized to view this page"))
             else:
-                resp = tk.h.redirect_to(config.login_endpoint())
+                came_from = None
+                if tk.config.get("ckan.auth.route_after_login"):
+                    came_from = h.url_for(tk.config.get("ckan.auth.route_after_login"))
+                resp = tk.h.redirect_to(
+                    config.login_endpoint(),
+                    came_from=came_from or tk.request.path
+                )
 
         resp.headers.update(
             {
                 "cache-control": "no-cache, no-store, must-revalidate",
                 "pragma": "no-cache",
                 "expires": "0",
             }
```

### Comparing `ckanext-vip-portal-0.2.2.post1/ckanext/vip_portal/utils.py` & `ckanext-vip-portal-0.2.3/ckanext/vip_portal/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/PKG-INFO` & `ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-vip-portal
-Version: 0.2.2.post1
+Version: 0.2.3
 Home-page: https://github.com/DataShades/ckanext-vip-portal
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -101,14 +101,20 @@
 ckanext.vip_portal.extra_allowed_prefixes = /dataset /organization /group /static
 
 # Allow anonymous user to access any path that ends with the following
 # suffixes
 # (optional, default: )
 ckanext.vip_portal.extra_allowed_suffixes = .svg .html .css
 
+# Allows to customize the route that the user will get redirected to
+# after a successful login. Empty value allow user to be redirected to the page 
+# requested before displaying login page
+# (optional, default: )
+ckan.auth.route_after_login = dataset.search
+
 ```
 
 
 ## Developer installation
 
 To install `ckanext-vip-portal` for development, activate your CKAN virtualenv and
 do:
```

### Comparing `ckanext-vip-portal-0.2.2.post1/ckanext_vip_portal.egg-info/SOURCES.txt` & `ckanext-vip-portal-0.2.3/ckanext_vip_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.2.post1/pyproject.toml` & `ckanext-vip-portal-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.2.post1/setup.cfg` & `ckanext-vip-portal-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-vip-portal
-version = 0.2.2.post1
+version = 0.2.3
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-vip-portal
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-vip-portal-0.2.2.post1/setup.py` & `ckanext-vip-portal-0.2.3/setup.py`

 * *Files identical despite different names*

