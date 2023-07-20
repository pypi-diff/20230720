# Comparing `tmp/verify4py-test-0.1.6.tar.gz` & `tmp/verify4py-test-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify4py-test-0.1.6.tar", last modified: Thu Jul 20 09:22:09 2023, max compression
+gzip compressed data, was "verify4py-test-0.1.7.tar", last modified: Thu Jul 20 09:24:57 2023, max compression
```

## Comparing `verify4py-test-0.1.6.tar` & `verify4py-test-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-20 09:22:09.087756 verify4py-test-0.1.6/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1065 2022-04-11 09:13:53.000000 verify4py-test-0.1.6/LICENSE
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9295 2023-07-20 09:22:09.087756 verify4py-test-0.1.6/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8762 2022-05-11 04:20:49.000000 verify4py-test-0.1.6/README.md
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2022-04-11 09:22:24.000000 verify4py-test-0.1.6/pyproject.toml
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2023-07-20 09:22:09.087756 verify4py-test-0.1.6/setup.cfg
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      907 2023-07-20 09:21:57.000000 verify4py-test-0.1.6/setup.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-20 09:22:09.083756 verify4py-test-0.1.6/src/
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-20 09:22:09.083756 verify4py-test-0.1.6/src/verify4py/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    10957 2022-10-20 09:46:08.000000 verify4py-test-0.1.6/src/verify4py/Issuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3815 2022-05-13 07:31:57.000000 verify4py-test-0.1.6/src/verify4py/JsonIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2909 2022-07-06 07:22:13.000000 verify4py-test-0.1.6/src/verify4py/PdfIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3662 2022-07-06 10:35:49.000000 verify4py-test-0.1.6/src/verify4py/UniversityDiplomaIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2022-04-11 09:38:54.000000 verify4py-test-0.1.6/src/verify4py/__init__.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27276 2022-07-01 08:52:48.000000 verify4py-test-0.1.6/src/verify4py/certify_sc_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2788 2022-05-10 06:21:26.000000 verify4py-test-0.1.6/src/verify4py/chainpoint.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2022-07-06 08:44:53.000000 verify4py-test-0.1.6/src/verify4py/json_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2022-07-06 07:08:53.000000 verify4py-test-0.1.6/src/verify4py/pdf.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    19898 2022-07-04 09:06:21.000000 verify4py-test-0.1.6/src/verify4py/university_abi.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1525 2022-05-12 09:38:07.000000 verify4py-test-0.1.6/src/verify4py/utils.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-20 09:22:09.087756 verify4py-test-0.1.6/src/verify4py_test.egg-info/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9295 2023-07-20 09:22:09.000000 verify4py-test-0.1.6/src/verify4py_test.egg-info/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      562 2023-07-20 09:22:09.000000 verify4py-test-0.1.6/src/verify4py_test.egg-info/SOURCES.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2023-07-20 09:22:09.000000 verify4py-test-0.1.6/src/verify4py_test.egg-info/dependency_links.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       43 2023-07-20 09:22:09.000000 verify4py-test-0.1.6/src/verify4py_test.egg-info/requires.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       10 2023-07-20 09:22:09.000000 verify4py-test-0.1.6/src/verify4py_test.egg-info/top_level.txt
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-20 09:24:57.475833 verify4py-test-0.1.7/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1065 2022-04-11 09:13:53.000000 verify4py-test-0.1.7/LICENSE
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9302 2023-07-20 09:24:57.475833 verify4py-test-0.1.7/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8762 2022-05-11 04:20:49.000000 verify4py-test-0.1.7/README.md
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2022-04-11 09:22:24.000000 verify4py-test-0.1.7/pyproject.toml
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2023-07-20 09:24:57.475833 verify4py-test-0.1.7/setup.cfg
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      914 2023-07-20 09:24:55.000000 verify4py-test-0.1.7/setup.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-20 09:24:57.471833 verify4py-test-0.1.7/src/
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-20 09:24:57.475833 verify4py-test-0.1.7/src/verify4py/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    10957 2022-10-20 09:46:08.000000 verify4py-test-0.1.7/src/verify4py/Issuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3815 2022-05-13 07:31:57.000000 verify4py-test-0.1.7/src/verify4py/JsonIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2909 2022-07-06 07:22:13.000000 verify4py-test-0.1.7/src/verify4py/PdfIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3662 2022-07-06 10:35:49.000000 verify4py-test-0.1.7/src/verify4py/UniversityDiplomaIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2022-04-11 09:38:54.000000 verify4py-test-0.1.7/src/verify4py/__init__.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27276 2022-07-01 08:52:48.000000 verify4py-test-0.1.7/src/verify4py/certify_sc_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2788 2022-05-10 06:21:26.000000 verify4py-test-0.1.7/src/verify4py/chainpoint.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2022-07-06 08:44:53.000000 verify4py-test-0.1.7/src/verify4py/json_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2022-07-06 07:08:53.000000 verify4py-test-0.1.7/src/verify4py/pdf.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    19898 2022-07-04 09:06:21.000000 verify4py-test-0.1.7/src/verify4py/university_abi.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1525 2022-05-12 09:38:07.000000 verify4py-test-0.1.7/src/verify4py/utils.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-20 09:24:57.475833 verify4py-test-0.1.7/src/verify4py_test.egg-info/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9302 2023-07-20 09:24:57.000000 verify4py-test-0.1.7/src/verify4py_test.egg-info/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      562 2023-07-20 09:24:57.000000 verify4py-test-0.1.7/src/verify4py_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2023-07-20 09:24:57.000000 verify4py-test-0.1.7/src/verify4py_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       43 2023-07-20 09:24:57.000000 verify4py-test-0.1.7/src/verify4py_test.egg-info/requires.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       10 2023-07-20 09:24:57.000000 verify4py-test-0.1.7/src/verify4py_test.egg-info/top_level.txt
```

### Comparing `verify4py-test-0.1.6/LICENSE` & `verify4py-test-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/PKG-INFO` & `verify4py-test-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: verify4py-test
-Version: 0.1.6
+Version: 0.1.7
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.6,<=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verify4py 
 Verify4py нь сертификат, диплом, дансны хуулга зэрэг бичиг баримтыг блокчэйн дээр
 баталгаажуулж өгөх https://github.com/corex-mn/certify-sc ухаалаг гэрээтэй харьцдаг python хэлний сан юм.
```

### Comparing `verify4py-test-0.1.6/README.md` & `verify4py-test-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/setup.py` & `verify4py-test-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="verify4py-test",
-    version="0.1.6",
+    version="0.1.7",
     author="Surenbayar Doloonjin",
     author_email="surenbayar@corex.mn",
     description="Issue certificates using blockchain and smart contract",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/teo-mn/verify4py",
     project_urls={
@@ -18,10 +18,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    python_requires=">=3.6,<=3.10",
     install_requires=['web3==5.28.0', 'merkletools==1.0.3', 'pdfrw==0.3']
 )
```

### Comparing `verify4py-test-0.1.6/src/verify4py/Issuer.py` & `verify4py-test-0.1.7/src/verify4py/Issuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/JsonIssuer.py` & `verify4py-test-0.1.7/src/verify4py/JsonIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/PdfIssuer.py` & `verify4py-test-0.1.7/src/verify4py/PdfIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/UniversityDiplomaIssuer.py` & `verify4py-test-0.1.7/src/verify4py/UniversityDiplomaIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/certify_sc_utils.py` & `verify4py-test-0.1.7/src/verify4py/certify_sc_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/chainpoint.py` & `verify4py-test-0.1.7/src/verify4py/chainpoint.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/json_utils.py` & `verify4py-test-0.1.7/src/verify4py/json_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/pdf.py` & `verify4py-test-0.1.7/src/verify4py/pdf.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/university_abi.py` & `verify4py-test-0.1.7/src/verify4py/university_abi.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py/utils.py` & `verify4py-test-0.1.7/src/verify4py/utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test-0.1.6/src/verify4py_test.egg-info/PKG-INFO` & `verify4py-test-0.1.7/src/verify4py_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: verify4py-test
-Version: 0.1.6
+Version: 0.1.7
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.6,<=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verify4py 
 Verify4py нь сертификат, диплом, дансны хуулга зэрэг бичиг баримтыг блокчэйн дээр
 баталгаажуулж өгөх https://github.com/corex-mn/certify-sc ухаалаг гэрээтэй харьцдаг python хэлний сан юм.
```

### Comparing `verify4py-test-0.1.6/src/verify4py_test.egg-info/SOURCES.txt` & `verify4py-test-0.1.7/src/verify4py_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

