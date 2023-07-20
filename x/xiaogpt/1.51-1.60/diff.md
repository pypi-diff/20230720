# Comparing `tmp/xiaogpt-1.51.tar.gz` & `tmp/xiaogpt-1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.51.tar", last modified: Mon Jul  3 01:31:05 2023, max compression
+gzip compressed data, was "xiaogpt-1.60.tar", last modified: Thu Jul 20 14:20:28 2023, max compression
```

## Comparing `xiaogpt-1.51.tar` & `xiaogpt-1.60.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-07-03 01:30:57.265165 xiaogpt-1.51/LICENSE
--rw-r--r--   0        0        0    11816 2023-07-03 01:30:57.265165 xiaogpt-1.51/README.md
--rw-r--r--   0        0        0      934 2023-07-03 01:31:05.665095 xiaogpt-1.51/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/__main__.py
--rw-r--r--   0        0        0      707 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      554 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3280 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1252 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1638 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1996 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3821 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/cli.py
--rw-r--r--   0        0        0     5366 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/config.py
--rw-r--r--   0        0        0     2071 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/utils.py
--rw-r--r--   0        0        0    18700 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    12425 1970-01-01 00:00:00.000000 xiaogpt-1.51/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-20 14:20:20.046138 xiaogpt-1.60/LICENSE
+-rw-r--r--   0        0        0    12174 2023-07-20 14:20:20.046138 xiaogpt-1.60/README.md
+-rw-r--r--   0        0        0      962 2023-07-20 14:20:28.814052 xiaogpt-1.60/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      780 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      774 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/bot/bard_bot.py
+-rw-r--r--   0        0        0      554 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3477 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1385 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1827 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     2156 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     4152 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5604 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/config.py
+-rw-r--r--   0        0        0     2071 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/utils.py
+-rw-r--r--   0        0        0    18769 2023-07-20 14:20:20.046138 xiaogpt-1.60/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    12819 1970-01-01 00:00:00.000000 xiaogpt-1.60/PKG-INFO
```

### Comparing `xiaogpt-1.51/LICENSE` & `xiaogpt-1.60/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.51/README.md` & `xiaogpt-1.60/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 gpt3 ai
 export OPENAI_API_KEY=${your_api_key}
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gpt3
 
 # 如果你想使用 ChatGLM api
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
+# 如果你想使用 google 的 bard
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_bard --bard_token ${bard_token}
 ```
 
 ## config.json
 如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 JSON 格式
 参数优先级
 - cli args > default > config
 
@@ -123,23 +125,25 @@
         "top_p": 0.9,
     }
 }
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
+Bard-API [参考](https://github.com/dsdanielpark/Bard-API)
 ## 配置项说明
 
 | 参数                  | 说明                                              | 默认值                              |
 | --------------------- | ------------------------------------------------- | ----------------------------------- |
 | hardware              | 设备型号                                          |                                     |
 | account               | 小爱账户                                          |                                     |
 | password              | 小爱账户密码                                      |                                     |
 | openai_key            | openai的apikey                                    |                                     |
 | glm_key               | chatglm 的 apikey                                    |                                     |
+| bard_token            | bard 的 token 参考 [Bard-API](https://github.com/dsdanielpark/Bard-API)                                 |                                     |
 | cookie                | 小爱账户cookie （如果用上面密码登录可以不填）     |                                     |
 | mi_did                | 设备did                                           |                                     |
 | use_command           | 使用 MI command 与小爱交互                        | `false`                             |
 | mute_xiaoai           | 快速停掉小爱自己的回答                            | `true`                              |
 | verbose               | 是否打印详细日志                                  | `false`                             |
 | bot                   | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing | `chatgptapi`                        |
 | enable_edge_tts       | 使用Edge TTS                                      | `false`                             |
```

### Comparing `xiaogpt-1.51/pyproject.toml` & `xiaogpt-1.60/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xiaogpt"
-description = "Play ChatGPT with xiaomi AI speaker"
+description = "Play ChatGPT or other LLM with xiaomi AI speaker"
 readme = "README.md"
 authors = [
     { name = "yihong0618", email = "zouzou0208@gmail.com" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -13,19 +13,20 @@
 requires-python = ">=3.7.1"
 dependencies = [
     "miservice_fork",
     "openai",
     "aiohttp",
     "rich",
     "zhipuai",
+    "bardapi",
     "edge-tts>=6.1.3",
     "EdgeGPT==0.1.26",
 ]
 dynamic = []
-version = "1.51"
+version = "1.60"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-1.51/xiaogpt/bot/__init__.py` & `xiaogpt-1.60/xiaogpt/bot/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 from xiaogpt.bot.base_bot import BaseBot
 from xiaogpt.bot.chatgptapi_bot import ChatGPTBot
 from xiaogpt.bot.gpt3_bot import GPT3Bot
 from xiaogpt.bot.newbing_bot import NewBingBot
 from xiaogpt.bot.glm_bot import GLMBot
+from xiaogpt.bot.bard_bot import BardBot
 from xiaogpt.config import Config
 
 BOTS: dict[str, type[BaseBot]] = {
     "gpt3": GPT3Bot,
     "newbing": NewBingBot,
     "chatgptapi": ChatGPTBot,
     "glm": GLMBot,
+    "bard": BardBot,
 }
 
 
 def get_bot(config: Config) -> BaseBot:
     try:
         return BOTS[config.bot].from_config(config)
     except KeyError:
         raise ValueError(f"Unsupported bot {config.bot}, must be one of {list(BOTS)}")
 
 
-__all__ = ["GPT3Bot", "ChatGPTBot", "NewBingBot", "GLMBot", "get_bot"]
+__all__ = ["GPT3Bot", "ChatGPTBot", "NewBingBot", "GLMBot", "BardBot", "get_bot"]
```

### Comparing `xiaogpt-1.51/xiaogpt/bot/base_bot.py` & `xiaogpt-1.60/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.51/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-1.60/xiaogpt/bot/chatgptapi_bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,19 @@
     async def ask(self, query, **options):
         ms = []
         for h in self.history:
             ms.append({"role": "user", "content": h[0]})
             ms.append({"role": "assistant", "content": h[1]})
         ms.append({"role": "user", "content": f"{query}"})
         kwargs = {**self.default_options, **options}
-        completion = await openai.ChatCompletion.acreate(messages=ms, **kwargs)
+        try:
+            completion = await openai.ChatCompletion.acreate(messages=ms, **kwargs)
+        except Exception as e:
+            print(str(e))
+            return ""
         message = (
             completion["choices"][0]
             .get("message")
             .get("content")
             .encode("utf8")
             .decode()
         )
@@ -68,17 +72,21 @@
         for h in self.history:
             ms.append({"role": "user", "content": h[0]})
             ms.append({"role": "assistant", "content": h[1]})
         ms.append({"role": "user", "content": f"{query}"})
         kwargs = {"model": "gpt-3.5-turbo", **options}
         if openai.api_type == "azure":
             kwargs["deployment_id"] = self.deployment_id
-        completion = await openai.ChatCompletion.acreate(
-            messages=ms, stream=True, **kwargs
-        )
+        try:
+            completion = await openai.ChatCompletion.acreate(
+                messages=ms, stream=True, **kwargs
+            )
+        except Exception as e:
+            print(str(e))
+            return
 
         async def text_gen():
             async for event in completion:
                 chunk_message = event["choices"][0]["delta"]
                 if "content" not in chunk_message:
                     continue
                 print(chunk_message["content"], end="")
```

### Comparing `xiaogpt-1.51/xiaogpt/bot/glm_bot.py` & `xiaogpt-1.60/xiaogpt/bot/glm_bot.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,21 +26,25 @@
         ms = []
         for h in self.history:
             ms.append({"role": "user", "content": h[0]})
             ms.append({"role": "assistant", "content": h[1]})
         kwargs = {**self.default_options, **options}
         kwargs["prompt"] = ms
         ms.append({"role": "user", "content": f"{query}"})
-        r = zhipuai.model_api.sse_invoke(**kwargs)
+        try:
+            r = zhipuai.model_api.sse_invoke(**kwargs)
+        except Exception as e:
+            print(str(e))
+            return
         message = ""
         for i in r.events():
             message += str(i.data)
 
         self.history.append([f"{query}", message])
         # only keep 5 history
         first_history = self.history.pop(0)
         self.history = [first_history] + self.history[-5:]
         print(message)
         return message
 
     def ask_stream(self, query: str, **options: Any):
-        pass
+        raise Exception("GLM do not support stream")
```

### Comparing `xiaogpt-1.51/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.60/xiaogpt/bot/gpt3_bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,29 +25,37 @@
             "prompt": query,
             "model": "text-davinci-003",
             "max_tokens": 1024,
             "temperature": 1,
             "top_p": 1,
             **options,
         }
-        completion = await openai.Completion.acreate(**data)
+        try:
+            completion = await openai.Completion.acreate(**data)
+        except Exception as e:
+            print(str(e))
+            return ""
         print(completion["choices"][0]["text"])
         return completion["choices"][0]["text"]
 
     async def ask_stream(self, query, **options):
         data = {
             "prompt": query,
             "model": "text-davinci-003",
             "max_tokens": 1024,
             "temperature": 1,
             "top_p": 1,
             "stream": True,
             **options,
         }
-        completion = await openai.Completion.acreate(**data)
+        try:
+            completion = await openai.Completion.acreate(**data)
+        except Exception as e:
+            print(str(e))
+            return
 
         async def text_gen():
             async for event in completion:
                 text = event["choices"][0]["text"]
                 print(text, end="")
                 yield text
```

### Comparing `xiaogpt-1.51/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.60/xiaogpt/bot/newbing_bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,21 +36,28 @@
         s = _reference_link_re.sub("", s)
         s = re.sub(r"\[[\^\d]+\]", "", s)
         return s.strip()
 
     async def ask(self, query, **options):
         kwargs = {"conversation_style": ConversationStyle.balanced, **options}
         completion = await self._bot.ask(prompt=query, **kwargs)
-        text = self.clean_text(completion["item"]["messages"][1]["text"])
+        try:
+            text = self.clean_text(completion["item"]["messages"][1]["text"])
+        except Exception as e:
+            print(str(e))
+            return
         print(text)
         return text
 
     async def ask_stream(self, query, **options):
         kwargs = {"conversation_style": ConversationStyle.balanced, **options}
-        completion = self._bot.ask_stream(prompt=query, **kwargs)
+        try:
+            completion = self._bot.ask_stream(prompt=query, **kwargs)
+        except Exception as e:
+            return
 
         async def text_gen():
             current = ""
             async for final, resp in completion:
                 if final:
                     break
                 text = self.clean_text(resp)
```

### Comparing `xiaogpt-1.51/xiaogpt/cli.py` & `xiaogpt-1.60/xiaogpt/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     )
     parser.add_argument(
         "--glm_key",
         dest="glm_key",
         help="chatglm api key",
     )
     parser.add_argument(
+        "--bard_token",
+        dest="bard_token",
+        help="google bard token see https://github.com/dsdanielpark/Bard-API",
+    )
+    parser.add_argument(
         "--proxy",
         dest="proxy",
         help="http proxy url like http://localhost:8080",
     )
     parser.add_argument(
         "--cookie",
         dest="cookie",
@@ -102,24 +107,31 @@
     group.add_argument(
         "--use_glm",
         dest="bot",
         action="store_const",
         const="glm",
         help="if use chatglm",
     )
+    group.add_argument(
+        "--use_bard",
+        dest="bot",
+        action="store_const",
+        const="bard",
+        help="if use bard",
+    )
     parser.add_argument(
         "--bing_cookie_path",
         dest="bing_cookie_path",
         help="new bing cookies path if use new bing",
     )
     group.add_argument(
         "--bot",
         dest="bot",
         help="bot type",
-        choices=["gpt3", "chatgptapi", "newbing", "glm"],
+        choices=["gpt3", "chatgptapi", "newbing", "glm", "bard"],
     )
     parser.add_argument(
         "--config",
         dest="config",
         help="config file path",
     )
     # args to change api_base
@@ -140,15 +152,15 @@
     parser.add_argument(
         "--deployment_id",
         dest="deployment_id",
         help="specify deployment id, only used when api_base points to azure",
     )
 
     options = parser.parse_args()
-    if options.bot == "glm" and options.stream:
+    if options.bot in ["glm", "bard"] and options.stream:
         raise Exception("For now ChatGLM do not support stream")
     config = Config.from_options(options)
 
     miboy = MiGPT(config)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(miboy.run_forever())
```

### Comparing `xiaogpt-1.51/xiaogpt/config.py` & `xiaogpt-1.60/xiaogpt/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 @dataclass
 class Config:
     hardware: str = "LX06"
     account: str = os.getenv("MI_USER", "")
     password: str = os.getenv("MI_PASS", "")
     openai_key: str = os.getenv("OPENAI_API_KEY", "")
     glm_key: str = os.getenv("CHATGLM_KEY", "")
+    bard_token: str = os.getenv("BARD_TOKEN", "")
     proxy: str | None = None
     mi_did: str = os.getenv("MI_DID", "")
     keyword: Iterable[str] = KEY_WORD
     change_prompt_keyword: Iterable[str] = CHANGE_PROMPT_KEY_WORD
     prompt: str = PROMPT
     mute_xiaoai: bool = False
     bot: str = "chatgpt"
@@ -135,9 +136,13 @@
                         value = [kw for kw in value if kw]
                     elif key == "use_chatgpt_api":
                         key, value = "bot", "chatgptapi"
                     elif key == "use_gpt3":
                         key, value = "bot", "gpt3"
                     elif key == "use_newbing":
                         key, value = "bot", "newbing"
+                    elif key == "use_glm":
+                        key, value = "bot", "glm"
+                    elif key == "use_bard":
+                        key, value = "bot", "bard"
                     result[key] = value
         return result
```

### Comparing `xiaogpt-1.51/xiaogpt/utils.py` & `xiaogpt-1.60/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.51/xiaogpt/xiaogpt.py` & `xiaogpt-1.60/xiaogpt/xiaogpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,15 @@
         return await miio_command(
             self.miio_service,
             self.config.mi_did,
             f"{self.config.wakeup_command} {WAKEUP_KEYWORD} 0",
         )
 
     async def run_forever(self):
+        ask_name = self.config.bot.upper()
         async with ClientSession() as session:
             await self.init_all_data(session)
             task = asyncio.create_task(self.poll_latest_ask())
             assert task is not None  # to keep the reference to task, do not remove this
             print(f"Running xiaogpt now, 用`{'/'.join(self.config.keyword)}`开头来提问")
             print(f"或用`{self.config.start_conversation}`开始持续对话")
             while True:
@@ -466,33 +467,33 @@
                 if not self.chatbot.history:
                     query = f"{query}，{self.config.prompt}"
                 if self.config.mute_xiaoai:
                     await self.stop_if_xiaoai_is_playing()
                 else:
                     # waiting for xiaoai speaker done
                     await asyncio.sleep(8)
-                await self.do_tts("正在问GPT请耐心等待")
+                await self.do_tts(f"正在问{ask_name}请耐心等待")
                 try:
                     print(
                         "以下是小爱的回答: ",
                         new_record.get("answers", [])[0].get("tts", {}).get("text"),
                     )
                 except IndexError:
                     print("小爱没回")
-                print("以下是GPT的回答: ", end="")
+                print(f"以下是 {ask_name} 的回答: ", end="")
                 try:
                     if not self.config.enable_edge_tts:
                         async for message in self.ask_gpt(query):
                             await self.do_tts(message, wait_for_finish=True)
                     else:
                         tts_lang = (
                             find_key_by_partial_string(EDGE_TTS_DICT, query)
                             or self.config.edge_tts_voice
                         )
                         # tts with edge_tts
                         await self.edge_tts(self.ask_gpt(query), tts_lang)
                     print("回答完毕")
                 except Exception as e:
-                    print(f"GPT回答出错 {str(e)}")
+                    print(f"{ask_name} 回答出错 {str(e)}")
                 if self.in_conversation:
                     print(f"继续对话, 或用`{self.config.end_conversation}`结束对话")
                     await self.wakeup_xiaoai()
```

### Comparing `xiaogpt-1.51/PKG-INFO` & `xiaogpt-1.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.51
-Summary: Play ChatGPT with xiaomi AI speaker
+Version: 1.60
+Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
 Requires-Python: >=3.7.1
 Requires-Dist: miservice_fork
 Requires-Dist: openai
 Requires-Dist: aiohttp
 Requires-Dist: rich
 Requires-Dist: zhipuai
+Requires-Dist: bardapi
 Requires-Dist: edge-tts>=6.1.3
 Requires-Dist: EdgeGPT==0.1.26
 Description-Content-Type: text/markdown
 
 # xiaogpt
 
 [![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
@@ -111,14 +112,16 @@
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 gpt3 ai
 export OPENAI_API_KEY=${your_api_key}
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gpt3
 
 # 如果你想使用 ChatGLM api
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
+# 如果你想使用 google 的 bard
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_bard --bard_token ${bard_token}
 ```
 
 ## config.json
 如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 JSON 格式
 参数优先级
 - cli args > default > config
 
@@ -143,23 +146,25 @@
         "top_p": 0.9,
     }
 }
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
+Bard-API [参考](https://github.com/dsdanielpark/Bard-API)
 ## 配置项说明
 
 | 参数                  | 说明                                              | 默认值                              |
 | --------------------- | ------------------------------------------------- | ----------------------------------- |
 | hardware              | 设备型号                                          |                                     |
 | account               | 小爱账户                                          |                                     |
 | password              | 小爱账户密码                                      |                                     |
 | openai_key            | openai的apikey                                    |                                     |
 | glm_key               | chatglm 的 apikey                                    |                                     |
+| bard_token            | bard 的 token 参考 [Bard-API](https://github.com/dsdanielpark/Bard-API)                                 |                                     |
 | cookie                | 小爱账户cookie （如果用上面密码登录可以不填）     |                                     |
 | mi_did                | 设备did                                           |                                     |
 | use_command           | 使用 MI command 与小爱交互                        | `false`                             |
 | mute_xiaoai           | 快速停掉小爱自己的回答                            | `true`                              |
 | verbose               | 是否打印详细日志                                  | `false`                             |
 | bot                   | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing | `chatgptapi`                        |
 | enable_edge_tts       | 使用Edge TTS                                      | `false`                             |
```

