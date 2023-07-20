# Comparing `tmp/hugie-0.3.0.tar.gz` & `tmp/hugie-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugie-0.3.0.tar", last modified: Fri Dec  9 19:55:52 2022, max compression
+gzip compressed data, was "hugie-0.3.1.tar", max compression
```

## Comparing `hugie-0.3.0.tar` & `hugie-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,11 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2022-12-09 19:55:52.374200 hugie-0.3.0/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1070 2022-11-04 11:34:23.000000 hugie-0.3.0/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3159 2022-12-09 19:55:52.374200 hugie-0.3.0/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     2682 2022-11-04 19:32:29.000000 hugie-0.3.0/README.md
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2022-12-09 19:55:52.374200 hugie-0.3.0/hugie/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2022-11-04 11:34:23.000000 hugie-0.3.0/hugie/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      250 2022-12-09 19:26:42.000000 hugie-0.3.0/hugie/cli.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3065 2022-12-09 19:26:42.000000 hugie-0.3.0/hugie/config.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     8914 2022-12-09 19:26:42.000000 hugie-0.3.0/hugie/endpoint.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     2141 2022-12-09 19:26:42.000000 hugie-0.3.0/hugie/models.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      306 2022-11-26 20:00:57.000000 hugie-0.3.0/hugie/settings.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      839 2022-11-26 17:16:05.000000 hugie-0.3.0/hugie/utils.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2022-12-09 19:55:52.374200 hugie-0.3.0/hugie.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3159 2022-12-09 19:55:52.000000 hugie-0.3.0/hugie.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      341 2022-12-09 19:55:52.000000 hugie-0.3.0/hugie.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2022-12-09 19:55:52.000000 hugie-0.3.0/hugie.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       40 2022-12-09 19:55:52.000000 hugie-0.3.0/hugie.egg-info/entry_points.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       90 2022-12-09 19:55:52.000000 hugie-0.3.0/hugie.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        6 2022-12-09 19:55:52.000000 hugie-0.3.0/hugie.egg-info/top_level.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      104 2022-11-04 11:34:23.000000 hugie-0.3.0/pyproject.toml
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      731 2022-12-09 19:55:52.374200 hugie-0.3.0/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2022-11-04 11:34:23.000000 hugie-0.3.0/setup.py
+-rw-r--r--   0        0        0     1070 2022-11-04 11:34:23.136928 hugie-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2809 2023-07-20 13:53:05.306209 hugie-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-09 22:06:47.311232 hugie-0.3.1/hugie/__init__.py
+-rw-r--r--   0        0        0      404 2023-07-20 13:53:05.306209 hugie-0.3.1/hugie/__main__.py
+-rw-r--r--   0        0        0     3077 2023-07-20 13:53:05.306209 hugie-0.3.1/hugie/config.py
+-rw-r--r--   0        0        0     9098 2023-07-20 13:53:05.306209 hugie-0.3.1/hugie/endpoint.py
+-rw-r--r--   0        0        0     2208 2023-07-20 13:53:05.306209 hugie-0.3.1/hugie/models.py
+-rw-r--r--   0        0        0      306 2023-03-09 22:06:47.311232 hugie-0.3.1/hugie/settings.py
+-rw-r--r--   0        0        0      839 2023-03-09 22:06:47.311232 hugie-0.3.1/hugie/utils.py
+-rw-r--r--   0        0        0      665 2023-07-20 13:59:54.593131 hugie-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 hugie-0.3.1/PKG-INFO
```

### Comparing `hugie-0.3.0/LICENSE` & `hugie-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hugie-0.3.0/PKG-INFO` & `hugie-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 Metadata-Version: 2.1
 Name: hugie
-Version: 0.3.0
-Summary: Package for managing huggingface inference endpoints
-Home-page: https://www.github.com/MantisAI/hfie
-Author: Matthew Upson, Nick Sorros
-Author-email: hi@mantisnlp.com
-Classifier: Programming Language :: Python :: 3
+Version: 0.3.1
+Summary: CLI for managing Hugging Face Inference Endpoints
+License: MIT
+Author: Matthew Upson
+Author-email: matt@mantisnlp.com
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: srsly (>=2.4.7,<3.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: wasabi (>=1.1.2,<2.0.0)
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
 
 # Hugie 🐻
 
 📖 Official [documentation](https://mantisai.github.io/hugie/)
 
 Hugie is a Command Line Interface (CLI) for working with the Huggingface Inference Endpoints API ([API docs](https://huggingface.co/docs/inference-endpoints/api_reference))
 
 # Getting started
 
-The package is pip installable and can be installed directly from github with:
+The package is pip installable and can be installed from PyPI
 
 ```
-pip install git+https://github.com/MantisAI/hugie.git
+pipx install hugie
 ```
 
 ⚠️  To get started, you must set your individual or organisation Huggingface token into an env var called `HUGGINGFACE_READ_TOKEN`.
 
 # Usage 📺
 
 tldr; watch the video:
 
 [![asciicast](https://asciinema.org/a/BkNNlNE8jTLbBa5rI5hPpdbIW.svg)](https://asciinema.org/a/BkNNlNE8jTLbBa5rI5hPpdbIW)
 
 # Commands ⌨️
 
 ```
+hugie
+>>>
+Usage: hugie [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help                          Show this message and exit.
+
+Commands:
+  config
+  endpoint
+  version   Show version.
+```
+
+# Endpoint
+
+```
 hugie endpoint --help
 >>>
 Usage: hugie endpoint[OPTIONS] COMMAND[ARGS]...
 
 Options:
   --help  Show this message and exit.
 
@@ -141,22 +163,23 @@
 ## For development
 
 Read our CONTRIBUTING.md then
 
 Create a virtual environment and install the package
 
 ```
-make virtualenv
+poetry install
 ```
 
 Run tests
 ```
 pytest
 ```
 
 To upload to PyPi run
-```
-python -m build
-twine upload dist/*
+
+``
+poetry publish
 ```
 
 you need the mantisnlp password to proceed. Ask Nick or Matt.
+
```

### Comparing `hugie-0.3.0/README.md` & `hugie-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,31 +2,47 @@
 
 📖 Official [documentation](https://mantisai.github.io/hugie/)
 
 Hugie is a Command Line Interface (CLI) for working with the Huggingface Inference Endpoints API ([API docs](https://huggingface.co/docs/inference-endpoints/api_reference))
 
 # Getting started
 
-The package is pip installable and can be installed directly from github with:
+The package is pip installable and can be installed from PyPI
 
 ```
-pip install git+https://github.com/MantisAI/hugie.git
+pipx install hugie
 ```
 
 ⚠️  To get started, you must set your individual or organisation Huggingface token into an env var called `HUGGINGFACE_READ_TOKEN`.
 
 # Usage 📺
 
 tldr; watch the video:
 
 [![asciicast](https://asciinema.org/a/BkNNlNE8jTLbBa5rI5hPpdbIW.svg)](https://asciinema.org/a/BkNNlNE8jTLbBa5rI5hPpdbIW)
 
 # Commands ⌨️
 
 ```
+hugie
+>>>
+Usage: hugie [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help                          Show this message and exit.
+
+Commands:
+  config
+  endpoint
+  version   Show version.
+```
+
+# Endpoint
+
+```
 hugie endpoint --help
 >>>
 Usage: hugie endpoint[OPTIONS] COMMAND[ARGS]...
 
 Options:
   --help  Show this message and exit.
 
@@ -126,22 +142,22 @@
 ## For development
 
 Read our CONTRIBUTING.md then
 
 Create a virtual environment and install the package
 
 ```
-make virtualenv
+poetry install
 ```
 
 Run tests
 ```
 pytest
 ```
 
 To upload to PyPi run
-```
-python -m build
-twine upload dist/*
+
+``
+poetry publish
 ```
 
 you need the mantisnlp password to proceed. Ask Nick or Matt.
```

### Comparing `hugie-0.3.0/hugie/config.py` & `hugie-0.3.1/hugie/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,18 @@
         config.provider.vendor = vendor
 
     if region:
         config.provider.region = region
 
     if overwrite:
         try:
-            srsly.write_json(path, config.dict())
+            srsly.write_json(path, config.model_dump())
             typer.secho(f"Updated config at {path}", fg=typer.colors.GREEN)
         except Exception:
             typer.secho(f"Failed to update config at {path}", fg=typer.colors.RED)
 
     else:
-        typer.secho(srsly.json_dumps(config.dict()), fg=typer.colors.YELLOW)
+        typer.secho(srsly.json_dumps(config.model_dump()), fg=typer.colors.YELLOW)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `hugie-0.3.0/hugie/endpoint.py` & `hugie-0.3.1/hugie/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 headers = {
     "Authorization": f"Bearer {settings.token}",
     "Content-Type": "application/json",
 }
 API_ERROR_MESSAGE = "An error occured while making the API call"
 
 
+class TokenNotSet(Exception):
+    def __str__(self):
+        return "You need to define a token using the environment variable HUGGINGFACE_READ_TOKEN"
+
+
+if not settings.token:
+    raise TokenNotSet
+
+
 @app.command("ls")
 @app.command("list")
 def list(
     json: Optional[bool] = typer.Option(
         None, "--json", help="Prints the full output in JSON."
     )
 ):
@@ -75,15 +84,15 @@
     """
     Create an endpoint
 
     Args:
         data (str): Path to JSON data to create the endpoint
     """
 
-    data = InferenceEndpointConfig.from_json(data).dict()
+    data = InferenceEndpointConfig.from_json(data).model_dump()
 
     try:
         response = requests.post(settings.endpoint_url, headers=headers, json=data)
         response.raise_for_status()
     except requests.exceptions.HTTPError as e:
         typer.secho("Error creating endpoint", fg=typer.colors.RED)
         raise SystemExit(e)
@@ -113,15 +122,15 @@
     json: Optional[bool] = typer.Option(
         None, "--json", help="Prints the full output in JSON."
     ),
 ):
     """
     Update an endpoint
     """
-    data = dict(InferenceEndpointConfig.from_json(data))
+    data = InferenceEndpointConfig.from_json(data).model_dump()
 
     try:
         response = requests.put(
             f"{settings.endpoint_url}/{name}", headers=headers, json=data
         )
     except requests.exceptions.HTTPError as e:
         if response.json().get("error"):
@@ -290,15 +299,15 @@
 
     info = response.json()
     url = info["status"]["url"]
 
     if input_file:
         data = load_json(input_file)
     else:
-        data = {"inputs": inputs, "parameters": {"top_k": 10}}
+        data = {"inputs": inputs}
 
     # Send a call to the endpoint
     try:
         response = requests.post(url, headers=headers, json=data)
         response.raise_for_status()
     except requests.exceptions.RequestException as e:
         typer.secho(API_ERROR_MESSAGE, fg=typer.colors.RED)
```

### Comparing `hugie-0.3.0/hugie/models.py` & `hugie-0.3.1/hugie/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import BaseModel, BaseSettings
+from pydantic import BaseModel
+from pydantic_settings import BaseSettings
+from typing import Optional
 
 from hugie.utils import load_json
 
 
 class ScalingModel(BaseModel):
     minReplica: int = 1
     maxReplica: int = 1
@@ -31,15 +33,15 @@
 
 
 class InferenceEndpointConfig(BaseSettings):
     """
     Config for the inference endpoint
     """
 
-    accountId: str = None
+    accountId: Optional[str] = None
     type: str = None
     compute: ComputeModel = ComputeModel()
     model: ModelModel = ModelModel()
     name: str = None
     provider: ProviderModel = ProviderModel()
 
     @classmethod
```

### Comparing `hugie-0.3.0/hugie/utils.py` & `hugie-0.3.1/hugie/utils.py`

 * *Files identical despite different names*

