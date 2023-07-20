# Comparing `tmp/GoogleBard-2.0.0.tar.gz` & `tmp/GoogleBard-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-2.0.0.tar", last modified: Thu Jul 20 07:03:15 2023, max compression
+gzip compressed data, was "GoogleBard-2.1.0.tar", last modified: Thu Jul 20 10:42:03 2023, max compression
```

## Comparing `GoogleBard-2.0.0.tar` & `GoogleBard-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:03:15.442940 GoogleBard-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 07:02:54.000000 GoogleBard-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-20 07:03:15.442940 GoogleBard-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-20 07:02:54.000000 GoogleBard-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 07:03:15.442940 GoogleBard-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 07:02:54.000000 GoogleBard-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:03:15.442940 GoogleBard-2.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-07-20 07:02:54.000000 GoogleBard-2.0.0/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:03:15.442940 GoogleBard-2.0.0/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-20 07:03:15.000000 GoogleBard-2.0.0/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-20 07:03:15.000000 GoogleBard-2.0.0/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:03:15.000000 GoogleBard-2.0.0/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 07:03:15.000000 GoogleBard-2.0.0/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 07:03:15.000000 GoogleBard-2.0.0/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:42:03.805634 GoogleBard-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 10:41:42.000000 GoogleBard-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-20 10:42:03.805634 GoogleBard-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-20 10:41:42.000000 GoogleBard-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:42:03.805634 GoogleBard-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 10:41:42.000000 GoogleBard-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:42:03.805634 GoogleBard-2.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-20 10:41:42.000000 GoogleBard-2.1.0/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:42:03.805634 GoogleBard-2.1.0/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-20 10:42:03.000000 GoogleBard-2.1.0/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-20 10:42:03.000000 GoogleBard-2.1.0/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:42:03.000000 GoogleBard-2.1.0/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 10:42:03.000000 GoogleBard-2.1.0/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 10:42:03.000000 GoogleBard-2.1.0/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-2.0.0/LICENSE` & `GoogleBard-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-2.0.0/PKG-INFO` & `GoogleBard-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 2.0.0
+Version: 2.1.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
@@ -32,49 +32,49 @@
 - Copy the values
   - Session: Go to Application → Cookies → `__Secure-1PSID` and `__Secure-1PSIDTS`. Copy the value of those cookie.
 
 ## Usage
 
 ```bash
 $ python3 -m Bard -h
-usage: Bard.py [-h] --session SESSION
+usage: Bard.py [-h] --session <__Secure-1PSID> --session_ts <__Secure-1PSIDTS>
 
 options:
   -h, --help         show this help message and exit
-  --__Secure_1PSID --__Secure_1PSIDTS       pass two cookies
+  --session --session_ts       pass two cookies
 ```
 
 ### Quick mode
 ```
 $ export BARD_QUICK="true"
-$ export BARD___Secure-1PSID="<__Secure-1PSID>"
-$ export BARD___Secure-1PSIDTS="<__Secure-1PSIDTS>"
+$ export BARD__Secure_1PSID="<__Secure-1PSID>"
+$ export BARD__Secure_1PSIDTS="<__Secure-1PSIDTS>"
 $ python3 -m Bard
 ```
 Environment variables can be placed in .zshrc.
 
 Example bash shortcut:
 ```bash
 # USAGE1: bard QUESTION
 # USAGE2: echo "QUESTION" | bard
 bard () {
 	export BARD_QUICK=true
-	export BARD___Secure-1PSID==<REDACTED>.
-	export BARD___Secure-1PSIDTS==<REDACTED>.
+	export BARD__Secure_1PSID=<__Secure-1PSID>
+	export BARD__Secure_1PSIDTS=<__Secure-1PSIDTS>
 	python3 -m Bard "${@:-$(</dev/stdin)}" | tail -n+7
 }
 ```
 
 ## [Developer Documentation](https://github.com/acheong08/Bard/blob/main/DOCUMENTATION.md)
 ```python
 from os import environ
 from Bard import Chatbot
 
-Secure_1PSID = environ.get("BARD__Secure-1PSID")
-Secure_1PSIDTS = environ.get("BARD__Secure-1PSIDTS")
+Secure_1PSID = environ.get("BARD__Secure_1PSID")
+Secure_1PSIDTS = environ.get("BARD__Secure_1PSIDTS")
 chatbot = Chatbot(Secure_1PSID, Secure_1PSIDTS)
 
 chatbot.ask("Hello, how are you?")
 
 ```
 
 Credits:
```

### Comparing `GoogleBard-2.0.0/README.md` & `GoogleBard-2.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,49 +13,49 @@
 - Copy the values
   - Session: Go to Application → Cookies → `__Secure-1PSID` and `__Secure-1PSIDTS`. Copy the value of those cookie.
 
 ## Usage
 
 ```bash
 $ python3 -m Bard -h
-usage: Bard.py [-h] --session SESSION
+usage: Bard.py [-h] --session <__Secure-1PSID> --session_ts <__Secure-1PSIDTS>
 
 options:
   -h, --help         show this help message and exit
-  --__Secure_1PSID --__Secure_1PSIDTS       pass two cookies
+  --session --session_ts       pass two cookies
 ```
 
 ### Quick mode
 ```
 $ export BARD_QUICK="true"
-$ export BARD___Secure-1PSID="<__Secure-1PSID>"
-$ export BARD___Secure-1PSIDTS="<__Secure-1PSIDTS>"
+$ export BARD__Secure_1PSID="<__Secure-1PSID>"
+$ export BARD__Secure_1PSIDTS="<__Secure-1PSIDTS>"
 $ python3 -m Bard
 ```
 Environment variables can be placed in .zshrc.
 
 Example bash shortcut:
 ```bash
 # USAGE1: bard QUESTION
 # USAGE2: echo "QUESTION" | bard
 bard () {
 	export BARD_QUICK=true
-	export BARD___Secure-1PSID==<REDACTED>.
-	export BARD___Secure-1PSIDTS==<REDACTED>.
+	export BARD__Secure_1PSID=<__Secure-1PSID>
+	export BARD__Secure_1PSIDTS=<__Secure-1PSIDTS>
 	python3 -m Bard "${@:-$(</dev/stdin)}" | tail -n+7
 }
 ```
 
 ## [Developer Documentation](https://github.com/acheong08/Bard/blob/main/DOCUMENTATION.md)
 ```python
 from os import environ
 from Bard import Chatbot
 
-Secure_1PSID = environ.get("BARD__Secure-1PSID")
-Secure_1PSIDTS = environ.get("BARD__Secure-1PSIDTS")
+Secure_1PSID = environ.get("BARD__Secure_1PSID")
+Secure_1PSIDTS = environ.get("BARD__Secure_1PSIDTS")
 chatbot = Chatbot(Secure_1PSID, Secure_1PSIDTS)
 
 chatbot.ask("Hello, how are you?")
 
 ```
 
 Credits:
```

### Comparing `GoogleBard-2.0.0/setup.py` & `GoogleBard-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="2.0.0",
+    version="2.1.0",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-2.0.0/src/Bard.py` & `GoogleBard-2.1.0/src/Bard.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,18 @@
         return self.loop.run_until_complete(self.async_chatbot.ask(message))
 
 
 class AsyncChatbot:
     """
     A class to interact with Google Bard.
     Parameters
-        session_id: str
-            The __Secure-1PSID cookie.
+        session: str
+            The __Secure_1PSID cookie.
+        session_ts: str
+            The __Secure_1PSIDTS cookie.
         proxy: str
         timeout: int
             Request timeout in seconds.
     """
 
     __slots__ = [
         "headers",
@@ -219,29 +221,29 @@
     async def __get_snlm0e(self):
         # Find "SNlM0e":"<ID>"
         if (
             not (self.secure_1psid and self.secure_1psidts)
             or self.secure_1psid[-1] != "."
         ):
             raise Exception(
-                "Enter correct __Secure-1PSID and __Secure-1PSIDTS value. __Secure-1PSID value must end with a single dot. ",
+                "Enter correct __Secure_1PSID and __Secure_1PSIDTS value. __Secure_1PSID value must end with a single dot. ",
             )
         resp = await self.session.get(
             "https://bard.google.com/",
             timeout=10,
             follow_redirects=True,
         )
         if resp.status_code != 200:
             raise Exception(
                 f"Response code not 200. Response Status is {resp.status_code}",
             )
         SNlM0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text)
         if not SNlM0e:
             raise Exception(
-                "SNlM0e value not found in response. Check __Secure-1PSID value.",
+                "SNlM0e value not found in response. Check __Secure_1PSID value.",
             )
         return SNlM0e.group(1)
 
     async def ask(self, message: str) -> dict:
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
@@ -303,19 +305,19 @@
         Repo: github.com/acheong08/Bard
 
         Enter `alt+enter` or `esc+enter` to send a message.
         """,
     )
     console = Console()
     if os.getenv("BARD_QUICK"):
-        Secure_1PSID = os.getenv("BARD___Secure-1PSID")
-        Secure_1PSIDTS = os.getenv("BARD__Secure-1PSIDTS")
+        Secure_1PSID = os.getenv("BARD__Secure_1PSID")
+        Secure_1PSIDTS = os.getenv("BARD__Secure_1PSIDTS")
         if not (Secure_1PSID and Secure_1PSIDTS):
             print(
-                "BARD___Secure-1PSID or BARD__Secure-1PSIDTS environment variable not set."
+                "BARD__Secure_1PSID or BARD__Secure_1PSIDTS environment variable not set.",
             )
             sys.exit(1)
         chatbot = Chatbot(Secure_1PSID, Secure_1PSIDTS)
         # Join arguments into a single string
         MESSAGE = " ".join(sys.argv[1:])
         response = chatbot.ask(MESSAGE)
         console.print(Markdown(response["content"]))
```

### Comparing `GoogleBard-2.0.0/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-2.1.0/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 2.0.0
+Version: 2.1.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
@@ -32,49 +32,49 @@
 - Copy the values
   - Session: Go to Application → Cookies → `__Secure-1PSID` and `__Secure-1PSIDTS`. Copy the value of those cookie.
 
 ## Usage
 
 ```bash
 $ python3 -m Bard -h
-usage: Bard.py [-h] --session SESSION
+usage: Bard.py [-h] --session <__Secure-1PSID> --session_ts <__Secure-1PSIDTS>
 
 options:
   -h, --help         show this help message and exit
-  --__Secure_1PSID --__Secure_1PSIDTS       pass two cookies
+  --session --session_ts       pass two cookies
 ```
 
 ### Quick mode
 ```
 $ export BARD_QUICK="true"
-$ export BARD___Secure-1PSID="<__Secure-1PSID>"
-$ export BARD___Secure-1PSIDTS="<__Secure-1PSIDTS>"
+$ export BARD__Secure_1PSID="<__Secure-1PSID>"
+$ export BARD__Secure_1PSIDTS="<__Secure-1PSIDTS>"
 $ python3 -m Bard
 ```
 Environment variables can be placed in .zshrc.
 
 Example bash shortcut:
 ```bash
 # USAGE1: bard QUESTION
 # USAGE2: echo "QUESTION" | bard
 bard () {
 	export BARD_QUICK=true
-	export BARD___Secure-1PSID==<REDACTED>.
-	export BARD___Secure-1PSIDTS==<REDACTED>.
+	export BARD__Secure_1PSID=<__Secure-1PSID>
+	export BARD__Secure_1PSIDTS=<__Secure-1PSIDTS>
 	python3 -m Bard "${@:-$(</dev/stdin)}" | tail -n+7
 }
 ```
 
 ## [Developer Documentation](https://github.com/acheong08/Bard/blob/main/DOCUMENTATION.md)
 ```python
 from os import environ
 from Bard import Chatbot
 
-Secure_1PSID = environ.get("BARD__Secure-1PSID")
-Secure_1PSIDTS = environ.get("BARD__Secure-1PSIDTS")
+Secure_1PSID = environ.get("BARD__Secure_1PSID")
+Secure_1PSIDTS = environ.get("BARD__Secure_1PSIDTS")
 chatbot = Chatbot(Secure_1PSID, Secure_1PSIDTS)
 
 chatbot.ask("Hello, how are you?")
 
 ```
 
 Credits:
```

