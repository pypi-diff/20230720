# Comparing `tmp/bitcoin_qrreader-0.1.1.tar.gz` & `tmp/bitcoin_qrreader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_qrreader-0.1.1.tar", last modified: Thu Jul 20 18:00:18 2023, max compression
+gzip compressed data, was "bitcoin_qrreader-0.1.2.tar", last modified: Thu Jul 20 18:02:14 2023, max compression
```

## Comparing `bitcoin_qrreader-0.1.1.tar` & `bitcoin_qrreader-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:00:18.854977 bitcoin_qrreader-0.1.1/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.1.1/LICENSE
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1128 2023-07-20 18:00:18.854977 bitcoin_qrreader-0.1.1/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      646 2023-07-20 17:59:03.000000 bitcoin_qrreader-0.1.1/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:00:18.850976 bitcoin_qrreader-0.1.1/bitcoin_qrreader/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    15502 2023-07-20 11:27:13.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader/bitcoin_qr.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1239 2023-07-20 11:32:56.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader/bitcoin_qr_gui.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3689 2023-07-19 13:09:39.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader/qr_qui.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:00:18.854977 bitcoin_qrreader-0.1.1/bitcoin_qrreader.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1128 2023-07-20 18:00:18.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      347 2023-07-20 18:00:18.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-07-20 18:00:18.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       47 2023-07-20 18:00:18.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       17 2023-07-20 18:00:18.000000 bitcoin_qrreader-0.1.1/bitcoin_qrreader.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-07-20 18:00:18.854977 bitcoin_qrreader-0.1.1/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1077 2023-07-20 17:59:42.000000 bitcoin_qrreader-0.1.1/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.1.2/LICENSE
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1128 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      646 2023-07-20 17:59:03.000000 bitcoin_qrreader-0.1.2/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/bitcoin_qrreader/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    15502 2023-07-20 11:27:13.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader/bitcoin_qr.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1239 2023-07-20 11:32:56.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader/bitcoin_qr_gui.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3689 2023-07-19 13:09:39.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader/qr_qui.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1128 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      347 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       47 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       17 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/top_level.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1077 2023-07-20 18:01:39.000000 bitcoin_qrreader-0.1.2/setup.py
```

### Comparing `bitcoin_qrreader-0.1.1/LICENSE` & `bitcoin_qrreader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.1.1/PKG-INFO` & `bitcoin_qrreader-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bitcoin_qrreader
-Version: 0.1.1
+Version: 0.1.2
 Summary: Bitcoin qr reader
-Home-page: https://github.com/andreasgriffin/bitcoin_qrreader
+Home-page: https://github.com/andreasgriffin/bitcoin-qrreader
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7,<4.0
```

### Comparing `bitcoin_qrreader-0.1.1/README.md` & `bitcoin_qrreader-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.1.1/bitcoin_qrreader/bitcoin_qr.py` & `bitcoin_qrreader-0.1.2/bitcoin_qrreader/bitcoin_qr.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.1.1/bitcoin_qrreader/bitcoin_qr_gui.py` & `bitcoin_qrreader-0.1.2/bitcoin_qrreader/bitcoin_qr_gui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.1.1/bitcoin_qrreader/qr_qui.py` & `bitcoin_qrreader-0.1.2/bitcoin_qrreader/qr_qui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.1.1/bitcoin_qrreader.egg-info/PKG-INFO` & `bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bitcoin-qrreader
-Version: 0.1.1
+Version: 0.1.2
 Summary: Bitcoin qr reader
-Home-page: https://github.com/andreasgriffin/bitcoin_qrreader
+Home-page: https://github.com/andreasgriffin/bitcoin-qrreader
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7,<4.0
```

### Comparing `bitcoin_qrreader-0.1.1/setup.py` & `bitcoin_qrreader-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="bitcoin_qrreader",
-    version="0.1.1",
+    version="0.1.2",
     author="Andreas Griffin",
     author_email="andreasgriffin@proton.me",
     description="Bitcoin qr reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/andreasgriffin/bitcoin_qrreader",
+    url="https://github.com/andreasgriffin/bitcoin-qrreader",
     packages=find_packages(),
     install_requires=reqs,
     classifiers=[
         "Development Status :: 3 - Alpha",  # Replace with the appropriate development status
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

