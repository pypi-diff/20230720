# Comparing `tmp/syncticketstoclickup-1.0.2.tar.gz` & `tmp/syncticketstoclickup-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncticketstoclickup-1.0.2.tar", last modified: Wed Jul 12 18:42:28 2023, max compression
+gzip compressed data, was "syncticketstoclickup-1.0.3.tar", last modified: Thu Jul 20 19:53:29 2023, max compression
```

## Comparing `syncticketstoclickup-1.0.2.tar` & `syncticketstoclickup-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.359915 syncticketstoclickup-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.359915 syncticketstoclickup-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/syncticketstoclickup/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/.env.example
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/clickup.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/zendesk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-12 18:42:08.000000 syncticketstoclickup-1.0.2/syncticketstoclickup/zendesk_to_clickup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:42:28.363915 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 18:42:28.000000 syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:53:29.388304 syncticketstoclickup-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:53:29.380304 syncticketstoclickup-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:53:29.384304 syncticketstoclickup-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-20 19:53:29.388304 syncticketstoclickup-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:53:29.388304 syncticketstoclickup-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:53:29.384304 syncticketstoclickup-1.0.3/syncticketstoclickup/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/syncticketstoclickup/.env.example
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/syncticketstoclickup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/syncticketstoclickup/clickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/syncticketstoclickup/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/syncticketstoclickup/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/syncticketstoclickup/zendesk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-20 19:53:17.000000 syncticketstoclickup-1.0.3/syncticketstoclickup/zendesk_to_clickup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:53:29.388304 syncticketstoclickup-1.0.3/syncticketstoclickup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-20 19:53:29.000000 syncticketstoclickup-1.0.3/syncticketstoclickup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 19:53:29.000000 syncticketstoclickup-1.0.3/syncticketstoclickup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:53:29.000000 syncticketstoclickup-1.0.3/syncticketstoclickup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 19:53:29.000000 syncticketstoclickup-1.0.3/syncticketstoclickup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 19:53:29.000000 syncticketstoclickup-1.0.3/syncticketstoclickup.egg-info/top_level.txt
```

### Comparing `syncticketstoclickup-1.0.2/.github/workflows/python-publish.yml` & `syncticketstoclickup-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.2/.gitignore` & `syncticketstoclickup-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.2/LICENSE` & `syncticketstoclickup-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.2/Makefile` & `syncticketstoclickup-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.2/PKG-INFO` & `syncticketstoclickup-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncticketstoclickup
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that allows to sync tickets from Zendesk to ClickUp.
 Author: abrahamprz (Abraham Perez)
 Author-email: fcoabrahamprz@gmail.com
 Keywords: python,zendesk,clickup,ticket,task,sync,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `syncticketstoclickup-1.0.2/README.md` & `syncticketstoclickup-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.2/syncticketstoclickup/clickup.py` & `syncticketstoclickup-1.0.3/syncticketstoclickup/clickup.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         Returns:
             dict: A dictionary containing the response from the API.
         """
         all_tasks = []
         page = 0
         url = f"https://api.clickup.com/api/v2/list/{list_id}/task"
         while True:
-            tqdm.write(f"Downloading page {page}")
+            tqdm.write(f"Downloading page {page} from ClickUp.")
             query = {
                 "archived": str(archived).lower(),
                 "page": str(page),
                 "include_closed": str(include_closed).lower(),
             }
             response = None
             while response is None:
```

### Comparing `syncticketstoclickup-1.0.2/syncticketstoclickup/zendesk.py` & `syncticketstoclickup-1.0.3/syncticketstoclickup/zendesk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from requests import get, post
 from base64 import b64encode
 from tqdm import tqdm
-from time import sleep
+from time import sleep, mktime, strptime
 from dotenv import load_dotenv, find_dotenv
 
 _ = load_dotenv(find_dotenv())  # read local .env file
 
 
 class ZendeskAPI:
     """This class represents an API client for the Zendesk API."""
@@ -32,34 +32,35 @@
         Returns:
             str: The encoded authentication string.
         """
         auth_string = f"{self.email}/token:{self.api_key}"
         return b64encode(auth_string.encode()).decode()
 
     def get_all_tickets(self) -> dict:
-        """Retrieves all the tickets from the Zendesk account.
+        """Retrieves all the tickets from the Zendesk account, including archived tickets. 
 
         Returns:
             dict: A dictionary containing the response from the API.
         """
         all_tickets = []
-        page = 1
+        start_time = int(mktime(strptime('01/01/2001', '%m/%d/%Y')))
+        page = f"/incremental/tickets.json?start_time={start_time}"
         while True:
-            endpoint = f"{self.base_url}/tickets.json?page={page}"
+            endpoint = f"{self.base_url}{page}"
             response = get(endpoint, headers=self.headers)
             tickets = response.json().get("tickets", [])
             all_tickets.extend(tickets)
-            tqdm.write(f"Downloaded {len(tickets)} tickets from page {page}")
+            tqdm.write(f"Downloaded {len(tickets)} tickets from Zendesk")
             if not response.json().get("next_page"):
                 break
-            page += 1
+            page = response.json().get("next_page").split(self.base_url)[1]
             sleep(1)  # Wait for 1 second before making the next API request
         tqdm.write(f"Downloaded {len(all_tickets)} tickets in total")
         return dict(tickets=all_tickets)
-
+        
     def get_specific_ticket(self, ticket_id: int) -> dict:
         """Retrieves a specific ticket from the Zendesk account.
 
         Args:
             ticket_id (int): The ID of the ticket to retrieve.
 
         Returns:
```

### Comparing `syncticketstoclickup-1.0.2/syncticketstoclickup/zendesk_to_clickup.py` & `syncticketstoclickup-1.0.3/syncticketstoclickup/zendesk_to_clickup.py`

 * *Files identical despite different names*

### Comparing `syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/PKG-INFO` & `syncticketstoclickup-1.0.3/syncticketstoclickup.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncticketstoclickup
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that allows to sync tickets from Zendesk to ClickUp.
 Author: abrahamprz (Abraham Perez)
 Author-email: fcoabrahamprz@gmail.com
 Keywords: python,zendesk,clickup,ticket,task,sync,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `syncticketstoclickup-1.0.2/syncticketstoclickup.egg-info/SOURCES.txt` & `syncticketstoclickup-1.0.3/syncticketstoclickup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

