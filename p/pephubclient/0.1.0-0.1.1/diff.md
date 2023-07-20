# Comparing `tmp/pephubclient-0.1.0.tar.gz` & `tmp/pephubclient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pephubclient-0.1.0.tar", last modified: Mon Apr 17 13:27:57 2023, max compression
+gzip compressed data, was "pephubclient-0.1.1.tar", last modified: Thu Jul 20 15:36:01 2023, max compression
```

## Comparing `pephubclient-0.1.0.tar` & `pephubclient-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:27:57.477575 pephubclient-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 13:27:44.000000 pephubclient-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 13:27:44.000000 pephubclient-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-17 13:27:57.477575 pephubclient-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-17 13:27:44.000000 pephubclient-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:27:57.477575 pephubclient-0.1.0/pephubclient/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/files_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:27:57.477575 pephubclient-0.1.0/pephubclient/pephub_oauth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/pephub_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/pephub_oauth/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/pephub_oauth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/pephub_oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/pephub_oauth/pephub_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-17 13:27:44.000000 pephubclient-0.1.0/pephubclient/pephubclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:27:57.477575 pephubclient-0.1.0/pephubclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-17 13:27:57.000000 pephubclient-0.1.0/pephubclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-17 13:27:57.000000 pephubclient-0.1.0/pephubclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:27:57.000000 pephubclient-0.1.0/pephubclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 13:27:57.000000 pephubclient-0.1.0/pephubclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 13:27:57.000000 pephubclient-0.1.0/pephubclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 13:27:57.000000 pephubclient-0.1.0/pephubclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:27:57.477575 pephubclient-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 13:27:44.000000 pephubclient-0.1.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:27:44.000000 pephubclient-0.1.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 13:27:44.000000 pephubclient-0.1.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:27:57.477575 pephubclient-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-17 13:27:44.000000 pephubclient-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:01.214481 pephubclient-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-20 15:35:49.000000 pephubclient-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 15:35:49.000000 pephubclient-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-20 15:36:01.214481 pephubclient-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-20 15:35:49.000000 pephubclient-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:01.206481 pephubclient-0.1.1/pephubclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:01.210481 pephubclient-0.1.1/pephubclient/pephub_oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/pephub_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/pephub_oauth/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/pephub_oauth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/pephub_oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/pephub_oauth/pephub_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-07-20 15:35:49.000000 pephubclient-0.1.1/pephubclient/pephubclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:01.206481 pephubclient-0.1.1/pephubclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-20 15:36:01.000000 pephubclient-0.1.1/pephubclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-20 15:36:01.000000 pephubclient-0.1.1/pephubclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:36:01.000000 pephubclient-0.1.1/pephubclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 15:36:01.000000 pephubclient-0.1.1/pephubclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 15:36:01.000000 pephubclient-0.1.1/pephubclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:36:01.000000 pephubclient-0.1.1/pephubclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:01.210481 pephubclient-0.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 15:35:49.000000 pephubclient-0.1.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:35:49.000000 pephubclient-0.1.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 15:35:49.000000 pephubclient-0.1.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:36:01.214481 pephubclient-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-20 15:35:49.000000 pephubclient-0.1.1/setup.py
```

### Comparing `pephubclient-0.1.0/LICENSE.txt` & `pephubclient-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pephubclient-0.1.0/PKG-INFO` & `pephubclient-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pephubclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: PEPhub command line interface.
 Home-page: https://github.com/databio/pephubclient/
 Author: Oleksandr Khoroshevskyi, Rafal Stepien
 License: BSD2
 Keywords: project,bioinformatics,metadata
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # `PEPHubClient`
 
 [![PEP compatible](https://pepkit.github.io/img/PEP-compatible-green.svg)](https://pepkit.github.io)
 ![Run pytests](https://github.com/pepkit/pephubclient/workflows/Run%20pytests/badge.svg)
+[![codecov](https://codecov.io/gh/pepkit/pephubclient/branch/dev/graph/badge.svg)](https://codecov.io/gh/pepkit/pephubclient)
 [![pypi-badge](https://img.shields.io/pypi/v/pephubclient)](https://pypi.org/project/pephubclient)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 `PEPHubClient` is a tool to provide Python API and CLI for [PEPhub](https://pephub.databio.org).
 
 `pephubclient` features: 
 1) `push` (upload) projects)
```

### Comparing `pephubclient-0.1.0/README.md` & `pephubclient-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # `PEPHubClient`
 
 [![PEP compatible](https://pepkit.github.io/img/PEP-compatible-green.svg)](https://pepkit.github.io)
 ![Run pytests](https://github.com/pepkit/pephubclient/workflows/Run%20pytests/badge.svg)
+[![codecov](https://codecov.io/gh/pepkit/pephubclient/branch/dev/graph/badge.svg)](https://codecov.io/gh/pepkit/pephubclient)
 [![pypi-badge](https://img.shields.io/pypi/v/pephubclient)](https://pypi.org/project/pephubclient)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 `PEPHubClient` is a tool to provide Python API and CLI for [PEPhub](https://pephub.databio.org).
 
 `pephubclient` features: 
 1) `push` (upload) projects)
```

### Comparing `pephubclient-0.1.0/pephubclient/cli.py` & `pephubclient-0.1.1/pephubclient/cli.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.1.0/pephubclient/constants.py` & `pephubclient-0.1.1/pephubclient/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Optional
 
 import pydantic
 from pydantic import BaseModel
 
-PEPHUB_BASE_URL = "https://pephub.databio.org/"
-# PEPHUB_BASE_URL = "http://0.0.0.0:8000/"
+# PEPHUB_BASE_URL = "https://pephub.databio.org/"
+PEPHUB_BASE_URL = "http://0.0.0.0:8000/"
 PEPHUB_PEP_API_BASE_URL = f"{PEPHUB_BASE_URL}api/v1/projects/"
 PEPHUB_PUSH_URL = f"{PEPHUB_BASE_URL}api/v1/namespaces/{{namespace}}/projects/json"
 
 
 class RegistryPath(BaseModel):
     protocol: Optional[str]
     namespace: str
```

### Comparing `pephubclient-0.1.0/pephubclient/exceptions.py` & `pephubclient-0.1.1/pephubclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.1.0/pephubclient/files_manager.py` & `pephubclient-0.1.1/pephubclient/files_manager.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.1.0/pephubclient/helpers.py` & `pephubclient-0.1.1/pephubclient/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,7 +78,9 @@
         func(**kwargs)
     except ConnectionError as err:
         MessageHandler.print_error(f"Failed to connect to server. Try later. {err}")
     except ResponseError as err:
         MessageHandler.print_error(f"{err}")
     except PEPExistsError as err:
         MessageHandler.print_warning(f"PEP already exists. {err}")
+    except OSError as err:
+        MessageHandler.print_error(f"{err}")
```

### Comparing `pephubclient-0.1.0/pephubclient/pephub_oauth/exceptions.py` & `pephubclient-0.1.1/pephubclient/pephub_oauth/exceptions.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.1.0/pephubclient/pephub_oauth/pephub_oauth.py` & `pephubclient-0.1.1/pephubclient/pephub_oauth/pephub_oauth.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.1.0/pephubclient/pephubclient.py` & `pephubclient-0.1.1/pephubclient/pephubclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 from typing import NoReturn, Optional
 
 import pandas as pd
 import peppy
+from peppy.const import NAME_KEY, DESC_KEY, CONFIG_KEY
 import requests
 import urllib3
 from pydantic.error_wrappers import ValidationError
 from ubiquerg import parse_registry_path
 
 from pephubclient.constants import (
     PEPHUB_PEP_API_BASE_URL,
@@ -141,15 +142,18 @@
         :return: None
         """
         jwt_data = FilesManager.load_jwt_data_from_file(self.PATH_TO_FILE_WITH_JWT)
         if name:
             project["name"] = name
 
         upload_data = ProjectUploadData(
-            pep_dict=project.to_dict(extended=True),
+            pep_dict=project.to_dict(
+                extended=True,
+                orient="records",
+            ),
             tag=tag,
             is_private=is_private,
             overwrite=force,
         )
         pephub_response = self.send_request(
             method="POST",
             url=self._build_push_request_url(namespace=namespace),
@@ -163,14 +167,18 @@
             )
         elif pephub_response.status_code == ResponseStatusCodes.CONFLICT:
             raise ResponseError(
                 "Project already exists. Set force to overwrite project."
             )
         elif pephub_response.status_code == ResponseStatusCodes.UNAUTHORIZED:
             raise ResponseError("Unauthorized! Failure in uploading project.")
+        elif pephub_response.status_code == ResponseStatusCodes.FORBIDDEN:
+            raise ResponseError(
+                "User does not have permission to write to this namespace!"
+            )
         else:
             raise ResponseError("Unexpected Response Error.")
         return None
 
     @staticmethod
     def _save_raw_pep(
         reg_path: str,
@@ -186,30 +194,30 @@
         """
         reg_path_model = RegistryPath(**parse_registry_path(reg_path))
         folder_path = FilesManager.create_project_folder(registry_path=reg_path_model)
 
         def full_path(fn: str) -> str:
             return os.path.join(folder_path, fn)
 
-        project_name = project_dict["name"]
+        project_name = project_dict[CONFIG_KEY][NAME_KEY]
         sample_table_filename = "sample_table.csv"
         yaml_full_path = full_path(f"{project_name}_config.yaml")
         sample_full_path = full_path(sample_table_filename)
         if not force:
             extant = [
                 p for p in [yaml_full_path, sample_full_path] if os.path.isfile(p)
             ]
             if extant:
                 raise PEPExistsError(
                     f"{len(extant)} file(s) exist(s): {', '.join(extant)}"
                 )
 
-        config_dict = project_dict.get("_config")
-        config_dict["name"] = project_name
-        config_dict["description"] = project_dict["description"]
+        config_dict = project_dict.get(CONFIG_KEY)
+        config_dict[NAME_KEY] = project_name
+        config_dict[DESC_KEY] = project_dict[CONFIG_KEY][DESC_KEY]
         config_dict["sample_table"] = sample_table_filename
 
         sample_pandas = pd.DataFrame(project_dict.get("_sample_dict", {}))
 
         subsample_list = [
             pd.DataFrame(sub_a) for sub_a in project_dict.get("_subsample_dict") or []
         ]
@@ -247,14 +255,16 @@
         Request PEPhub and return the requested project as peppy.Project object.
 
         :param registry_path: Project namespace, eg. "geo/GSE124224:tag"
         :param query_param: Optional variables to be passed to PEPhub
         :param jwt_data: JWT token.
         :return: Raw project in dict.
         """
+        if not jwt_data:
+            jwt_data = FilesManager.load_jwt_data_from_file(self.PATH_TO_FILE_WITH_JWT)
         query_param = query_param or {}
         query_param["raw"] = "true"
 
         self._set_registry_data(registry_path)
         pephub_response = self.send_request(
             method="GET",
             url=self._build_pull_request_url(query_param=query_param),
@@ -267,15 +277,17 @@
 
             # This step is necessary because of this issue: https://github.com/pepkit/pephub/issues/124
             return correct_proj_dict.dict(by_alias=True)
 
         if pephub_response.status_code == ResponseStatusCodes.NOT_EXIST:
             raise ResponseError("File does not exist, or you are unauthorized.")
         if pephub_response.status_code == ResponseStatusCodes.INTERNAL_ERROR:
-            raise ResponseError("Internal server error.")
+            raise ResponseError(
+                f"Internal server error. Unexpected return value. Error: {pephub_response.status_code}"
+            )
 
     def _set_registry_data(self, query_string: str) -> None:
         """
         Parse provided query string to extract project name, sample name, etc.
 
         :param query_string: Passed by user. Contain information needed to locate the project.
         :return: Parsed query string.
```

### Comparing `pephubclient-0.1.0/pephubclient.egg-info/PKG-INFO` & `pephubclient-0.1.1/pephubclient.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pephubclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: PEPhub command line interface.
 Home-page: https://github.com/databio/pephubclient/
 Author: Oleksandr Khoroshevskyi, Rafal Stepien
 License: BSD2
 Keywords: project,bioinformatics,metadata
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # `PEPHubClient`
 
 [![PEP compatible](https://pepkit.github.io/img/PEP-compatible-green.svg)](https://pepkit.github.io)
 ![Run pytests](https://github.com/pepkit/pephubclient/workflows/Run%20pytests/badge.svg)
+[![codecov](https://codecov.io/gh/pepkit/pephubclient/branch/dev/graph/badge.svg)](https://codecov.io/gh/pepkit/pephubclient)
 [![pypi-badge](https://img.shields.io/pypi/v/pephubclient)](https://pypi.org/project/pephubclient)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 `PEPHubClient` is a tool to provide Python API and CLI for [PEPhub](https://pephub.databio.org).
 
 `pephubclient` features: 
 1) `push` (upload) projects)
```

### Comparing `pephubclient-0.1.0/pephubclient.egg-info/SOURCES.txt` & `pephubclient-0.1.1/pephubclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pephubclient-0.1.0/setup.py` & `pephubclient-0.1.1/setup.py`

 * *Files identical despite different names*

