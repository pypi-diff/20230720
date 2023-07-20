# Comparing `tmp/configuretron-0.2.0.tar.gz` & `tmp/configuretron-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configuretron-0.2.0.tar", last modified: Thu Dec 29 18:20:36 2022, max compression
+gzip compressed data, was "configuretron-0.2.1.tar", last modified: Thu Jul 20 19:57:00 2023, max compression
```

## Comparing `configuretron-0.2.0.tar` & `configuretron-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 18:20:36.690513 configuretron-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-29 18:20:23.000000 configuretron-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2022-12-29 18:20:23.000000 configuretron-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-29 18:20:23.000000 configuretron-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-29 18:20:23.000000 configuretron-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-29 18:20:23.000000 configuretron-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2022-12-29 18:20:36.690513 configuretron-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2022-12-29 18:20:23.000000 configuretron-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 18:20:36.686513 configuretron-0.2.0/configuretron/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2022-12-29 18:20:23.000000 configuretron-0.2.0/configuretron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-29 18:20:23.000000 configuretron-0.2.0/configuretron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2022-12-29 18:20:23.000000 configuretron-0.2.0/configuretron/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2022-12-29 18:20:23.000000 configuretron-0.2.0/configuretron/configuretron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 18:20:36.686513 configuretron-0.2.0/configuretron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2022-12-29 18:20:36.000000 configuretron-0.2.0/configuretron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-29 18:20:36.000000 configuretron-0.2.0/configuretron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 18:20:36.000000 configuretron-0.2.0/configuretron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-29 18:20:36.000000 configuretron-0.2.0/configuretron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 18:20:36.000000 configuretron-0.2.0/configuretron.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-29 18:20:36.000000 configuretron-0.2.0/configuretron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-29 18:20:36.000000 configuretron-0.2.0/configuretron.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 18:20:36.690513 configuretron-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4853 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-29 18:20:23.000000 configuretron-0.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      385 2022-12-29 18:20:36.690513 configuretron-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2022-12-29 18:20:23.000000 configuretron-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 18:20:36.690513 configuretron-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-29 18:20:23.000000 configuretron-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-29 18:20:23.000000 configuretron-0.2.0/tests/config_basic.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2022-12-29 18:20:23.000000 configuretron-0.2.0/tests/config_encrypted.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2022-12-29 18:20:23.000000 configuretron-0.2.0/tests/private_key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2022-12-29 18:20:23.000000 configuretron-0.2.0/tests/test_configuretron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:59.997139 configuretron-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 19:56:48.000000 configuretron-0.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-20 19:56:48.000000 configuretron-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 19:56:48.000000 configuretron-0.2.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:56:48.000000 configuretron-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-20 19:56:48.000000 configuretron-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-20 19:56:59.997139 configuretron-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-20 19:56:48.000000 configuretron-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:59.993139 configuretron-0.2.1/configuretron/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-20 19:56:48.000000 configuretron-0.2.1/configuretron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-20 19:56:48.000000 configuretron-0.2.1/configuretron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-20 19:56:48.000000 configuretron-0.2.1/configuretron/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-20 19:56:48.000000 configuretron-0.2.1/configuretron/configuretron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:59.997139 configuretron-0.2.1/configuretron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-20 19:56:59.000000 configuretron-0.2.1/configuretron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 19:56:59.000000 configuretron-0.2.1/configuretron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:56:59.000000 configuretron-0.2.1/configuretron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 19:56:59.000000 configuretron-0.2.1/configuretron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:56:59.000000 configuretron-0.2.1/configuretron.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 19:56:59.000000 configuretron-0.2.1/configuretron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 19:56:59.000000 configuretron-0.2.1/configuretron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:59.997139 configuretron-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4853 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 19:56:48.000000 configuretron-0.2.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-20 19:56:59.997139 configuretron-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-20 19:56:48.000000 configuretron-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:56:59.997139 configuretron-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 19:56:48.000000 configuretron-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 19:56:48.000000 configuretron-0.2.1/tests/config_basic.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-20 19:56:48.000000 configuretron-0.2.1/tests/config_encrypted.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-20 19:56:48.000000 configuretron-0.2.1/tests/private_key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-20 19:56:48.000000 configuretron-0.2.1/tests/test_configuretron.py
```

### Comparing `configuretron-0.2.0/CONTRIBUTING.rst` & `configuretron-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/LICENSE` & `configuretron-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/PKG-INFO` & `configuretron-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuretron
-Version: 0.2.0
+Version: 0.2.1
 Summary: Configuration and Secrets for Python applications
 Home-page: https://github.com/channelcat/configuretron
 Author: Channel Cat
 Author-email: channelcat@gmail.com
 License: MIT license
 Keywords: configuretron
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `configuretron-0.2.0/README.rst` & `configuretron-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/configuretron/cli.py` & `configuretron-0.2.1/configuretron/cli.py`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/configuretron/configuretron.py` & `configuretron-0.2.1/configuretron/configuretron.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,45 @@
 import rsa
 from typing import Any, TypeVar
 import yaml
 
 T = TypeVar("T")
 
 
-def from_yaml(config_class: T, file: str, env: str = None, private_key: bytes = None) -> T:
+def from_yaml(
+    config_class: T,
+    file: str,
+    env: str = None,
+    private_key: bytes = None,
+    decrypt: bool = True,
+) -> T:
     config_dict = yaml_to_dict(file)
 
-    return from_dict(config_class=config_class, config_dict=config_dict, env=env, private_key=private_key)
-
-
-def from_dict(config_class: T, config_dict: dict, private_key: bytes = None, env: str = None) -> T:
-    config_args = dict_to_args(config_dict=config_dict, env=env, private_key=private_key)
+    return from_dict(
+        config_class=config_class,
+        config_dict=config_dict,
+        env=env,
+        private_key=private_key,
+        decrypt=decrypt,
+    )
+
+
+def from_dict(
+    config_class: T,
+    config_dict: dict,
+    env: str = None,
+    private_key: bytes = None,
+    decrypt: bool = True,
+) -> T:
+    config_args = dict_to_args(
+        config_dict=config_dict,
+        env=env,
+        private_key=private_key,
+        decrypt=decrypt,
+    )
 
     # Load data into dataclass
     try:
         config = config_class(**config_args)
     except Exception as e:
         raise ValueError(f"Configuration data does not match config class: {e}")
 
@@ -45,35 +68,48 @@
         config_dict = yaml.load(config_string, Loader=yaml.FullLoader)
     except Exception as e:
         raise SyntaxError(f"Cannot parse configuration file: {e}")
 
     return config_dict
 
 
-def dict_to_args(config_dict: dict, private_key: bytes = None, env: str = None):
+def dict_to_args(
+    config_dict: dict,
+    env: str = None,
+    private_key: bytes = None,
+    decrypt: bool = True,
+):
     if not "config" in config_dict:
         raise KeyError("Config is missing config section")
 
     # Copy new config
     config_args = dict(config_dict["config"])
 
     # Layer environment data
     if env is not None:
         overlay_config_env(config_dict, config_args, env)
 
     # Decrypt Secrets
-    if config_has_secrets(config_args):
-        if not private_key:
-            raise KeyError("Config has encrypted secrets, but no private key was provided")
-        try:
-            rsa_private_key = rsa.PrivateKey.load_pkcs1(private_key)
-        except Exception as e:
-            raise KeyError(f"Private key provided was invalid: {e}")
-
-        decrypt_config_keys(config_args, rsa_private_key)
+    if decrypt:
+        if config_has_secrets(config_args):
+            if not private_key:
+                raise KeyError(
+                    "Config has encrypted secrets, but no private key was provided"
+                )
+            try:
+                rsa_private_key = rsa.PrivateKey.load_pkcs1(private_key)
+            except Exception as e:
+                raise KeyError(f"Private key provided was invalid: {e}")
+
+            decrypt_config_keys(config_args, rsa_private_key)
+    else:
+        for key in list(config_args.keys()):
+            if key.endswith(".encrypted"):
+                config_args[key[:-10]] = None
+                del config_args[key]
 
     return config_args
 
 
 ################### Config Helpers ###################
```

### Comparing `configuretron-0.2.0/configuretron.egg-info/PKG-INFO` & `configuretron-0.2.1/configuretron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuretron
-Version: 0.2.0
+Version: 0.2.1
 Summary: Configuration and Secrets for Python applications
 Home-page: https://github.com/channelcat/configuretron
 Author: Channel Cat
 Author-email: channelcat@gmail.com
 License: MIT license
 Keywords: configuretron
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `configuretron-0.2.0/configuretron.egg-info/SOURCES.txt` & `configuretron-0.2.1/configuretron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/docs/Makefile` & `configuretron-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/docs/conf.py` & `configuretron-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/docs/installation.rst` & `configuretron-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/docs/make.bat` & `configuretron-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/setup.py` & `configuretron-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     include_package_data=True,
     keywords="configuretron",
     name="configuretron",
     packages=find_packages(include=["configuretron", "configuretron.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/channelcat/configuretron",
-    version="0.2.0",
+    version="0.2.1",
     zip_safe=False,
 )
```

### Comparing `configuretron-0.2.0/tests/config_encrypted.yml` & `configuretron-0.2.1/tests/config_encrypted.yml`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/tests/private_key.pem` & `configuretron-0.2.1/tests/private_key.pem`

 * *Files identical despite different names*

### Comparing `configuretron-0.2.0/tests/test_configuretron.py` & `configuretron-0.2.1/tests/test_configuretron.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,19 +53,29 @@
     assert basic_config.test_inherit == "inherited"
     assert basic_config.test_override == "global"
     assert prod_config.test_inherit == "inherited"
     assert prod_config.test_override == "prod"
 
 
 def test_encryption():
-    config = configuretron.from_yaml(EncryptedConfig, ENCRYPTED_CONFIG_YAML, private_key=private_key)
+    config = configuretron.from_yaml(
+        EncryptedConfig, ENCRYPTED_CONFIG_YAML, private_key=private_key
+    )
     assert config.secret == "secret"
     assert config.secret_list == [1, 2, 3]
 
 
+def test_encryption_disable():
+    config = configuretron.from_yaml(
+        EncryptedConfig, ENCRYPTED_CONFIG_YAML, decrypt=False
+    )
+    assert config.secret == None
+    assert config.secret_list == None
+
+
 def test_command_line_interface():
     """Test the CLI."""
     runner = CliRunner()
     result = runner.invoke(cli.cli)
     assert result.exit_code == 0
     assert "Usage: " in result.output
     help_result = runner.invoke(cli.cli, ["--help"])
```

