# Comparing `tmp/iitkgp_erp_login-2.0.0.tar.gz` & `tmp/iitkgp_erp_login-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitkgp_erp_login-2.0.0.tar", last modified: Fri Jul 14 07:50:47 2023, max compression
+gzip compressed data, was "iitkgp_erp_login-2.0.1.tar", last modified: Thu Jul 20 10:13:30 2023, max compression
```

## Comparing `iitkgp_erp_login-2.0.0.tar` & `iitkgp_erp_login-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.980011 iitkgp_erp_login-2.0.0/
--rw-r--r--   0 proffapt   (501) staff       (20)     1074 2023-07-09 19:05:06.000000 iitkgp_erp_login-2.0.0/LICENSE
--rw-r--r--   0 proffapt   (501) staff       (20)    13088 2023-07-14 07:50:47.979727 iitkgp_erp_login-2.0.0/PKG-INFO
--rw-r--r--   0 proffapt   (501) staff       (20)    12530 2023-07-14 07:49:02.000000 iitkgp_erp_login-2.0.0/README.md
--rw-r--r--   0 proffapt   (501) staff       (20)      773 2023-07-14 07:50:41.000000 iitkgp_erp_login-2.0.0/pyproject.toml
--rw-r--r--   0 proffapt   (501) staff       (20)       38 2023-07-14 07:50:47.980085 iitkgp_erp_login-2.0.0/setup.cfg
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.975859 iitkgp_erp_login-2.0.0/src/
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.977877 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/
--rw-r--r--   0 proffapt   (501) staff       (20)        0 2023-07-09 19:54:19.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/__init__.py
--rw-r--r--   0 proffapt   (501) staff       (20)      403 2023-07-09 21:13:18.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/endpoints.py
--rw-r--r--   0 proffapt   (501) staff       (20)     3561 2023-07-13 22:50:20.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/erp.py
--rw-r--r--   0 proffapt   (501) staff       (20)     2373 2023-07-09 21:37:06.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/read_mail.py
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.979014 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/
--rw-r--r--   0 proffapt   (501) staff       (20)    13088 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/PKG-INFO
--rw-r--r--   0 proffapt   (501) staff       (20)      394 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/SOURCES.txt
--rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/dependency_links.txt
--rw-r--r--   0 proffapt   (501) staff       (20)       92 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/requires.txt
--rw-r--r--   0 proffapt   (501) staff       (20)       17 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/top_level.txt
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.979186 iitkgp_erp_login-2.0.0/tests/
--rw-r--r--   0 proffapt   (501) staff       (20)      491 2023-07-13 21:24:40.000000 iitkgp_erp_login-2.0.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:13:30.803556 iitkgp_erp_login-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-07-20 10:13:30.799556 iitkgp_erp_login-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-20 10:13:21.000000 iitkgp_erp_login-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:13:30.803556 iitkgp_erp_login-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:13:30.799556 iitkgp_erp_login-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:13:30.799556 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/erp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/read_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:13:30.799556 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/top_level.txt
```

### Comparing `iitkgp_erp_login-2.0.0/LICENSE` & `iitkgp_erp_login-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.0.0/PKG-INFO` & `iitkgp_erp_login-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp_erp_login
-Version: 2.0.0
+Version: 2.0.1
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.0.0 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.0.1 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module A python package/module to automate login process in
```

### Comparing `iitkgp_erp_login-2.0.0/README.md` & `iitkgp_erp_login-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.0.0/pyproject.toml` & `iitkgp_erp_login-2.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iitkgp_erp_login"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Arpit Bhardwaj", email="proffapt@pm.me" },
 ]
 description = "A package to automate login process in ERP for IIT-KGP"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/erp.py` & `iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/erp.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         else:
             print ("Your secret question: " + secret_question)
             secret_answer = getpass.getpass("Enter the answer to the secret question: ")
     except (requests.exceptions.RequestException, KeyError) as e:
         raise ErpLoginError(f"Failed to fetch Security Question: {str(e)}")
 
     try:
-        r = session.post(OTP_URL, data={'typeee': 'SI', 'loginid': ROLL_NUMBER}, headers=headers)
+        r = session.post(OTP_URL, data={'typeee': 'SI', 'loginid': ROLL_NUMBER, 'pass': PASSWORD}, headers=headers)
     except requests.exceptions.RequestException as e:
         raise ErpLoginError(f"Failed to request OTP: {str(e)}")
     
     login_details = {
         'user_id': ROLL_NUMBER,
         'password': PASSWORD,
         'answer': secret_answer,
```

### Comparing `iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/read_mail.py` & `iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/read_mail.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/PKG-INFO` & `iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp-erp-login
-Version: 2.0.0
+Version: 2.0.1
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.0.0 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.0.1 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module A python package/module to automate login process in
```

