# Comparing `tmp/bitcoin_p2p-0.3.3.tar.gz` & `tmp/bitcoin_p2p-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_p2p-0.3.3.tar", last modified: Mon Jun 19 16:36:05 2023, max compression
+gzip compressed data, was "bitcoin_p2p-0.3.4.tar", last modified: Thu Jul 20 16:15:55 2023, max compression
```

## Comparing `bitcoin_p2p-0.3.3.tar` & `bitcoin_p2p-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-19 16:36:05.443604 bitcoin_p2p-0.3.3/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_p2p-0.3.3/LICENSE
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4543 2023-06-19 16:36:05.443604 bitcoin_p2p-0.3.3/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4047 2023-06-19 16:35:14.000000 bitcoin_p2p-0.3.3/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-19 16:36:05.443604 bitcoin_p2p-0.3.3/bitcoin_p2p/
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-19 16:36:05.443604 bitcoin_p2p-0.3.3/bitcoin_p2p/bitcoin_p2p.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4543 2023-06-19 16:36:05.000000 bitcoin_p2p-0.3.3/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      260 2023-06-19 16:36:05.000000 bitcoin_p2p-0.3.3/bitcoin_p2p/bitcoin_p2p.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-19 16:36:05.000000 bitcoin_p2p-0.3.3/bitcoin_p2p/bitcoin_p2p.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       48 2023-06-19 16:36:05.000000 bitcoin_p2p-0.3.3/bitcoin_p2p/bitcoin_p2p.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-19 16:36:05.000000 bitcoin_p2p-0.3.3/bitcoin_p2p/bitcoin_p2p.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-06-19 16:36:05.443604 bitcoin_p2p-0.3.3/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1177 2023-06-19 16:35:32.000000 bitcoin_p2p-0.3.3/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 16:15:55.739786 bitcoin_p2p-0.3.4/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_p2p-0.3.4/LICENSE
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4527 2023-07-20 16:15:55.739786 bitcoin_p2p-0.3.4/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4031 2023-07-20 12:12:30.000000 bitcoin_p2p-0.3.4/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 16:15:55.739786 bitcoin_p2p-0.3.4/bitcoin_p2p/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       25 2023-06-10 09:37:00.000000 bitcoin_p2p-0.3.4/bitcoin_p2p/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    18601 2023-06-11 11:18:01.000000 bitcoin_p2p-0.3.4/bitcoin_p2p/p2p.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2599 2023-06-10 06:34:47.000000 bitcoin_p2p-0.3.4/bitcoin_p2p/tools.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 16:15:55.739786 bitcoin_p2p-0.3.4/bitcoin_p2p.egg-info/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4527 2023-07-20 16:15:55.000000 bitcoin_p2p-0.3.4/bitcoin_p2p.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      264 2023-07-20 16:15:55.000000 bitcoin_p2p-0.3.4/bitcoin_p2p.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-07-20 16:15:55.000000 bitcoin_p2p-0.3.4/bitcoin_p2p.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       48 2023-07-20 16:15:55.000000 bitcoin_p2p-0.3.4/bitcoin_p2p.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       12 2023-07-20 16:15:55.000000 bitcoin_p2p-0.3.4/bitcoin_p2p.egg-info/top_level.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-07-20 16:15:55.739786 bitcoin_p2p-0.3.4/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1090 2023-07-20 16:15:47.000000 bitcoin_p2p-0.3.4/setup.py
```

### Comparing `bitcoin_p2p-0.3.3/LICENSE` & `bitcoin_p2p-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_p2p-0.3.3/PKG-INFO` & `bitcoin_p2p-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin_p2p
-Version: 0.3.3
+Version: 0.3.4
 Summary: Bitcoin p2p communication tools in python
 Home-page: https://github.com/andreasgriffin/bitcoin-p2p
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -87,12 +87,12 @@
 
 
 
 ###  From git
 
 ```shell
 python setup.py sdist bdist_wheel
-pip install dist/bitcoin_p2p-0.1-py3-none-any.whl  --force-reinstall
+pip install dist/bitcoin_p2p-0.1-py3-none-any.whl   
 ```
```

### Comparing `bitcoin_p2p-0.3.3/README.md` & `bitcoin_p2p-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -72,12 +72,12 @@
 
 
 
 ###  From git
 
 ```shell
 python setup.py sdist bdist_wheel
-pip install dist/bitcoin_p2p-0.1-py3-none-any.whl  --force-reinstall
+pip install dist/bitcoin_p2p-0.1-py3-none-any.whl   
 ```
```

### Comparing `bitcoin_p2p-0.3.3/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO` & `bitcoin_p2p-0.3.4/bitcoin_p2p.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin-p2p
-Version: 0.3.3
+Version: 0.3.4
 Summary: Bitcoin p2p communication tools in python
 Home-page: https://github.com/andreasgriffin/bitcoin-p2p
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -87,12 +87,12 @@
 
 
 
 ###  From git
 
 ```shell
 python setup.py sdist bdist_wheel
-pip install dist/bitcoin_p2p-0.1-py3-none-any.whl  --force-reinstall
+pip install dist/bitcoin_p2p-0.1-py3-none-any.whl   
 ```
```

### Comparing `bitcoin_p2p-0.3.3/setup.py` & `bitcoin_p2p-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,22 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="bitcoin_p2p",
-    version="0.3.3",
+    version="0.3.4",
     author="Andreas Griffin",
     author_email="andreasgriffin@proton.me",
     description="Bitcoin p2p communication tools in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andreasgriffin/bitcoin-p2p",
-    packages=find_namespace_packages("bitcoin_p2p", include=["bitcoin_p2p.*"]),
-    package_dir={"": "bitcoin_p2p"},
+    packages=find_packages(),
     install_requires=reqs,
     classifiers=[
         "Development Status :: 3 - Alpha",  # Replace with the appropriate development status
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
```

