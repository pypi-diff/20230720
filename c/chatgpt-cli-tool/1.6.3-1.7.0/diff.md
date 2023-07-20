# Comparing `tmp/chatgpt-cli-tool-1.6.3.tar.gz` & `tmp/chatgpt-cli-tool-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-cli-tool-1.6.3.tar", last modified: Sat Apr  1 09:38:57 2023, max compression
+gzip compressed data, was "chatgpt-cli-tool-1.7.0.tar", last modified: Thu Jul 20 18:03:23 2023, max compression
```

## Comparing `chatgpt-cli-tool-1.6.3.tar` & `chatgpt-cli-tool-1.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 09:38:57.210487 chatgpt-cli-tool-1.6.3/
--rw-rw-rw-   0        0        0     1094 2023-03-02 17:58:50.000000 chatgpt-cli-tool-1.6.3/LICENSE
--rw-rw-rw-   0        0        0     7264 2023-04-01 09:38:57.210487 chatgpt-cli-tool-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     6458 2023-04-01 08:33:18.000000 chatgpt-cli-tool-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 09:38:57.201488 chatgpt-cli-tool-1.6.3/chatgpt_cli_tool.egg-info/
--rw-rw-rw-   0        0        0     7264 2023-04-01 09:38:57.000000 chatgpt-cli-tool-1.6.3/chatgpt_cli_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-04-01 09:38:57.000000 chatgpt-cli-tool-1.6.3/chatgpt_cli_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 09:38:57.000000 chatgpt-cli-tool-1.6.3/chatgpt_cli_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-01 09:38:57.000000 chatgpt-cli-tool-1.6.3/chatgpt_cli_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-04-01 09:38:57.000000 chatgpt-cli-tool-1.6.3/chatgpt_cli_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-01 09:38:57.000000 chatgpt-cli-tool-1.6.3/chatgpt_cli_tool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-01 09:38:57.205487 chatgpt-cli-tool-1.6.3/cli/
--rw-rw-rw-   0        0        0       23 2023-04-01 09:35:38.000000 chatgpt-cli-tool-1.6.3/cli/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 09:38:57.208486 chatgpt-cli-tool-1.6.3/cli/command/
--rw-rw-rw-   0        0        0        0 2023-03-05 12:12:19.000000 chatgpt-cli-tool-1.6.3/cli/command/__init__.py
--rw-rw-rw-   0        0        0     1063 2023-04-01 08:33:18.000000 chatgpt-cli-tool-1.6.3/cli/command/ai.py
--rw-rw-rw-   0        0        0     2209 2023-04-01 08:33:18.000000 chatgpt-cli-tool-1.6.3/cli/command/img.py
--rw-rw-rw-   0        0        0     6212 2023-03-31 18:06:39.000000 chatgpt-cli-tool-1.6.3/cli/core.py
--rw-rw-rw-   0        0        0     4349 2023-04-01 09:36:35.000000 chatgpt-cli-tool-1.6.3/cli/main.py
--rw-rw-rw-   0        0        0      164 2023-04-01 09:38:57.211490 chatgpt-cli-tool-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1387 2023-03-31 18:06:39.000000 chatgpt-cli-tool-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:03:23.906378 chatgpt-cli-tool-1.7.0/
+-rw-rw-rw-   0        0        0     1094 2023-03-02 17:58:50.000000 chatgpt-cli-tool-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0     7500 2023-07-20 18:03:23.906378 chatgpt-cli-tool-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6694 2023-07-20 18:01:56.000000 chatgpt-cli-tool-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 18:03:23.897367 chatgpt-cli-tool-1.7.0/chatgpt_cli_tool.egg-info/
+-rw-rw-rw-   0        0        0     7500 2023-07-20 18:03:23.000000 chatgpt-cli-tool-1.7.0/chatgpt_cli_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-20 18:03:23.000000 chatgpt-cli-tool-1.7.0/chatgpt_cli_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 18:03:23.000000 chatgpt-cli-tool-1.7.0/chatgpt_cli_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-07-20 18:03:23.000000 chatgpt-cli-tool-1.7.0/chatgpt_cli_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-07-20 18:03:23.000000 chatgpt-cli-tool-1.7.0/chatgpt_cli_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-20 18:03:23.000000 chatgpt-cli-tool-1.7.0/chatgpt_cli_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 18:03:23.901369 chatgpt-cli-tool-1.7.0/cli/
+-rw-rw-rw-   0        0        0       23 2023-07-20 18:02:51.000000 chatgpt-cli-tool-1.7.0/cli/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:03:23.904366 chatgpt-cli-tool-1.7.0/cli/command/
+-rw-rw-rw-   0        0        0        0 2023-03-05 12:12:19.000000 chatgpt-cli-tool-1.7.0/cli/command/__init__.py
+-rw-rw-rw-   0        0        0     1242 2023-07-20 18:01:56.000000 chatgpt-cli-tool-1.7.0/cli/command/ai.py
+-rw-rw-rw-   0        0        0     2209 2023-04-01 08:33:18.000000 chatgpt-cli-tool-1.7.0/cli/command/img.py
+-rw-rw-rw-   0        0        0     6685 2023-07-20 18:01:56.000000 chatgpt-cli-tool-1.7.0/cli/core.py
+-rw-rw-rw-   0        0        0     5255 2023-07-20 18:01:56.000000 chatgpt-cli-tool-1.7.0/cli/main.py
+-rw-rw-rw-   0        0        0      164 2023-07-20 18:03:23.907364 chatgpt-cli-tool-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1387 2023-03-31 18:06:39.000000 chatgpt-cli-tool-1.7.0/setup.py
```

### Comparing `chatgpt-cli-tool-1.6.3/LICENSE` & `chatgpt-cli-tool-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.6.3/PKG-INFO` & `chatgpt-cli-tool-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-tool
-Version: 1.6.3
+Version: 1.7.0
 Summary: Command-line interface tool for interacting with ChatGPT using terminal
 Home-page: https://github.com/lmatosevic/chatgpt-cli
-Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.6.3.tar.gz
+Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.7.0.tar.gz
 Author: luka
 Author-email: lukamatosevic5@gmail.com
 License: MIT
 Keywords: chatgpt,openai,dall-e,cli,chat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -57,26 +57,27 @@
 1. Create an **~/.chatgpt-cli/.env** file with variable **OPENAI_API_KEY**
 2. Create an **.env** file in the working directory with variable **OPENAI_API_KEY**
 3. Set it through environment variable **OPENAI_API_KEY**
 4. Pass it as the first argument when executing this tool (e.g. `chatgpt-cli my_api_key [out_file]`)
 
 All configurable environment variables for ChatGPT can be found in [.env.example](.env.example) file:
 
-| Variable name   | Description                                                                                         | Default value                                              |
-|-----------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------|
-| OPENAI_API_KEY  | OpenAI API key used to send request                                                                 | -                                                          |
-| GPT_MODEL       | GPT model used for chat completion                                                                  | gpt-3.5-turbo                                              |
-| GPT_TEMPERATURE | GPT temperature value (between 0 and 2), lower values provide more focused and deterministic output | 1                                                          |
-| GPT_SYSTEM_DESC | The description for the system on how to best tailor answers (disable with "None")                  | You are a very direct and straight-to-the-point assistant. |
-| GPT_IMAGE_SIZE  | The generated image size (256x256, 512x512 or 1024x1024)                                            | 512x512                                                    |
-| HISTORY_SIZE    | Number of last messages to keep in history as a context for the next question                       | 3                                                          |
-| CHAT_TEXT_WIDTH | Maximum number of characters to display per line in interactive chat mode (0 - as much as possible) | 0                                                          |
-| CHAT_COLORED    | Enable this to use colors in interactive chat mode                                                  | true                                                       |
-| CHAT_COLOR_YOU  | The color used for your inputs                                                                      | green                                                      |
-| CHAT_COLOR_AI   | The colore of AI responses                                                                          | white                                                      |
+| Variable name       | Description                                                                                         | Default value                                              |
+|---------------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------|
+| OPENAI_API_KEY      | OpenAI API key used to send request                                                                 | -                                                          |
+| GPT_MODEL           | GPT model used for chat completion                                                                  | gpt-3.5-turbo                                              |
+| GPT_TEMPERATURE     | GPT temperature value (between 0 and 2), lower values provide more focused and deterministic output | 1                                                          |
+| GPT_STREAM_RESPONSE | Enable OpenAI client to use Server Sent Events for streaming tokens from the API                    | true                                                       |
+| GPT_SYSTEM_DESC     | The description for the system on how to best tailor answers (disable with "None")                  | You are a very direct and straight-to-the-point assistant. |
+| GPT_IMAGE_SIZE      | The generated image size (256x256, 512x512 or 1024x1024)                                            | 512x512                                                    |
+| HISTORY_SIZE        | Number of last messages to keep in history as a context for the next question                       | 3                                                          |
+| CHAT_TEXT_WIDTH     | Maximum number of characters to display per line in interactive chat mode (0 - as much as possible) | 0                                                          |
+| CHAT_COLORED        | Enable this to use colors in interactive chat mode                                                  | true                                                       |
+| CHAT_COLOR_YOU      | The color used for your inputs                                                                      | green                                                      |
+| CHAT_COLOR_AI       | The colore of AI responses                                                                          | white                                                      |
 
 _Supported ANSI colors are: black, red, green, yellow, blue, magenta, cyan, and white_
 
 ## Running the CLI
 
 If you installed the tool using pip, then simply start the cli using any of the following commands:
```

### Comparing `chatgpt-cli-tool-1.6.3/README.md` & `chatgpt-cli-tool-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,27 @@
 1. Create an **~/.chatgpt-cli/.env** file with variable **OPENAI_API_KEY**
 2. Create an **.env** file in the working directory with variable **OPENAI_API_KEY**
 3. Set it through environment variable **OPENAI_API_KEY**
 4. Pass it as the first argument when executing this tool (e.g. `chatgpt-cli my_api_key [out_file]`)
 
 All configurable environment variables for ChatGPT can be found in [.env.example](.env.example) file:
 
-| Variable name   | Description                                                                                         | Default value                                              |
-|-----------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------|
-| OPENAI_API_KEY  | OpenAI API key used to send request                                                                 | -                                                          |
-| GPT_MODEL       | GPT model used for chat completion                                                                  | gpt-3.5-turbo                                              |
-| GPT_TEMPERATURE | GPT temperature value (between 0 and 2), lower values provide more focused and deterministic output | 1                                                          |
-| GPT_SYSTEM_DESC | The description for the system on how to best tailor answers (disable with "None")                  | You are a very direct and straight-to-the-point assistant. |
-| GPT_IMAGE_SIZE  | The generated image size (256x256, 512x512 or 1024x1024)                                            | 512x512                                                    |
-| HISTORY_SIZE    | Number of last messages to keep in history as a context for the next question                       | 3                                                          |
-| CHAT_TEXT_WIDTH | Maximum number of characters to display per line in interactive chat mode (0 - as much as possible) | 0                                                          |
-| CHAT_COLORED    | Enable this to use colors in interactive chat mode                                                  | true                                                       |
-| CHAT_COLOR_YOU  | The color used for your inputs                                                                      | green                                                      |
-| CHAT_COLOR_AI   | The colore of AI responses                                                                          | white                                                      |
+| Variable name       | Description                                                                                         | Default value                                              |
+|---------------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------|
+| OPENAI_API_KEY      | OpenAI API key used to send request                                                                 | -                                                          |
+| GPT_MODEL           | GPT model used for chat completion                                                                  | gpt-3.5-turbo                                              |
+| GPT_TEMPERATURE     | GPT temperature value (between 0 and 2), lower values provide more focused and deterministic output | 1                                                          |
+| GPT_STREAM_RESPONSE | Enable OpenAI client to use Server Sent Events for streaming tokens from the API                    | true                                                       |
+| GPT_SYSTEM_DESC     | The description for the system on how to best tailor answers (disable with "None")                  | You are a very direct and straight-to-the-point assistant. |
+| GPT_IMAGE_SIZE      | The generated image size (256x256, 512x512 or 1024x1024)                                            | 512x512                                                    |
+| HISTORY_SIZE        | Number of last messages to keep in history as a context for the next question                       | 3                                                          |
+| CHAT_TEXT_WIDTH     | Maximum number of characters to display per line in interactive chat mode (0 - as much as possible) | 0                                                          |
+| CHAT_COLORED        | Enable this to use colors in interactive chat mode                                                  | true                                                       |
+| CHAT_COLOR_YOU      | The color used for your inputs                                                                      | green                                                      |
+| CHAT_COLOR_AI       | The colore of AI responses                                                                          | white                                                      |
 
 _Supported ANSI colors are: black, red, green, yellow, blue, magenta, cyan, and white_
 
 ## Running the CLI
 
 If you installed the tool using pip, then simply start the cli using any of the following commands:
```

### Comparing `chatgpt-cli-tool-1.6.3/chatgpt_cli_tool.egg-info/PKG-INFO` & `chatgpt-cli-tool-1.7.0/chatgpt_cli_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-tool
-Version: 1.6.3
+Version: 1.7.0
 Summary: Command-line interface tool for interacting with ChatGPT using terminal
 Home-page: https://github.com/lmatosevic/chatgpt-cli
-Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.6.3.tar.gz
+Download-URL: https://github.com/lmatosevic/chatgpt-cli/archive/refs/tags/1.7.0.tar.gz
 Author: luka
 Author-email: lukamatosevic5@gmail.com
 License: MIT
 Keywords: chatgpt,openai,dall-e,cli,chat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -57,26 +57,27 @@
 1. Create an **~/.chatgpt-cli/.env** file with variable **OPENAI_API_KEY**
 2. Create an **.env** file in the working directory with variable **OPENAI_API_KEY**
 3. Set it through environment variable **OPENAI_API_KEY**
 4. Pass it as the first argument when executing this tool (e.g. `chatgpt-cli my_api_key [out_file]`)
 
 All configurable environment variables for ChatGPT can be found in [.env.example](.env.example) file:
 
-| Variable name   | Description                                                                                         | Default value                                              |
-|-----------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------|
-| OPENAI_API_KEY  | OpenAI API key used to send request                                                                 | -                                                          |
-| GPT_MODEL       | GPT model used for chat completion                                                                  | gpt-3.5-turbo                                              |
-| GPT_TEMPERATURE | GPT temperature value (between 0 and 2), lower values provide more focused and deterministic output | 1                                                          |
-| GPT_SYSTEM_DESC | The description for the system on how to best tailor answers (disable with "None")                  | You are a very direct and straight-to-the-point assistant. |
-| GPT_IMAGE_SIZE  | The generated image size (256x256, 512x512 or 1024x1024)                                            | 512x512                                                    |
-| HISTORY_SIZE    | Number of last messages to keep in history as a context for the next question                       | 3                                                          |
-| CHAT_TEXT_WIDTH | Maximum number of characters to display per line in interactive chat mode (0 - as much as possible) | 0                                                          |
-| CHAT_COLORED    | Enable this to use colors in interactive chat mode                                                  | true                                                       |
-| CHAT_COLOR_YOU  | The color used for your inputs                                                                      | green                                                      |
-| CHAT_COLOR_AI   | The colore of AI responses                                                                          | white                                                      |
+| Variable name       | Description                                                                                         | Default value                                              |
+|---------------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------|
+| OPENAI_API_KEY      | OpenAI API key used to send request                                                                 | -                                                          |
+| GPT_MODEL           | GPT model used for chat completion                                                                  | gpt-3.5-turbo                                              |
+| GPT_TEMPERATURE     | GPT temperature value (between 0 and 2), lower values provide more focused and deterministic output | 1                                                          |
+| GPT_STREAM_RESPONSE | Enable OpenAI client to use Server Sent Events for streaming tokens from the API                    | true                                                       |
+| GPT_SYSTEM_DESC     | The description for the system on how to best tailor answers (disable with "None")                  | You are a very direct and straight-to-the-point assistant. |
+| GPT_IMAGE_SIZE      | The generated image size (256x256, 512x512 or 1024x1024)                                            | 512x512                                                    |
+| HISTORY_SIZE        | Number of last messages to keep in history as a context for the next question                       | 3                                                          |
+| CHAT_TEXT_WIDTH     | Maximum number of characters to display per line in interactive chat mode (0 - as much as possible) | 0                                                          |
+| CHAT_COLORED        | Enable this to use colors in interactive chat mode                                                  | true                                                       |
+| CHAT_COLOR_YOU      | The color used for your inputs                                                                      | green                                                      |
+| CHAT_COLOR_AI       | The colore of AI responses                                                                          | white                                                      |
 
 _Supported ANSI colors are: black, red, green, yellow, blue, magenta, cyan, and white_
 
 ## Running the CLI
 
 If you installed the tool using pip, then simply start the cli using any of the following commands:
```

### Comparing `chatgpt-cli-tool-1.6.3/cli/command/ai.py` & `chatgpt-cli-tool-1.7.0/cli/command/ai.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,18 @@
     if valid_input(query):
         messages.append({'role': 'user', 'content': str(query)})
 
     response = chatgpt_response(messages)
     if response is None:
         sys.exit(2)
 
-    print(response)
+    if isinstance(response, str):
+        print(response)
+    else:
+        stream_content = ''
+        for token in response:
+            stream_content += token
+        print(stream_content)
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `chatgpt-cli-tool-1.6.3/cli/command/img.py` & `chatgpt-cli-tool-1.7.0/cli/command/img.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-tool-1.6.3/cli/core.py` & `chatgpt-cli-tool-1.7.0/cli/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 import sys
-from typing import List, TypedDict, Union, Optional, Tuple
+from typing import List, TypedDict, Union, Optional, Tuple, Iterable
 
 import openai
 from dotenv import load_dotenv
 
 from cli import __version__
 
 home_env_file = os.path.expanduser('~') + '/.chatgpt-cli/.env'
 env_file = os.getcwd() + '/.env'
 
 load_dotenv(home_env_file)
 load_dotenv(env_file)
 
 default_model = 'gpt-3.5-turbo'
 default_temperature = '1'
+default_stream_response = 'true'
 default_system_desc = 'You are a very direct and straight-to-the-point assistant.'
 default_image_size = '512x512'
 
 MessageType = TypedDict('MessageType', {'role': str, 'content': str})
 
 
 def ensure_api_key(default: str = None, prompt: bool = False, use_args_key: bool = True) -> str:
@@ -95,29 +96,39 @@
                 content = sys.stdin.read()
     except Exception as e:
         print(f'Error on stdin input: {e}')
         pass
     return content
 
 
-def chatgpt_response(messages: List[MessageType]) -> Union[str, None]:
+def chatgpt_response(messages: List[MessageType]) -> Union[str, Iterable[str], None]:
     if messages is None or len(messages) == 0:
         print('No messages provided')
         return None
 
     model = get_env('GPT_MODEL', default_model)
     temperature = float(get_env('GPT_TEMPERATURE', default_temperature))
+    stream = icase_contains(get_env('GPT_STREAM_RESPONSE', default_stream_response), ['true', 'yes', 'on'])
     system_desc = get_env('GPT_SYSTEM_DESC', default_system_desc)
 
     if system_desc.lower() != 'none':
         messages.insert(0, {'role': 'system', 'content': system_desc})
 
     try:
-        response = openai.ChatCompletion.create(model=model, temperature=temperature, messages=messages)
-        return response.choices[0].message.content.strip('\n')
+        response = openai.ChatCompletion.create(model=model, temperature=temperature, messages=messages, stream=stream)
+        if not stream:
+            return response.choices[0].message.content.strip('\n')
+
+        def stream_response() -> Iterable[str]:
+            for line in response:
+                chunk = line['choices'][0].get('delta', {}).get('content', '')
+                if chunk:
+                    yield chunk
+
+        return stream_response()
     except openai.error.APIError as e:
         print(f'OpenAI API returned an API Error: {e}')
         return None
     except openai.error.APIConnectionError as e:
         print(f'Failed to connect to OpenAI API: {e}')
         return None
     except openai.error.AuthenticationError as e:
```

### Comparing `chatgpt-cli-tool-1.6.3/cli/main.py` & `chatgpt-cli-tool-1.7.0/cli/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         prefix = '\n\n' if os.path.getsize(file_out) > 0 else ''
         file.write(f'{prefix}[{now.isoformat()}]\n')
         file.flush()
 
     end = False
     chat_history = []
     while end is False:
+        stream_content = ''
+        stream_in_progress = False
         try:
             try:
                 style = PromptStyle.from_dict(
                     {'': f'ansi{color_you.lower()}' if color_you_ansi != '' else ''})
                 question = prompt('You: ', style=style)
             except Exception:
                 question = input(f'{color_you_ansi}You: ')
@@ -95,35 +97,56 @@
                 message
             ]
 
             response = chatgpt_response(messages)
             if response is None:
                 break
 
-            if file:
+            if file and isinstance(response, str):
                 file.write(f'\nAI: {response}\n')
                 file.flush()
 
             chat_history.append(message)
-            chat_history.append({'role': 'assistant', 'content': response})
-            if len(chat_history) >= (history_size + 1) * 2:
-                chat_history = chat_history[2:]
+
+            if isinstance(response, str):
+                chat_history.append({'role': 'assistant', 'content': response})
+            else:
+                stream_in_progress = True
 
             print(f'\n{color_ai_ansi}AI: ', end=color_end)
             count = 0
-            for char in response:
-                count += 1
-                print(f'{color_ai_ansi}{char}', end=color_end, flush=True)
-                if 0 < text_width <= count:
-                    print('')
-                    count = 0
-                time.sleep(0.01)
+            for token in response:
+                for char in token:
+                    count += 1
+                    stream_content += char
+                    print(f'{color_ai_ansi}{char}', end=color_end, flush=True)
+                    if 0 < text_width <= count:
+                        print('')
+                        count = 0
+                    time.sleep(0.01)
             print('\n')
+            stream_in_progress = False
+
+            if not isinstance(response, str):
+                chat_history.append({'role': 'assistant', 'content': stream_content})
+                if file:
+                    file.write(f'\nAI: {stream_content}\n')
+                    file.flush()
+
+            if len(chat_history) >= (history_size + 1) * 2:
+                chat_history = chat_history[2:]
         except KeyboardInterrupt:
-            break
+            if stream_in_progress:
+                chat_history.append({'role': 'assistant', 'content': stream_content})
+                if file:
+                    file.write(f'\nAI: {stream_content}\n')
+                    file.flush()
+                print('\n')
+            else:
+                break
     print(f'\n{color_ai_ansi}AI: Goodbye', end=color_end)
     if file:
         file.write(f'\nAI: Goodbye\n')
         file.close()
 
 
 if __name__ == '__main__':
```

### Comparing `chatgpt-cli-tool-1.6.3/setup.py` & `chatgpt-cli-tool-1.7.0/setup.py`

 * *Files identical despite different names*

