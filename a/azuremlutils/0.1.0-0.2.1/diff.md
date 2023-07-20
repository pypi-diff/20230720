# Comparing `tmp/azuremlutils-0.1.0.tar.gz` & `tmp/azuremlutils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azuremlutils-0.1.0.tar", max compression
+gzip compressed data, was "azuremlutils-0.2.1.tar", max compression
```

## Comparing `azuremlutils-0.1.0.tar` & `azuremlutils-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-07-20 17:19:26.986711 azuremlutils-0.1.0/LICENSE
--rw-r--r--   0        0        0     1863 2023-07-20 17:22:10.577503 azuremlutils-0.1.0/README.md
--rw-r--r--   0        0        0     2401 2023-07-20 18:45:13.975366 azuremlutils-0.1.0/azuremlutils/cluster.py
--rw-r--r--   0        0        0      845 2023-07-20 17:28:57.601671 azuremlutils-0.1.0/azuremlutils/credential.py
--rw-r--r--   0        0        0     1973 2023-07-20 18:45:13.960328 azuremlutils-0.1.0/azuremlutils/data.py
--rw-r--r--   0        0        0     2051 2023-07-20 18:45:13.988819 azuremlutils-0.1.0/azuremlutils/environment.py
--rw-r--r--   0        0        0      824 2023-07-20 18:45:13.977894 azuremlutils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 azuremlutils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 17:19:26.986711 azuremlutils-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2760 2023-07-20 21:25:13.761314 azuremlutils-0.2.1/README.md
+-rw-r--r--   0        0        0     2051 2023-07-20 21:15:29.127010 azuremlutils-0.2.1/azuremlutils/__init__.py
+-rw-r--r--   0        0        0     2401 2023-07-20 18:45:13.975366 azuremlutils-0.2.1/azuremlutils/cluster.py
+-rw-r--r--   0        0        0     2868 2023-07-20 21:13:49.075763 azuremlutils-0.2.1/azuremlutils/credential.py
+-rw-r--r--   0        0        0     1973 2023-07-20 18:45:13.960328 azuremlutils-0.2.1/azuremlutils/data.py
+-rw-r--r--   0        0        0     2051 2023-07-20 18:45:13.988819 azuremlutils-0.2.1/azuremlutils/environment.py
+-rw-r--r--   0        0        0      766 2023-07-20 21:25:32.724928 azuremlutils-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 azuremlutils-0.2.1/PKG-INFO
```

### Comparing `azuremlutils-0.1.0/LICENSE` & `azuremlutils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azuremlutils-0.1.0/README.md` & `azuremlutils-0.2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 Here is a simple example of how to use azuremlutils:
 
 ```python
 from azuremlutils import setup_infrastructure
 
 # Your original directory and configuration
 original_dir = <Your Original Directory>
-cfg = <Your Configuration>
+cfg = <Your Hydra Configuration>
 
 # Setting up the infrastructure
 azure_credential, data, compute, env = setup_infrastructure(cfg, original_dir)
 ```
 
 Please note that you need to provide your own directory and configuration parameters.
 
@@ -45,7 +45,22 @@
 # License
 
 This project is licensed under the MIT License - see the LICENSE.md file for details.
 
 
 Please modify the contents to better match your project requirements and details. For instance, you might want to add 
 more usage examples, a section about the project's dependencies, instructions for how to run tests, etc.
+
+
+# Versioning
+The versioning system that you mentioned, 0.0.0.0, is known as semantic versioning (SemVer). It's a versioning scheme 
+for software that aims to convey meaning about the underlying changes in a release.
+
+In general, SemVer's structure is MAJOR.MINOR.PATCH, where:
+
+* MAJOR version increments indicate incompatible API changes. This means a user may need to make changes to their 
+code to use the new version.
+* MINOR version increments indicate the addition of functionality in a backwards-compatible manner. This means new 
+features were added but existing functionality has not been removed or altered in a way that would break existing 
+usage.
+* PATCH version increments indicate backwards-compatible bug fixes. This means that issues or bugs within the software 
+have been fixed and it should be even more reliable without any changes to the existing API or functionality.
```

### Comparing `azuremlutils-0.1.0/azuremlutils/cluster.py` & `azuremlutils-0.2.1/azuremlutils/cluster.py`

 * *Files identical despite different names*

### Comparing `azuremlutils-0.1.0/azuremlutils/data.py` & `azuremlutils-0.2.1/azuremlutils/data.py`

 * *Files identical despite different names*

### Comparing `azuremlutils-0.1.0/azuremlutils/environment.py` & `azuremlutils-0.2.1/azuremlutils/environment.py`

 * *Files identical despite different names*

### Comparing `azuremlutils-0.1.0/pyproject.toml` & `azuremlutils-0.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 [tool.poetry]
 name = "azuremlutils"
-version = "0.1.0"
+version = "0.2.1"
 description = "azuremlutils is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects."
 authors = ["Henrique Malta <vlezyitalia@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 azure-ai-ml = "^1.8.0"
 urllib3 = "1.26.9"
 azure-identity = "^1.13.0"
-
-
-[tool.poetry.group.test.dependencies]
-pytest = "^7.4.0"
-pytest-mock = "^3.11.1"
-
+python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 yapf = "^0.40.1"
 pylint = "^2.17.4"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `azuremlutils-0.1.0/PKG-INFO` & `azuremlutils-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: azuremlutils
-Version: 0.1.0
+Version: 0.2.1
 Summary: azuremlutils is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects.
 License: MIT
 Author: Henrique Malta
 Author-email: vlezyitalia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-ai-ml (>=1.8.0,<2.0.0)
 Requires-Dist: azure-identity (>=1.13.0,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: urllib3 (==1.26.9)
 Description-Content-Type: text/markdown
 
 # azuremlutils
 azuremlutils is a Python utility package aimed at simplifying and streamlining workflows on Azure Machine Learning 
 (Azure ML). It provides a set of high-level APIs that make it easy to set up Azure ML infrastructure such as clusters 
 and environments, authenticate with Azure ML, and manage datasets. This package is designed with a focus on 
@@ -41,15 +42,15 @@
 Here is a simple example of how to use azuremlutils:
 
 ```python
 from azuremlutils import setup_infrastructure
 
 # Your original directory and configuration
 original_dir = <Your Original Directory>
-cfg = <Your Configuration>
+cfg = <Your Hydra Configuration>
 
 # Setting up the infrastructure
 azure_credential, data, compute, env = setup_infrastructure(cfg, original_dir)
 ```
 
 Please note that you need to provide your own directory and configuration parameters.
 
@@ -63,7 +64,21 @@
 
 This project is licensed under the MIT License - see the LICENSE.md file for details.
 
 
 Please modify the contents to better match your project requirements and details. For instance, you might want to add 
 more usage examples, a section about the project's dependencies, instructions for how to run tests, etc.
 
+
+# Versioning
+The versioning system that you mentioned, 0.0.0.0, is known as semantic versioning (SemVer). It's a versioning scheme 
+for software that aims to convey meaning about the underlying changes in a release.
+
+In general, SemVer's structure is MAJOR.MINOR.PATCH, where:
+
+* MAJOR version increments indicate incompatible API changes. This means a user may need to make changes to their 
+code to use the new version.
+* MINOR version increments indicate the addition of functionality in a backwards-compatible manner. This means new 
+features were added but existing functionality has not been removed or altered in a way that would break existing 
+usage.
+* PATCH version increments indicate backwards-compatible bug fixes. This means that issues or bugs within the software 
+have been fixed and it should be even more reliable without any changes to the existing API or functionality.
```

