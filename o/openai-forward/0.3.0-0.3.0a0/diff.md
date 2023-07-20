# Comparing `tmp/openai_forward-0.3.0.tar.gz` & `tmp/openai_forward-0.3.0a0.tar.gz`

## Comparing `openai_forward-0.3.0.tar` & `openai_forward-0.3.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/__init__.py
--rwxr-xr-x   0        0        0     1978 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/__main__.py
--rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/app.py
--rwxr-xr-x   0        0        0     5429 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/base.py
--rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/config.py
--rwxr-xr-x   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/openai.py
--rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/tool.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/content/__init__.py
--rwxr-xr-x   0        0        0     2720 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/content/chat.py
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/content/whisper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/routers/__init__.py
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/routers/openai_v1.py
--rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.3.0/openai_forward/routers/schemas.py
--rwxr-xr-x   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.3.0/.gitignore
--rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.3.0/LICENSE
--rwxr-xr-x   0        0        0    11028 2020-02-02 00:00:00.000000 openai_forward-0.3.0/README.md
--rwxr-xr-x   0        0        0     1627 2020-02-02 00:00:00.000000 openai_forward-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    12224 2020-02-02 00:00:00.000000 openai_forward-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/__main__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/app.py
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/base.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/config.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/openai.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/content/chat.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/content/whisper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0    12172 2020-02-02 00:00:00.000000 openai_forward-0.3.0a0/PKG-INFO
```

### Comparing `openai_forward-0.3.0/openai_forward/__main__.py` & `openai_forward-0.3.0a0/openai_forward/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/openai_forward/base.py` & `openai_forward-0.3.0a0/openai_forward/base.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/openai_forward/config.py` & `openai_forward-0.3.0a0/openai_forward/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/openai_forward/openai.py` & `openai_forward-0.3.0a0/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/openai_forward/tool.py` & `openai_forward-0.3.0a0/openai_forward/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,27 +74,25 @@
                 messages.append(content)
             else:
                 assistant.append(content)
     return messages, assistant
 
 
 def convert_chatlog_to_jsonl(log_path: str, target_path: str):
-    """Convert single chatlog to jsonl"""
     message_list, assistant_list = parse_log_to_list(log_path)
     content_list = get_matches(messages=message_list, assistants=assistant_list)
     json_dump(content_list, target_path, indent_2=True)
 
 
-def get_log_files_from_folder(log_path: str):
+def sort_logname_by_datetime(log_path: str):
     return ls(log_path, "*.log", relp=False)
 
 
 def convert_folder_to_jsonl(folder_path: str, target_path: str):
-    """Convert chatlog folder to jsonl"""
-    log_files = get_log_files_from_folder(folder_path)
+    log_files = sort_logname_by_datetime(folder_path)
     messages = []
     assistants = []
     for log_path in log_files:
         msg, ass = parse_log_to_list(log_path)
 
         msg_len, ass_len = len(msg), len(ass)
         if msg_len != ass_len:
```

### Comparing `openai_forward-0.3.0/openai_forward/content/chat.py` & `openai_forward-0.3.0a0/openai_forward/content/chat.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/openai_forward/routers/openai_v1.py` & `openai_forward-0.3.0a0/openai_forward/routers/openai_v1.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/openai_forward/routers/schemas.py` & `openai_forward-0.3.0a0/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/.gitignore` & `openai_forward-0.3.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/LICENSE` & `openai_forward-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.3.0/README.md` & `openai_forward-0.3.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,18 +119,20 @@
    <summary> details</summary>  
 
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="sk-******" \
     -e BASE_URL="https://api.openai-forward.com" \
-    -e CODE="******" \
+    -e CODE="kunyuan" \
     yidadaa/chatgpt-next-web 
 ``` 
 
+这里部署了一个，供大家轻度使用:  
+https://chat.beidongjiedeguang.top , 访问密码: `kunyuan`
 </details>
 
 ### 在代码中使用
 
 **Python**
 
 ```diff
@@ -179,25 +181,25 @@
 ```
 
 </details>
 
 ## 配置选项
 
 配置的设置方式支持两种  
-一种为在命令行中执行`aifd run` 的运行参数(如`--port=8000`)中指定;  
+一种为在命令行中执行`openai-forward run`的运行参数(如`--port=8000`)中指定;  
 另一种为读取环境变量的方式指定。
 
 ### 命令行参数
 
-可通过 `aifd run --help` 查看
+可通过 `openai-forward run --help` 查看
 
 <details open>
   <summary>Click for more details</summary>
 
-**`aifd run`参数配置项**
+**`openai-forward run`参数配置项**
 
 | 配置项 | 说明                |          默认值           |
 |-----------------|-------------------|:----------------------:|
 | --port | 服务端口号             |          8000          |
 | --workers | 工作进程数             |           1            |
 | --base_url | 同 OPENAI_BASE_URL | https://api.openai.com |
 | --api_key | 同 OPENAI_API_KEY  |         `None`         |
@@ -271,47 +273,45 @@
 
 ## 对话日志
 
 默认不记录对话日志，若要开启需设置环境变量`LOG_CHAT=true`
 <details open>
   <summary>Click for more details</summary>
 
-保存路径在当前目录下的`Log/chat`路径中。  
+保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
-{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3', 'datetime': '2023-07-18 14:01:21'}
-{'assistant': 'Hello there! How can I assist you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
-{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7', 'datetime': '2023-07-18 14:01:23'}
+{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'assistant': 'Hello! How can I assist you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
 {'assistant': 'Hi there! How can I assist you today?', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
 ```
 
 转换为`json`格式：
 
 ```bash
-aifd convert
+openai-forward convert
 ```
 
 得到`chat.json`：
 
 ```json
 [
     {
-        "datetime": "2023-07-18 14:01:21",
         "forwarded-for": "",
         "model": "gpt-3.5-turbo",
         "messages": [
             {
                 "user": "hi"
             }
         ],
         "assistant": "Hello there! How can I assist you today?"
     },
     {
-        "datetime": "2023-07-18 14:01:23",
         "forwarded-for": "",
         "model": "gpt-3.5-turbo",
         "messages": [
             {
                 "user": "Hello!"
             }
         ],
```

#### html2text {}

```diff
@@ -37,36 +37,39 @@
 [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) > https://
 cloudflare.page.openai-forward.com ## åºç¨ ### [èå¤©åºç¨](https://
 chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
 github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
 æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å   details ```bash docker
 run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://
-api.openai-forward.com" \ -e CODE="******" \ yidadaa/chatgpt-next-web ```  ###
-å¨ä»£ç ä¸­ä½¿ç¨ **Python** ```diff import openai + openai.api_base = "https:
-//api.openai-forward.com/v1" openai.api_key = "sk-******" ```  More Examples
-**JS/TS** ```diff import { Configuration } from "openai"; const configuration =
-new Configuration({ + basePath: "https://api.openai-forward.com/v1", apiKey:
-"sk-******", }); ``` **gpt-3.5-turbo** ```bash curl https://api.openai-
-forward.com/v1/chat/completions \ -H "Content-Type: application/json" \ -
-H "Authorization: Bearer sk-******" \ -d '{ "model": "gpt-3.5-turbo",
-"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Image Generation
-(DALL-E)** ```bash curl --location 'https://api.openai-forward.com/v1/images/
-generations' \ --header 'Authorization: Bearer sk-******' \ --header 'Content-
-Type: application/json' \ --data '{ "prompt": "A photo of a cat", "n": 1,
-"size": "512x512" }' ```  ## éç½®éé¡¹ éç½®çè®¾ç½®æ¹å¼æ¯æä¸¤ç§
-ä¸ç§ä¸ºå¨å½ä»¤è¡ä¸­æ§è¡`aifd run` çè¿è¡åæ°(å¦`--
+api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
+è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
+chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
+**Python** ```diff import openai + openai.api_base = "https://api.openai-
+forward.com/v1" openai.api_key = "sk-******" ```  More Examples **JS/TS**
+```diff import { Configuration } from "openai"; const configuration = new
+Configuration({ + basePath: "https://api.openai-forward.com/v1", apiKey: "sk-
+******", }); ``` **gpt-3.5-turbo** ```bash curl https://api.openai-forward.com/
+v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization:
+Bearer sk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role":
+"user", "content": "Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl
+--location 'https://api.openai-forward.com/v1/images/generations' \ --header
+'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
+--data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ```  ##
+éç½®éé¡¹ éç½®çè®¾ç½®æ¹å¼æ¯æä¸¤ç§
+ä¸ç§ä¸ºå¨å½ä»¤è¡ä¸­æ§è¡`openai-forward run`çè¿è¡åæ°(å¦`--
 port=8000`)ä¸­æå®; å¦ä¸ç§ä¸ºè¯»åç¯å¢åéçæ¹å¼æå®ã ###
-å½ä»¤è¡åæ° å¯éè¿ `aifd run --help` æ¥ç  Click for more details
-**`aifd run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ | é»è®¤å¼ | |-------------
-----|-------------------|:----------------------:| | --port | æå¡ç«¯å£å· |
-8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --base_url | å OPENAI_BASE_URL |
-https://api.openai.com | | --api_key | å OPENAI_API_KEY | `None` | | --
-forward_key | å FORWARD_KEY | `None` | | --route_prefix | å ROUTE_PREFIX |
-`None` | | --log_chat | å LOG_CHAT | `False` |  ### ç¯å¢åééç½®é¡¹
+å½ä»¤è¡åæ° å¯éè¿ `openai-forward run --help` æ¥ç  Click for more
+details **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
+é»è®¤å¼ | |-----------------|-------------------|:----------------------:| |
+--port | æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --
+base_url | å OPENAI_BASE_URL | https://api.openai.com | | --api_key | å
+OPENAI_API_KEY | `None` | | --forward_key | å FORWARD_KEY | `None` | | --
+route_prefix | å ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT |
+`False` |  ### ç¯å¢åééç½®é¡¹
 æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å | ç¯å¢åé | è¯´æ |
 é»è®¤å¼ | |-----------------|------------------------------------------------
 -------------------------------------------------------------------------------
 ----|:------------------------:| | OPENAI_BASE_URL | é»è®¤ openaiå®æ¹ api
 å°å | https://api.openai.com | | OPENAI_API_KEY | é»è®¤openai api
 keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | |
 FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
@@ -89,24 +92,22 @@
 fk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user",
 "content": "Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base
 = "https://api.openai-forward.com/v1" - openai.api_key = "sk-******" +
 openai.api_key = "fk-******" ``` **Web application** ```bash docker run -d \ -
 p 3000:3000 \ -e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-
 forward.com" \ -e CODE="" \ yidadaa/chatgpt-next-web ```  ## å¯¹è¯æ¥å¿
 é»è®¤ä¸è®°å½å¯¹è¯æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
-Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/chat`è·¯å¾ä¸­ã
-è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-
-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3',
-'datetime': '2023-07-18 14:01:21'} {'assistant': 'Hello there! How can I assist
-you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [
-{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid':
-'f844d156-e747-4887-aef8-e40d977b5ee7', 'datetime': '2023-07-18 14:01:23'}
-{'assistant': 'Hi there! How can I assist you today?', 'uid': 'f844d156-e747-
-4887-aef8-e40d977b5ee7'} ``` è½¬æ¢ä¸º`json`æ ¼å¼ï¼ ```bash aifd convert ```
-å¾å°`chat.json`ï¼ ```json [ { "datetime": "2023-07-18 14:01:21", "forwarded-
-for": "", "model": "gpt-3.5-turbo", "messages": [ { "user": "hi" } ],
-"assistant": "Hello there! How can I assist you today?" }, { "datetime": "2023-
-07-18 14:01:23", "forwarded-for": "", "model": "gpt-3.5-turbo", "messages": [
-{ "user": "Hello!" } ], "assistant": "Hi there! How can I assist you today?" }
-] ```  ## Backer and Sponsor [.github/images/jetbrains.svg] ## License OpenAI-
-Forward is licensed under the [MIT](https://opensource.org/license/mit/
-) license.
+Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
+chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
+'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-
+e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
+'467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
+'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-
+e40d977b5ee7'} {'assistant': 'Hi there! How can I assist you today?', 'uid':
+'f844d156-e747-4887-aef8-e40d977b5ee7'} ``` è½¬æ¢ä¸º`json`æ ¼å¼ï¼ ```bash
+openai-forward convert ``` å¾å°`chat.json`ï¼ ```json [ { "forwarded-for":
+"", "model": "gpt-3.5-turbo", "messages": [ { "user": "hi" } ], "assistant":
+"Hello there! How can I assist you today?" }, { "forwarded-for": "", "model":
+"gpt-3.5-turbo", "messages": [ { "user": "Hello!" } ], "assistant": "Hi there!
+How can I assist you today?" } ] ```  ## Backer and Sponsor [.github/images/
+jetbrains.svg] ## License OpenAI-Forward is licensed under the [MIT](https://
+opensource.org/license/mit/) license.
```

### Comparing `openai_forward-0.3.0/pyproject.toml` & `openai_forward-0.3.0a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 
 dependencies = [
-    "loguru>=0.7.0",
+    "loguru",
     "sparrow-python>=0.1.5",
-    "fastapi>=0.90.0",
-    "uvicorn>=0.23.1",
-    "orjson>=3.9.2",
+    "fastapi",
+    "uvicorn",
+    "orjson",
     "python-dotenv",
-    "httpx>=0.24.1",
+    "httpx",
     "pytz",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/beidongjiedeguang/openai-forward"
 Documentation = "https://github.com/beidongjiedeguang/openai-forward#openai-forward"
 Issues = "https://github.com/beidongjiedeguang/openai-forward/issues"
 Source = "https://github.com/beidongjiedeguang/openai-forward"
 
 [project.optional-dependencies]
 test = [
-    "openai>=0.27.8",
+    "openai",
     "pytest",
 ]
 
 [project.scripts]
 openai_forward = "openai_forward.__main__:main"
 openai-forward = "openai_forward.__main__:main"
-aifd = "openai_forward.__main__:main"
+aifwd = "openai_forward.__main__:main"
 
 [tool.hatch.version]
 path = "openai_forward/__init__.py"
 
 [tool.isort]
 profile = "black"
```

### Comparing `openai_forward-0.3.0/PKG-INFO` & `openai_forward-0.3.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.3.0
+Version: 0.3.0a0
 Summary: 🚀 OpenAI API Reverse Proxy · ChatGPT API Proxy
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: OpenAI API Forwarding,chatgpt,fastapi,openai,openai-api,openai-proxy,python,streaming-api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
-Requires-Dist: fastapi>=0.90.0
-Requires-Dist: httpx>=0.24.1
-Requires-Dist: loguru>=0.7.0
-Requires-Dist: orjson>=3.9.2
+Requires-Dist: fastapi
+Requires-Dist: httpx
+Requires-Dist: loguru
+Requires-Dist: orjson
 Requires-Dist: python-dotenv
 Requires-Dist: pytz
 Requires-Dist: sparrow-python>=0.1.5
-Requires-Dist: uvicorn>=0.23.1
+Requires-Dist: uvicorn
 Provides-Extra: test
-Requires-Dist: openai>=0.27.8; extra == 'test'
+Requires-Dist: openai; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 **中文** | ~~[**English**](./README_EN.md)~~
 
 <h1 align="center">
     <br>
@@ -148,18 +148,20 @@
    <summary> details</summary>  
 
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="sk-******" \
     -e BASE_URL="https://api.openai-forward.com" \
-    -e CODE="******" \
+    -e CODE="kunyuan" \
     yidadaa/chatgpt-next-web 
 ``` 
 
+这里部署了一个，供大家轻度使用:  
+https://chat.beidongjiedeguang.top , 访问密码: `kunyuan`
 </details>
 
 ### 在代码中使用
 
 **Python**
 
 ```diff
@@ -208,25 +210,25 @@
 ```
 
 </details>
 
 ## 配置选项
 
 配置的设置方式支持两种  
-一种为在命令行中执行`aifd run` 的运行参数(如`--port=8000`)中指定;  
+一种为在命令行中执行`openai-forward run`的运行参数(如`--port=8000`)中指定;  
 另一种为读取环境变量的方式指定。
 
 ### 命令行参数
 
-可通过 `aifd run --help` 查看
+可通过 `openai-forward run --help` 查看
 
 <details open>
   <summary>Click for more details</summary>
 
-**`aifd run`参数配置项**
+**`openai-forward run`参数配置项**
 
 | 配置项 | 说明                |          默认值           |
 |-----------------|-------------------|:----------------------:|
 | --port | 服务端口号             |          8000          |
 | --workers | 工作进程数             |           1            |
 | --base_url | 同 OPENAI_BASE_URL | https://api.openai.com |
 | --api_key | 同 OPENAI_API_KEY  |         `None`         |
@@ -300,47 +302,45 @@
 
 ## 对话日志
 
 默认不记录对话日志，若要开启需设置环境变量`LOG_CHAT=true`
 <details open>
   <summary>Click for more details</summary>
 
-保存路径在当前目录下的`Log/chat`路径中。  
+保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
-{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3', 'datetime': '2023-07-18 14:01:21'}
-{'assistant': 'Hello there! How can I assist you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
-{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7', 'datetime': '2023-07-18 14:01:23'}
+{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'assistant': 'Hello! How can I assist you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
 {'assistant': 'Hi there! How can I assist you today?', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
 ```
 
 转换为`json`格式：
 
 ```bash
-aifd convert
+openai-forward convert
 ```
 
 得到`chat.json`：
 
 ```json
 [
     {
-        "datetime": "2023-07-18 14:01:21",
         "forwarded-for": "",
         "model": "gpt-3.5-turbo",
         "messages": [
             {
                 "user": "hi"
             }
         ],
         "assistant": "Hello there! How can I assist you today?"
     },
     {
-        "datetime": "2023-07-18 14:01:23",
         "forwarded-for": "",
         "model": "gpt-3.5-turbo",
         "messages": [
             {
                 "user": "Hello!"
             }
         ],
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.3.0 Summary: ð OpenAI
-API Reverse Proxy Â· ChatGPT API Proxy Project-URL: Homepage, https://
+Metadata-Version: 2.1 Name: openai_forward Version: 0.3.0a0 Summary: ð
+OpenAI API Reverse Proxy Â· ChatGPT API Proxy Project-URL: Homepage, https://
 github.com/beidongjiedeguang/openai-forward Project-URL: Documentation, https:/
 /github.com/beidongjiedeguang/openai-forward#openai-forward Project-URL:
 Issues, https://github.com/beidongjiedeguang/openai-forward/issues Project-URL:
 Source, https://github.com/beidongjiedeguang/openai-forward Author-email:
 kunyuan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: OpenAI API
 Forwarding,chatgpt,fastapi,openai,openai-api,openai-proxy,python,streaming-api
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6 Requires-Dist: fastapi>=0.90.0 Requires-Dist:
-httpx>=0.24.1 Requires-Dist: loguru>=0.7.0 Requires-Dist: orjson>=3.9.2
-Requires-Dist: python-dotenv Requires-Dist: pytz Requires-Dist: sparrow-
-python>=0.1.5 Requires-Dist: uvicorn>=0.23.1 Provides-Extra: test Requires-
-Dist: openai>=0.27.8; extra == 'test' Requires-Dist: pytest; extra == 'test'
-Description-Content-Type: text/markdown **ä¸­æ** | ~~[**English**](./
-README_EN.md)~~
+Requires-Python: >=3.6 Requires-Dist: fastapi Requires-Dist: httpx Requires-
+Dist: loguru Requires-Dist: orjson Requires-Dist: python-dotenv Requires-Dist:
+pytz Requires-Dist: sparrow-python>=0.1.5 Requires-Dist: uvicorn Provides-
+Extra: test Requires-Dist: openai; extra == 'test' Requires-Dist: pytest; extra
+== 'test' Description-Content-Type: text/markdown **ä¸­æ** | ~~[**English**]
+(./README_EN.md)~~
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
@@ -54,36 +53,39 @@
 [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) > https://
 cloudflare.page.openai-forward.com ## åºç¨ ### [èå¤©åºç¨](https://
 chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
 github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
 æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å   details ```bash docker
 run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://
-api.openai-forward.com" \ -e CODE="******" \ yidadaa/chatgpt-next-web ```  ###
-å¨ä»£ç ä¸­ä½¿ç¨ **Python** ```diff import openai + openai.api_base = "https:
-//api.openai-forward.com/v1" openai.api_key = "sk-******" ```  More Examples
-**JS/TS** ```diff import { Configuration } from "openai"; const configuration =
-new Configuration({ + basePath: "https://api.openai-forward.com/v1", apiKey:
-"sk-******", }); ``` **gpt-3.5-turbo** ```bash curl https://api.openai-
-forward.com/v1/chat/completions \ -H "Content-Type: application/json" \ -
-H "Authorization: Bearer sk-******" \ -d '{ "model": "gpt-3.5-turbo",
-"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Image Generation
-(DALL-E)** ```bash curl --location 'https://api.openai-forward.com/v1/images/
-generations' \ --header 'Authorization: Bearer sk-******' \ --header 'Content-
-Type: application/json' \ --data '{ "prompt": "A photo of a cat", "n": 1,
-"size": "512x512" }' ```  ## éç½®éé¡¹ éç½®çè®¾ç½®æ¹å¼æ¯æä¸¤ç§
-ä¸ç§ä¸ºå¨å½ä»¤è¡ä¸­æ§è¡`aifd run` çè¿è¡åæ°(å¦`--
+api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
+è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
+chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
+**Python** ```diff import openai + openai.api_base = "https://api.openai-
+forward.com/v1" openai.api_key = "sk-******" ```  More Examples **JS/TS**
+```diff import { Configuration } from "openai"; const configuration = new
+Configuration({ + basePath: "https://api.openai-forward.com/v1", apiKey: "sk-
+******", }); ``` **gpt-3.5-turbo** ```bash curl https://api.openai-forward.com/
+v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization:
+Bearer sk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role":
+"user", "content": "Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl
+--location 'https://api.openai-forward.com/v1/images/generations' \ --header
+'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
+--data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ```  ##
+éç½®éé¡¹ éç½®çè®¾ç½®æ¹å¼æ¯æä¸¤ç§
+ä¸ç§ä¸ºå¨å½ä»¤è¡ä¸­æ§è¡`openai-forward run`çè¿è¡åæ°(å¦`--
 port=8000`)ä¸­æå®; å¦ä¸ç§ä¸ºè¯»åç¯å¢åéçæ¹å¼æå®ã ###
-å½ä»¤è¡åæ° å¯éè¿ `aifd run --help` æ¥ç  Click for more details
-**`aifd run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ | é»è®¤å¼ | |-------------
-----|-------------------|:----------------------:| | --port | æå¡ç«¯å£å· |
-8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --base_url | å OPENAI_BASE_URL |
-https://api.openai.com | | --api_key | å OPENAI_API_KEY | `None` | | --
-forward_key | å FORWARD_KEY | `None` | | --route_prefix | å ROUTE_PREFIX |
-`None` | | --log_chat | å LOG_CHAT | `False` |  ### ç¯å¢åééç½®é¡¹
+å½ä»¤è¡åæ° å¯éè¿ `openai-forward run --help` æ¥ç  Click for more
+details **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
+é»è®¤å¼ | |-----------------|-------------------|:----------------------:| |
+--port | æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --
+base_url | å OPENAI_BASE_URL | https://api.openai.com | | --api_key | å
+OPENAI_API_KEY | `None` | | --forward_key | å FORWARD_KEY | `None` | | --
+route_prefix | å ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT |
+`False` |  ### ç¯å¢åééç½®é¡¹
 æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å | ç¯å¢åé | è¯´æ |
 é»è®¤å¼ | |-----------------|------------------------------------------------
 -------------------------------------------------------------------------------
 ----|:------------------------:| | OPENAI_BASE_URL | é»è®¤ openaiå®æ¹ api
 å°å | https://api.openai.com | | OPENAI_API_KEY | é»è®¤openai api
 keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | |
 FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
@@ -106,24 +108,22 @@
 fk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user",
 "content": "Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base
 = "https://api.openai-forward.com/v1" - openai.api_key = "sk-******" +
 openai.api_key = "fk-******" ``` **Web application** ```bash docker run -d \ -
 p 3000:3000 \ -e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-
 forward.com" \ -e CODE="" \ yidadaa/chatgpt-next-web ```  ## å¯¹è¯æ¥å¿
 é»è®¤ä¸è®°å½å¯¹è¯æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
-Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/chat`è·¯å¾ä¸­ã
-è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-
-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3',
-'datetime': '2023-07-18 14:01:21'} {'assistant': 'Hello there! How can I assist
-you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [
-{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid':
-'f844d156-e747-4887-aef8-e40d977b5ee7', 'datetime': '2023-07-18 14:01:23'}
-{'assistant': 'Hi there! How can I assist you today?', 'uid': 'f844d156-e747-
-4887-aef8-e40d977b5ee7'} ``` è½¬æ¢ä¸º`json`æ ¼å¼ï¼ ```bash aifd convert ```
-å¾å°`chat.json`ï¼ ```json [ { "datetime": "2023-07-18 14:01:21", "forwarded-
-for": "", "model": "gpt-3.5-turbo", "messages": [ { "user": "hi" } ],
-"assistant": "Hello there! How can I assist you today?" }, { "datetime": "2023-
-07-18 14:01:23", "forwarded-for": "", "model": "gpt-3.5-turbo", "messages": [
-{ "user": "Hello!" } ], "assistant": "Hi there! How can I assist you today?" }
-] ```  ## Backer and Sponsor [.github/images/jetbrains.svg] ## License OpenAI-
-Forward is licensed under the [MIT](https://opensource.org/license/mit/
-) license.
+Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
+chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
+'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-
+e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
+'467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
+'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-
+e40d977b5ee7'} {'assistant': 'Hi there! How can I assist you today?', 'uid':
+'f844d156-e747-4887-aef8-e40d977b5ee7'} ``` è½¬æ¢ä¸º`json`æ ¼å¼ï¼ ```bash
+openai-forward convert ``` å¾å°`chat.json`ï¼ ```json [ { "forwarded-for":
+"", "model": "gpt-3.5-turbo", "messages": [ { "user": "hi" } ], "assistant":
+"Hello there! How can I assist you today?" }, { "forwarded-for": "", "model":
+"gpt-3.5-turbo", "messages": [ { "user": "Hello!" } ], "assistant": "Hi there!
+How can I assist you today?" } ] ```  ## Backer and Sponsor [.github/images/
+jetbrains.svg] ## License OpenAI-Forward is licensed under the [MIT](https://
+opensource.org/license/mit/) license.
```

