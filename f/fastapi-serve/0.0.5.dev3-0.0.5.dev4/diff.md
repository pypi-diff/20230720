# Comparing `tmp/fastapi-serve-0.0.5.dev3.tar.gz` & `tmp/fastapi-serve-0.0.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.5.dev3.tar", last modified: Thu Jul 20 05:57:54 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.5.dev4.tar", last modified: Thu Jul 20 08:13:17 2023, max compression
```

## Comparing `fastapi-serve-0.0.5.dev3.tar` & `fastapi-serve-0.0.5.dev4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:57:54.046659 fastapi-serve-0.0.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-20 05:57:54.046659 fastapi-serve-0.0.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:57:54.042659 fastapi-serve-0.0.5.dev3/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 05:57:53.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:57:54.042659 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:57:54.042659 fastapi-serve-0.0.5.dev3/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:57:54.042659 fastapi-serve-0.0.5.dev3/fastapi_serve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/utils/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:57:54.046659 fastapi-serve-0.0.5.dev3/fastapi_serve/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/utils/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/utils/blob/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/fastapi_serve/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:57:54.042659 fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-20 05:57:54.000000 fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 05:57:54.000000 fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 05:57:54.000000 fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 05:57:54.000000 fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 05:57:54.000000 fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 05:57:54.000000 fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 05:57:54.000000 fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 05:57:54.046659 fastapi-serve-0.0.5.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-20 05:57:49.000000 fastapi-serve-0.0.5.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:17.693980 fastapi-serve-0.0.5.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-20 08:13:17.693980 fastapi-serve-0.0.5.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:17.689980 fastapi-serve-0.0.5.dev4/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 08:13:17.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:17.693980 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:17.693980 fastapi-serve-0.0.5.dev4/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:17.693980 fastapi-serve-0.0.5.dev4/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:17.693980 fastapi-serve-0.0.5.dev4/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:17.689980 fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-20 08:13:17.000000 fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 08:13:17.000000 fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:13:17.000000 fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 08:13:17.000000 fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:13:17.000000 fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 08:13:17.000000 fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 08:13:17.000000 fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:13:17.693980 fastapi-serve-0.0.5.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-20 08:13:13.000000 fastapi-serve-0.0.5.dev4/setup.py
```

### Comparing `fastapi-serve-0.0.5.dev3/LICENSE` & `fastapi-serve-0.0.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/PKG-INFO` & `fastapi-serve-0.0.5.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.5.dev3
+Version: 0.0.5.dev4
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.5.dev3 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.5.dev4 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.5.dev3/README.md` & `fastapi-serve-0.0.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/__main__.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,18 @@
     export_options,
     get_app_status_on_jcloud,
     get_jinaai_uri,
     hubble_push_options,
     jcloud_deploy_options,
     jcloud_list_options,
     list_apps_on_jcloud,
+    local_deploy_options,
     push_app_to_hubble,
     remove_app_on_jcloud,
+    serve_locally,
     serve_on_jcloud,
 )
 from fastapi_serve.helper import syncify
 
 
 @click.group()
 @click.version_option(__version__, "-v", "--version", prog_name="fastapi-serve")
@@ -47,18 +49,17 @@
 @serve.group(help="Deploy the app.")
 @click.help_option("-h", "--help")
 def deploy():
     pass
 
 
 @deploy.command(help="Deploy the app locally")
-@click.help_option("-h", "--help")
-@syncify
-async def local():
-    pass
+@local_deploy_options
+def local(app, port, env):
+    serve_locally(app=app, port=port, env=env)
 
 
 @deploy.command(help="Deploy the app to Jina AI Cloud")
 @jcloud_deploy_options
 @syncify
 async def jcloud(
     app,
```

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from tempfile import TemporaryDirectory
 from typing import Dict, List, Tuple
 
 import yaml
 from dotenv import dotenv_values
 
 from fastapi_serve.cloud.config import (
@@ -19,15 +20,15 @@
     asyncio_run_property,
     get_random_name,
 )
 from fastapi_serve.utils.helper import FlowUserEnvVar, get_jina_userid
 
 
 def get_gateway_config_yaml_path() -> str:
-    return os.path.join(os.path.dirname(__file__), 'config.yml')
+    return os.path.join(os.path.dirname(os.path.dirname(__file__)), 'config.yml')
 
 
 def get_gateway_uses(id: str) -> str:
     if id is not None:
         if id.startswith('jinahub+docker') or id.startswith('jinaai+docker'):
             return id
     return f'jinahub+docker://{id}'
@@ -337,14 +338,33 @@
     from jcloud.flow import CloudFlow
     from rich import print
 
     await CloudFlow(flow_id=app_id).__aexit__()
     print(f'App [bold][green]{app_id}[/green][/bold] removed successfully!')
 
 
+def serve_locally(
+    app: str,
+    port: int = 8080,
+    env: str = None,
+):
+    from jina import Flow
+
+    sys.path.append(os.getcwd())
+    f_yaml = get_flow_yaml(
+        app=app,
+        jcloud=False,
+        port=port,
+        env=env,
+    )
+    with Flow.load_config(f_yaml) as f:
+        # TODO: add local description
+        f.block()
+
+
 async def serve_on_jcloud(
     app: str,
     app_dir: str = None,
     name: str = APP_NAME,
     uses: str = None,
     app_id: str = None,
     version: str = 'latest',
```

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/export.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/export.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/cloud/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,36 @@
 from jcloud.constants import Phase
 
 from fastapi_serve.cloud.config import APP_NAME, validate_jcloud_config_callback
 from fastapi_serve.cloud.export import ExportKind
 
 _help_option = [click.help_option('-h', '--help')]
 
+_local_deploy_options = [
+    click.argument(
+        'app',
+        type=str,
+        required=True,
+    ),
+    click.option(
+        '--port',
+        type=int,
+        default=8080,
+        help='Port to be used for the FastAPI app.',
+        show_default=True,
+    ),
+    click.option(
+        '--env',
+        '--envs',
+        type=click.Path(exists=True),
+        help='Path to the environment file (should be a .env file)',
+        show_default=False,
+    ),
+]
+
 _common_options = [
     click.argument(
         'app',
         type=str,
         required=True,
     ),
     click.option(
@@ -159,21 +181,28 @@
         help='Name of the app.',
         show_default=True,
     ),
 ]
 
 
 __all__ = [
+    'local_deploy_options',
     'hubble_push_options',
     'jcloud_deploy_options',
     'jcloud_list_options',
     'export_options',
 ]
 
 
+def local_deploy_options(func):
+    for option in reversed(_local_deploy_options + _help_option):
+        func = option(func)
+    return func
+
+
 def hubble_push_options(func):
     for option in reversed(
         _common_options + _hubble_only_options + _hubble_common_options + _help_option
     ):
         func = option(func)
     return func
```

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/helper.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/utils/auth.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/utils/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/utils/blob/storage.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/utils/blob/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve/utils/helper.py` & `fastapi-serve-0.0.5.dev4/fastapi_serve/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.5.dev3
+Version: 0.0.5.dev4
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.5.dev3 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.5.dev4 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.5.dev3/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.5.dev4/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.5.dev3/setup.py` & `fastapi-serve-0.0.5.dev4/setup.py`

 * *Files identical despite different names*

