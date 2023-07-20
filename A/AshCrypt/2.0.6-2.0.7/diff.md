# Comparing `tmp/AshCrypt-2.0.6.tar.gz` & `tmp/AshCrypt-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-2.0.6.tar", last modified: Thu Jul 20 21:03:50 2023, max compression
+gzip compressed data, was "dist/AshCrypt-2.0.7.tar", last modified: Thu Jul 20 21:11:51 2023, max compression
```

## Comparing `AshCrypt-2.0.6.tar` & `AshCrypt-2.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/AshCryptGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-07-20 21:03:38.000000 AshCrypt-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-20 21:03:38.000000 AshCrypt-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/AshCryptGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/setup.py
```

### Comparing `AshCrypt-2.0.6/AshCrypt/AshCryptGUI.py` & `AshCrypt-2.0.7/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.6/AshCrypt/clicrypt.py` & `AshCrypt-2.0.7/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.6/AshCrypt/crypt.py` & `AshCrypt-2.0.7/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.6/AshCrypt/database.py` & `AshCrypt-2.0.7/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.6/AshCrypt/filecrypt.py` & `AshCrypt-2.0.7/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.6/AshCrypt/textcrypt.py` & `AshCrypt-2.0.7/AshCrypt/textcrypt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from AshCrypt import crypt
+from AshCrypt import crypt as cp
 from typing import Union
 
 
-
 class KeyLengthError(Exception):
     def __init__(self):
         self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
 
 
 class Crypt:
@@ -15,15 +14,15 @@
         if self.keyverify(key) == 1:
             self.key = key
         else:
             raise KeyError()
 
     @staticmethod
     def genkey() -> str:
-        return crypt.Enc.genkey()
+        return cp.Enc.genkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
         if isinstance(key, str):
             try:
                 a = bytes.fromhex(key.strip())
                 if len(a) == 32:
@@ -33,27 +32,27 @@
 
         else:
             return 2
 
     def encrypt(self) -> tuple:
         if self.text:
             try:
-                ins = crypt.Enc(self.text, self.key)
+                ins = cp.Enc(self.text, self.key)
                 new_content = ins.enc_to_str()
                 return 1, new_content
             except BaseException:
                 output = 'E'
                 return 0, output
         else:
             return 0.0, 0.0
 
     def decrypt(self) -> tuple:
         if self.text:
             try:
-                dec_instance = crypt.Dec(message=self.text, mainkey=self.key)
+                dec_instance = cp.Dec(message=self.text, mainkey=self.key)
                 a = dec_instance.dec_to_str()
                 output = a
                 return 1, output
             except Exception:
                 output = self.text
                 return 0, output
         else:
```

### Comparing `AshCrypt-2.0.6/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-2.0.7/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.6/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-2.0.7/AshCrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.6
+Version: 2.0.7
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.6/PKG-INFO` & `AshCrypt-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.6
+Version: 2.0.7
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.6/README.md` & `AshCrypt-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.6/setup.py` & `AshCrypt-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='2.0.6',
+    version='2.0.7',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

