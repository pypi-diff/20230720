# Comparing `tmp/bitnob-1.2.7.tar.gz` & `tmp/bitnob-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitnob-1.2.7.tar", last modified: Thu Aug 11 16:49:50 2022, max compression
+gzip compressed data, was "bitnob-1.2.8.tar", last modified: Thu Jul 20 10:43:33 2023, max compression
```

## Comparing `bitnob-1.2.7.tar` & `bitnob-1.2.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.430806 bitnob-1.2.7/
--rw-r--r--   0 gabby      (501) staff       (20)     4640 2022-08-11 16:49:50.430677 bitnob-1.2.7/PKG-INFO
--rw-r--r--   0 gabby      (501) staff       (20)     4153 2022-02-20 16:41:50.000000 bitnob-1.2.7/README.md
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.424347 bitnob-1.2.7/bitnob/
--rw-r--r--   0 gabby      (501) staff       (20)      459 2022-05-12 20:22:23.000000 bitnob-1.2.7/bitnob/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     2755 2022-03-15 12:22:32.000000 bitnob-1.2.7/bitnob/base.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.425364 bitnob-1.2.7/bitnob/customer/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:02:35.000000 bitnob-1.2.7/bitnob/customer/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)      277 2022-03-03 22:56:33.000000 bitnob-1.2.7/bitnob/customer/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     2930 2022-03-15 11:02:39.000000 bitnob-1.2.7/bitnob/customer/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.425781 bitnob-1.2.7/bitnob/exceptions/
--rw-r--r--   0 gabby      (501) staff       (20)      200 2022-02-20 16:49:05.000000 bitnob-1.2.7/bitnob/exceptions/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     1800 2022-02-20 16:49:05.000000 bitnob-1.2.7/bitnob/exceptions/exceptions.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.426316 bitnob-1.2.7/bitnob/hosted_checkout/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:04:50.000000 bitnob-1.2.7/bitnob/hosted_checkout/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     1830 2022-05-17 17:44:31.000000 bitnob-1.2.7/bitnob/hosted_checkout/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     3234 2022-05-17 17:44:46.000000 bitnob-1.2.7/bitnob/hosted_checkout/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.426892 bitnob-1.2.7/bitnob/lightning/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:22.000000 bitnob-1.2.7/bitnob/lightning/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     1722 2022-03-03 23:00:29.000000 bitnob-1.2.7/bitnob/lightning/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     4809 2022-05-17 17:41:48.000000 bitnob-1.2.7/bitnob/lightning/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.427446 bitnob-1.2.7/bitnob/ln_url/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-05-12 20:16:47.000000 bitnob-1.2.7/bitnob/ln_url/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)      505 2022-03-17 20:39:17.000000 bitnob-1.2.7/bitnob/ln_url/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     5564 2022-03-17 20:54:31.000000 bitnob-1.2.7/bitnob/ln_url/services.py
--rw-r--r--   0 gabby      (501) staff       (20)      250 2022-03-13 23:47:17.000000 bitnob-1.2.7/bitnob/model.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.427813 bitnob-1.2.7/bitnob/onchain/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:29.000000 bitnob-1.2.7/bitnob/onchain/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-03-03 22:48:54.000000 bitnob-1.2.7/bitnob/onchain/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     2991 2022-05-17 17:42:03.000000 bitnob-1.2.7/bitnob/onchain/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.428286 bitnob-1.2.7/bitnob/stablecoin/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:18:11.000000 bitnob-1.2.7/bitnob/stablecoin/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)      836 2022-08-11 16:48:09.000000 bitnob-1.2.7/bitnob/stablecoin/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     3200 2022-08-11 16:47:55.000000 bitnob-1.2.7/bitnob/stablecoin/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.429018 bitnob-1.2.7/bitnob/virtual_card/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:38.000000 bitnob-1.2.7/bitnob/virtual_card/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     2513 2022-08-09 09:26:36.000000 bitnob-1.2.7/bitnob/virtual_card/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     9438 2022-08-09 12:34:35.000000 bitnob-1.2.7/bitnob/virtual_card/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.429513 bitnob-1.2.7/bitnob/wallet/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:46.000000 bitnob-1.2.7/bitnob/wallet/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     1120 2022-05-17 17:43:29.000000 bitnob-1.2.7/bitnob/wallet/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     1551 2022-03-10 18:39:16.000000 bitnob-1.2.7/bitnob/wallet/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.424977 bitnob-1.2.7/bitnob.egg-info/
--rw-r--r--   0 gabby      (501) staff       (20)     4640 2022-08-11 16:49:50.000000 bitnob-1.2.7/bitnob.egg-info/PKG-INFO
--rw-r--r--   0 gabby      (501) staff       (20)     1043 2022-08-11 16:49:50.000000 bitnob-1.2.7/bitnob.egg-info/SOURCES.txt
--rw-r--r--   0 gabby      (501) staff       (20)        1 2022-08-11 16:49:50.000000 bitnob-1.2.7/bitnob.egg-info/dependency_links.txt
--rw-r--r--   0 gabby      (501) staff       (20)        9 2022-08-11 16:49:50.000000 bitnob-1.2.7/bitnob.egg-info/requires.txt
--rw-r--r--   0 gabby      (501) staff       (20)       13 2022-08-11 16:49:50.000000 bitnob-1.2.7/bitnob.egg-info/top_level.txt
--rw-r--r--   0 gabby      (501) staff       (20)       38 2022-08-11 16:49:50.430871 bitnob-1.2.7/setup.cfg
--rw-r--r--   0 gabby      (501) staff       (20)      766 2022-08-11 16:49:46.000000 bitnob-1.2.7/setup.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2022-08-11 16:49:50.430425 bitnob-1.2.7/tests/
--rw-r--r--   0 gabby      (501) staff       (20)       28 2022-02-20 16:42:43.000000 bitnob-1.2.7/tests/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)      452 2022-02-20 17:33:40.000000 bitnob-1.2.7/tests/test_customer.py
--rw-r--r--   0 gabby      (501) staff       (20)      239 2022-02-20 21:20:16.000000 bitnob-1.2.7/tests/test_onchain.py
--rw-r--r--   0 gabby      (501) staff       (20)     1188 2022-05-25 13:00:21.000000 bitnob-1.2.7/tests/test_stablecoins.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.459930 bitnob-1.2.8/
+-rw-r--r--   0 gabby      (501) staff       (20)     4640 2023-07-20 10:43:33.459810 bitnob-1.2.8/PKG-INFO
+-rw-r--r--   0 gabby      (501) staff       (20)     4153 2022-02-20 16:41:50.000000 bitnob-1.2.8/README.md
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.455144 bitnob-1.2.8/bitnob/
+-rw-r--r--   0 gabby      (501) staff       (20)      459 2022-05-12 20:22:23.000000 bitnob-1.2.8/bitnob/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     2754 2023-07-20 09:58:05.000000 bitnob-1.2.8/bitnob/base.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.456204 bitnob-1.2.8/bitnob/customer/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:02:35.000000 bitnob-1.2.8/bitnob/customer/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)      277 2022-03-03 22:56:33.000000 bitnob-1.2.8/bitnob/customer/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     2929 2023-07-20 09:58:17.000000 bitnob-1.2.8/bitnob/customer/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.456541 bitnob-1.2.8/bitnob/exceptions/
+-rw-r--r--   0 gabby      (501) staff       (20)      200 2022-02-20 16:49:05.000000 bitnob-1.2.8/bitnob/exceptions/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1800 2022-02-20 16:49:05.000000 bitnob-1.2.8/bitnob/exceptions/exceptions.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.456935 bitnob-1.2.8/bitnob/hosted_checkout/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:04:50.000000 bitnob-1.2.8/bitnob/hosted_checkout/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1830 2022-05-17 17:44:31.000000 bitnob-1.2.8/bitnob/hosted_checkout/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     3233 2023-07-20 09:58:17.000000 bitnob-1.2.8/bitnob/hosted_checkout/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.457335 bitnob-1.2.8/bitnob/lightning/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:22.000000 bitnob-1.2.8/bitnob/lightning/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1722 2022-03-03 23:00:29.000000 bitnob-1.2.8/bitnob/lightning/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     4912 2023-07-20 10:07:41.000000 bitnob-1.2.8/bitnob/lightning/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.457718 bitnob-1.2.8/bitnob/ln_url/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-05-12 20:16:47.000000 bitnob-1.2.8/bitnob/ln_url/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)      505 2022-03-17 20:39:17.000000 bitnob-1.2.8/bitnob/ln_url/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     5560 2023-07-20 09:58:17.000000 bitnob-1.2.8/bitnob/ln_url/services.py
+-rw-r--r--   0 gabby      (501) staff       (20)      250 2022-03-13 23:47:17.000000 bitnob-1.2.8/bitnob/model.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.458055 bitnob-1.2.8/bitnob/onchain/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:29.000000 bitnob-1.2.8/bitnob/onchain/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-03-03 22:48:54.000000 bitnob-1.2.8/bitnob/onchain/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     3090 2023-07-20 10:06:55.000000 bitnob-1.2.8/bitnob/onchain/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.458394 bitnob-1.2.8/bitnob/stablecoin/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:18:11.000000 bitnob-1.2.8/bitnob/stablecoin/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)      836 2022-08-11 16:48:09.000000 bitnob-1.2.8/bitnob/stablecoin/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     3751 2023-07-20 10:04:32.000000 bitnob-1.2.8/bitnob/stablecoin/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.458754 bitnob-1.2.8/bitnob/virtual_card/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:38.000000 bitnob-1.2.8/bitnob/virtual_card/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     2513 2022-08-09 09:26:36.000000 bitnob-1.2.8/bitnob/virtual_card/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     9437 2023-07-20 09:58:17.000000 bitnob-1.2.8/bitnob/virtual_card/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.459103 bitnob-1.2.8/bitnob/wallet/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:46.000000 bitnob-1.2.8/bitnob/wallet/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1576 2023-07-20 10:01:51.000000 bitnob-1.2.8/bitnob/wallet/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     4123 2023-07-20 10:02:33.000000 bitnob-1.2.8/bitnob/wallet/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.455850 bitnob-1.2.8/bitnob.egg-info/
+-rw-r--r--   0 gabby      (501) staff       (20)     4640 2023-07-20 10:43:33.000000 bitnob-1.2.8/bitnob.egg-info/PKG-INFO
+-rw-r--r--   0 gabby      (501) staff       (20)     1043 2023-07-20 10:43:33.000000 bitnob-1.2.8/bitnob.egg-info/SOURCES.txt
+-rw-r--r--   0 gabby      (501) staff       (20)        1 2023-07-20 10:43:33.000000 bitnob-1.2.8/bitnob.egg-info/dependency_links.txt
+-rw-r--r--   0 gabby      (501) staff       (20)        9 2023-07-20 10:43:33.000000 bitnob-1.2.8/bitnob.egg-info/requires.txt
+-rw-r--r--   0 gabby      (501) staff       (20)       13 2023-07-20 10:43:33.000000 bitnob-1.2.8/bitnob.egg-info/top_level.txt
+-rw-r--r--   0 gabby      (501) staff       (20)       38 2023-07-20 10:43:33.459968 bitnob-1.2.8/setup.cfg
+-rw-r--r--   0 gabby      (501) staff       (20)      766 2023-07-20 10:40:58.000000 bitnob-1.2.8/setup.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-20 10:43:33.459592 bitnob-1.2.8/tests/
+-rw-r--r--   0 gabby      (501) staff       (20)       28 2022-02-20 16:42:43.000000 bitnob-1.2.8/tests/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)      452 2022-02-20 17:33:40.000000 bitnob-1.2.8/tests/test_customer.py
+-rw-r--r--   0 gabby      (501) staff       (20)      239 2022-02-20 21:20:16.000000 bitnob-1.2.8/tests/test_onchain.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1188 2022-05-25 13:00:21.000000 bitnob-1.2.8/tests/test_stablecoins.py
```

### Comparing `bitnob-1.2.7/PKG-INFO` & `bitnob-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitnob
-Version: 1.2.7
+Version: 1.2.8
 Summary: Python SDK for the Bitnob"s API
 Home-page: https://github.com/bitnob/bitnob_python_sdk
 Author: Bitnob
 Author-email: info@bitnob.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bitnob-1.2.7/README.md` & `bitnob-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.7/bitnob/base.py` & `bitnob-1.2.8/bitnob/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 exception = exception_class.get(data["statusCode"])
                 raise exception(data["message"])
             except KeyError:
                 return data
         except (HTTPError, ConnectionError) as e:
             return e
     
-    def check_required_datas(self, required_data, passed_param):
+    def check_required_data(self, required_data, passed_param):
         """
         function to check required params 
         """
         for key in required_data:
             if key not in passed_param.keys():
                 added_message = "The following are required: " + ",".join(required_data)
                 message = f'{key} is required! ' + added_message
```

### Comparing `bitnob-1.2.7/bitnob/customer/services.py` & `bitnob-1.2.8/bitnob/customer/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             "phone": "9xxxxxxxx",
             "countryCode": "+234"
         }
 
         - POST Request
         """
         required_data = ["email", "firstName", "lastName", "phone", "countryCode"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
         
         response = self.send_request("POST", "customers", json=body)
         return self.__generate_user_object(data=response.get("data"))
 
 
 
     def list_customers(self, **kwargs):
```

### Comparing `bitnob-1.2.7/bitnob/exceptions/exceptions.py` & `bitnob-1.2.8/bitnob/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.7/bitnob/hosted_checkout/model.py` & `bitnob-1.2.8/bitnob/hosted_checkout/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.7/bitnob/hosted_checkout/services.py` & `bitnob-1.2.8/bitnob/hosted_checkout/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             successUrl: "htpps://domain.com/successUrl",
             reference: "reference"
         }
 
         - POST Request
         """
         required_data =  ["amount", "description", "customerEmail", "notificationEmail", "callbackUrl", "successUrl", "reference"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
         
         response = self.send_request("POST", "checkout", json=body)
         return self.__generate_checkout_object(data=response.get("data"))
 
     def list_checkouts(self, **kwargs):
         """
         Listing checkouts
```

### Comparing `bitnob-1.2.7/bitnob/lightning/model.py` & `bitnob-1.2.8/bitnob/lightning/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.7/bitnob/lightning/services.py` & `bitnob-1.2.8/bitnob/lightning/services.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,33 +9,36 @@
         return Invoice(
             description = data.get("description"),
             tokens=data.get("tokens"),
             request=data.get("request")
         )
     
     def __generate_transaction_object(self, data):
+        
         return Transaction(            
             reference = data.get("reference"),
             description = data.get("description"),
             amount = data.get("amount"),
+            btc_amount = data.get("btcAmount"),
             sat_amount = data.get("satAmount"),
             fees = data.get("fees"),
             btc_fees = data.get("btcFees"),
             sat_fees = data.get("satFees"),
             action = data.get("action"),
             transaction_type = data.get("type"),
             status = data.get("status"),
-            id=data.get("id"),
-            invoice_id=data.get("invoiceId"),
-            channel=data.get("channel"),
-            address=data.get("address"),
-            payment_request=data.get("paymentRequest"),
-            spot_price=data.get("spotPrice"),
-            hash=data.get("hash"),
-            confirmations=data.get("confirmations")
+            id = data.get("id"),
+            companyId = data.get("companyId"),
+            spot_price = data.get("spotPrice"),
+            createdAt = data.get("createdAt"), 
+            updatedAt = data.get("updatedAt"),
+            address = data.get("address"),
+            channel = data.get("channel"),
+            chain = data.get("chain"),
+            customerId = data.get("customerId")
         )
     
     def create_invoice(self, body:dict):
         """
         Creating lightning invoice for customer
 
         body = {
@@ -48,15 +51,15 @@
         }
 
         required_data = "description", "tokens", "customerEmail"
 
         - POST Request
         """
         required_data = ["description", "tokens", "customerEmail"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "wallets/ln/createinvoice", json=body)
         return self.__generate_invoice_object(data=response["data"])
 
 
     def pay_invoice(self, body:dict):
         """
@@ -68,15 +71,15 @@
         }
 
         required_data = "request", "reference"
 
         - POST Request
         """
         required_data = ["request", "reference"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "wallets/ln/pay", json=body)
         return self.__generate_transaction_object(data=response["data"])
     
     def initiate_payment(self, invoice_request):
         """
         Initiate payment on lighting network.
```

### Comparing `bitnob-1.2.7/bitnob/ln_url/services.py` & `bitnob-1.2.8/bitnob/ln_url/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         }
 
         required_data = "identifier", "tld", "customerEmail"
 
         - POST Request
         """
         required_data = ["identifier", "tld", "customerEmail"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
         response = self.send_request("POST", "lnurl", json=body)
         return self.__generate_ln_url_object(data=response.get("data"))
 
     def decode_lnurl(self, encoded_lnurl):
         """
         Decode LnUrl
 
@@ -64,15 +64,15 @@
         }
 
         required_data = "encodedLnUrl", "reference", "satoshis", "customerEmail"
 
         - POST Request
         """
         required_data = ["encodedLnUrl", "reference", "satoshis", "customerEmail"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "lnurl/paylnurl", json=body)
         return response
     
 
     def create_ln_withdrawal(self, body:dict):
         """
@@ -85,15 +85,15 @@
         }
 
         required_data = "description", "satoshis", "customerEmail"
 
         - POST Request
         """
         required_data =  ["description", "satoshis", "customerEmail"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "lnurl/createLnUrlWithdrawal", json=body)
         return response
     
     def decode_lnaddress(self, ln_address):
         """
         Decode lnaddress
@@ -120,15 +120,15 @@
         }
 
         required_data = "encodedLnUrl", "reference", "satoshis", "customerEmail"
 
         - POST Request
         """
         required_data = ["lnAddress", "reference", "satoshis", "customerEmail"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "lnurl/paylnaddress", json=body)
         return response
     
     def list_lnurls(self, **kwargs):
         """
         Listing lnurls
```

### Comparing `bitnob-1.2.7/bitnob/onchain/services.py` & `bitnob-1.2.8/bitnob/onchain/services.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,36 +8,38 @@
         return WalletAddress(
             address = data.get("address"),
             address_type=data.get("addressType"),
             label=data.get("label")
         )
     
     def __generate_transaction_object(self, data):
+        
         return Transaction(            
             reference = data.get("reference"),
             description = data.get("description"),
             amount = data.get("amount"),
+            btc_amount = data.get("btcAmount"),
             sat_amount = data.get("satAmount"),
             fees = data.get("fees"),
             btc_fees = data.get("btcFees"),
             sat_fees = data.get("satFees"),
             action = data.get("action"),
             transaction_type = data.get("type"),
             status = data.get("status"),
-            id=data.get("id"),
-            invoice_id=data.get("invoiceId"),
-            channel=data.get("channel"),
-            address=data.get("address"),
-            payment_request=data.get("paymentRequest"),
-            spot_price=data.get("spotPrice"),
-            hash=data.get("hash"),
-            confirmations=data.get("confirmations")
+            id = data.get("id"),
+            companyId = data.get("companyId"),
+            spot_price = data.get("spotPrice"),
+            createdAt = data.get("createdAt"), 
+            updatedAt = data.get("updatedAt"),
+            address = data.get("address"),
+            channel = data.get("channel"),
+            chain = data.get("chain"),
+            customerId = data.get("customerId")
         )
 
-    
     def send_bitcoin(self, body:dict):
         """
         Sending bitcoin
 
         body = {
             "satoshis": 3000,
             "address": "tb1q9h0yjdupyfpxfjg24rpx755xrplvzd9hz2nj7v",
@@ -47,15 +49,15 @@
         }
 
         required_data = "satoshis", "address", "customerEmail"
 
         - POST Request
         """
         required_data = ["satoshis", "address", "customerEmail"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "wallets/send_bitcoin", json=body)
         return self.__generate_transaction_object(data=response["data"])
 
     def generate_address(self, body:dict):
         """
         Generate Address for Customer
@@ -64,15 +66,15 @@
             "label": "purchase xbox",
             "customerEmail": "customer@gmail.com"
         }
 
         - POST Request
         """
         required_data = ["customerEmail"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "addresses/generate", json=body)
         return self.__generate_address_object(data=response["data"])
     
     def list_addresses(self, **kwargs):
         """
         Getting addresses attached to company
@@ -82,9 +84,9 @@
         url_params = None
         if kwargs != {}:
             url_params = pagination_filter(**kwargs)
         response =  self.send_request("GET", f"/addresses/?{url_params}",)
         data = response.get("data")
         return [self.__generate_address_object(address_data) for address_data in data]
     
-    def get_recommeded_btc_fes(self):
+    def get_recommended_btc_fes(self):
         return self.send_request("GET", "recommended-fees/btc")
```

### Comparing `bitnob-1.2.7/bitnob/stablecoin/model.py` & `bitnob-1.2.8/bitnob/stablecoin/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.7/bitnob/stablecoin/services.py` & `bitnob-1.2.8/bitnob/stablecoin/services.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 from bitnob.base import Bitnob
 from abc import ABC, abstractmethod
 from bitnob.stablecoin.model import Receipt
-from bitnob.wallet.model import WalletAddress
+from bitnob.wallet.model import WalletAddress, Transaction
 
 class StableCoin(ABC):
 
     @abstractmethod
     def send(self):
         pass
 
     @abstractmethod
     def generate_address(self):
         pass
 
-    def generate_address_object(self, data):
+    def __generate_address_object(self, data):
         return WalletAddress(
             address = data.get("address"),
             address_type=data.get("addressType"),
             label=data.get("label")
         )
     
-    def generate_receipt_object(self, data):
-        return Receipt(
+    def ____generate_transaction_object(self, data):
+        
+        return Transaction(            
             reference = data.get("reference"),
             description = data.get("description"),
             amount = data.get("amount"),
+            btc_amount = data.get("btcAmount"),
+            sat_amount = data.get("satAmount"),
             fees = data.get("fees"),
+            btc_fees = data.get("btcFees"),
+            sat_fees = data.get("satFees"),
             action = data.get("action"),
-            receipt_type = data.get("type"),
+            transaction_type = data.get("type"),
             status = data.get("status"),
-            id=data.get("id")
-            hash=data.get("hash")
+            id = data.get("id"),
+            companyId = data.get("companyId"),
+            spot_price = data.get("spotPrice"),
+            createdAt = data.get("createdAt"), 
+            updatedAt = data.get("updatedAt"),
+            address = data.get("address"),
+            channel = data.get("channel"),
+            chain = data.get("chain"),
+            customerId = data.get("customerId")
         )
     
 
 
 
 class USDC(StableCoin, Bitnob): 
     
@@ -48,18 +60,18 @@
             chain: "BSC"
             description: "lorem ipsum",
         } 
 
         - POST Request
         """
         required_data = ["amount", "address", "chain"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "wallets/send-usdc", json=body)
-        return self.generate_receipt_object(data=response["data"])
+        return self.(data=response["data"])
 
 
     def generate_address(self, body:dict):
         """
         Generate Address for Customer
 
         body = {
@@ -67,18 +79,18 @@
             "customerEmail": "customer@gmail.com",
             "chain": "BSC"
         }
 
         - POST Request
         """
         required_data = ["customerEmail", "chain"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response =  self.send_request("POST", "addresses/generate/usdc", json=body)
-        return self.generate_address_object(data=response["data"])
+        return self.__generate_address_object(data=response["data"])
 
 class USDT(StableCoin, Bitnob): 
     
     def send(self, body:dict):
         """
         Sending USDC
 
@@ -88,29 +100,29 @@
             chain: "BSC",
             description: "lorem ipsum",
         } 
 
         - POST Request
         """
         required_data = ["amount", "address", "chain"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "wallets/send-usdt", json=body)
-        return self.generate_receipt_object(data=response["data"])
+        return self.__generate_transaction_object(data=response["data"])
 
     def generate_address(self, body:dict):
         """
         Generate Address for Customer
 
         body = {
             "label": "purchase xbox",
             "customerEmail": "customer@gmail.com"
             "chain": "BSC"
         }
 
         - POST Request
         """
         required_data = ["customerEmail", "chain"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
 
         response =  self.send_request("POST", "addresses/generate/usdt", json=body)
-        return self.generate_address_object(data=response["data"])
+        return self.__generate_address_object(data=response["data"])
```

### Comparing `bitnob-1.2.7/bitnob/virtual_card/model.py` & `bitnob-1.2.8/bitnob/virtual_card/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.7/bitnob/virtual_card/services.py` & `bitnob-1.2.8/bitnob/virtual_card/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             line1: "38 West Street",
             line2: "Apt. 1",
         }
 
         - POST Request
         """
         required_data = ["customerEmail", "idNumber", "idNumber", "firstName", "lastName", "city", "state", "country", "zipCode", "line1", "phoneNumber", "userPhoto"]
-        self.check_required_datas(required_data, body)
+        self.check_required_data(required_data, body)
         
         response = self.send_request("POST", "virtualcards/registercarduser", json=body)
         return self.__generate_card_user_object(data=response["data"])
         
     def create_card(self, body:dict):
         """
         Create Card for customer
```

### Comparing `bitnob-1.2.7/bitnob.egg-info/PKG-INFO` & `bitnob-1.2.8/bitnob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitnob
-Version: 1.2.7
+Version: 1.2.8
 Summary: Python SDK for the Bitnob"s API
 Home-page: https://github.com/bitnob/bitnob_python_sdk
 Author: Bitnob
 Author-email: info@bitnob.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bitnob-1.2.7/bitnob.egg-info/SOURCES.txt` & `bitnob-1.2.8/bitnob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.7/setup.py` & `bitnob-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="bitnob",
-    version="1.2.7",
+    version="1.2.8",
     description="Python SDK for the Bitnob\"s API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bitnob/bitnob_python_sdk",
     author="Bitnob",
     author_email="info@bitnob.com",
     license="MIT",
```

### Comparing `bitnob-1.2.7/tests/test_stablecoins.py` & `bitnob-1.2.8/tests/test_stablecoins.py`

 * *Files identical despite different names*

