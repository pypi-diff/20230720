# Comparing `tmp/pydantic_settings_yaml-0.1.3.tar.gz` & `tmp/pydantic_settings_yaml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_settings_yaml-0.1.3.tar", last modified: Thu Jul 20 07:08:43 2023, max compression
+gzip compressed data, was "pydantic_settings_yaml-0.2.0.tar", last modified: Thu Jul 20 08:36:23 2023, max compression
```

## Comparing `pydantic_settings_yaml-0.1.3.tar` & `pydantic_settings_yaml-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:43.426473 pydantic_settings_yaml-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:43.422473 pydantic_settings_yaml-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:43.426473 pydantic_settings_yaml-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/.github/workflows/test_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-20 07:08:43.426473 pydantic_settings_yaml-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 07:08:43.426473 pydantic_settings_yaml-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:43.422473 pydantic_settings_yaml-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:43.426473 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml/base_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:43.426473 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-20 07:08:43.000000 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-20 07:08:43.000000 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:08:43.000000 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 07:08:43.000000 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 07:08:43.000000 pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:43.426473 pydantic_settings_yaml-0.1.3/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:08:43.426473 pydantic_settings_yaml-0.1.3/src/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/src/tests/data/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/src/tests/data/database_password
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/src/tests/data/database_username
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/src/tests/test_base_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 07:08:34.000000 pydantic_settings_yaml-0.1.3/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:23.486558 pydantic_settings_yaml-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:23.482558 pydantic_settings_yaml-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:23.486558 pydantic_settings_yaml-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/.github/workflows/test_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-20 08:36:23.486558 pydantic_settings_yaml-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 08:36:23.486558 pydantic_settings_yaml-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:23.482558 pydantic_settings_yaml-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:23.486558 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml/base_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:23.486558 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-20 08:36:23.000000 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-20 08:36:23.000000 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:36:23.000000 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 08:36:23.000000 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 08:36:23.000000 pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:23.486558 pydantic_settings_yaml-0.2.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:36:23.486558 pydantic_settings_yaml-0.2.0/src/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/src/tests/data/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/src/tests/data/database_password
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/src/tests/data/database_username
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/src/tests/test_base_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 08:36:14.000000 pydantic_settings_yaml-0.2.0/test_requirements.txt
```

### Comparing `pydantic_settings_yaml-0.1.3/.github/workflows/test_and_publish.yml` & `pydantic_settings_yaml-0.2.0/.github/workflows/test_and_publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   test_before_publish:
     name: Test on Python ${{ matrix.python_version }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: ['3.7', '3.8', '3.9']
+        python_version: ['3.8', '3.9', '3.10', '3.11']
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python_version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python_version }}
     - name: Install dependencies
```

### Comparing `pydantic_settings_yaml-0.1.3/.gitignore` & `pydantic_settings_yaml-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic_settings_yaml-0.1.3/LICENSE` & `pydantic_settings_yaml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings_yaml-0.1.3/PKG-INFO` & `pydantic_settings_yaml-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Metadata-Version: 2.1
-Name: pydantic_settings_yaml
-Version: 0.1.3
-Summary: Yaml support for Pydantic settings
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pydantic-settings-yaml
 
+***Note: 2.x needs Pydantic>2.0,<3.0. Install 1.x if you still need Pydantic 1.x.***
 
 Yaml support for Pydantic settings. Load a yaml config file 
 as nested Pydantic models. 
 
 Allows to use <file:xxxx> placeholders in the yaml config file
 for secrets. A placeholder is replaced with the contents of the
 file. Paths are relative to the 'secrets_dir' setting (see below).
@@ -33,29 +25,30 @@
 ```
 
 
 Python code example:
 ``` 
     from pydantic import BaseModel
     from pydantic_settings_yaml import YamlBaseSettings
+    from pydantic_settings import SettingsConfigDict
 
     class Database(BaseModel):
         username: str
         password: str
 
 
     class Settings(YamlBaseSettings):
         database: Database
 
-        class Config:
-            secrets_dir = "/secrets"
-            yaml_file = "/config/config.yaml"
+        # configure paths to secrets directory and YAML config file
+        model_config = SettingsConfigDict(
+            secrets_dir="/secrets", yaml_file="/config/config.yaml")
 
     settings = Settings()
 
     assert settings.dict() == {
         "database": {
             "password": "my_secret_database_password", 
             "username": "my_database_username"
         }
     }
-```
+```
```

### Comparing `pydantic_settings_yaml-0.1.3/README.md` & `pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+Metadata-Version: 2.1
+Name: pydantic-settings-yaml
+Version: 0.2.0
+Summary: Yaml support for Pydantic settings
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pydantic-settings-yaml
 
+***Note: 2.x needs Pydantic>2.0,<3.0. Install 1.x if you still need Pydantic 1.x.***
 
 Yaml support for Pydantic settings. Load a yaml config file 
 as nested Pydantic models. 
 
 Allows to use <file:xxxx> placeholders in the yaml config file
 for secrets. A placeholder is replaced with the contents of the
 file. Paths are relative to the 'secrets_dir' setting (see below).
@@ -24,29 +34,30 @@
 ```
 
 
 Python code example:
 ``` 
     from pydantic import BaseModel
     from pydantic_settings_yaml import YamlBaseSettings
+    from pydantic_settings import SettingsConfigDict
 
     class Database(BaseModel):
         username: str
         password: str
 
 
     class Settings(YamlBaseSettings):
         database: Database
 
-        class Config:
-            secrets_dir = "/secrets"
-            yaml_file = "/config/config.yaml"
+        # configure paths to secrets directory and YAML config file
+        model_config = SettingsConfigDict(
+            secrets_dir="/secrets", yaml_file="/config/config.yaml")
 
     settings = Settings()
 
     assert settings.dict() == {
         "database": {
             "password": "my_secret_database_password", 
             "username": "my_database_username"
         }
     }
-```
+```
```

### Comparing `pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml.egg-info/PKG-INFO` & `pydantic_settings_yaml-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
-Name: pydantic-settings-yaml
-Version: 0.1.3
+Name: pydantic_settings_yaml
+Version: 0.2.0
 Summary: Yaml support for Pydantic settings
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydantic-settings-yaml
 
+***Note: 2.x needs Pydantic>2.0,<3.0. Install 1.x if you still need Pydantic 1.x.***
 
 Yaml support for Pydantic settings. Load a yaml config file 
 as nested Pydantic models. 
 
 Allows to use <file:xxxx> placeholders in the yaml config file
 for secrets. A placeholder is replaced with the contents of the
 file. Paths are relative to the 'secrets_dir' setting (see below).
@@ -33,26 +34,27 @@
 ```
 
 
 Python code example:
 ``` 
     from pydantic import BaseModel
     from pydantic_settings_yaml import YamlBaseSettings
+    from pydantic_settings import SettingsConfigDict
 
     class Database(BaseModel):
         username: str
         password: str
 
 
     class Settings(YamlBaseSettings):
         database: Database
 
-        class Config:
-            secrets_dir = "/secrets"
-            yaml_file = "/config/config.yaml"
+        # configure paths to secrets directory and YAML config file
+        model_config = SettingsConfigDict(
+            secrets_dir="/secrets", yaml_file="/config/config.yaml")
 
     settings = Settings()
 
     assert settings.dict() == {
         "database": {
             "password": "my_secret_database_password", 
             "username": "my_database_username"
```

### Comparing `pydantic_settings_yaml-0.1.3/src/pydantic_settings_yaml.egg-info/SOURCES.txt` & `pydantic_settings_yaml-0.2.0/src/pydantic_settings_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings_yaml-0.1.3/src/tests/test_base_settings.py` & `pydantic_settings_yaml-0.2.0/src/tests/test_base_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pathlib import Path
+from typing import List
 from unittest.mock import Mock
 
 import pytest
 from pydantic import BaseModel
+from pydantic_settings import SettingsConfigDict
 
 from pydantic_settings_yaml import YamlBaseSettings
 from pydantic_settings_yaml.base_settings import (
     replace_secrets,
     yaml_config_settings_source,
 )
 
@@ -50,61 +52,77 @@
     with pytest.raises(FileNotFoundError):
         replace_secrets(Path("src/tests/data"), data)
 
 
 @pytest.fixture()
 def mocked_yamlbasesettings():
     settings = Mock()
-    settings.__config__ = Mock()
-    settings.__config__.yaml_file = "src/tests/data/config.yaml"
-    settings.__config__.secrets_dir = "src/tests/data"
+    settings.model_config = SettingsConfigDict(
+        secrets_dir="src/tests/data", yaml_file="src/tests/data/config.yaml"
+    )
     return settings
 
 
 def test_yaml_config_settings_source(mocked_yamlbasesettings):
     data = yaml_config_settings_source(mocked_yamlbasesettings)
     assert data == {
+        "debug": True,
+        "allowed_hosts": [{"name": "domain.com"}, {"name": "example.com"}],
         "database": {
             "password": "dummy_database_password",
-            "username": "dummy_database_username",
-        }
+            "user": {"username": "dummy_database_username"},
+        },
     }
 
 
 def test_yaml_config_settings_source_no_files(mocked_yamlbasesettings):
-    mocked_yamlbasesettings.__config__.yaml_file = ""
+    mocked_yamlbasesettings.model_config["yaml_file"] = ""
     with pytest.raises(AssertionError):
         yaml_config_settings_source(mocked_yamlbasesettings)
 
-    mocked_yamlbasesettings.__config__.yaml_file = (
-        "/src/tests/data/not_existing_config.yaml"
-    )
+    mocked_yamlbasesettings.model_config[
+        "yaml_file"
+    ] = "/src/tests/data/not_existing_config.yaml"
     with pytest.raises(FileNotFoundError):
         yaml_config_settings_source(mocked_yamlbasesettings)
 
-    mocked_yamlbasesettings.__config__.yaml_file = "/src/tests/data/config.yaml"
-    mocked_yamlbasesettings.__config__.secrets_dir = None
+    mocked_yamlbasesettings.model_config["yaml_file"] = "/src/tests/data/config.yaml"
+    mocked_yamlbasesettings.model_config["secrets_dir"] = None
     with pytest.raises(AssertionError):
         yaml_config_settings_source(mocked_yamlbasesettings)
 
 
-class Database(BaseModel):
+class User(BaseModel):
     username: str
+
+
+class Database(BaseModel):
+    user: User
     password: str
 
 
+class Host(BaseModel):
+    name: str
+
+
 class Settings(YamlBaseSettings):
+    debug: bool = False
     database: Database
+    allowed_hosts: List[Host]
 
-    class Config:
-        secrets_dir = "src/tests/data"
-        yaml_file = "src/tests/data/config.yaml"
+    model_config = SettingsConfigDict(
+        secrets_dir="src/tests/data", yaml_file="src/tests/data/config.yaml"
+    )
 
 
 def test_yaml_base_settings():
     s = Settings()
-    assert s.dict() == {
+    assert s.model_dump() == {
+        "debug": True,
+        "allowed_hosts": [{"name": "domain.com"}, {"name": "example.com"}],
         "database": {
             "password": "dummy_database_password",
-            "username": "dummy_database_username",
-        }
+            "user": {
+                "username": "dummy_database_username",
+            },
+        },
     }
```

