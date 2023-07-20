# Comparing `tmp/secrets-vault-0.1.1.tar.gz` & `tmp/secrets-vault-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.1.tar", last modified: Thu Jul 20 13:56:59 2023, max compression
+gzip compressed data, was "secrets-vault-0.1.2.tar", last modified: Thu Jul 20 14:07:55 2023, max compression
```

## Comparing `secrets-vault-0.1.1.tar` & `secrets-vault-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-20 13:56:59.813350 secrets-vault-0.1.1/
--rw-r--r--   0 anthony    (501) staff       (20)     1070 2023-07-20 11:23:28.000000 secrets-vault-0.1.1/LICENSE
--rw-r--r--   0 anthony    (501) staff       (20)     4081 2023-07-20 13:56:59.813225 secrets-vault-0.1.1/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)     2682 2023-07-20 13:54:34.000000 secrets-vault-0.1.1/README.md
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-20 13:56:59.812158 secrets-vault-0.1.1/secrets_vault/
--rw-r--r--   0 anthony    (501) staff       (20)     4239 2023-07-20 13:34:23.000000 secrets-vault-0.1.1/secrets_vault/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     2584 2023-07-20 13:34:23.000000 secrets-vault-0.1.1/secrets_vault/__main__.py
--rw-r--r--   0 anthony    (501) staff       (20)       93 2023-07-20 13:34:21.000000 secrets-vault-0.1.1/secrets_vault/constants.py
--rw-r--r--   0 anthony    (501) staff       (20)      293 2023-07-20 13:34:21.000000 secrets-vault-0.1.1/secrets_vault/exceptions.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-20 13:56:59.812813 secrets-vault-0.1.1/secrets_vault.egg-info/
--rw-r--r--   0 anthony    (501) staff       (20)     4081 2023-07-20 13:56:59.000000 secrets-vault-0.1.1/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)      339 2023-07-20 13:56:59.000000 secrets-vault-0.1.1/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 anthony    (501) staff       (20)        1 2023-07-20 13:56:59.000000 secrets-vault-0.1.1/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 anthony    (501) staff       (20)       63 2023-07-20 13:56:59.000000 secrets-vault-0.1.1/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 anthony    (501) staff       (20)       14 2023-07-20 13:56:59.000000 secrets-vault-0.1.1/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 anthony    (501) staff       (20)       38 2023-07-20 13:56:59.813396 secrets-vault-0.1.1/setup.cfg
--rw-r--r--   0 anthony    (501) staff       (20)     1003 2023-07-20 13:54:29.000000 secrets-vault-0.1.1/setup.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-20 13:56:59.812924 secrets-vault-0.1.1/tests/
--rw-r--r--   0 anthony    (501) staff       (20)     3472 2023-07-20 13:35:15.000000 secrets-vault-0.1.1/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/secrets_vault/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 14:07:55.000000 secrets-vault-0.1.2/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:55.851503 secrets-vault-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-20 14:07:34.000000 secrets-vault-0.1.2/tests/test_e2e.py
```

### Comparing `secrets-vault-0.1.1/LICENSE` & `secrets-vault-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.1/README.md` & `secrets-vault-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
-### 0.1.1
+### 0.1.2
 - Initial release
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
```

### Comparing `secrets-vault-0.1.1/secrets_vault/__init__.py` & `secrets-vault-0.1.2/secrets_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.1/secrets_vault/__main__.py` & `secrets-vault-0.1.2/secrets_vault/__main__.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.1/setup.py` & `secrets-vault-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 
 setup(
     name="secrets-vault",
-    version="0.1.1",
+    version="0.1.2",
     author="Anthony N. Simon",
     url="https://github.com/anthonynsimon/secrets-vault",
     description="Simple encrypted secrets for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
```

### Comparing `secrets-vault-0.1.1/tests/test_e2e.py` & `secrets-vault-0.1.2/tests/test_e2e.py`

 * *Files identical despite different names*

