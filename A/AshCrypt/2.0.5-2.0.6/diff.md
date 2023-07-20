# Comparing `tmp/AshCrypt-2.0.5.tar.gz` & `tmp/AshCrypt-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-2.0.5.tar", last modified: Wed Jul 19 09:53:15 2023, max compression
+gzip compressed data, was "dist/AshCrypt-2.0.6.tar", last modified: Thu Jul 20 21:03:50 2023, max compression
```

## Comparing `AshCrypt-2.0.5.tar` & `AshCrypt-2.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/AshCryptGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/AshCryptGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-20 21:03:37.000000 AshCrypt-2.0.6/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-07-20 21:03:38.000000 AshCrypt-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:03:50.000000 AshCrypt-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-20 21:03:38.000000 AshCrypt-2.0.6/setup.py
```

### Comparing `AshCrypt-2.0.5/AshCrypt/AshCryptGUI.py` & `AshCrypt-2.0.6/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.5/AshCrypt/clicrypt.py` & `AshCrypt-2.0.6/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.5/AshCrypt/crypt.py` & `AshCrypt-2.0.6/AshCrypt/crypt.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import hmac as hmc
 import bcrypt
 import base64
 import struct
 import os
 
 
-class IterationsOutofaRangeError(Exception):
+class IterationsOutofRangeError(Exception):
     def __init__(self, num: any) -> None:
         self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num} '
         super().__init__(self.display)
 
 
 class Enc:
     def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
@@ -25,15 +25,15 @@
 
         self.mainkey = mainkey
         self.iv = os.urandom(16)
         self.salt = os.urandom(16)
         self.pepper = os.urandom(16)
         self.iterations = 50
         if self.iterations < 50 or self.iterations > 100000:
-            raise IterationsOutofaRangeError(self.iterations)
+            raise IterationsOutofRangeError(self.iterations)
         self.encKey = self.derkey(self.mainkey, self.salt, self.iterations)
         self.hmac_key = self.derkey(self.mainkey, self.pepper, self.iterations)
 
     @staticmethod
     def derkey(mainkey: str, salt_pepper: bytes, iterations: int) -> bytes:
         return bcrypt.kdf(
             password=mainkey.encode('UTF-8'),
@@ -62,26 +62,26 @@
         padder = padding.PKCS7(128).padder()
         return padder.update(self.message) + padder.finalize()
 
     def ciphertext(self) -> bytes:
         return self.cipher_encryptor().update(self.padded_message()) + \
             self.cipher_encryptor().finalize()
 
-    def HMAC(self) -> bytes:
+    def hmac(self) -> bytes:
         h = self.hmac_key
         h = hmac.HMAC(h, hashes.SHA512())
         h.update(self.ciphertext())
         return h.finalize()
 
     def setup_iterations(self) -> bytes:
         iters_bytes = struct.pack('!I', self.iterations)
         return iters_bytes
 
     def enc_to_bytes(self) -> bytes:
-        return self.HMAC() + self.iv + self.salt + self.pepper + \
+        return self.hmac() + self.iv + self.salt + self.pepper + \
             self.setup_iterations() + self.ciphertext()
 
     def enc_to_str(self) -> str:
         return base64.urlsafe_b64encode(self.enc_to_bytes()).decode('UTF-8')
 
 
 class MessageTamperingError(Exception):
@@ -100,32 +100,32 @@
         self.key = mainkey
         self.rec_hmac = self.message[:64]
         self.rec_iv = self.message[64:80]
         self.rec_salt = self.message[80:96]
         self.rec_pepper = self.message[96:112]
         self.rec_iterations = struct.unpack('!I', self.message[112:116])[0]
         if self.rec_iterations < 50 or self.rec_iterations > 100000:
-            raise IterationsOutofaRangeError(self.rec_iterations)
+            raise IterationsOutofRangeError(self.rec_iterations)
         self.rec_ciphertext = self.message[116:]
         self.decKey = Enc.derkey(self.key, self.rec_salt, self.rec_iterations)
         self.hmac_k = Enc.derkey(
             self.key,
             self.rec_pepper,
             self.rec_iterations)
-        if self.verifyHMAC() is False:
+        if self.verify_hmac() is False:
             raise MessageTamperingError()
 
-    def actualHMAC(self) -> bytes:
+    def calculated_hmac(self) -> bytes:
         h = self.hmac_k
         h = hmac.HMAC(h, hashes.SHA512())
         h.update(self.rec_ciphertext)
         return h.finalize()
 
-    def verifyHMAC(self) -> bool:
-        return hmc.compare_digest(self.actualHMAC(), self.rec_hmac)
+    def verify_hmac(self) -> bool:
+        return hmc.compare_digest(self.calculated_hmac(), self.rec_hmac)
 
     def mode(self):
         return modes.CBC(self.rec_iv)
 
     def cipher(self):
         return Cipher(
             algorithms.AES(
```

### Comparing `AshCrypt-2.0.5/AshCrypt/database.py` & `AshCrypt-2.0.6/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.5/AshCrypt/filecrypt.py` & `AshCrypt-2.0.6/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.5/AshCrypt/textcrypt.py` & `AshCrypt-2.0.6/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.5/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-2.0.6/AshCrypt/unittests/unittest_crypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def test_KeyLength(self):
         self.assertEqual(32, bytes.fromhex(cp.Enc.genkey()).__len__())
 
     def test_KeyType(self):
         self.assertIs(str, type(cp.Enc.genkey()))
 
     def test_HMAC(self):
-        self.assertTrue(self.bytes_message[:64] == self.ins1.HMAC())
+        self.assertTrue(self.bytes_message[:64] == self.ins1.hmac())
 
     def test_IV(self):
         self.assertTrue(self.bytes_message[64:80] == self.ins1.iv)
 
     def test_Salt(self):
         self.assertTrue(self.bytes_message[80:96] == self.ins1.salt)
 
@@ -50,15 +50,15 @@
     def test_EncOutputBytes(self):
         self.assertIs(bytes, type(self.ins1.enc_to_bytes()))
 
     def test_EncOutputString(self):
         self.assertIs(str, type(self.ins1.enc_to_str()))
 
     def test_HMAC_Comp(self):
-        self.assertEqual(self.ins1.HMAC(), self.ins2.rec_hmac)
+        self.assertEqual(self.ins1.hmac(), self.ins2.rec_hmac)
 
     def test_IV_Comp(self):
         self.assertEqual(self.ins1.iv, self.ins2.rec_iv)
 
     def test_Salt_Comp(self):
         self.assertEqual(self.ins1.salt, self.ins2.rec_salt)
 
@@ -76,15 +76,15 @@
         tampered_message = tampered_hmac + self.ins1.enc_to_bytes()[64:]
         with self.assertRaises(cp.MessageTamperingError):
             cp.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_IterationsOutOfRangeError2(self):
         enb = self.ins1.enc_to_bytes()
         tampered_message = enb[:112] + struct.pack('!I', 100001) + enb[116:]
-        with self.assertRaises(cp.IterationsOutofaRangeError):
+        with self.assertRaises(cp.IterationsOutofRangeError):
             cp.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_DecOutputBytes(self):
         self.assertEqual(bytes, type(self.ins2.dec_to_bytes()))
 
     def test_DecOutputString(self):
         self.assertEqual(str, type(self.ins2.dec_to_str()))
```

### Comparing `AshCrypt-2.0.5/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-2.0.6/AshCrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.5
+Version: 2.0.6
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.5/PKG-INFO` & `AshCrypt-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.5
+Version: 2.0.6
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.5/README.md` & `AshCrypt-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.5/setup.py` & `AshCrypt-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='2.0.5',
+    version='2.0.6',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

