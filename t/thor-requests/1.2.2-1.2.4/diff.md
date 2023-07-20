# Comparing `tmp/thor-requests-1.2.2.tar.gz` & `tmp/thor-requests-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thor-requests-1.2.2.tar", last modified: Thu Feb 10 05:54:23 2022, max compression
+gzip compressed data, was "thor-requests-1.2.4.tar", last modified: Thu Jul 20 08:36:43 2023, max compression
```

## Comparing `thor-requests-1.2.2.tar` & `thor-requests-1.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 bernard    (501) staff       (20)        0 2022-02-10 05:54:23.865169 thor-requests-1.2.2/
--rw-r--r--   0 bernard    (501) staff       (20)    35149 2022-02-06 12:36:07.000000 thor-requests-1.2.2/LICENSE
--rw-r--r--   0 bernard    (501) staff       (20)    15099 2022-02-10 05:54:23.864609 thor-requests-1.2.2/PKG-INFO
--rw-r--r--   0 bernard    (501) staff       (20)    14202 2022-02-06 12:36:07.000000 thor-requests-1.2.2/README.md
--rw-r--r--   0 bernard    (501) staff       (20)       38 2022-02-10 05:54:23.865295 thor-requests-1.2.2/setup.cfg
--rw-r--r--   0 bernard    (501) staff       (20)     1220 2022-02-10 05:49:33.000000 thor-requests-1.2.2/setup.py
-drwxr-xr-x   0 bernard    (501) staff       (20)        0 2022-02-10 05:54:23.855028 thor-requests-1.2.2/tests/
--rw-r--r--   0 bernard    (501) staff       (20)        0 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/__init__.py
--rw-r--r--   0 bernard    (501) staff       (20)     1893 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/fixtures.py
--rw-r--r--   0 bernard    (501) staff       (20)      424 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_contract.py
--rw-r--r--   0 bernard    (501) staff       (20)     7379 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_fee_delegation.py
--rw-r--r--   0 bernard    (501) staff       (20)     2435 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_integration.py
--rw-r--r--   0 bernard    (501) staff       (20)     1781 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_multi.py
--rw-r--r--   0 bernard    (501) staff       (20)     2534 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_replay.py
--rw-r--r--   0 bernard    (501) staff       (20)      295 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_ticker.py
--rw-r--r--   0 bernard    (501) staff       (20)      545 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_timeout.py
--rw-r--r--   0 bernard    (501) staff       (20)      930 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_vet.py
--rw-r--r--   0 bernard    (501) staff       (20)     3460 2022-02-06 12:36:07.000000 thor-requests-1.2.2/tests/test_vtho.py
-drwxr-xr-x   0 bernard    (501) staff       (20)        0 2022-02-10 05:54:23.861199 thor-requests-1.2.2/thor_requests/
--rw-r--r--   0 bernard    (501) staff       (20)        0 2022-02-06 12:36:07.000000 thor-requests-1.2.2/thor_requests/__init__.py
--rw-r--r--   0 bernard    (501) staff       (20)     2253 2022-02-06 12:36:07.000000 thor-requests-1.2.2/thor_requests/clause.py
--rw-r--r--   0 bernard    (501) staff       (20)    23011 2022-02-10 05:48:05.000000 thor-requests-1.2.2/thor_requests/connect.py
--rw-r--r--   0 bernard    (501) staff       (20)     5792 2022-02-06 12:36:07.000000 thor-requests-1.2.2/thor_requests/const.py
--rw-r--r--   0 bernard    (501) staff       (20)     3194 2022-02-06 12:36:07.000000 thor-requests-1.2.2/thor_requests/contract.py
--rw-r--r--   0 bernard    (501) staff       (20)      147 2022-02-06 12:36:07.000000 thor-requests-1.2.2/thor_requests/file_utils.py
--rw-r--r--   0 bernard    (501) staff       (20)    12212 2022-02-06 12:36:07.000000 thor-requests-1.2.2/thor_requests/utils.py
--rw-r--r--   0 bernard    (501) staff       (20)     1956 2022-02-06 12:36:07.000000 thor-requests-1.2.2/thor_requests/wallet.py
-drwxr-xr-x   0 bernard    (501) staff       (20)        0 2022-02-10 05:54:23.863875 thor-requests-1.2.2/thor_requests.egg-info/
--rw-r--r--   0 bernard    (501) staff       (20)    15099 2022-02-10 05:54:23.000000 thor-requests-1.2.2/thor_requests.egg-info/PKG-INFO
--rw-r--r--   0 bernard    (501) staff       (20)      644 2022-02-10 05:54:23.000000 thor-requests-1.2.2/thor_requests.egg-info/SOURCES.txt
--rw-r--r--   0 bernard    (501) staff       (20)        1 2022-02-10 05:54:23.000000 thor-requests-1.2.2/thor_requests.egg-info/dependency_links.txt
--rw-r--r--   0 bernard    (501) staff       (20)       59 2022-02-10 05:54:23.000000 thor-requests-1.2.2/thor_requests.egg-info/requires.txt
--rw-r--r--   0 bernard    (501) staff       (20)       20 2022-02-10 05:54:23.000000 thor-requests-1.2.2/thor_requests.egg-info/top_level.txt
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 08:36:43.877236 thor-requests-1.2.4/
+-rw-r--r--   0 rollo      (501) staff       (20)    35149 2021-06-21 02:58:12.000000 thor-requests-1.2.4/LICENSE
+-rw-r--r--   0 rollo      (501) staff       (20)    15099 2023-07-20 08:36:43.876728 thor-requests-1.2.4/PKG-INFO
+-rw-r--r--   0 rollo      (501) staff       (20)    14202 2022-01-11 06:49:45.000000 thor-requests-1.2.4/README.md
+-rw-r--r--   0 rollo      (501) staff       (20)       38 2023-07-20 08:36:43.877306 thor-requests-1.2.4/setup.cfg
+-rw-r--r--   0 rollo      (501) staff       (20)     1220 2023-07-20 08:35:01.000000 thor-requests-1.2.4/setup.py
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 08:36:43.873848 thor-requests-1.2.4/tests/
+-rw-r--r--   0 rollo      (501) staff       (20)        0 2021-06-21 02:58:12.000000 thor-requests-1.2.4/tests/__init__.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1893 2021-11-19 09:29:56.000000 thor-requests-1.2.4/tests/fixtures.py
+-rw-r--r--   0 rollo      (501) staff       (20)      424 2021-06-21 02:58:12.000000 thor-requests-1.2.4/tests/test_contract.py
+-rw-r--r--   0 rollo      (501) staff       (20)     7379 2022-01-12 08:23:44.000000 thor-requests-1.2.4/tests/test_fee_delegation.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2435 2021-07-08 05:58:35.000000 thor-requests-1.2.4/tests/test_integration.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1781 2021-11-16 06:35:57.000000 thor-requests-1.2.4/tests/test_multi.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2534 2021-06-21 02:58:12.000000 thor-requests-1.2.4/tests/test_replay.py
+-rw-r--r--   0 rollo      (501) staff       (20)      295 2021-06-28 06:19:29.000000 thor-requests-1.2.4/tests/test_ticker.py
+-rw-r--r--   0 rollo      (501) staff       (20)      545 2021-06-21 07:44:29.000000 thor-requests-1.2.4/tests/test_timeout.py
+-rw-r--r--   0 rollo      (501) staff       (20)      930 2021-06-22 06:18:46.000000 thor-requests-1.2.4/tests/test_vet.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3460 2022-01-11 06:49:45.000000 thor-requests-1.2.4/tests/test_vtho.py
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 08:36:43.875782 thor-requests-1.2.4/thor_requests/
+-rw-r--r--   0 rollo      (501) staff       (20)        0 2021-06-21 02:58:12.000000 thor-requests-1.2.4/thor_requests/__init__.py
+-rw-r--r--   0 rollo      (501) staff       (20)     2253 2021-11-16 05:48:50.000000 thor-requests-1.2.4/thor_requests/clause.py
+-rw-r--r--   0 rollo      (501) staff       (20)    23011 2023-07-20 08:34:55.000000 thor-requests-1.2.4/thor_requests/connect.py
+-rw-r--r--   0 rollo      (501) staff       (20)     5792 2021-06-21 07:22:07.000000 thor-requests-1.2.4/thor_requests/const.py
+-rw-r--r--   0 rollo      (501) staff       (20)     3194 2021-10-20 03:43:35.000000 thor-requests-1.2.4/thor_requests/contract.py
+-rw-r--r--   0 rollo      (501) staff       (20)      147 2021-06-21 02:58:12.000000 thor-requests-1.2.4/thor_requests/file_utils.py
+-rw-r--r--   0 rollo      (501) staff       (20)    12212 2022-01-12 08:23:44.000000 thor-requests-1.2.4/thor_requests/utils.py
+-rw-r--r--   0 rollo      (501) staff       (20)     1956 2021-06-21 03:07:21.000000 thor-requests-1.2.4/thor_requests/wallet.py
+drwxr-xr-x   0 rollo      (501) staff       (20)        0 2023-07-20 08:36:43.876464 thor-requests-1.2.4/thor_requests.egg-info/
+-rw-r--r--   0 rollo      (501) staff       (20)    15099 2023-07-20 08:36:43.000000 thor-requests-1.2.4/thor_requests.egg-info/PKG-INFO
+-rw-r--r--   0 rollo      (501) staff       (20)      644 2023-07-20 08:36:43.000000 thor-requests-1.2.4/thor_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 rollo      (501) staff       (20)        1 2023-07-20 08:36:43.000000 thor-requests-1.2.4/thor_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 rollo      (501) staff       (20)       59 2023-07-20 08:36:43.000000 thor-requests-1.2.4/thor_requests.egg-info/requires.txt
+-rw-r--r--   0 rollo      (501) staff       (20)       20 2023-07-20 08:36:43.000000 thor-requests-1.2.4/thor_requests.egg-info/top_level.txt
```

### Comparing `thor-requests-1.2.2/LICENSE` & `thor-requests-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/PKG-INFO` & `thor-requests-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thor-requests
-Version: 1.2.2
+Version: 1.2.4
 Summary: Simple network VeChain SDK for human to interact with the blockchain
 Home-page: https://github.com/laalaguer/thor-requests
 Author: laalaguer
 Author-email: laalaguer@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/laalaguer/thor-requests
 Project-URL: Source, https://github.com/laalaguer/thor-requests
```

### Comparing `thor-requests-1.2.2/README.md` & `thor-requests-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/setup.py` & `thor-requests-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 long_description = ""
 with open("README.md", "r") as fh:
     long_description = fh.read()
 assert long_description
 
 setuptools.setup(
     name="thor-requests",
-    version="1.2.2",
+    version="1.2.4",
     author="laalaguer",
     author_email="laalaguer@gmail.com",
     description="Simple network VeChain SDK for human to interact with the blockchain",
     keywords="vechain thor blockchain sdk requests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `thor-requests-1.2.2/tests/fixtures.py` & `thor-requests-1.2.4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/tests/test_fee_delegation.py` & `thor-requests-1.2.4/tests/test_fee_delegation.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/tests/test_integration.py` & `thor-requests-1.2.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/tests/test_multi.py` & `thor-requests-1.2.4/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/tests/test_replay.py` & `thor-requests-1.2.4/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/tests/test_timeout.py` & `thor-requests-1.2.4/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/tests/test_vet.py` & `thor-requests-1.2.4/tests/test_vet.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/tests/test_vtho.py` & `thor-requests-1.2.4/tests/test_vtho.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/thor_requests/clause.py` & `thor-requests-1.2.4/thor_requests/clause.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/thor_requests/connect.py` & `thor-requests-1.2.4/thor_requests/connect.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/thor_requests/const.py` & `thor-requests-1.2.4/thor_requests/const.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/thor_requests/contract.py` & `thor-requests-1.2.4/thor_requests/contract.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/thor_requests/utils.py` & `thor-requests-1.2.4/thor_requests/utils.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/thor_requests/wallet.py` & `thor-requests-1.2.4/thor_requests/wallet.py`

 * *Files identical despite different names*

### Comparing `thor-requests-1.2.2/thor_requests.egg-info/PKG-INFO` & `thor-requests-1.2.4/thor_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thor-requests
-Version: 1.2.2
+Version: 1.2.4
 Summary: Simple network VeChain SDK for human to interact with the blockchain
 Home-page: https://github.com/laalaguer/thor-requests
 Author: laalaguer
 Author-email: laalaguer@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/laalaguer/thor-requests
 Project-URL: Source, https://github.com/laalaguer/thor-requests
```

### Comparing `thor-requests-1.2.2/thor_requests.egg-info/SOURCES.txt` & `thor-requests-1.2.4/thor_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

