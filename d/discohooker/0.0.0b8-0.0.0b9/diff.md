# Comparing `tmp/discohooker-0.0.0b8.tar.gz` & `tmp/discohooker-0.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-0.0.0b8.tar", last modified: Thu Jul 20 05:03:45 2023, max compression
+gzip compressed data, was "discohooker-0.0.0b9.tar", last modified: Thu Jul 20 07:25:58 2023, max compression
```

## Comparing `discohooker-0.0.0b8.tar` & `discohooker-0.0.0b9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 05:03:45.628378 discohooker-0.0.0b8/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.0b8/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2023-07-20 05:03:45.628378 discohooker-0.0.0b8/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      724 2023-07-20 04:04:14.000000 discohooker-0.0.0b8/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 05:03:45.624378 discohooker-0.0.0b8/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-19 13:55:35.000000 discohooker-0.0.0b8/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-19 16:01:13.000000 discohooker-0.0.0b8/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      414 2023-07-20 04:27:13.000000 discohooker-0.0.0b8/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2210 2023-07-20 04:20:51.000000 discohooker-0.0.0b8/discohooker/message.py
--rw-r--r--   0 runner    (1000) runner    (1000)      967 2023-07-20 05:03:21.000000 discohooker-0.0.0b8/discohooker/tasks.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2407 2023-07-20 03:52:53.000000 discohooker-0.0.0b8/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 05:03:45.628378 discohooker-0.0.0b8/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2023-07-20 05:03:45.000000 discohooker-0.0.0b8/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-20 05:03:45.000000 discohooker-0.0.0b8/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-20 05:03:45.000000 discohooker-0.0.0b8/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-20 05:03:45.000000 discohooker-0.0.0b8/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-20 05:03:45.000000 discohooker-0.0.0b8/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      472 2023-07-15 08:52:33.000000 discohooker-0.0.0b8/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-20 05:03:45.628378 discohooker-0.0.0b8/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      714 2023-07-20 05:03:36.000000 discohooker-0.0.0b8/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 07:25:58.642659 discohooker-0.0.0b9/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.0b9/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1190 2023-07-20 07:25:58.642659 discohooker-0.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      724 2023-07-20 04:04:14.000000 discohooker-0.0.0b9/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 07:25:58.638659 discohooker-0.0.0b9/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-19 13:55:35.000000 discohooker-0.0.0b9/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-19 16:01:13.000000 discohooker-0.0.0b9/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      414 2023-07-20 04:27:13.000000 discohooker-0.0.0b9/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2211 2023-07-20 07:25:12.000000 discohooker-0.0.0b9/discohooker/message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      967 2023-07-20 05:03:21.000000 discohooker-0.0.0b9/discohooker/tasks.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2407 2023-07-20 03:52:53.000000 discohooker-0.0.0b9/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 07:25:58.642659 discohooker-0.0.0b9/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1190 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-20 07:25:58.000000 discohooker-0.0.0b9/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-0.0.0b9/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-20 07:25:58.642659 discohooker-0.0.0b9/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      714 2023-07-20 07:24:53.000000 discohooker-0.0.0b9/setup.py
```

### Comparing `discohooker-0.0.0b8/LICENSE` & `discohooker-0.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b8/PKG-INFO` & `discohooker-0.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.0b8
+Version: 0.0.0b9
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-0.0.0b8/README.md` & `discohooker-0.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b8/discohooker/embed.py` & `discohooker-0.0.0b9/discohooker/embed.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b8/discohooker/message.py` & `discohooker-0.0.0b9/discohooker/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests
 
 
 class Message:
     def __init__(self, webhook: Webhook, message_id: int):
         self.webhook=webhook
         response=requests.get(f"{self.webhook.weburl}/messages/{message_id}").json()
-        if response["author"]["id"] == self.webhook.id
+        if response["author"]["id"] == self.webhook.id:
             self.is_sent_by_webhook=True
         else:
             self.is_sent_by_webhook=False
         self.id=response["id"]
         self.content=response["content"]
         self.is_pinned=response["pinned"]
         self.embeds=[]
```

### Comparing `discohooker-0.0.0b8/discohooker/tasks.py` & `discohooker-0.0.0b9/discohooker/tasks.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b8/discohooker/webhook.py` & `discohooker-0.0.0b9/discohooker/webhook.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b8/discohooker.egg-info/PKG-INFO` & `discohooker-0.0.0b9/discohooker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.0b8
+Version: 0.0.0b9
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-0.0.0b8/setup.py` & `discohooker-0.0.0b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="0.0.0b8",
+    version="0.0.0b9",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

