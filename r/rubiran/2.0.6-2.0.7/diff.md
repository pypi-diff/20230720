# Comparing `tmp/rubiran-2.0.6.tar.gz` & `tmp/rubiran-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubiran-2.0.6.tar", last modified: Thu Jul 20 20:14:44 2023, max compression
+gzip compressed data, was "rubiran-2.0.7.tar", last modified: Thu Jul 20 20:29:12 2023, max compression
```

## Comparing `rubiran-2.0.6.tar` & `rubiran-2.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:14:44.034005 rubiran-2.0.6/
--rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.6/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)     1593 2023-07-20 20:14:44.038005 rubiran-2.0.6/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.6/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:14:43.878005 rubiran-2.0.6/rubiran/
--rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.6/rubiran/An_Wb.py
--rw-rw----   0 root         (0) everybody  (9997)     1103 2023-07-20 20:12:52.000000 rubiran-2.0.6/rubiran/How.py
--rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.6/rubiran/Socket.py
--rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.6/rubiran/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    53654 2023-07-20 20:10:48.000000 rubiran-2.0.6/rubiran/client.py
--rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.6/rubiran/encryption.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:14:44.014005 rubiran-2.0.6/rubiran.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1593 2023-07-20 20:14:43.000000 rubiran-2.0.6/rubiran.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 20:14:43.000000 rubiran-2.0.6/rubiran.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 20:14:43.000000 rubiran-2.0.6/rubiran.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 20:14:43.000000 rubiran-2.0.6/rubiran.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 20:14:44.046005 rubiran-2.0.6/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1837 2023-07-20 20:13:07.000000 rubiran-2.0.6/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:29:12.382005 rubiran-2.0.7/
+-rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.7/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     1593 2023-07-20 20:29:12.386005 rubiran-2.0.7/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.7/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:29:12.078005 rubiran-2.0.7/rubiran/
+-rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.7/rubiran/An_Wb.py
+-rw-rw----   0 root         (0) everybody  (9997)     1103 2023-07-20 20:26:39.000000 rubiran-2.0.7/rubiran/How.py
+-rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.7/rubiran/Socket.py
+-rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.7/rubiran/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    53857 2023-07-20 20:21:36.000000 rubiran-2.0.7/rubiran/client.py
+-rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.7/rubiran/encryption.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:29:12.342005 rubiran-2.0.7/rubiran.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1593 2023-07-20 20:29:10.000000 rubiran-2.0.7/rubiran.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 20:29:10.000000 rubiran-2.0.7/rubiran.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 20:29:10.000000 rubiran-2.0.7/rubiran.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 20:29:10.000000 rubiran-2.0.7/rubiran.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 20:29:12.406005 rubiran-2.0.7/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1837 2023-07-20 20:26:31.000000 rubiran-2.0.7/setup.py
```

### Comparing `rubiran-2.0.6/LICENCE` & `rubiran-2.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.6/PKG-INFO` & `rubiran-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.6
+Version: 2.0.7
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
@@ -48,15 +48,15 @@
 ``` bash
 from rubiran import rubiran
 ```
 
 ### How to install the library
 
 ``` bash
-pip install rubiran==2.0.6
+pip install rubiran==2.0.7
 ```
 
 ### My ID in Rubika
 
 ``` bash
 @professor_102
 ```
```

### Comparing `rubiran-2.0.6/rubiran/An_Wb.py` & `rubiran-2.0.7/rubiran/An_Wb.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.6/rubiran/How.py` & `rubiran-2.0.7/rubiran/How.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       white = '\033[97m'
       bold = '\033[1m'
       underline = '\033[4m'
       black='\033[30m'
 
 class chup:
       x_coder = f"""{color.bold}
-{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.6
+{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.7
  
 
 {color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐂𝐎𝐏𝐘𝐑𝐈𝐆𝐇𝐓 (𝐂) {color.red} 2023 {color.green}𝐌𝐀𝐌𝐀𝐃 𝐂𝐎𝐃𝐄𝐑   
 
 {color.white} [⏦] - {color.cyan} 𝐃𝐄𝐕𝐄𝐋𝐎𝐏𝐄𝐑  {color.yellow} 𝐑𝐔𝐁𝐈𝐊𝐀 {color.red} 𝐂𝐇𝐀𝐍𝐍𝐄𝐋 : {color.green} @python_java_source
 
 {color.white}╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾
```

### Comparing `rubiran-2.0.6/rubiran/Socket.py` & `rubiran-2.0.7/rubiran/Socket.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.6/rubiran/client.py` & `rubiran-2.0.7/rubiran/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,23 @@
 import math
 
 async def get(url,headers=None):
 	async with aiohttp.ClientSession() as session:
 		async with session.get(url,headers=headers) as response:
 			Post =  await response.text()
 			return Post
+async def postJ(url,data,headers=None):
+	async with aiohttp.ClientSession() as session:
+		async with session.post(url,data=dumps(data),headers=headers) as respon:
+			post = await respon.text()
+			return post
 
 async def post(url,data,headers=None):
 	async with aiohttp.ClientSession() as session:
-		async with session.post(url,data=dumps(data),headers=headers) as respon:
+		async with session.post(url,data=data,headers=headers) as respon:
 			post = await respon.text()
 			return post
 
 class rubiran:
 	def __init__(self, auth,privateKey):
 		self.Auth =  auth
 		self.print = chup.x_coder
@@ -51,15 +56,15 @@
                     'Origin': 'https://web.rubika.ir',
 					'Referer': f'https://web.rubika.ir/',
 					'Host':url.replace("https://","").replace("/",""),
 					'User-Agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"}
 
 		while True:
 		      try:
-		      	return asyncio.run(post(url,data=Indata,headers=headers))
+		      	return asyncio.run(postJ(url,data=Indata,headers=headers))
 		      except:continue
 		      
 	def send_post(self,inData):
 		
 		enc = self.enc
 		data = dumps(inData)
 		url = rubiran._getURL()
@@ -71,15 +76,15 @@
 					'Referer': f'https://web.rubika.ir/',
 					'Host':url.replace("https://","").replace("/",""),
 					'User-Agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"}
 		
 		
 		while True:
 		      try:
-		      	return asyncio.run(post(url,data=Indata,headers=headers))
+		      	return asyncio.run(postJ(url,data=Indata,headers=headers))
 		      except:continue
 
 	def registerDevice(self):
 	    inData = {"method":"registerDevice","input":{"app_version":"WB_4.1.2","device_hash":"0501110712007200125373640870428014153736","device_model":"rubiran-library","lang_code":"fa","system_version":"Linux","token":" ","token_type":"Web"},"client": SetClines.web}
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
```

### Comparing `rubiran-2.0.6/rubiran/encryption.py` & `rubiran-2.0.7/rubiran/encryption.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.6/rubiran.egg-info/PKG-INFO` & `rubiran-2.0.7/rubiran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.6
+Version: 2.0.7
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
@@ -48,15 +48,15 @@
 ``` bash
 from rubiran import rubiran
 ```
 
 ### How to install the library
 
 ``` bash
-pip install rubiran==2.0.6
+pip install rubiran==2.0.7
 ```
 
 ### My ID in Rubika
 
 ``` bash
 @professor_102
 ```
```

### Comparing `rubiran-2.0.6/setup.py` & `rubiran-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ``` bash
 from rubiran import rubiran
 ```
 
 ### How to install the library
 
 ``` bash
-pip install rubiran==2.0.6
+pip install rubiran==2.0.7
 ```
 
 ### My ID in Rubika
 
 ``` bash
 @professor_102
 ```
@@ -44,15 +44,15 @@
 ``` bash
 @python_java_source 
 ```
 """
 
 setup(
     name = "rubiran",
-    version = "2.0.6",
+    version = "2.0.7",
     author = "mamadcoder",
     author_email = "mamadcoder@gmail.com",
     description = ("Another example of the library making the Rubik's robot"),
     license = "MIT",
     keywords = ["rubika","bot","robot","library","rubikalib","rubikalib.ml","rubikalib.ir","rubika.ir","Rubika","Python","Pyrubika","pyrubika"],
     url = "https://rubika.ir/python_java_source",
     packages=['rubiran'],
```

