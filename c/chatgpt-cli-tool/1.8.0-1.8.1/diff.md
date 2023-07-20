# Comparing `tmp/chatgpt-cli-tool-1.8.0.tar.gz` & `tmp/chatgpt-cli-tool-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-cli-tool-1.8.0.tar", last modified: Thu Jul 20 21:47:36 2023, max compression
+gzip compressed data, was "chatgpt-cli-tool-1.8.1.tar", last modified: Thu Jul 20 21:51:19 2023, max compression
```

## Comparing `chatgpt-cli-tool-1.8.0.tar` & `chatgpt-cli-tool-1.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 21:47:36.447836 chatgpt-cli-tool-1.8.0/
--rw-rw-rw-   0        0        0     1094 2023-03-02 17:58:50.000000 chatgpt-cli-tool-1.8.0/LICENSE
--rw-rw-rw-   0        0        0     7500 2023-07-20 21:47:36.447836 chatgpt-cli-tool-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     6694 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 21:47:36.438838 chatgpt-cli-tool-1.8.0/chatgpt_cli_tool.egg-info/
--rw-rw-rw-   0        0        0     7500 2023-07-20 21:47:36.000000 chatgpt-cli-tool-1.8.0/chatgpt_cli_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-07-20 21:47:36.000000 chatgpt-cli-tool-1.8.0/chatgpt_cli_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 21:47:36.000000 chatgpt-cli-tool-1.8.0/chatgpt_cli_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-07-20 21:47:36.000000 chatgpt-cli-tool-1.8.0/chatgpt_cli_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-07-20 21:47:36.000000 chatgpt-cli-tool-1.8.0/chatgpt_cli_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-20 21:47:36.000000 chatgpt-cli-tool-1.8.0/chatgpt_cli_tool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 21:47:36.441851 chatgpt-cli-tool-1.8.0/cli/
--rw-rw-rw-   0        0        0       23 2023-07-20 21:47:22.000000 chatgpt-cli-tool-1.8.0/cli/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 21:47:36.445838 chatgpt-cli-tool-1.8.0/cli/command/
--rw-rw-rw-   0        0        0        0 2023-03-05 12:12:19.000000 chatgpt-cli-tool-1.8.0/cli/command/__init__.py
--rw-rw-rw-   0        0        0     1242 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.0/cli/command/ai.py
--rw-rw-rw-   0        0        0     2209 2023-04-01 08:33:18.000000 chatgpt-cli-tool-1.8.0/cli/command/img.py
--rw-rw-rw-   0        0        0     6685 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.0/cli/core.py
--rw-rw-rw-   0        0        0     7816 2023-07-20 21:46:54.000000 chatgpt-cli-tool-1.8.0/cli/main.py
--rw-rw-rw-   0        0        0      164 2023-07-20 21:47:36.448843 chatgpt-cli-tool-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1387 2023-03-31 18:06:39.000000 chatgpt-cli-tool-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:51:19.278497 chatgpt-cli-tool-1.8.1/
+-rw-rw-rw-   0        0        0     1094 2023-03-02 17:58:50.000000 chatgpt-cli-tool-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0     7649 2023-07-20 21:51:19.278497 chatgpt-cli-tool-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6843 2023-07-20 21:50:30.000000 chatgpt-cli-tool-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 21:51:19.269497 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/
+-rw-rw-rw-   0        0        0     7649 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-20 21:51:19.000000 chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 21:51:19.273497 chatgpt-cli-tool-1.8.1/cli/
+-rw-rw-rw-   0        0        0       23 2023-07-20 21:51:18.000000 chatgpt-cli-tool-1.8.1/cli/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:51:19.276501 chatgpt-cli-tool-1.8.1/cli/command/
+-rw-rw-rw-   0        0        0        0 2023-03-05 12:12:19.000000 chatgpt-cli-tool-1.8.1/cli/command/__init__.py
+-rw-rw-rw-   0        0        0     1242 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.1/cli/command/ai.py
+-rw-rw-rw-   0        0        0     2209 2023-04-01 08:33:18.000000 chatgpt-cli-tool-1.8.1/cli/command/img.py
+-rw-rw-rw-   0        0        0     6685 2023-07-20 18:17:42.000000 chatgpt-cli-tool-1.8.1/cli/core.py
+-rw-rw-rw-   0        0        0     7816 2023-07-20 21:46:54.000000 chatgpt-cli-tool-1.8.1/cli/main.py
+-rw-rw-rw-   0        0        0      164 2023-07-20 21:51:19.279497 chatgpt-cli-tool-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1387 2023-03-31 18:06:39.000000 chatgpt-cli-tool-1.8.1/setup.py
```

### Comparing `chatgpt-cli-tool-1.8.0/LICENSE` & `chatgpt-cli-tool-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.0/PKG-INFO` & `chatgpt-cli-tool-1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-tool
-Version: 1.8.0
+Version: 1.8.1
 Summary: Command-line interface tool for interacting with ChatGPT using terminal
 Home-page: https://github.com/lmatosevic/chatgpt-cli
-Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.8.0.tar.gz
+Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.8.1.tar.gz
 Author: luka
 Author-email: lukamatosevic5@gmail.com
 License: MIT
 Keywords: chatgpt,openai,dall-e,cli,chat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -96,15 +96,19 @@
 chatgpt-cli chat.txt
 
 # without any arguments, api key is used from env variable and conversation is not saved to file
 chatgpt-cli
 ```
 
 If file does not exist it will be created together with all parent directories. Otherwise, if the file already exists
-the current chat conversation will be appended to the end of file.
+the user is prompted with 3 options on how to handle the existing file content:
+
+1. Continue conversation
+2. Keep previous content and start new conversation
+3. Delete previous content and start new conversation
 
 ### gpt-ai [api_key] [query]
 
 This comand sends single chat completion prompt for given query or content, and prints the result on stdout.
 
 ```sh
 # with api key and query argument
```

### Comparing `chatgpt-cli-tool-1.8.0/README.md` & `chatgpt-cli-tool-1.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,19 @@
 chatgpt-cli chat.txt
 
 # without any arguments, api key is used from env variable and conversation is not saved to file
 chatgpt-cli
 ```
 
 If file does not exist it will be created together with all parent directories. Otherwise, if the file already exists
-the current chat conversation will be appended to the end of file.
+the user is prompted with 3 options on how to handle the existing file content:
+
+1. Continue conversation
+2. Keep previous content and start new conversation
+3. Delete previous content and start new conversation
 
 ### gpt-ai [api_key] [query]
 
 This comand sends single chat completion prompt for given query or content, and prints the result on stdout.
 
 ```sh
 # with api key and query argument
```

### Comparing `chatgpt-cli-tool-1.8.0/chatgpt_cli_tool.egg-info/PKG-INFO` & `chatgpt-cli-tool-1.8.1/chatgpt_cli_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-tool
-Version: 1.8.0
+Version: 1.8.1
 Summary: Command-line interface tool for interacting with ChatGPT using terminal
 Home-page: https://github.com/lmatosevic/chatgpt-cli
-Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.8.0.tar.gz
+Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.8.1.tar.gz
 Author: luka
 Author-email: lukamatosevic5@gmail.com
 License: MIT
 Keywords: chatgpt,openai,dall-e,cli,chat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -96,15 +96,19 @@
 chatgpt-cli chat.txt
 
 # without any arguments, api key is used from env variable and conversation is not saved to file
 chatgpt-cli
 ```
 
 If file does not exist it will be created together with all parent directories. Otherwise, if the file already exists
-the current chat conversation will be appended to the end of file.
+the user is prompted with 3 options on how to handle the existing file content:
+
+1. Continue conversation
+2. Keep previous content and start new conversation
+3. Delete previous content and start new conversation
 
 ### gpt-ai [api_key] [query]
 
 This comand sends single chat completion prompt for given query or content, and prints the result on stdout.
 
 ```sh
 # with api key and query argument
```

### Comparing `chatgpt-cli-tool-1.8.0/cli/command/ai.py` & `chatgpt-cli-tool-1.8.1/cli/command/ai.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.0/cli/command/img.py` & `chatgpt-cli-tool-1.8.1/cli/command/img.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.0/cli/core.py` & `chatgpt-cli-tool-1.8.1/cli/core.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.0/cli/main.py` & `chatgpt-cli-tool-1.8.1/cli/main.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.8.0/setup.py` & `chatgpt-cli-tool-1.8.1/setup.py`

 * *Files identical despite different names*

