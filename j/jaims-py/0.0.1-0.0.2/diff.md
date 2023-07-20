# Comparing `tmp/jaims-py-0.0.1.tar.gz` & `tmp/jaims-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaims-py-0.0.1.tar", last modified: Thu Jul 20 09:01:45 2023, max compression
+gzip compressed data, was "jaims-py-0.0.2.tar", last modified: Thu Jul 20 18:35:34 2023, max compression
```

## Comparing `jaims-py-0.0.1.tar` & `jaims-py-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 09:01:45.698891 jaims-py-0.0.1/
--rw-r--r--   0 mush       (501) staff       (20)     4196 2023-07-20 09:01:45.698794 jaims-py-0.0.1/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)     3866 2023-07-08 14:08:37.000000 jaims-py-0.0.1/README.md
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 09:01:45.698060 jaims-py-0.0.1/jaims/
--rw-r--r--   0 mush       (501) staff       (20)      169 2023-07-20 08:54:39.000000 jaims-py-0.0.1/jaims/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)    10450 2023-07-20 08:54:39.000000 jaims-py-0.0.1/jaims/agent.py
--rw-r--r--   0 mush       (501) staff       (20)     1134 2023-07-20 08:54:39.000000 jaims-py-0.0.1/jaims/exceptions.py
--rw-r--r--   0 mush       (501) staff       (20)     7276 2023-07-20 08:54:39.000000 jaims-py-0.0.1/jaims/function_handler.py
--rw-r--r--   0 mush       (501) staff       (20)     7698 2023-07-20 08:54:39.000000 jaims-py-0.0.1/jaims/histroy_manager.py
--rw-r--r--   0 mush       (501) staff       (20)     3512 2023-07-20 08:54:39.000000 jaims-py-0.0.1/jaims/openai_wrappers.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 09:01:45.698614 jaims-py-0.0.1/jaims_py.egg-info/
--rw-r--r--   0 mush       (501) staff       (20)     4196 2023-07-20 09:01:45.000000 jaims-py-0.0.1/jaims_py.egg-info/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)      306 2023-07-20 09:01:45.000000 jaims-py-0.0.1/jaims_py.egg-info/SOURCES.txt
--rw-r--r--   0 mush       (501) staff       (20)        1 2023-07-20 09:01:45.000000 jaims-py-0.0.1/jaims_py.egg-info/dependency_links.txt
--rw-r--r--   0 mush       (501) staff       (20)       31 2023-07-20 09:01:45.000000 jaims-py-0.0.1/jaims_py.egg-info/requires.txt
--rw-r--r--   0 mush       (501) staff       (20)        6 2023-07-20 09:01:45.000000 jaims-py-0.0.1/jaims_py.egg-info/top_level.txt
--rw-r--r--   0 mush       (501) staff       (20)       38 2023-07-20 09:01:45.698927 jaims-py-0.0.1/setup.cfg
--rw-r--r--   0 mush       (501) staff       (20)      606 2023-07-20 08:57:05.000000 jaims-py-0.0.1/setup.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 18:35:34.767037 jaims-py-0.0.2/
+-rw-r--r--   0 mush       (501) staff       (20)     4181 2023-07-20 18:35:34.766901 jaims-py-0.0.2/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)     3851 2023-07-20 18:35:26.000000 jaims-py-0.0.2/README.md
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 18:35:34.765982 jaims-py-0.0.2/jaims/
+-rw-r--r--   0 mush       (501) staff       (20)      169 2023-07-20 08:54:39.000000 jaims-py-0.0.2/jaims/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)    11006 2023-07-20 18:35:26.000000 jaims-py-0.0.2/jaims/agent.py
+-rw-r--r--   0 mush       (501) staff       (20)     1134 2023-07-20 08:54:39.000000 jaims-py-0.0.2/jaims/exceptions.py
+-rw-r--r--   0 mush       (501) staff       (20)     7636 2023-07-20 18:35:26.000000 jaims-py-0.0.2/jaims/function_handler.py
+-rw-r--r--   0 mush       (501) staff       (20)     7698 2023-07-20 08:54:39.000000 jaims-py-0.0.2/jaims/histroy_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)     3512 2023-07-20 08:54:39.000000 jaims-py-0.0.2/jaims/openai_wrappers.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 18:35:34.766616 jaims-py-0.0.2/jaims_py.egg-info/
+-rw-r--r--   0 mush       (501) staff       (20)     4181 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)      306 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mush       (501) staff       (20)        1 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mush       (501) staff       (20)       31 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/requires.txt
+-rw-r--r--   0 mush       (501) staff       (20)        6 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/top_level.txt
+-rw-r--r--   0 mush       (501) staff       (20)       38 2023-07-20 18:35:34.767105 jaims-py-0.0.2/setup.cfg
+-rw-r--r--   0 mush       (501) staff       (20)      606 2023-07-20 18:35:26.000000 jaims-py-0.0.2/setup.py
```

### Comparing `jaims-py-0.0.1/PKG-INFO` & `jaims-py-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: OpenAI GPT-3 and GPT-4 function enabled agent
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,36 +17,38 @@
 _My name is Bot, jAIMs Bot._ 🕶️
 
 jAIms is a lightweight Python framework built on top of the OpenAI library that lets you create powerful LLM agents.
 It is designed with simplicity and ease of use in mind and only depends on `openai` and `tiktoken`.
 
 ## Installation
 
-TODO: add to pypi
+```bash
+pip install jaims-py
+```
 
 ## 👨‍💻 Usage
 
 Building an agent is as simple as this:
 
 ```python
 from jaims import JAImsAgent
 
 agent = JAImsAgent()
 
-response = agent.send_messages([
+response = agent.run([
     {
         "role": "user",
         "content": "Hi!"
     }
 ])
 
 print(response)
 ```
 
-The messages accepted by the `send_messages` function are those specified in the [official OpenAI docs](https://platform.openai.com/docs/api-reference/chat/create).
+The parameters accepted by the `run` method are those specified in the [official OpenAI docs](https://platform.openai.com/docs/api-reference/chat/create).
 
 ### ⚙️ Functions
 
 Of course, an agent is just a chatbot if it doesn't support functions. jAIms uses the built-in OpenAI function feature to call functions you pass to it. Here's an example where we create a simple sum function and make a simple agent that lets you sum two numbers:
 
 ```python
 import jaims
@@ -83,15 +85,15 @@
 )
 
 # a simple loop that simulates a chatbot
 while True:
     user_input = input("> ")
     if user_input == "exit":
         break
-    response = agent.send_messages(
+    response = agent.run(
         [{"role": "user", "content": user_input}],
         stream=True,
     )
 
     for chunk in response:
         print(chunk, end="", flush=True)
```

### Comparing `jaims-py-0.0.1/README.md` & `jaims-py-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,38 @@
 _My name is Bot, jAIMs Bot._ 🕶️
 
 jAIms is a lightweight Python framework built on top of the OpenAI library that lets you create powerful LLM agents.
 It is designed with simplicity and ease of use in mind and only depends on `openai` and `tiktoken`.
 
 ## Installation
 
-TODO: add to pypi
+```bash
+pip install jaims-py
+```
 
 ## 👨‍💻 Usage
 
 Building an agent is as simple as this:
 
 ```python
 from jaims import JAImsAgent
 
 agent = JAImsAgent()
 
-response = agent.send_messages([
+response = agent.run([
     {
         "role": "user",
         "content": "Hi!"
     }
 ])
 
 print(response)
 ```
 
-The messages accepted by the `send_messages` function are those specified in the [official OpenAI docs](https://platform.openai.com/docs/api-reference/chat/create).
+The parameters accepted by the `run` method are those specified in the [official OpenAI docs](https://platform.openai.com/docs/api-reference/chat/create).
 
 ### ⚙️ Functions
 
 Of course, an agent is just a chatbot if it doesn't support functions. jAIms uses the built-in OpenAI function feature to call functions you pass to it. Here's an example where we create a simple sum function and make a simple agent that lets you sum two numbers:
 
 ```python
 import jaims
@@ -72,15 +74,15 @@
 )
 
 # a simple loop that simulates a chatbot
 while True:
     user_input = input("> ")
     if user_input == "exit":
         break
-    response = agent.send_messages(
+    response = agent.run(
         [{"role": "user", "content": user_input}],
         stream=True,
     )
 
     for chunk in response:
         print(chunk, end="", flush=True)
```

### Comparing `jaims-py-0.0.1/jaims/agent.py` & `jaims-py-0.0.2/jaims/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,16 +53,16 @@
             the maximum number of consecutive function calls that can be made by the agent, defaults to 5
             for safety reasons, to avoid unwanted loops that might impact up token usage
         openai_api_key: str
             the openai api key, defaults to the OPENAI_API_KEY environment variable if not provided
 
     Methods
     -------
-        send_messages(messages, stream: bool optional) -> JAImsResponse
-            sends a list of messages to GPT and returns the response
+        run(messages, stream: bool optional) -> JAImsResponse
+            performs the call to OpenAI and returns the response
         clear_history()
             clears the agent history
         get_expenses() -> List[JaimsTokensExpense]
             returns the currently spent tokens for this agent session, one for each model used
 
     Raises
     ------
@@ -108,35 +108,47 @@
         self.__history_manager = HistoryManager(
             model=self.model,
             functions=self.functions,
             mandatory_context=self.initial_prompts,
             optimize_history=optimize_context,
         )
 
-    def send_messages(
+    def run(
         self,
-        messages,
-        max_tokens=DEFAULT_MAX_TOKENS,
-        stream=False,
-        temperature=0.0,
-        top_p=None,
-        n=1,
+        messages: List[dict] = [],
+        max_tokens: int = DEFAULT_MAX_TOKENS,
+        stream: bool = False,
+        temperature: float = 0.0,
+        top_p: Optional[int] = None,
+        n: int = 1,
+        function_call: str = "auto",
     ) -> Union[str, Generator[str, None, None]]:
         """
-        Sends a list of messages to GPT and returns the response.
+        Calls OpenAI with the passed parameters and returns or streams the response.
 
         Parameters
         ----------
             messages : list
                 the list of messages to be sent
             stream : bool (optional)
                 whether to stream the response or not, defaults to False
-            response_buffer : int (optional)
-                how much spase to leave in the context for the Agent Response when sending a new message.
+            max_tokens : int (optional)
+                the maximum tokens to be used to generate the answer
                 defaults to 512
+            temperature : float (optional)
+                the temperature to be used to generate the answer
+                defaults to 0.0
+            top_p : float (optional)
+                the top_p to be used to generate the answer
+                defaults to None
+            n : int (optional)
+                the number of answers to be generated
+                defaults to 1
+            function_call : str (optional)
+                the function call to be used, defaults to "auto"
 
         Returns
         -------
             JAImsResponse
                 the response object
         """
 
@@ -148,15 +160,15 @@
             "top_p": top_p,
             "stream": stream,
             "max_tokens": max_tokens,
             "n": n,
         }
 
         if self.functions:
-            kwargs["function_call"] = "auto"
+            kwargs["function_call"] = function_call
             kwargs["functions"] = parse_functions_to_json(self.functions)
 
         call_context = OpenaiCallContext(kwargs)
 
         return self.__call_openai(call_context)
 
     def __call_openai(
```

### Comparing `jaims-py-0.0.1/jaims/exceptions.py` & `jaims-py-0.0.2/jaims/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaims-py-0.0.1/jaims/function_handler.py` & `jaims-py-0.0.2/jaims/function_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from enum import Enum
 import json
 from typing import Any, List, Dict, Optional, Callable
 
 from jaims.exceptions import JAImsUnexpectedFunctionCall
 
 
@@ -26,38 +27,40 @@
         description : str
             the parameter description
         json_type : JsonType:
             the parameter json type
         attributes_params_descriptors : list of JAImsParamDescriptor
             the list of parameters descriptors for the attributes of the parameter
             in case the parameter is an object, defualts to None
-        array_type_descriptor : JAImsParamDescriptor
-            the parameter descriptor for the array type in case the parameter is an array, defaults to None
+        array_type_descriptors : list of JAImsParamDescriptor
+            the parameter descriptors for the array type in case the parameter is an array, defaults to None
         enum_values:
             the list of values in case the parameter is an enum, defaults to None
         required : bool
             whether the parameter is required or not, defaults to True
 
     """
 
     def __init__(
         self,
         name: str,
         description: str,
         json_type: JAImsJsonSchemaType,
-        attributes_params_descriptors: Optional[List["JAImsParamDescriptor"]] = None,
-        array_type_descriptor: Optional["JAImsParamDescriptor"] = None,
+        attributes_params_descriptors: Optional[List[JAImsParamDescriptor]] = None,
+        array_type_descriptors: Optional[List[JAImsParamDescriptor]] = None,
+        array_type_any_valid: bool = True,
         enum_values: Optional[List[Any]] = None,
         required: bool = True,
     ):
         self.name = name
         self.description = description
         self.json_type = json_type
         self.attributes_params_descriptors = attributes_params_descriptors
-        self.array_type_descriptor = array_type_descriptor
+        self.array_type_descriptors = array_type_descriptors
+        self.array_type_any_valid = array_type_any_valid
         self.enum_values = enum_values
         self.required = required
 
     def get_jsonapi_schema(self) -> Dict[str, Any]:
         """
         Returns the jsonapi schema for the parameter.
         """
@@ -73,16 +76,22 @@
             schema["properties"] = {}
             schema["required"] = []
             for param in self.attributes_params_descriptors:
                 schema["properties"][param.name] = param.get_jsonapi_schema()
                 if param.required:
                     schema["required"].append(param.name)
 
-        if self.json_type == JAImsJsonSchemaType.ARRAY and self.array_type_descriptor:
-            schema["items"] = {"type": self.array_type_descriptor.json_type.value}
+        if self.json_type == JAImsJsonSchemaType.ARRAY and self.array_type_descriptors:
+            items_schema = [
+                desc.get_jsonapi_schema() for desc in self.array_type_descriptors
+            ]
+            if self.array_type_any_valid:
+                schema["items"] = {"anyOf": items_schema}
+            else:
+                schema["items"] = [items_schema]
 
         if self.enum_values:
             schema["enum"] = self.enum_values
 
         return schema
```

### Comparing `jaims-py-0.0.1/jaims/histroy_manager.py` & `jaims-py-0.0.2/jaims/histroy_manager.py`

 * *Files identical despite different names*

### Comparing `jaims-py-0.0.1/jaims/openai_wrappers.py` & `jaims-py-0.0.2/jaims/openai_wrappers.py`

 * *Files identical despite different names*

### Comparing `jaims-py-0.0.1/jaims_py.egg-info/PKG-INFO` & `jaims-py-0.0.2/jaims_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: OpenAI GPT-3 and GPT-4 function enabled agent
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,36 +17,38 @@
 _My name is Bot, jAIMs Bot._ 🕶️
 
 jAIms is a lightweight Python framework built on top of the OpenAI library that lets you create powerful LLM agents.
 It is designed with simplicity and ease of use in mind and only depends on `openai` and `tiktoken`.
 
 ## Installation
 
-TODO: add to pypi
+```bash
+pip install jaims-py
+```
 
 ## 👨‍💻 Usage
 
 Building an agent is as simple as this:
 
 ```python
 from jaims import JAImsAgent
 
 agent = JAImsAgent()
 
-response = agent.send_messages([
+response = agent.run([
     {
         "role": "user",
         "content": "Hi!"
     }
 ])
 
 print(response)
 ```
 
-The messages accepted by the `send_messages` function are those specified in the [official OpenAI docs](https://platform.openai.com/docs/api-reference/chat/create).
+The parameters accepted by the `run` method are those specified in the [official OpenAI docs](https://platform.openai.com/docs/api-reference/chat/create).
 
 ### ⚙️ Functions
 
 Of course, an agent is just a chatbot if it doesn't support functions. jAIms uses the built-in OpenAI function feature to call functions you pass to it. Here's an example where we create a simple sum function and make a simple agent that lets you sum two numbers:
 
 ```python
 import jaims
@@ -83,15 +85,15 @@
 )
 
 # a simple loop that simulates a chatbot
 while True:
     user_input = input("> ")
     if user_input == "exit":
         break
-    response = agent.send_messages(
+    response = agent.run(
         [{"role": "user", "content": user_input}],
         stream=True,
     )
 
     for chunk in response:
         print(chunk, end="", flush=True)
```

### Comparing `jaims-py-0.0.1/setup.py` & `jaims-py-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read requirements.txt
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="jaims-py",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     description="A Python package for creating simple AI Agents using the OpenAI API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Marco Musella",
     url="https://github.com/dev-mush/jaims-py",
     license="MIT",
```

