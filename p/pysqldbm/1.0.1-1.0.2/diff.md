# Comparing `tmp/pysqldbm-1.0.1.tar.gz` & `tmp/pysqldbm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqldbm-1.0.1.tar", last modified: Thu Jul 20 07:57:08 2023, max compression
+gzip compressed data, was "pysqldbm-1.0.2.tar", last modified: Thu Jul 20 08:15:05 2023, max compression
```

## Comparing `pysqldbm-1.0.1.tar` & `pysqldbm-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:57:08.791784 pysqldbm-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-20 07:57:08.791784 pysqldbm-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 07:56:59.000000 pysqldbm-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 07:57:08.791784 pysqldbm-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 07:56:59.000000 pysqldbm-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:57:08.787784 pysqldbm-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:57:08.787784 pysqldbm-1.0.1/src/pysqldbm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 07:56:59.000000 pysqldbm-1.0.1/src/pysqldbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 07:56:59.000000 pysqldbm-1.0.1/src/pysqldbm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 07:56:59.000000 pysqldbm-1.0.1/src/pysqldbm/rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:57:08.791784 pysqldbm-1.0.1/src/pysqldbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-20 07:57:08.000000 pysqldbm-1.0.1/src/pysqldbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 07:57:08.000000 pysqldbm-1.0.1/src/pysqldbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:57:08.000000 pysqldbm-1.0.1/src/pysqldbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 07:57:08.000000 pysqldbm-1.0.1/src/pysqldbm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 07:57:08.000000 pysqldbm-1.0.1/src/pysqldbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 07:57:08.000000 pysqldbm-1.0.1/src/pysqldbm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:57:08.791784 pysqldbm-1.0.1/src/pysqldbm_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 07:56:59.000000 pysqldbm-1.0.1/src/pysqldbm_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-20 07:56:59.000000 pysqldbm-1.0.1/src/pysqldbm_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.928705 pysqldbm-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-20 08:15:05.928705 pysqldbm-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:15:05.928705 pysqldbm-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-20 08:14:58.000000 pysqldbm-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.924704 pysqldbm-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.924704 pysqldbm-1.0.2/src/pysqldbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm/rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.924704 pysqldbm-1.0.2/src/pysqldbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.924704 pysqldbm-1.0.2/src/pysqldbm_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm_cli/run.py
```

### Comparing `pysqldbm-1.0.1/PKG-INFO` & `pysqldbm-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqldbm
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library to wrap SQLdbm API
 Home-page: https://github.com/drewsonne/pysqldbm
 Author: Drew J. Sonne
 Author-email: drew.sonne@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pysqldbm-1.0.1/README.md` & `pysqldbm-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pysqldbm-1.0.1/setup.py` & `pysqldbm-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # The text of the README file
 with (Path(__file__).parent / "README.md").open(encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="pysqldbm",
-    version="1.0.1",
+    version = "1.0.2",
     url="https://github.com/drewsonne/pysqldbm",
     license="Apache",
     author="Drew J. Sonne",
     author_email="drew.sonne@gmail.com",
     description="A library to wrap SQLdbm API",
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `pysqldbm-1.0.1/src/pysqldbm/client.py` & `pysqldbm-1.0.2/src/pysqldbm/client.py`

 * *Files identical despite different names*

### Comparing `pysqldbm-1.0.1/src/pysqldbm/rest_client.py` & `pysqldbm-1.0.2/src/pysqldbm/rest_client.py`

 * *Files identical despite different names*

### Comparing `pysqldbm-1.0.1/src/pysqldbm.egg-info/PKG-INFO` & `pysqldbm-1.0.2/src/pysqldbm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqldbm
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library to wrap SQLdbm API
 Home-page: https://github.com/drewsonne/pysqldbm
 Author: Drew J. Sonne
 Author-email: drew.sonne@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pysqldbm-1.0.1/src/pysqldbm_cli/run.py` & `pysqldbm-1.0.2/src/pysqldbm_cli/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import inspect
 import json
-from typing import Union, Dict, List
+from types import GeneratorType
+from typing import Union, Dict, List, Generator
 
 import click
 
 import pysqldbm
 from pysqldbm.client import Client
 
 
@@ -13,15 +15,15 @@
 def run(ctx: click.Context, api_key: str):
     ctx.obj = pysqldbm.client(api_key)
 
 
 @run.command("list-projects")
 @click.pass_obj
 def list_projects(client: Client):
-    print_json(*client.list_projects())
+    print_json(client.list_projects())
 
 
 @run.command("get-project")
 @click.option("--id", "id_", type=int, required=True)
 @click.pass_obj
 def get(client: Client, id_: str):
     for project in client.list_projects():
@@ -31,15 +33,15 @@
 
 
 # Revisions
 @run.command("list-revisions")
 @click.option("--project-id", type=int, required=True)
 @click.pass_obj
 def list_revisions(client: Client, project_id: str):
-    print_json(*client.list_revisions(project_id))
+    print_json(client.list_revisions(project_id))
 
 
 @run.command("get-revision")
 @click.option("--project-id", type=int, required=True)
 @click.option("--revision-id", type=int, required=True)
 @click.pass_obj
 def get_revisions(client: Client, project_id: str, revision_id: str):
@@ -68,15 +70,15 @@
     print_json(client.get_last_ddl(project_id))
 
 
 @run.command("list-environments")
 @click.option("--project-id", type=int, required=True)
 @click.pass_obj
 def list_environments(client: Client, project_id: str):
-    print_json(*client.list_environments(project_id))
+    print_json(client.list_environments(project_id))
 
 
 @run.command("get-latest-alter-statement")
 @click.option("--project-id", type=int, required=True)
 @click.option("--raw/--no-raw", default=False)
 @click.pass_obj
 def get_latest_alter_statement(client: Client, project_id: str, raw: bool):
@@ -109,14 +111,17 @@
     )
     if raw:
         click.echo(statement)
     else:
         print_json({"statement": statement})
 
 
-def print_json(obj: Union[Dict, List[Dict]]):
+def print_json(obj: Union[Dict, List[Dict], Generator[Dict, None, None]]):
+    if isinstance(obj, GeneratorType):
+        obj = [o for o in obj]
+
     """Prints a JSON object to the console with syntax highlighting."""
     click.echo(click.style(json.dumps(obj, indent=2, sort_keys=True), fg="green"))
 
 
 if __name__ == "__main__":
     run()
```

