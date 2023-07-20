# Comparing `tmp/alis_build_client-0.0.1.tar.gz` & `tmp/alis_build_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alis_build_client-0.0.1.tar", max compression
+gzip compressed data, was "alis_build_client-0.0.2.tar", max compression
```

## Comparing `alis_build_client-0.0.1.tar` & `alis_build_client-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      776 2023-07-14 08:58:21.794233 alis_build_client-0.0.1/README.md
--rw-r--r--   0        0        0       75 2023-07-14 08:48:39.896818 alis_build_client-0.0.1/alis/build/client/__init__.py
--rw-r--r--   0        0        0     2770 2023-07-16 16:35:27.451293 alis_build_client-0.0.1/alis/build/client/grpc.py
--rw-r--r--   0        0        0      809 2023-07-20 09:00:42.253078 alis_build_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1622 1970-01-01 00:00:00.000000 alis_build_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      958 2023-07-20 09:58:07.011522 alis_build_client-0.0.2/README.md
+-rw-r--r--   0        0        0       75 2023-07-14 08:48:39.896818 alis_build_client-0.0.2/alis/build/client/__init__.py
+-rw-r--r--   0        0        0     2770 2023-07-16 16:35:27.451293 alis_build_client-0.0.2/alis/build/client/grpc.py
+-rw-r--r--   0        0        0      809 2023-07-20 09:58:19.142038 alis_build_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 alis_build_client-0.0.2/PKG-INFO
```

### Comparing `alis_build_client-0.0.1/README.md` & `alis_build_client-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,11 +4,19 @@
 ## Usage
 Before you can use this project, you need to install [Poetry](https://python-poetry.org/docs/), a tool for dependency management and packaging in Python.
 On Unix-based systems (like Linux and MacOS), you can install Poetry using this command:
 ```bash
 curl -sSL https://install.python-poetry.org | python3 -
 ```
 
-To run tests, from `alis-build-client/alis/build`: ```python -m unittest discover test```
-To install the package locally: ```poetry install```
-To build the package: ```poetry build```
-To publish the package: ```poetry config pypi-token.pypi <your-pypi-token> && poetry publish```
+- To run tests, from `alis-build-client/alis/build`: ```python -m unittest discover test``` \
+- To install the package locally: ```poetry install``` \
+- To build the package: ```poetry build``` \
+- To publish the package: \
+    - Populate dist/ by building the package from source \
+    - Set up ~/.pypirc \
+```[pypi]
+    username = __token__
+    password = <API_KEY>```
+    - Publish dist/ with twine \
+```pip install twine```
+```twine upload -r pypi dist/*```
```

### Comparing `alis_build_client-0.0.1/alis/build/client/grpc.py` & `alis_build_client-0.0.2/alis/build/client/grpc.py`

 * *Files identical despite different names*

### Comparing `alis_build_client-0.0.1/pyproject.toml` & `alis_build_client-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "alis-build-client"
-version = "0.0.1"
+version = "0.0.2"
 description = "A grpc client package for python applications."
 authors = ["Thomas Scholtz <tom.scholtz@alisx.com>"]
 readme = "README.md"
 homepage = "https://github.com/yourusername/grpc_client"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
```

