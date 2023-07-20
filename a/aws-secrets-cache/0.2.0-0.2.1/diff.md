# Comparing `tmp/aws_secrets_cache-0.2.0.tar.gz` & `tmp/aws_secrets_cache-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_secrets_cache-0.2.0.tar", max compression
+gzip compressed data, was "aws_secrets_cache-0.2.1.tar", max compression
```

## Comparing `aws_secrets_cache-0.2.0.tar` & `aws_secrets_cache-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1399 2023-07-18 13:24:45.732550 aws_secrets_cache-0.2.0/LICENSE
--rw-r--r--   0        0        0      386 2023-07-18 13:24:45.732550 aws_secrets_cache-0.2.0/README.md
--rw-r--r--   0        0        0     1922 2023-07-18 13:24:45.732550 aws_secrets_cache-0.2.0/aws_secrets_cache/__init__.py
--rw-r--r--   0        0        0      509 2023-07-18 13:24:45.732550 aws_secrets_cache-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 aws_secrets_cache-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1399 2023-07-20 12:25:20.494289 aws_secrets_cache-0.2.1/LICENSE
+-rw-r--r--   0        0        0      386 2023-07-20 12:25:20.494289 aws_secrets_cache-0.2.1/README.md
+-rw-r--r--   0        0        0     1908 2023-07-20 12:25:20.494289 aws_secrets_cache-0.2.1/aws_secrets_cache/__init__.py
+-rw-r--r--   0        0        0      509 2023-07-20 12:25:20.494289 aws_secrets_cache-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 aws_secrets_cache-0.2.1/PKG-INFO
```

### Comparing `aws_secrets_cache-0.2.0/LICENSE` & `aws_secrets_cache-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_secrets_cache-0.2.0/aws_secrets_cache/__init__.py` & `aws_secrets_cache-0.2.1/aws_secrets_cache/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                     'KmsKeyId': self.kms_key_id
                 })
             else:
                 raise err
         self.cache[key] = CacheEntry(value=val)
 
     def fetch_secret(self, key):
-        key = self.prefix + key
+        key = key
         found = self.client.get_secret_value(SecretId=key)
         value = found.get('SecretString') or found['SecretBinary']
         return CacheEntry(value=value)
 
     def __getitem__(self, key):
         key = self.prefix + key
         try:
```

### Comparing `aws_secrets_cache-0.2.0/PKG-INFO` & `aws_secrets_cache-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-secrets-cache
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: BSD-3-Clause
 Author: Łukasz Kostka
 Author-email: lukasz.kostka@mirumee.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

