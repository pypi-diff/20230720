# Comparing `tmp/secrets-vault-0.1.2.tar.gz` & `tmp/secrets-vault-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.2.tar", last modified: Thu Jul 20 14:07:55 2023, max compression
+gzip compressed data, was "secrets-vault-0.1.3.tar", last modified: Thu Jul 20 15:11:18 2023, max compression
```

## Comparing `secrets-vault-0.1.2.tar` & `secrets-vault-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/secrets_vault/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/secrets_vault/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/tests/test_e2e.py
```

### Comparing `secrets-vault-0.1.2/LICENSE` & `secrets-vault-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.2/PKG-INFO` & `secrets-vault-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -62,18 +62,48 @@
 password = vault.get('my-password')
 
 ```
 
 
 ## Editing secrets
 
+### Interactive editor
+
 To edit secrets, run `secrets-vault edit`, the file will be decrypted and your editor will open.
 
+```bash
+$ secrets-vault edit
+
+>>> Opening secrets file in editor...
+{
+  "foo": "bar"
+}
+```
+
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
+### CLI command
+
+You can also set secrets from the CLI with a key and value:
+
+```bash
+$ secrets-vault set foo bar
+```
+
+### In code
+
+You can also edit secrets from code:
+
+```python
+from secrets_vault import SecretsVault
+
+vault = SecretsVault()
+vault.set('foo', 'bar')
+vault.persist()
+```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
 ### Environment variable
@@ -106,14 +136,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.3
+- Add set command
+
 ### 0.1.2
 - Initial release
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
```

### Comparing `secrets-vault-0.1.2/README.md` & `secrets-vault-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,48 @@
 password = vault.get('my-password')
 
 ```
 
 
 ## Editing secrets
 
+### Interactive editor
+
 To edit secrets, run `secrets-vault edit`, the file will be decrypted and your editor will open.
 
+```bash
+$ secrets-vault edit
+
+>>> Opening secrets file in editor...
+{
+  "foo": "bar"
+}
+```
+
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
+### CLI command
+
+You can also set secrets from the CLI with a key and value:
+
+```bash
+$ secrets-vault set foo bar
+```
+
+### In code
+
+You can also edit secrets from code:
+
+```python
+from secrets_vault import SecretsVault
+
+vault = SecretsVault()
+vault.set('foo', 'bar')
+vault.persist()
+```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
 ### Environment variable
@@ -91,14 +121,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.3
+- Add set command
+
 ### 0.1.2
 - Initial release
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
```

### Comparing `secrets-vault-0.1.2/secrets_vault/__init__.py` & `secrets-vault-0.1.3/secrets_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.2/secrets_vault/__main__.py` & `secrets-vault-0.1.3/secrets_vault/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,23 @@
     )
     parser.add_argument(
         "-m",
         "--master-key-filepath",
         help=f"The location of the master.key file (default: {constants.DEFAULT_MASTER_KEY_FILEPATH})",
     )
     parser.add_argument(
-        "command", choices=["init", "get", "edit"], help="Command to run"
+        "command", choices=["init", "get", "set", "edit"], help="Command to run"
     )
     parser.add_argument(
         "key",
         nargs="?",
-        help="When using the 'get' command, you can optionally provide a key to retrieve a specific item",
+    )
+    parser.add_argument(
+        "value",
+        nargs="?",
     )
 
     args = parser.parse_args()
 
     kwargs = {
         "secrets_filepath": args.secrets_filepath or constants.DEFAULT_SECRETS_FILEPATH,
         "master_key_filepath": args.master_key_filepath
@@ -64,13 +67,23 @@
             else:
                 for key, value in vault.secrets.items():
                     print(f"{key}: {value}")
         except exceptions.MasterKeyNotFound:
             print(
                 f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{args.master_key_filepath}'"
             )
+    elif args.command == "set":
+        (args.key and args.value) or parser.error("key and value are required")
+        try:
+            vault = SecretsVault(**kwargs)
+            vault.set(args.key, args.value)
+            vault.persist()
+        except exceptions.MasterKeyNotFound:
+            print(
+                f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{args.master_key_filepath}'"
+            )
     else:
         raise NotImplementedError(f"Unknown command {args.command}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `secrets-vault-0.1.2/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.1.3/secrets_vault.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -62,18 +62,48 @@
 password = vault.get('my-password')
 
 ```
 
 
 ## Editing secrets
 
+### Interactive editor
+
 To edit secrets, run `secrets-vault edit`, the file will be decrypted and your editor will open.
 
+```bash
+$ secrets-vault edit
+
+>>> Opening secrets file in editor...
+{
+  "foo": "bar"
+}
+```
+
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
+### CLI command
+
+You can also set secrets from the CLI with a key and value:
+
+```bash
+$ secrets-vault set foo bar
+```
+
+### In code
+
+You can also edit secrets from code:
+
+```python
+from secrets_vault import SecretsVault
+
+vault = SecretsVault()
+vault.set('foo', 'bar')
+vault.persist()
+```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
 ### Environment variable
@@ -106,14 +136,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.3
+- Add set command
+
 ### 0.1.2
 - Initial release
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
```

### Comparing `secrets-vault-0.1.2/setup.py` & `secrets-vault-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 
 setup(
     name="secrets-vault",
-    version="0.1.2",
+    version="0.1.3",
     author="Anthony N. Simon",
     url="https://github.com/anthonynsimon/secrets-vault",
     description="Simple encrypted secrets for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
```

### Comparing `secrets-vault-0.1.2/tests/test_e2e.py` & `secrets-vault-0.1.3/tests/test_e2e.py`

 * *Files identical despite different names*

