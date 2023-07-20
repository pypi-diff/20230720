# Comparing `tmp/pyakamai-1.23-py3-none-any.whl.zip` & `tmp/pyakamai-1.25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 28266 bytes, number of entries: 19
+Zip file size: 29368 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      454 b- defN 23-May-01 03:11 pyakamai/__init__.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Jul-20 07:24 pyakamai/akamaiapidefinition.py
 -rw-r--r--  2.0 unx     3819 b- defN 23-Jul-09 12:14 pyakamai/akamaicasemanagement.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-May-01 03:29 pyakamai/akamaicpcode.py
 -rw-r--r--  2.0 unx     2332 b- defN 23-Apr-30 11:30 pyakamai/akamaicps.py
 -rw-r--r--  2.0 unx     9439 b- defN 23-Jun-08 00:37 pyakamai/akamaidatastream.py
 -rw-r--r--  2.0 unx     4408 b- defN 23-Apr-30 10:57 pyakamai/akamaiedns.py
 -rw-r--r--  2.0 unx     2843 b- defN 23-Apr-30 15:28 pyakamai/akamaiehn.py
 -rw-r--r--  2.0 unx    14193 b- defN 23-May-01 03:54 pyakamai/akamaiksd1.py
 -rw-r--r--  2.0 unx     5689 b- defN 23-May-01 03:31 pyakamai/akamaiksd2.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-Jul-09 11:44 pyakamai/akamailds.py
 -rw-r--r--  2.0 unx     3878 b- defN 23-Jun-08 00:38 pyakamai/akamaimsl.py
 -rw-r--r--  2.0 unx    29604 b- defN 23-Jul-04 02:23 pyakamai/akamaiproperty.py
 -rw-r--r--  2.0 unx     3506 b- defN 23-Apr-30 15:04 pyakamai/akamaipurge.py
--rw-r--r--  2.0 unx     8058 b- defN 23-Jun-20 14:25 pyakamai/http_calls.py
--rw-r--r--  2.0 unx     2624 b- defN 23-Jun-08 00:08 pyakamai/pyakamai.py
--rw-r--r--  2.0 unx    12832 b- defN 23-Jul-09 14:37 pyakamai-1.23.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 14:37 pyakamai-1.23.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 14:37 pyakamai-1.23.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1499 b- defN 23-Jul-09 14:37 pyakamai-1.23.dist-info/RECORD
-19 files, 109195 bytes uncompressed, 25854 bytes compressed:  76.3%
+-rw-r--r--  2.0 unx     8308 b- defN 23-Jul-20 07:45 pyakamai/http_calls.py
+-rw-r--r--  2.0 unx     2830 b- defN 23-Jul-20 07:10 pyakamai/pyakamai.py
+-rw-r--r--  2.0 unx    12832 b- defN 23-Jul-20 08:29 pyakamai-1.25.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 08:29 pyakamai-1.25.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-20 08:29 pyakamai-1.25.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1587 b- defN 23-Jul-20 08:29 pyakamai-1.25.dist-info/RECORD
+20 files, 111978 bytes uncompressed, 26818 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: pyakamai/__init__.py
 Comment: 
 
+Filename: pyakamai/akamaiapidefinition.py
+Comment: 
+
 Filename: pyakamai/akamaicasemanagement.py
 Comment: 
 
 Filename: pyakamai/akamaicpcode.py
 Comment: 
 
 Filename: pyakamai/akamaicps.py
@@ -39,20 +42,20 @@
 
 Filename: pyakamai/http_calls.py
 Comment: 
 
 Filename: pyakamai/pyakamai.py
 Comment: 
 
-Filename: pyakamai-1.23.dist-info/METADATA
+Filename: pyakamai-1.25.dist-info/METADATA
 Comment: 
 
-Filename: pyakamai-1.23.dist-info/WHEEL
+Filename: pyakamai-1.25.dist-info/WHEEL
 Comment: 
 
-Filename: pyakamai-1.23.dist-info/top_level.txt
+Filename: pyakamai-1.25.dist-info/top_level.txt
 Comment: 
 
-Filename: pyakamai-1.23.dist-info/RECORD
+Filename: pyakamai-1.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyakamai/http_calls.py

```diff
@@ -45,14 +45,15 @@
         """ Executes a GET API call and returns the JSON output """
         path = endpoint
         endpoint_result = self.session.get(parse.urljoin(self.baseurl,path), headers=headers,params=params)
         if self.verbose: print (">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
         status = endpoint_result.status_code
         if self.verbose: print( "LOG: GET %s %s %s" % (endpoint,status,endpoint_result.headers["content-type"]))
         self.httpErrors(endpoint_result.status_code, path, endpoint_result.json())
+        formattedjson = json.dumps(endpoint_result.json(),indent=2)
         return status,endpoint_result.json()
 
 
     def postResult(self, endpoint, body,params=None,headers=None):
         """ Executes a GET API call and returns the JSON output """
         if headers == None:
             headers = {'content-type': 'application/json'}
@@ -64,15 +65,17 @@
             print("LOG: POST %s %s %s" % (path, status, endpoint_result.headers["content-type"]))
         if status == 204:
             return status,{}
         self.httpErrors(endpoint_result.status_code, path, endpoint_result.json())
 
         if self.verbose:
             print(">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
-        return status,endpoint_result.json()
+        formattedjson = json.dumps(endpoint_result.json(),indent=2)
+        return status,formattedjson
+    
 
     def patchResult(self, endpoint, body, parameters=None):
         """ Executes a GET API call and returns the JSON output """
         headers = {'content-type': 'application/json-patch+json'}
         path = endpoint
         endpoint_result = self.session.patch(parse.urljoin(self.baseurl, path), data=body, headers=headers, params=parameters)
         status = endpoint_result.status_code
@@ -80,15 +83,16 @@
             print("LOG: POST %s %s %s" % (path, status, endpoint_result.headers["content-type"]))
         if status == 204:
             return {}
         self.httpErrors(endpoint_result.status_code, path, endpoint_result.json())
 
         if self.verbose:
             print(">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
-        return status,endpoint_result.json()
+        formattedjson = json.dumps(endpoint_result.json(),indent=2)
+        return status,formattedjson
 
     def postFiles(self, endpoint, file):
         """ Executes a POST API call and returns the JSON output """
         path = endpoint
         endpoint_result = self.session.post(parse.urljoin(self.baseurl, path), files=file)
         status = endpoint_result.status_code
         if self.verbose:
@@ -111,15 +115,16 @@
         status = endpoint_result.status_code
         if self.verbose:
             print("LOG: PUT %s %s %s" % (endpoint, status, endpoint_result.headers["content-type"]))
         if status == 204:
             return status,{}
         if self.verbose:
             print(">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
-        return status,endpoint_result.json()
+        formattedjson = json.dumps(endpoint_result.json(),indent=2)
+        return status,formattedjson
 
     def deleteResult(self, endpoint):
         """ Executes a DELETE API call and returns the JSON output """
         endpoint_result = self.session.delete(parse.urljoin(self.baseurl,endpoint))
         status = endpoint_result.status_code
         if self.verbose:
             print("LOG: DELETE %s %s %s" % (endpoint, status, endpoint_result.headers["content-type"]))
```

## pyakamai/pyakamai.py

```diff
@@ -5,14 +5,15 @@
 from .akamaidatastream import AkamaiDataStream
 from .akamaiedns import AkamaiEDNS
 from .akamaicps import AkamaiCPS
 from .akamailds import AkamaiLDS
 from .akamaipurge import AkamaiPurge
 from .akamaiehn import AkamaiEdgeHostName
 from .akamaicasemanagement import AkamaiCaseManagement
+from .akamaiapidefinition import AkamaiAPIDefinition
 import sys
 import os
 import requests
 import logging
 import json
 
 if sys.version_info[0] >= 3:
@@ -64,11 +65,14 @@
         elif product == 'purge':
             class_obj = AkamaiPurge(self._prdHttpCaller,*args)
         
         elif product == 'ehn':
             class_obj = AkamaiEdgeHostName(self._prdHttpCaller,self.accountSwitchKey,*args)
 
         elif product in ['case','casemanagement']:
-            class_obj = AkamaiCaseManagement(self._prdHttpCaller,self.accountSwitchKey,*args)            
+            class_obj = AkamaiCaseManagement(self._prdHttpCaller,self.accountSwitchKey,*args)     
+
+        elif product in ['apidefinition','apigateway']:
+            class_obj = AkamaiAPIDefinition(self._prdHttpCaller,self.accountSwitchKey,*args)          
 
 
         return class_obj
```

## Comparing `pyakamai-1.23.dist-info/METADATA` & `pyakamai-1.25.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyakamai
-Version: 1.23
+Version: 1.25
 Summary: A Boto3 like SDK for Akamai
 Home-page: https://github.com/Achuthananda/pyakamai
 Author: Achuthananda M P
 Author-email: achuthadivine@gmail.com
 Project-URL: Source, https://github.com/Achuthananda/pyakamai
 Keywords: Akamai Python CDN SDK Edge
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyakamai-1.23.dist-info/RECORD` & `pyakamai-1.25.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 pyakamai/__init__.py,sha256=JER0abqNyr-F_5XlBsXxh3NEbppAZa4pygHLoBmtMEU,454
+pyakamai/akamaiapidefinition.py,sha256=VdEs5O4Kg3H183isRaayTckdwhEgG9V-LWfpL5ymDP0,2239
 pyakamai/akamaicasemanagement.py,sha256=WHZt-mfILmuhnOaiiuLZrXZ9gK--uICyM0DURpOod_Q,3819
 pyakamai/akamaicpcode.py,sha256=yQ31HE7krGBo_7tn8iGBwt0UtBHMM-wnTP33hwsamiI,1473
 pyakamai/akamaicps.py,sha256=6WOARWxWlkauMawOH4BE2-VJKdMgpqKdtcX8TXLKIgs,2332
 pyakamai/akamaidatastream.py,sha256=TaU8glzaoiZMdwk3n1vdzsOKAP1nWhfEBQSz0lki9F8,9439
 pyakamai/akamaiedns.py,sha256=ROh3xQjOxalGnya97FyxE-iYZgZniD8GAGH1mhwjvRs,4408
 pyakamai/akamaiehn.py,sha256=aZ2U6YG54IKP5vuQPd5GygalsJqVuEzvCnALjjszRFI,2843
 pyakamai/akamaiksd1.py,sha256=7RslIDB6oR3KA4nyC7infxXqH4Jr7dM0t3znyDfCUPI,14193
 pyakamai/akamaiksd2.py,sha256=CWo_ejWDPoyiTWROrbc_OTmcq7RXZBb8n8xOYVXQ3w8,5689
 pyakamai/akamailds.py,sha256=Rt4Lp4Hmu6T5sx0jCp3iB7YMowKSdIrk6E2NP_JWYXA,2443
 pyakamai/akamaimsl.py,sha256=ykRv_yy-qVWs37Wu2auDddX4IEuSWiO-1g9p59LTYww,3878
 pyakamai/akamaiproperty.py,sha256=jh1ooqCel03ADDtKhTOWUoW_F03ez-SH2U5iaqhF3cs,29604
 pyakamai/akamaipurge.py,sha256=FLwfjbhjn0PZyRRq68SpKFF9f8JPk76DKvCmmVg2NtU,3506
-pyakamai/http_calls.py,sha256=vH5oWXTuMtSq64crAycijH5EFQC-9QAQf--Da-qlS-I,8058
-pyakamai/pyakamai.py,sha256=xqX5Ms9Rcl4qTxkvpI5tm_AUI0qgIEyf0Jda6b-gP9c,2624
-pyakamai-1.23.dist-info/METADATA,sha256=e7QkyVwzQhKfSsXKTXOYyNzKkQfP6HbeZaZx2KEnrdc,12832
-pyakamai-1.23.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyakamai-1.23.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
-pyakamai-1.23.dist-info/RECORD,,
+pyakamai/http_calls.py,sha256=S20uXu1_czpu5jUMqsV9sHz91UJDRjtdFv6AHnb3ceQ,8308
+pyakamai/pyakamai.py,sha256=pBI6CoOcV0JOBRntQ7YfU_Wn6gKC07LwnDRg4JfqDMQ,2830
+pyakamai-1.25.dist-info/METADATA,sha256=t1DyUKeU-s7c1IJm8UI8awphi3Wccli1Vb2bDmKrbTE,12832
+pyakamai-1.25.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyakamai-1.25.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
+pyakamai-1.25.dist-info/RECORD,,
```

