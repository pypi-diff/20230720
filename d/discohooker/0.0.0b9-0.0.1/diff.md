# Comparing `tmp/discohooker-0.0.0b9.tar.gz` & `tmp/discohooker-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-0.0.0b9.tar", last modified: Thu Jul 20 07:25:58 2023, max compression
+gzip compressed data, was "discohooker-0.0.1.tar", last modified: Thu Jul 20 13:11:40 2023, max compression
```

## Comparing `discohooker-0.0.0b9.tar` & `discohooker-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 07:25:58.642659 discohooker-0.0.0b9/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.0b9/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2023-07-20 07:25:58.642659 discohooker-0.0.0b9/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      724 2023-07-20 04:04:14.000000 discohooker-0.0.0b9/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 07:25:58.638659 discohooker-0.0.0b9/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-19 13:55:35.000000 discohooker-0.0.0b9/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-19 16:01:13.000000 discohooker-0.0.0b9/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      414 2023-07-20 04:27:13.000000 discohooker-0.0.0b9/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2211 2023-07-20 07:25:12.000000 discohooker-0.0.0b9/discohooker/message.py
--rw-r--r--   0 runner    (1000) runner    (1000)      967 2023-07-20 05:03:21.000000 discohooker-0.0.0b9/discohooker/tasks.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2407 2023-07-20 03:52:53.000000 discohooker-0.0.0b9/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 07:25:58.642659 discohooker-0.0.0b9/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-0.0.0b9/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-20 07:25:58.642659 discohooker-0.0.0b9/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      714 2023-07-20 07:24:53.000000 discohooker-0.0.0b9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:11:40.746048 discohooker-0.0.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1298 2023-07-20 13:11:40.746048 discohooker-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      834 2023-07-20 13:11:14.000000 discohooker-0.0.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:11:40.742048 discohooker-0.0.1/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-0.0.1/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-0.0.1/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      414 2023-07-20 07:39:57.000000 discohooker-0.0.1/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2217 2023-07-20 08:58:45.000000 discohooker-0.0.1/discohooker/message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1191 2023-07-20 12:56:48.000000 discohooker-0.0.1/discohooker/tasks.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2177 2023-07-20 13:07:03.000000 discohooker-0.0.1/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:11:40.742048 discohooker-0.0.1/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1298 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-20 13:11:40.746048 discohooker-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-20 13:07:31.000000 discohooker-0.0.1/setup.py
```

### Comparing `discohooker-0.0.0b9/LICENSE` & `discohooker-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b9/PKG-INFO` & `discohooker-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.0b9
+Version: 0.0.1
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Quickly Start
+----------------
 **Step 1:**
 > Install Discohooker in Shell.
 > 
 > ```pip install discohooker```
-
-
+----------------
 **Step 2:**
 > Get your Webhook link in [Discord](https://discord.com/channels/@me).
-
-
+---------------
 **Step 3:**
-> Import Discohooker and asyncio.
+> Import Discohooker.
 >
 > ```py
-> import discohooker, asyncio
+> import discohooker
 > ```
-
-
+-------------
 **Step 4:**
 > Setup Webhook.
 >
 > ```py
 > webhook=discohooker.Webhook(
 >     weburl="YOUR DISCORD WEBHOOK URL",
 >     name="DISCORD WEBHOOK NAME(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)",
 >     avatar_url="DISCORD WEBHOOK AVATAR URL(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)"
 > )
-> 
->loop=asyncio.get_event_loop()
->loop.run_until_complete(webhook.send_message("I am made by Discohooker!"))
 > ```
-
-
+------------
 **Step 5:**
-> Done!
+> Send Message.
+>
+> ```py
+> @discohooker.tasks.worker
+> async def run():
+>     await webhook.send_message("I am made by Discohooker!")
+--------------
+DONE! Do you feel very easy?
```

### Comparing `discohooker-0.0.0b9/discohooker/embed.py` & `discohooker-0.0.1/discohooker/embed.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b9/discohooker/message.py` & `discohooker-0.0.1/discohooker/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .erros import Errors
+from .errors import Errors
 from .embed import Embed
 from .webhook import Webhook
 import asyncio
 import requests
 
 
 class Message:
@@ -23,14 +23,15 @@
             self.embeds.appead(_embed)
         self.timestamp=response["timestamp"]
         self.mentions_id=[]
         for user in response["mentions"]:
             self.memtions_id.appead(user["id"])
         self.channel_id=response["channel_id"]
 
+    
     async def edit(self, content: str=None, embeds: list[Embed]=[], delete_after: int=None):
         if self.is_sent_by_webhook == False:
             raise Errors.MessageErro("This message is not sent by this Webhook!")
         message_id=self.id
         _embeds=[]
         for embed in embeds:
             _embeds.append(embed._to_dict)
```

### Comparing `discohooker-0.0.0b9/discohooker/tasks.py` & `discohooker-0.0.1/discohooker/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .error import Errors
+from .errors import Errors
 from datetime import datetime
 import asyncio
 import pytz
 
 
 class Tasks:
 
@@ -19,11 +19,18 @@
                     else:
                         now=datetime.now(pytz.timezone(timezone))
                     if f"{now.date}-{now.month}-{now.year}" == date:
                         running=False
                     else:
                         loop=asyncio.get_event_loop()
                         loop.run_until_complete(asyncio.sleep(1))
-                return fun()
+                loop=asyncio.get_event_loop()
+                return loop.run_until_complete(fun())
             return wait()
         return decorator()
-    
+
+
+    def worker(fun):
+        def work():
+            loop=asyncio.get_event_loop()
+            return loop.run_until_complete(fun())
+        return work()
```

### Comparing `discohooker-0.0.0b9/discohooker/webhook.py` & `discohooker-0.0.1/discohooker/webhook.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from .errors import Errors
 from .embed import Embed
-from .message import Message
-import asyncio
 import requests
 
 
 class Webhook:
     def __init__(self, weburl: str, name: str=None, avatar_url: str=None):
         if not weburl.startswith("https://discord.com/api/webhooks/"):
             raise Errors.WebhookURLError("This is not Discord Webhook URL! Please check your URL and change the URL to the correct URL!")
         response=requests.get(weburl).json()
         if avatar_url == None:
-            self.avatar_url=response["avatar_url"]
+            self.avatar_url=avatar_url
         elif not avatar_url.startswith("https://"):
             raise Errors.URLError("This is not URL! Please check and change your URL!")
         else:
             self.avatar_url=avatar_url
         self.weburl=weburl
         if name == None:
             self.name=response["name"]
@@ -34,33 +32,29 @@
 
 
     @property
     def url(self):
         return self.weburl
 
 
-    def edit(self, channel_id: int, name: str, avatar_url: str=None):
+    async def edit(self, channel_id: int, name: str, avatar_url: str=None):
         if not avatar_url.startswith("https!//") and avatar_url != None:
             raise Errors.URLError("This is not URL! Please check and change your URL!")
         _jdata={"name": name, "channel_id": channel_id, "avatar": avatar_url}
         return requests.patch(self.weburl, data=_jdata)
 
 
     def get_message(self, message_id: int):
+        from .message import Message
         return Message(self, message_id)
 
     
-    async def send_message(self, content: str=None, embeds: list[Embed]=[], delete_after: int=None):
+    async def send_message(self, content: str=None, embeds: list[Embed]=[]):
         _embeds=[]
         for embed in embeds:
             _embeds.append(embed._to_dict)
         if content == None:
             _content=""
         else:
             _content=content
-        _jdata={"content": _content, "embeds": _embeds}
-        response=requests.post(self.weburl, data=_jdata)
-        if delete_after == None:
-            return Message(self, response["id"])
-        message_id=response.json()["message_id"]
-        await asyncio.sleep(delete_after)
-        return requests.delete(f"{self.weburl}/messages/{message_id}/")
+        _jdata={"content": _content, "embeds": _embeds, "username": self.name, "avatar_url": self.avatar_url}
+        return requests.post(self.weburl, data=_jdata)
```

### Comparing `discohooker-0.0.0b9/discohooker.egg-info/PKG-INFO` & `discohooker-0.0.1/discohooker.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.0b9
+Version: 0.0.1
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Quickly Start
+----------------
 **Step 1:**
 > Install Discohooker in Shell.
 > 
 > ```pip install discohooker```
-
-
+----------------
 **Step 2:**
 > Get your Webhook link in [Discord](https://discord.com/channels/@me).
-
-
+---------------
 **Step 3:**
-> Import Discohooker and asyncio.
+> Import Discohooker.
 >
 > ```py
-> import discohooker, asyncio
+> import discohooker
 > ```
-
-
+-------------
 **Step 4:**
 > Setup Webhook.
 >
 > ```py
 > webhook=discohooker.Webhook(
 >     weburl="YOUR DISCORD WEBHOOK URL",
 >     name="DISCORD WEBHOOK NAME(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)",
 >     avatar_url="DISCORD WEBHOOK AVATAR URL(IF YOU HAVE SET IN DISCORD ALREADY, YOU MUST NOT ENTER.)"
 > )
-> 
->loop=asyncio.get_event_loop()
->loop.run_until_complete(webhook.send_message("I am made by Discohooker!"))
 > ```
-
-
+------------
 **Step 5:**
-> Done!
+> Send Message.
+>
+> ```py
+> @discohooker.tasks.worker
+> async def run():
+>     await webhook.send_message("I am made by Discohooker!")
+--------------
+DONE! Do you feel very easy?
```

### Comparing `discohooker-0.0.0b9/setup.py` & `discohooker-0.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="0.0.0b9",
+    version="0.0.1",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

