# Comparing `tmp/discohooker-0.0.1.tar.gz` & `tmp/discohooker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-0.0.1.tar", last modified: Thu Jul 20 13:11:40 2023, max compression
+gzip compressed data, was "discohooker-1.0.0.tar", last modified: Thu Jul 20 13:44:01 2023, max compression
```

## Comparing `discohooker-0.0.1.tar` & `discohooker-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:11:40.746048 discohooker-0.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1298 2023-07-20 13:11:40.746048 discohooker-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      834 2023-07-20 13:11:14.000000 discohooker-0.0.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:11:40.742048 discohooker-0.0.1/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-0.0.1/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-0.0.1/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      414 2023-07-20 07:39:57.000000 discohooker-0.0.1/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2217 2023-07-20 08:58:45.000000 discohooker-0.0.1/discohooker/message.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1191 2023-07-20 12:56:48.000000 discohooker-0.0.1/discohooker/tasks.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2177 2023-07-20 13:07:03.000000 discohooker-0.0.1/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:11:40.742048 discohooker-0.0.1/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1298 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-20 13:11:40.000000 discohooker-0.0.1/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-20 13:11:40.746048 discohooker-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-20 13:07:31.000000 discohooker-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:44:01.965225 discohooker-1.0.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1298 2023-07-20 13:44:01.965225 discohooker-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      834 2023-07-20 13:43:32.000000 discohooker-1.0.0/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:44:01.961225 discohooker-1.0.0/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.0/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.0/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      414 2023-07-20 07:39:57.000000 discohooker-1.0.0/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2217 2023-07-20 08:58:45.000000 discohooker-1.0.0/discohooker/message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1191 2023-07-20 12:56:48.000000 discohooker-1.0.0/discohooker/tasks.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2177 2023-07-20 13:07:03.000000 discohooker-1.0.0/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-20 13:44:01.965225 discohooker-1.0.0/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1298 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-20 13:44:01.000000 discohooker-1.0.0/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-20 13:44:01.965225 discohooker-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-20 13:43:51.000000 discohooker-1.0.0/setup.py
```

### Comparing `discohooker-0.0.1/LICENSE` & `discohooker-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.1/PKG-INFO` & `discohooker-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.1
+Version: 1.0.0
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,12 +41,12 @@
 > )
 > ```
 ------------
 **Step 5:**
 > Send Message.
 >
 > ```py
-> @discohooker.tasks.worker
+> @discohooker.Tasks.worker
 > async def run():
 >     await webhook.send_message("I am made by Discohooker!")
 --------------
 DONE! Do you feel very easy?
```

### Comparing `discohooker-0.0.1/README.md` & `discohooker-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 > )
 > ```
 ------------
 **Step 5:**
 > Send Message.
 >
 > ```py
-> @discohooker.tasks.worker
+> @discohooker.Tasks.worker
 > async def run():
 >     await webhook.send_message("I am made by Discohooker!")
 --------------
 DONE! Do you feel very easy?
```

### Comparing `discohooker-0.0.1/discohooker/embed.py` & `discohooker-1.0.0/discohooker/embed.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.1/discohooker/message.py` & `discohooker-1.0.0/discohooker/message.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.1/discohooker/tasks.py` & `discohooker-1.0.0/discohooker/tasks.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.1/discohooker/webhook.py` & `discohooker-1.0.0/discohooker/webhook.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.1/discohooker.egg-info/PKG-INFO` & `discohooker-1.0.0/discohooker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.1
+Version: 1.0.0
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,12 +41,12 @@
 > )
 > ```
 ------------
 **Step 5:**
 > Send Message.
 >
 > ```py
-> @discohooker.tasks.worker
+> @discohooker.Tasks.worker
 > async def run():
 >     await webhook.send_message("I am made by Discohooker!")
 --------------
 DONE! Do you feel very easy?
```

### Comparing `discohooker-0.0.1/setup.py` & `discohooker-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="0.0.1",
+    version="1.0.0",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

