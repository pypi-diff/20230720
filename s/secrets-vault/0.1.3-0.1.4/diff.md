# Comparing `tmp/secrets-vault-0.1.3.tar.gz` & `tmp/secrets-vault-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.3.tar", last modified: Thu Jul 20 15:11:18 2023, max compression
+gzip compressed data, was "secrets-vault-0.1.4.tar", last modified: Thu Jul 20 15:57:34 2023, max compression
```

## Comparing `secrets-vault-0.1.3.tar` & `secrets-vault-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/secrets_vault/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:11:18.000000 secrets-vault-0.1.3/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:11:18.943743 secrets-vault-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-20 15:11:02.000000 secrets-vault-0.1.3/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:57:34.404354 secrets-vault-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-20 15:57:34.404354 secrets-vault-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:57:34.400354 secrets-vault-0.1.4/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/secrets_vault/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:57:34.400354 secrets-vault-0.1.4/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:57:34.404354 secrets-vault-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:57:34.400354 secrets-vault-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/tests/test_e2e.py
```

### Comparing `secrets-vault-0.1.3/LICENSE` & `secrets-vault-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.3/PKG-INFO` & `secrets-vault-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -97,14 +97,32 @@
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 vault.set('foo', 'bar')
 vault.persist()
 ```
 
+### Deleting secrets
+
+You can delete secrets from the CLI with a key:
+
+```bash
+$ secrets-vault del foo
+```
+
+Or via the application code like this:
+
+```python
+from secrets_vault import SecretsVault
+
+vault = SecretsVault()
+vault.delete('foo')
+vault.persist()
+```
+
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
 ### Environment variable
 You can also provide it via an environment variable `MASTER_KEY`. For example:
@@ -136,14 +154,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.4
+- Add del command
+
 ### 0.1.3
 - Add set command
 
 ### 0.1.2
 - Initial release
```

### Comparing `secrets-vault-0.1.3/README.md` & `secrets-vault-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,32 @@
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 vault.set('foo', 'bar')
 vault.persist()
 ```
 
+### Deleting secrets
+
+You can delete secrets from the CLI with a key:
+
+```bash
+$ secrets-vault del foo
+```
+
+Or via the application code like this:
+
+```python
+from secrets_vault import SecretsVault
+
+vault = SecretsVault()
+vault.delete('foo')
+vault.persist()
+```
+
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
 ### Environment variable
 You can also provide it via an environment variable `MASTER_KEY`. For example:
@@ -121,14 +139,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.4
+- Add del command
+
 ### 0.1.3
 - Add set command
 
 ### 0.1.2
 - Initial release
```

### Comparing `secrets-vault-0.1.3/secrets_vault/__init__.py` & `secrets-vault-0.1.4/secrets_vault/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,15 @@
         secrets_filepath=DEFAULT_SECRETS_FILEPATH,
         master_key_filepath=DEFAULT_MASTER_KEY_FILEPATH,
     ):
         """
         Create a new secrets file and returns the master key - keep it safe!
         """
         if Path(secrets_filepath).exists():
-            raise SecretsFileAlreadyExists(
-                f"Secrets file {secrets_filepath} already exists"
-            )
+            raise SecretsFileAlreadyExists(f"Secrets file {secrets_filepath} already exists")
 
         log.info(f"Creating new secrets file {secrets_filepath}")
         Path(secrets_filepath).touch()
 
         master_key = Fernet.generate_key().decode()
         with open(master_key_filepath, "w") as fout:
             fout.write(master_key)
@@ -70,14 +68,18 @@
 
     def get(self, key, default=None):
         return self.secrets.get(key, default)
 
     def set(self, key, value):
         self.secrets[key] = value
 
+    def delete(self, key):
+        if key in self.secrets:
+            del self.secrets[key]
+
     def edit_secrets(self):
         """
         Decrypts and opens the secrets file in an editor. On save, the file is encrypted again.
         """
         self._load_secrets()
         EDITOR = os.environ.get("EDITOR", "vim").split(" ")  # 'could be "code --wait"'
         with tempfile.NamedTemporaryFile(suffix=".tmp.yml") as tf:
@@ -97,34 +99,28 @@
         with open(self.secrets_filename, "wb") as fout:
             fout.write(self.fernet.encrypt(self._serialize()))
         log.info(f"Wrote encrypted secrets to {self.secrets_filename}")
 
     @staticmethod
     def _load_master_key(master_key_filepath=None):
         master_key = os.environ.get("MASTER_KEY")
-        if (
-            not master_key
-            and master_key_filepath
-            and os.path.exists(master_key_filepath)
-        ):
+        if not master_key and master_key_filepath and os.path.exists(master_key_filepath):
             with open(Path(master_key_filepath).absolute()) as fin:
                 master_key = fin.read().strip()
         if not master_key:
             raise MasterKeyNotFound(
                 "Could not find encryption master key. "
                 f"Set it as an environment variable 'MASTER_KEY', or in a file '{master_key_filepath}'"
             )
         return master_key
 
     def _load_secrets(self):
         log.info(f"Loading encrypted secrets from {self.secrets_filename}")
         if not os.path.exists(self.secrets_filename):
-            raise SecretsFileNotFound(
-                f"Could not find secrets file {self.secrets_filename}"
-            )
+            raise SecretsFileNotFound(f"Could not find secrets file {self.secrets_filename}")
         with open(self.secrets_filename, "r") as fin:
             contents = fin.read()
             if contents:
                 self.secrets = json.loads(self.fernet.decrypt(contents))
             else:
                 self.secrets = dict()
```

### Comparing `secrets-vault-0.1.3/secrets_vault/__main__.py` & `secrets-vault-0.1.4/secrets_vault/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,96 @@
 import argparse
 import logging
 
 from secrets_vault import SecretsVault, exceptions, constants
 
 
-def main():
-    parser = argparse.ArgumentParser(
-        description="Encrypt and decrypt a local secrets file using a master.key"
-    )
+def secrets_key_already_exists():
+    print("Secrets file already exists, skipping init")
+    exit(1)
 
-    parser.add_argument(
-        "-v", "--verbose", action="store_true", help="Enable verbose output"
+
+def no_master_key():
+    print(
+        f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{args.master_key_filepath}'"
     )
+    exit(1)
+
+
+def main():
+    parser = argparse.ArgumentParser(description="Encrypt and decrypt a local secrets file using a master.key")
+
+    parser.add_argument("-v", "--verbose", action="store_true", help="Enable verbose output")
     parser.add_argument(
         "-s",
         "--secrets-filepath",
         help=f"The location of the secrets file (default: {constants.DEFAULT_SECRETS_FILEPATH})",
     )
     parser.add_argument(
         "-m",
         "--master-key-filepath",
         help=f"The location of the master.key file (default: {constants.DEFAULT_MASTER_KEY_FILEPATH})",
     )
-    parser.add_argument(
-        "command", choices=["init", "get", "set", "edit"], help="Command to run"
-    )
+    parser.add_argument("command", choices=["init", "get", "set", "del", "edit"], help="Command to run")
     parser.add_argument(
         "key",
         nargs="?",
     )
     parser.add_argument(
         "value",
         nargs="?",
     )
 
     args = parser.parse_args()
 
     kwargs = {
         "secrets_filepath": args.secrets_filepath or constants.DEFAULT_SECRETS_FILEPATH,
-        "master_key_filepath": args.master_key_filepath
-        or constants.DEFAULT_MASTER_KEY_FILEPATH,
+        "master_key_filepath": args.master_key_filepath or constants.DEFAULT_MASTER_KEY_FILEPATH,
     }
 
     logging.basicConfig(level=logging.INFO if args.verbose else logging.ERROR)
 
     if args.command == "init":
         try:
             vault, master_key = SecretsVault.init()
-            print(
-                f"Generated new encryption master key:\n\n{master_key}\n\nKeep it safe! It will not be shown again."
-            )
+            print(f"Generated new encryption master key:\n\n{master_key}\n\nKeep it safe! It will not be shown again.")
         except exceptions.SecretsFileAlreadyExists:
-            print("Secrets file already exists, skipping init")
+            secrets_key_already_exists()
     elif args.command == "edit":
         try:
             SecretsVault(**kwargs).edit_secrets()
         except exceptions.MasterKeyNotFound:
-            print(
-                f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{args.master_key_filepath}'"
-            )
+            no_master_key()
     elif args.command == "get":
         try:
             vault = SecretsVault(**kwargs)
             if args.key:
                 print(vault.get(args.key))
             else:
                 for key, value in vault.secrets.items():
                     print(f"{key}: {value}")
         except exceptions.MasterKeyNotFound:
-            print(
-                f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{args.master_key_filepath}'"
-            )
+            no_master_key()
     elif args.command == "set":
         (args.key and args.value) or parser.error("key and value are required")
         try:
             vault = SecretsVault(**kwargs)
             vault.set(args.key, args.value)
             vault.persist()
+            no_master_key()
+        except exceptions.MasterKeyNotFound:
+            no_master_key()
+    elif args.command == "del":
+        args.key or parser.error("key is required")
+        try:
+            vault = SecretsVault(**kwargs)
+            vault.delete(args.key)
+            vault.persist()
         except exceptions.MasterKeyNotFound:
-            print(
-                f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{args.master_key_filepath}'"
-            )
+            no_master_key()
     else:
-        raise NotImplementedError(f"Unknown command {args.command}")
+        print(f"Unknown command {args.command}")
+        exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `secrets-vault-0.1.3/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.1.4/secrets_vault.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -97,14 +97,32 @@
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 vault.set('foo', 'bar')
 vault.persist()
 ```
 
+### Deleting secrets
+
+You can delete secrets from the CLI with a key:
+
+```bash
+$ secrets-vault del foo
+```
+
+Or via the application code like this:
+
+```python
+from secrets_vault import SecretsVault
+
+vault = SecretsVault()
+vault.delete('foo')
+vault.persist()
+```
+
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
 ### Environment variable
 You can also provide it via an environment variable `MASTER_KEY`. For example:
@@ -136,14 +154,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.4
+- Add del command
+
 ### 0.1.3
 - Add set command
 
 ### 0.1.2
 - Initial release
```

### Comparing `secrets-vault-0.1.3/setup.py` & `secrets-vault-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 
 setup(
     name="secrets-vault",
-    version="0.1.3",
+    version="0.1.4",
     author="Anthony N. Simon",
     url="https://github.com/anthonynsimon/secrets-vault",
     description="Simple encrypted secrets for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
@@ -26,11 +26,12 @@
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "secrets-vault=secrets_vault.__main__:main",
+            "secrets=secrets_vault.__main__:main",
         ]
     },
     tests_require=[],
 )
```

### Comparing `secrets-vault-0.1.3/tests/test_e2e.py` & `secrets-vault-0.1.4/tests/test_e2e.py`

 * *Files identical despite different names*

