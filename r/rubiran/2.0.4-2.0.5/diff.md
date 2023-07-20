# Comparing `tmp/rubiran-2.0.4.tar.gz` & `tmp/rubiran-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubiran-2.0.4.tar", last modified: Thu Jul 20 19:42:59 2023, max compression
+gzip compressed data, was "rubiran-2.0.5.tar", last modified: Thu Jul 20 19:55:41 2023, max compression
```

## Comparing `rubiran-2.0.4.tar` & `rubiran-2.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:42:59.682005 rubiran-2.0.4/
--rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.4/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)     1586 2023-07-20 19:42:59.686005 rubiran-2.0.4/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.4/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:42:59.522005 rubiran-2.0.4/rubiran/
--rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.4/rubiran/An_Wb.py
--rw-rw----   0 root         (0) everybody  (9997)     1102 2023-07-20 19:41:19.000000 rubiran-2.0.4/rubiran/How.py
--rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.4/rubiran/Socket.py
--rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.4/rubiran/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    53638 2023-07-20 19:37:26.000000 rubiran-2.0.4/rubiran/client.py
--rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.4/rubiran/encryption.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:42:59.650005 rubiran-2.0.4/rubiran.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1586 2023-07-20 19:42:58.000000 rubiran-2.0.4/rubiran.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 19:42:58.000000 rubiran-2.0.4/rubiran.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 19:42:58.000000 rubiran-2.0.4/rubiran.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 19:42:58.000000 rubiran-2.0.4/rubiran.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 19:42:59.694005 rubiran-2.0.4/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1830 2023-07-20 19:41:43.000000 rubiran-2.0.4/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:55:41.814005 rubiran-2.0.5/
+-rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.5/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     1597 2023-07-20 19:55:41.822005 rubiran-2.0.5/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.5/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:55:41.638005 rubiran-2.0.5/rubiran/
+-rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.5/rubiran/An_Wb.py
+-rw-rw----   0 root         (0) everybody  (9997)     1102 2023-07-20 19:52:25.000000 rubiran-2.0.5/rubiran/How.py
+-rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.5/rubiran/Socket.py
+-rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.5/rubiran/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    53638 2023-07-20 19:52:06.000000 rubiran-2.0.5/rubiran/client.py
+-rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.5/rubiran/encryption.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:55:41.778005 rubiran-2.0.5/rubiran.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1597 2023-07-20 19:55:41.000000 rubiran-2.0.5/rubiran.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 19:55:41.000000 rubiran-2.0.5/rubiran.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 19:55:41.000000 rubiran-2.0.5/rubiran.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 19:55:41.000000 rubiran-2.0.5/rubiran.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 19:55:41.834005 rubiran-2.0.5/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1842 2023-07-20 19:53:49.000000 rubiran-2.0.5/setup.py
```

### Comparing `rubiran-2.0.4/LICENCE` & `rubiran-2.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.4/PKG-INFO` & `rubiran-2.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.4
+Version: 2.0.5
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
@@ -32,15 +32,16 @@
 auth = ""
 bot = rubiran(auth,key)
 
 gap = "guids"
 
 bot.sendMessage(gap,"rubiran")
 ```
-###how to install library
+### How to install  library
+
 ```bash
 pip install aiohttp
 pip install pycryptodome
 pip install pillow
 ```
 
 ### How to import the Rubik's library
@@ -54,14 +55,14 @@
 ``` bash
 pip install rubiran
 ```
 
 ### My ID in Rubika
 
 ``` bash
-@professor_102
+### @professor_102
 ```
 ## And My ID Channel in Rubika
 
 ``` bash
-@python_java_source 
+### @python_java_source 
 ```
```

### Comparing `rubiran-2.0.4/rubiran/An_Wb.py` & `rubiran-2.0.5/rubiran/An_Wb.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.4/rubiran/How.py` & `rubiran-2.0.5/rubiran/How.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       white = '\033[97m'
       bold = '\033[1m'
       underline = '\033[4m'
       black='\033[30m'
 
 class chup:
       x_coder = f"""{color.bold}
-{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.4  
+{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.5  
 
 {color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐂𝐎𝐏𝐘𝐑𝐈𝐆𝐇𝐓 (𝐂) {color.red} 2023 {color.green}𝐌𝐀𝐌𝐀𝐃 𝐂𝐎𝐃𝐄𝐑   
 
 {color.white} [⏦] - {color.cyan} 𝐃𝐄𝐕𝐄𝐋𝐎𝐏𝐄𝐑  {color.yellow} 𝐑𝐔𝐁𝐈𝐊𝐀 {color.red} 𝐂𝐇𝐀𝐍𝐍𝐄𝐋 : {color.green} @python_java_source
 
 {color.white}╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾
 """
```

### Comparing `rubiran-2.0.4/rubiran/Socket.py` & `rubiran-2.0.5/rubiran/Socket.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.4/rubiran/client.py` & `rubiran-2.0.5/rubiran/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                     'Origin': 'https://web.rubika.ir',
 					'Referer': f'https://web.rubika.ir/',
 					'Host':url.replace("https://","").replace("/",""),
 					'User-Agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"}
 		
 		while True:
 		      try:
-		      	return asyncio.run(post(url,json=Indata,headers=headers))
+		      	return asyncio.run(post(url,data=Indata,headers=headers))
 		      except:continue
 		      
 	def send_post(self,inData):
 		enc = self.enc
 		data = dumps(inData)
 		url = rubiran._getURL()
 		Indata = {"api_version": "6","auth": self.Auth,"data_enc":enc.encrypt(data),"sign": enc.makeSignFromData(enc.encrypt(data))}
@@ -68,15 +68,15 @@
                     'Origin': 'https://web.rubika.ir',
 					'Referer': f'https://web.rubika.ir/',
 					'Host':url.replace("https://","").replace("/",""),
 					'User-Agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"}
 		
 		while True:
 		      try:
-		      	return asyncio.run(post(url,json=Indata,headers=headers))
+		      	return asyncio.run(post(url,data=Indata,headers=headers))
 		      except:continue
 
 	def registerDevice(self):
 	    inData = {"method":"registerDevice","input":{"app_version":"WB_4.1.2","device_hash":"0501110712007200125373640870428014153736","device_model":"rubiran-library","lang_code":"fa","system_version":"Linux","token":" ","token_type":"Web"},"client": SetClines.web}
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
```

### Comparing `rubiran-2.0.4/rubiran/encryption.py` & `rubiran-2.0.5/rubiran/encryption.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.4/rubiran.egg-info/PKG-INFO` & `rubiran-2.0.5/rubiran.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.4
+Version: 2.0.5
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
@@ -32,15 +32,16 @@
 auth = ""
 bot = rubiran(auth,key)
 
 gap = "guids"
 
 bot.sendMessage(gap,"rubiran")
 ```
-###how to install library
+### How to install  library
+
 ```bash
 pip install aiohttp
 pip install pycryptodome
 pip install pillow
 ```
 
 ### How to import the Rubik's library
@@ -54,14 +55,14 @@
 ``` bash
 pip install rubiran
 ```
 
 ### My ID in Rubika
 
 ``` bash
-@professor_102
+### @professor_102
 ```
 ## And My ID Channel in Rubika
 
 ``` bash
-@python_java_source 
+### @python_java_source 
 ```
```

### Comparing `rubiran-2.0.4/setup.py` & `rubiran-2.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 auth = ""
 bot = rubiran(auth,key)
 
 gap = "guids"
 
 bot.sendMessage(gap,"rubiran")
 ```
-###how to install library
+### How to install  library
+
 ```bash
 pip install aiohttp
 pip install pycryptodome
 pip install pillow
 ```
 
 ### How to import the Rubik's library
@@ -33,26 +34,26 @@
 ``` bash
 pip install rubiran
 ```
 
 ### My ID in Rubika
 
 ``` bash
-@professor_102
+### @professor_102
 ```
 ## And My ID Channel in Rubika
 
 ``` bash
-@python_java_source 
+### @python_java_source 
 ```
 """
 
 setup(
     name = "rubiran",
-    version = "2.0.4",
+    version = "2.0.5",
     author = "mamadcoder",
     author_email = "mamadcoder@gmail.com",
     description = ("Another example of the library making the Rubik's robot"),
     license = "MIT",
     keywords = ["rubika","bot","robot","library","rubikalib","rubikalib.ml","rubikalib.ir","rubika.ir","Rubika","Python","Pyrubika","pyrubika"],
     url = "https://rubika.ir/python_java_source",
     packages=['rubiran'],
```

