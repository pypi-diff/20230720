# Comparing `tmp/thor-devkit-1.0.8.tar.gz` & `tmp/thor-devkit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thor-devkit-1.0.8.tar", last modified: Tue Feb  9 05:53:43 2021, max compression
+gzip compressed data, was "dist/thor-devkit-1.0.9.tar", last modified: Thu Mar 25 06:48:47 2021, max compression
```

## Comparing `thor-devkit-1.0.8.tar` & `thor-devkit-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 doncoleone   (501) staff       (20)        0 2021-02-09 05:53:43.460267 thor-devkit-1.0.8/
--rw-r--r--   0 doncoleone   (501) staff       (20)    20348 2021-02-09 05:53:43.459749 thor-devkit-1.0.8/PKG-INFO
--rw-r--r--   0 doncoleone   (501) staff       (20)    15205 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/README.md
--rw-r--r--   0 doncoleone   (501) staff       (20)       38 2021-02-09 05:53:43.460397 thor-devkit-1.0.8/setup.cfg
--rw-r--r--   0 doncoleone   (501) staff       (20)     1196 2021-02-09 05:52:04.000000 thor-devkit-1.0.8/setup.py
-drwxr-xr-x   0 doncoleone   (501) staff       (20)        0 2021-02-09 05:53:43.451590 thor-devkit-1.0.8/thor_devkit/
--rw-r--r--   0 doncoleone   (501) staff       (20)       24 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/__init__.py
--rw-r--r--   0 doncoleone   (501) staff       (20)    10454 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/abi.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     3314 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/bloom.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     3071 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/certificate.py
-drwxr-xr-x   0 doncoleone   (501) staff       (20)        0 2021-02-09 05:53:43.458808 thor-devkit-1.0.8/thor_devkit/cry/
--rw-r--r--   0 doncoleone   (501) staff       (20)      165 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/__init__.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     1977 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/address.py
--rw-r--r--   0 doncoleone   (501) staff       (20)      616 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/blake2b.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     7183 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/hdnode.py
--rw-r--r--   0 doncoleone   (501) staff       (20)      556 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/keccak.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     2472 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/keystore.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     2580 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/mnemonic.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     3954 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/secp256k1.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     1247 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/cry/utils.py
--rw-r--r--   0 doncoleone   (501) staff       (20)    16253 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/rlp.py
--rw-r--r--   0 doncoleone   (501) staff       (20)     9772 2021-02-09 05:49:10.000000 thor-devkit-1.0.8/thor_devkit/transaction.py
-drwxr-xr-x   0 doncoleone   (501) staff       (20)        0 2021-02-09 05:53:43.454111 thor-devkit-1.0.8/thor_devkit.egg-info/
--rw-r--r--   0 doncoleone   (501) staff       (20)    20348 2021-02-09 05:53:43.000000 thor-devkit-1.0.8/thor_devkit.egg-info/PKG-INFO
--rw-r--r--   0 doncoleone   (501) staff       (20)      573 2021-02-09 05:53:43.000000 thor-devkit-1.0.8/thor_devkit.egg-info/SOURCES.txt
--rw-r--r--   0 doncoleone   (501) staff       (20)        1 2021-02-09 05:53:43.000000 thor-devkit-1.0.8/thor_devkit.egg-info/dependency_links.txt
--rw-r--r--   0 doncoleone   (501) staff       (20)      154 2021-02-09 05:53:43.000000 thor-devkit-1.0.8/thor_devkit.egg-info/requires.txt
--rw-r--r--   0 doncoleone   (501) staff       (20)       12 2021-02-09 05:53:43.000000 thor-devkit-1.0.8/thor_devkit.egg-info/top_level.txt
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2021-03-25 06:48:47.375540 thor-devkit-1.0.9/
+-rw-r--r--   0 rollo      (501) staff       (20)    20116 2021-03-25 06:48:47.373508 thor-devkit-1.0.9/PKG-INFO
+-rw-r--r--   0 rollo      (501) staff       (20)    15029 2021-03-25 06:39:42.000000 thor-devkit-1.0.9/README.md
+-rw-r--r--   0 rollo      (501) staff       (20)       38 2021-03-25 06:48:47.375802 thor-devkit-1.0.9/setup.cfg
+-rw-r--r--   0 rollo      (501) staff       (20)     1196 2021-03-25 06:48:00.000000 thor-devkit-1.0.9/setup.py
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2021-03-25 06:48:47.363419 thor-devkit-1.0.9/thor_devkit/
+-rw-r--r--   0 rollo      (501) staff       (20)       24 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/__init__.py
+-rw-r--r--   0 rollo      (501) staff       (20)    10454 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/abi.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3314 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/bloom.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3071 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/certificate.py
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2021-03-25 06:48:47.372631 thor-devkit-1.0.9/thor_devkit/cry/
+-rw-r--r--   0 rollo      (501) staff       (20)      165 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/__init__.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1977 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/address.py
+-rw-r--r--   0 rollo      (501) staff       (20)      616 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/blake2b.py
+-rw-r--r--   0 rollo      (501) staff       (20)     7183 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/hdnode.py
+-rw-r--r--   0 rollo      (501) staff       (20)      556 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/keccak.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2472 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/keystore.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2580 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/mnemonic.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3954 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/secp256k1.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1247 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/cry/utils.py
+-rw-r--r--   0 rollo      (501) staff       (20)    16253 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/rlp.py
+-rw-r--r--   0 rollo      (501) staff       (20)     9772 2021-03-23 03:45:45.000000 thor-devkit-1.0.9/thor_devkit/transaction.py
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2021-03-25 06:48:47.367028 thor-devkit-1.0.9/thor_devkit.egg-info/
+-rw-r--r--   0 rollo      (501) staff       (20)    20116 2021-03-25 06:48:47.000000 thor-devkit-1.0.9/thor_devkit.egg-info/PKG-INFO
+-rw-r--r--   0 rollo      (501) staff       (20)      573 2021-03-25 06:48:47.000000 thor-devkit-1.0.9/thor_devkit.egg-info/SOURCES.txt
+-rw-r--r--   0 rollo      (501) staff       (20)        1 2021-03-25 06:48:47.000000 thor-devkit-1.0.9/thor_devkit.egg-info/dependency_links.txt
+-rw-r--r--   0 rollo      (501) staff       (20)      166 2021-03-25 06:48:47.000000 thor-devkit-1.0.9/thor_devkit.egg-info/requires.txt
+-rw-r--r--   0 rollo      (501) staff       (20)       12 2021-03-25 06:48:47.000000 thor-devkit-1.0.9/thor_devkit.egg-info/top_level.txt
```

### Comparing `thor-devkit-1.0.8/PKG-INFO` & `thor-devkit-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thor-devkit
-Version: 1.0.8
+Version: 1.0.9
 Summary: SDK to interact with VeChain Thor public blockchain.
 Home-page: https://github.com/laalaguer/thor-devkit.py
 Author: laalaguer
 Author-email: laalaguer@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/laalaguer/thor-devkit.py
 Project-URL: Source, https://github.com/laalaguer/thor-devkit.py
@@ -515,25 +515,18 @@
             │   └── utils.py
             ├── rlp.py
             └── transaction.py
         ```
         
         ## Local Development
         ```bash
-        mkdir .env && python3 -m venv .env # Make virtualenv
-        
-        source .env/bin/activate # Activate virtualenv
-        
-        pip3 install -r requirements.txt # Install packages.
-        
-        ... write code ...
-        
-        ./test.sh # Run tests
-        
-        deactivate # Get out of virtualenv
+        # install dependencies
+        make install
+        # test code
+        make test
         ```
         
         ## Knowledge
         
         |     Name     | Bytes |                  Description                   |
         | ------------ | ----- | ---------------------------------------------- |
         | private key  | 32    | random number                                  |
```

### Comparing `thor-devkit-1.0.8/README.md` & `thor-devkit-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -504,25 +504,18 @@
     │   └── utils.py
     ├── rlp.py
     └── transaction.py
 ```
 
 ## Local Development
 ```bash
-mkdir .env && python3 -m venv .env # Make virtualenv
-
-source .env/bin/activate # Activate virtualenv
-
-pip3 install -r requirements.txt # Install packages.
-
-... write code ...
-
-./test.sh # Run tests
-
-deactivate # Get out of virtualenv
+# install dependencies
+make install
+# test code
+make test
 ```
 
 ## Knowledge
 
 |     Name     | Bytes |                  Description                   |
 | ------------ | ----- | ---------------------------------------------- |
 | private key  | 32    | random number                                  |
```

### Comparing `thor-devkit-1.0.8/setup.py` & `thor-devkit-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 long_description = ''
 with open("README.md", "r") as fh:
     long_description = fh.read()
 assert long_description
 
 setuptools.setup(
     name="thor-devkit",
-    version="1.0.8",
+    version="1.0.9",
     author="laalaguer",
     author_email="laalaguer@gmail.com",
     description="SDK to interact with VeChain Thor public blockchain.",
     keywords="vechain thor blockchain sdk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `thor-devkit-1.0.8/thor_devkit/abi.py` & `thor-devkit-1.0.9/thor_devkit/abi.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/bloom.py` & `thor-devkit-1.0.9/thor_devkit/bloom.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/certificate.py` & `thor-devkit-1.0.9/thor_devkit/certificate.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/cry/address.py` & `thor-devkit-1.0.9/thor_devkit/cry/address.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/cry/blake2b.py` & `thor-devkit-1.0.9/thor_devkit/cry/blake2b.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/cry/hdnode.py` & `thor-devkit-1.0.9/thor_devkit/cry/hdnode.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/cry/keccak.py` & `thor-devkit-1.0.9/thor_devkit/cry/keccak.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/cry/keystore.py` & `thor-devkit-1.0.9/thor_devkit/cry/keystore.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/cry/mnemonic.py` & `thor-devkit-1.0.9/thor_devkit/cry/mnemonic.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/cry/secp256k1.py` & `thor-devkit-1.0.9/thor_devkit/cry/secp256k1.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/cry/utils.py` & `thor-devkit-1.0.9/thor_devkit/cry/utils.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/rlp.py` & `thor-devkit-1.0.9/thor_devkit/rlp.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit/transaction.py` & `thor-devkit-1.0.9/thor_devkit/transaction.py`

 * *Files identical despite different names*

### Comparing `thor-devkit-1.0.8/thor_devkit.egg-info/PKG-INFO` & `thor-devkit-1.0.9/thor_devkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thor-devkit
-Version: 1.0.8
+Version: 1.0.9
 Summary: SDK to interact with VeChain Thor public blockchain.
 Home-page: https://github.com/laalaguer/thor-devkit.py
 Author: laalaguer
 Author-email: laalaguer@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/laalaguer/thor-devkit.py
 Project-URL: Source, https://github.com/laalaguer/thor-devkit.py
@@ -515,25 +515,18 @@
             │   └── utils.py
             ├── rlp.py
             └── transaction.py
         ```
         
         ## Local Development
         ```bash
-        mkdir .env && python3 -m venv .env # Make virtualenv
-        
-        source .env/bin/activate # Activate virtualenv
-        
-        pip3 install -r requirements.txt # Install packages.
-        
-        ... write code ...
-        
-        ./test.sh # Run tests
-        
-        deactivate # Get out of virtualenv
+        # install dependencies
+        make install
+        # test code
+        make test
         ```
         
         ## Knowledge
         
         |     Name     | Bytes |                  Description                   |
         | ------------ | ----- | ---------------------------------------------- |
         | private key  | 32    | random number                                  |
```

### Comparing `thor-devkit-1.0.8/thor_devkit.egg-info/SOURCES.txt` & `thor-devkit-1.0.9/thor_devkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

