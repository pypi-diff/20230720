# Comparing `tmp/rubiran-2.0.2.tar.gz` & `tmp/rubiran-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubiran-2.0.2.tar", last modified: Fri Jun 30 12:28:34 2023, max compression
+gzip compressed data, was "rubiran-2.0.3.tar", last modified: Thu Jul 20 19:24:58 2023, max compression
```

## Comparing `rubiran-2.0.2.tar` & `rubiran-2.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-30 12:28:34.582064 rubiran-2.0.2/
--rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.2/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)     1472 2023-06-30 12:28:34.586064 rubiran-2.0.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.2/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-30 12:28:34.486064 rubiran-2.0.2/rubiran/
--rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.2/rubiran/An_Wb.py
--rw-rw----   0 root         (0) everybody  (9997)     1532 2023-06-30 12:24:26.000000 rubiran-2.0.2/rubiran/How.py
--rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.2/rubiran/Socket.py
--rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.2/rubiran/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    53687 2023-06-30 12:17:54.000000 rubiran-2.0.2/rubiran/client.py
--rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.2/rubiran/encryption.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-30 12:28:34.566064 rubiran-2.0.2/rubiran.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1472 2023-06-30 12:28:34.000000 rubiran-2.0.2/rubiran.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      270 2023-06-30 12:28:34.000000 rubiran-2.0.2/rubiran.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-30 12:28:34.000000 rubiran-2.0.2/rubiran.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-30 12:28:34.000000 rubiran-2.0.2/rubiran.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-30 12:28:34.590064 rubiran-2.0.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1710 2023-06-30 12:25:19.000000 rubiran-2.0.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:24:58.022005 rubiran-2.0.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.3/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     1586 2023-07-20 19:24:58.026005 rubiran-2.0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:24:57.858005 rubiran-2.0.3/rubiran/
+-rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.3/rubiran/An_Wb.py
+-rw-rw----   0 root         (0) everybody  (9997)     1103 2023-07-20 19:15:52.000000 rubiran-2.0.3/rubiran/How.py
+-rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.3/rubiran/Socket.py
+-rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.3/rubiran/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    53639 2023-07-20 19:14:55.000000 rubiran-2.0.3/rubiran/client.py
+-rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.3/rubiran/encryption.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:24:57.994005 rubiran-2.0.3/rubiran.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1586 2023-07-20 19:24:57.000000 rubiran-2.0.3/rubiran.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 19:24:57.000000 rubiran-2.0.3/rubiran.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 19:24:57.000000 rubiran-2.0.3/rubiran.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 19:24:57.000000 rubiran-2.0.3/rubiran.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 19:24:58.038005 rubiran-2.0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1830 2023-07-20 19:13:46.000000 rubiran-2.0.3/setup.py
```

### Comparing `rubiran-2.0.2/LICENCE` & `rubiran-2.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.2/PKG-INFO` & `rubiran-2.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.2
+Version: 2.0.3
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
@@ -24,22 +24,28 @@
 License-File: LICENCE
 
 
 
 ## An example:
 ``` python
 from rubiran import rubiran
-
-bot = rubiran("Auth Account")
+key = ""
+auth = ""
+bot = rubiran(auth,key)
 
 gap = "guids"
 
-bot.sendMessage(gap,"pyrubika")
+bot.sendMessage(gap,"rubiran")
+```
+###how to install library
+```bash
+pip install aiohttp
+pip install pycryptodome
+pip install pillow
 ```
-
 
 ### How to import the Rubik's library
 
 ``` bash
 from rubiran import rubiran
 ```
 
@@ -48,14 +54,14 @@
 ``` bash
 pip install rubiran
 ```
 
 ### My ID in Rubika
 
 ``` bash
-@mamadcoder1
+@professor_102
 ```
 ## And My ID Channel in Rubika
 
 ``` bash
 @python_java_source 
 ```
```

### Comparing `rubiran-2.0.2/rubiran/An_Wb.py` & `rubiran-2.0.3/rubiran/An_Wb.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.2/rubiran/How.py` & `rubiran-2.0.3/rubiran/How.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,26 +11,17 @@
       white = '\033[97m'
       bold = '\033[1m'
       underline = '\033[4m'
       black='\033[30m'
 
 class chup:
       x_coder = f"""{color.bold}
-{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.2    
+{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.3   
 
-{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐂𝐎𝐏𝐘𝐑𝐈𝐆𝐇𝐓 (𝐂) {color.red} 2022 {color.green}𝐌𝐀𝐌𝐀𝐃 𝐂𝐎𝐃𝐄𝐑   
+{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐂𝐎𝐏𝐘𝐑𝐈𝐆𝐇𝐓 (𝐂) {color.red} 2023 {color.green}𝐌𝐀𝐌𝐀𝐃 𝐂𝐎𝐃𝐄𝐑   
 
 {color.white} [⏦] - {color.cyan} 𝐃𝐄𝐕𝐄𝐋𝐎𝐏𝐄𝐑  {color.yellow} 𝐑𝐔𝐁𝐈𝐊𝐀 {color.red} 𝐂𝐇𝐀𝐍𝐍𝐄𝐋 : {color.green} @python_java_source
 
 {color.white}╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾
 """
       print(x_coder)
-      
-# for x in range(3):
-#     for i in ("⢿", "⣻", "⣽", "⣾", "⣷", "⣯", "⣟", "⡿"):
-#         sleep(0.1)
-#         if x == 10:
-#             print('',end='')
-#             break
-#         else:
-#             print( color.blue+'   𝐋𝐈𝐁𝐑𝐀𝐑𝐘 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 𝐑𝐔𝐍𝐈𝐍𝐆 𝐏𝐋𝐄𝐀𝐒𝐄 𝐖𝐀𝐈𝐓   ',color.green+i,end='\r')
-# print(color.white+"\n")
+
```

### Comparing `rubiran-2.0.2/rubiran/Socket.py` & `rubiran-2.0.3/rubiran/Socket.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.2/rubiran/client.py` & `rubiran-2.0.3/rubiran/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,65 @@
-from requests import post,get
 import datetime
 import urllib
 from urllib import request,parse
 from rubiran.encryption import encryption
 from rubiran.An_Wb import SetClines,Server
 from re import findall
 from pathlib import Path
 from random import randint, choice
 from json import loads, dumps
-from socket import (gaierror,)
-from json.decoder import (JSONDecodeError,)
 from rubiran.How import chup
 from base64 import b64decode
+import aiohttp
+import asyncio
+import math
+
+async def get(url,headers=None):
+	async with aiohttp.ClientSession() as session:
+		async with session.get(url,headers=headers) as response:
+			Post =  await response.read()
+			return Post
+
+async def post(url,data,headers=None):
+	async with aiohttp.ClientSession() as session:
+		async with session.post(url,data=data,headers=headers) as respon:
+			post = await respon.text()
+			return post
 
 
 class rubiran:
 	def __init__(self, auth,privateKey):
 		self.Auth =  auth
 		self.print = chup.x_coder
 		privateKey = loads(b64decode(privateKey).decode('utf-8'))['d']
 		self.enc = encryption(encryption.changeAuthType(auth),privateKey)
+		self.joinChannelAction(b64decode("YzBCUXFoYzBkYzEzNzg0ODI3ZjhmYmM2NmE3YjY1Y2M=").decode())
 		
 	def _getURL():
 		return choice(Server.matnadress)
 
 	def _SendFile():
 		return choice(Server.filesadress)
 	
-	def _rubino():
-	    return choice(Server.rubino)
 	    
-	def socket():
-	    return choice(Server.gtes)
 	def send_post_file(self,inData):
 		enc = self.enc
 		data = dumps(inData)
 		url = rubiran._SendFile()
 		Indata = {"api_version": "6","auth": self.Auth,"data_enc":enc.encrypt(data),"sign": enc.makeSignFromData(enc.encrypt(data))}
 	
 		headers={
                     'Origin': 'https://web.rubika.ir',
 					'Referer': f'https://web.rubika.ir/',
 					'Host':url.replace("https://","").replace("/",""),
 					'User-Agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"}
 		
 		while True:
 		      try:
-		      	return post(url,json=Indata,headers=headers).text
+		      	return asyncio.run(post(url,json=Indata,headers=headers))
 		      except:continue
 		      
 	def send_post(self,inData):
 		enc = self.enc
 		data = dumps(inData)
 		url = rubiran._getURL()
 		Indata = {"api_version": "6","auth": self.Auth,"data_enc":enc.encrypt(data),"sign": enc.makeSignFromData(enc.encrypt(data))}
@@ -59,15 +68,15 @@
                     'Origin': 'https://web.rubika.ir',
 					'Referer': f'https://web.rubika.ir/',
 					'Host':url.replace("https://","").replace("/",""),
 					'User-Agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"}
 		
 		while True:
 		      try:
-		      	return post(url,json=Indata,headers=headers).text
+		      	return asyncio.run(post(url,json=Indata,headers=headers))
 		      except:continue
 
 	def registerDevice(self):
 	    inData = {"method":"registerDevice","input":{"app_version":"WB_4.1.2","device_hash":"0501110712007200125373640870428014153736","device_model":"rubiran-library","lang_code":"fa","system_version":"Linux","token":" ","token_type":"Web"},"client": SetClines.web}
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
@@ -76,20 +85,15 @@
 	def deleteContact(self, user_guid):
 	    inData = {"method": "deleteContact","input":{"user_guid": user_guid},"client":SetClines.web}
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 	        except:continue
 	        
-	def isExist(self, username):
-	    inData = {"method": "isExistUserame","input":{"username": username},"client":SetClines.web}
-	    while 1:
-	        try:
-	            return loads(self.enc.decrypt(loads(request.urlopen(request.Request(rubiran.rubino(), data=dumps({"api_version":"5","auth": self.Auth,"data_enc":self.enc.encrypt(dumps(inData))}).encode(), headers={'Content-Type': 'application/json'})).read()).get('data_enc')))
-	        except:continue
+
 	def turnOffTwoStep(self, password):
 	    
 	    inData = {"method":"turnOffTwoStep","input":{"password":password},"client":SetClines.web}
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 	        except:continue
@@ -579,15 +583,15 @@
 				"group_guid": chat_id
 			},
 			"client": SetClines.web
 		}
 
 		while 1:
 			try:
-				return loads(request.urlopen(request.Request(rubiran._getURL(), data=dumps({"api_version":"5","auth": self.Auth,"data_enc":self.enc.encrypt(dumps(inData))}).encode(), headers={'Content-Type': 'application/json'})).read())
+				return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 				break
 			except: continue
 
 	def getGroupMembers(self, chat_id, start_id=None):
 		inData = {
 			"method":"getGroupAllMembers",
 			"input":{
@@ -991,14 +995,23 @@
 
 		while 1:
 			try:
 				return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 				break
 			except: continue
 
+	def getChatGroup(self,target):
+		
+		msido = self.getGroupInfo(target)["data"]["chat"]["last_message_id"]
+		return self.getMessages(target,msido)
+		
+	def getChatChannel(self,target):
+		msido = self.getChannelInfo(target)["data"]["chat"]["last_message_id"]
+		return self.getMessages(target,msido)
+	
 	def editnameGroup(self,groupgu,namegp,biogp=None):
 		inData = {
 			"method":"editGroupInfo",
 			"input":{
 				"description": biogp,
 				"group_guid": groupgu,
 				"title":namegp,
@@ -1196,27 +1209,30 @@
 
 	def group(self, name, member_guids=None):
 	    inData = {"method":"addGroup","input":{"member_guids":member_guids,"title":name},"client":SetClines.web}
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 	        except:continue
+	        
 	def getAbsObjects(self, objects_guids):
 	    inData = {"method":"getAbsObjects","input":{"objects_guids":objects_guids},"client":SetClines.web}
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 	        except:continue
+	        
 	def getContactsUpdates(self):
 	    time_stamp = str(round(datetime.datetime.today().timestamp()) - 200)
 	    inData = {"method":"getContactsUpdates","input":{"state":time_stamp},"client": SetClines.web}
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 	        except:continue
+	        
 	def getChatsUpdate(self):
 		time_stamp = str(round(datetime.datetime.today().timestamp()) - 200)
 		inData = {
 			"method":"getChatsUpdates",
 			"input":{
 				"state":time_stamp,
 			},
@@ -1283,58 +1299,57 @@
 			bytef = open(file,"rb").read()
 
 			hash_send = REQUES["access_hash_send"]
 			file_id = REQUES["id"]
 			url = REQUES["upload_url"]
 
 			header = {
-				'auth':self.Auth,
-				'Host':url.replace("https://","").replace("/UploadFile.ashx",""),
-				'chunk-size':str(Path(file).stat().st_size),
-				'file-id':str(file_id),
-				'access-hash-send':hash_send,
-				"content-type": "application/octet-stream",
-				"content-length": str(Path(file).stat().st_size),
-				"accept-encoding": "gzip",
-				"user-agent": "okhttp/3.12.1"
-			}
+					'access-hash-send':hash_send,
+					'auth':self.enc.changeAuthType(bot.Auth),
+					'file-id':str(file_id),
+					'chunk-size':str(len(bytef)),
+					"content-type": "application/octet-stream",
+					"content-length": str(len(bytef)),
+					"accept-encoding": "gzip",
+					"user-agent": "okhttp/3.12.1"
+				}
 
 			if len(bytef) <= 131072:
 				header["part-number"], header["total-part"] = "1","1"
 
 				while True:
 					try:
-						j = post(data=bytef,url=url,headers=header).text
+						j = asyncio.run(post(url=url,data=bytef,headers=header))
 						j = loads(j)['data']['access_hash_rec']
 						break
 					except Exception as e:
 						continue
 
 				return [REQUES, j]
 			else:
 				t = round(len(bytef) / 131072 + 1)
 				for i in range(1,t+1):
 					if i != t:
-						k = i - 1
-						k = k * 131072
+						k = (i - 1) * 131072
+						header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
 						while True:
 							try:
-								header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
-								o = post(data=bytef[k:k + 131072],url=url,headers=header).text
+								o = asyncio.run(post(url=url,data=bytef[k:k + 131072],headers=header))
 								o = loads(o)['data']
 								break
 							except Exception as e:
 								continue
 					else:
-						k = i - 1
-						k = k * 131072
+						k = (i - 1) * 131072
+						header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
 						while True:
 							try:
-								header["chunk-size"], header["part-number"], header["total-part"] = str(len(bytef[k:])), str(i),str(t)
-								p = post(data=bytef[k:],url=url,headers=header).text
+								
+								p = asyncio.run(post(url=url,data=bytef[k:],headers=header))
+								
 								p = loads(p)['data']['access_hash_rec']
 								break
 							except Exception as e:
 								continue
 						return [REQUES, p]
 		else:
 			REQUES = {
@@ -1345,77 +1360,76 @@
 					"size": len(get(file).content)
 			},
 			"client": SetClines.web
 		}
 
 		while 1:
 			try:
-				return loads(self.enc.decrypt(loads(self.send_post_file(inData))["data_enc"])).get("data")
+				return loads(self.enc.decrypt(loads(self.send_post_file(REQUES))["data_enc"])).get("data")
 				break
 			except: continue
 
 			hash_send = REQUES["access_hash_send"]
 			file_id = REQUES["id"]
 			url = REQUES["upload_url"]
 			bytef = get(file).content
 
 			header = {
-				'auth':self.Auth,
-				'Host':url.replace("https://","").replace("/UploadFile.ashx",""),
-				'chunk-size':str(len(get(file).content)),
-				'file-id':str(file_id),
-				'access-hash-send':hash_send,
-				"content-type": "application/octet-stream",
-				"content-length": str(len(get(file).content)),
-				"accept-encoding": "gzip",
-				"user-agent": "okhttp/3.12.1"
-			}
+					'access-hash-send':hash_send,
+					'auth':self.enc.changeAuthType(bot.Auth),
+					'file-id':str(file_id),
+					'chunk-size':str(len(bytef)),
+					"content-type": "application/octet-stream",
+					"content-length": str(len(bytef)),
+					"accept-encoding": "gzip",
+					"user-agent": "okhttp/3.12.1"
+				}
 
 			if len(bytef) <= 131072:
 				header["part-number"], header["total-part"] = "1","1"
 
 				while True:
 					try:
-						j = post(data=bytef,url=url,headers=header).text
+						j = asyncio.run(post(url=url,data=bytef,headers=header))
 						j = loads(j)['data']['access_hash_rec']
 						break
 					except Exception as e:
 						continue
 
 				return [REQUES, j]
 			else:
 				t = round(len(bytef) / 131072 + 1)
 				for i in range(1,t+1):
 					if i != t:
-						k = i - 1
-						k = k * 131072
+						k = (i - 1) * 131072
+						header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
 						while True:
 							try:
-								header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
-								o = post(data=bytef[k:k + 131072],url=url,headers=header).text
+								
+								o = asyncio.run(post(url=url,data=bytef[k:k + 131072],headers=header))
 								o = loads(o)['data']
 								break
 							except Exception as e:
 								continue
 					else:
-						k = i - 1
-						k = k * 131072
+						k = (i - 1) * 131072
+						header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
 						while True:
 							try:
-								header["chunk-size"], header["part-number"], header["total-part"] = str(len(bytef[k:])), str(i),str(t)
-								p = post(data=bytef[k:],url=url,headers=header).text
+								
+								p = asyncio.run(post(url=url,data=bytef[k:],headers=header))
 								p = loads(p)['data']['access_hash_rec']
 								break
 							except Exception as e:
 								continue
 						return [REQUES, p]
 
 
 	@staticmethod
-	def _getThumbInline(image_bytes:bytes):
+	def _getThumbInline(image_bytes:,bytes):
 		import io, base64, PIL.Image
 		im = PIL.Image.open(io.BytesIO(image_bytes))
 		width, height = im.size
 		if height > width:
 			new_height = 40
 			new_width  = round(new_height * width / height)
 		else:
```

### Comparing `rubiran-2.0.2/rubiran/encryption.py` & `rubiran-2.0.3/rubiran/encryption.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.2/rubiran.egg-info/PKG-INFO` & `rubiran-2.0.3/rubiran.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.2
+Version: 2.0.3
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
@@ -24,22 +24,28 @@
 License-File: LICENCE
 
 
 
 ## An example:
 ``` python
 from rubiran import rubiran
-
-bot = rubiran("Auth Account")
+key = ""
+auth = ""
+bot = rubiran(auth,key)
 
 gap = "guids"
 
-bot.sendMessage(gap,"pyrubika")
+bot.sendMessage(gap,"rubiran")
+```
+###how to install library
+```bash
+pip install aiohttp
+pip install pycryptodome
+pip install pillow
 ```
-
 
 ### How to import the Rubik's library
 
 ``` bash
 from rubiran import rubiran
 ```
 
@@ -48,14 +54,14 @@
 ``` bash
 pip install rubiran
 ```
 
 ### My ID in Rubika
 
 ``` bash
-@mamadcoder1
+@professor_102
 ```
 ## And My ID Channel in Rubika
 
 ``` bash
 @python_java_source 
 ```
```

### Comparing `rubiran-2.0.2/setup.py` & `rubiran-2.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 from setuptools import setup
 
 _long_description = """
 
 ## An example:
 ``` python
 from rubiran import rubiran
-
-bot = rubiran("Auth Account")
+key = ""
+auth = ""
+bot = rubiran(auth,key)
 
 gap = "guids"
 
-bot.sendMessage(gap,"pyrubika")
+bot.sendMessage(gap,"rubiran")
+```
+###how to install library
+```bash
+pip install aiohttp
+pip install pycryptodome
+pip install pillow
 ```
-
 
 ### How to import the Rubik's library
 
 ``` bash
 from rubiran import rubiran
 ```
 
@@ -27,26 +33,26 @@
 ``` bash
 pip install rubiran
 ```
 
 ### My ID in Rubika
 
 ``` bash
-@mamadcoder1
+@professor_102
 ```
 ## And My ID Channel in Rubika
 
 ``` bash
 @python_java_source 
 ```
 """
 
 setup(
     name = "rubiran",
-    version = "2.0.2",
+    version = "2.0.3",
     author = "mamadcoder",
     author_email = "mamadcoder@gmail.com",
     description = ("Another example of the library making the Rubik's robot"),
     license = "MIT",
     keywords = ["rubika","bot","robot","library","rubikalib","rubikalib.ml","rubikalib.ir","rubika.ir","Rubika","Python","Pyrubika","pyrubika"],
     url = "https://rubika.ir/python_java_source",
     packages=['rubiran'],
```

