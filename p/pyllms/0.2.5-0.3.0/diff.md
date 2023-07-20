# Comparing `tmp/pyllms-0.2.5.tar.gz` & `tmp/pyllms-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.2.5.tar", last modified: Fri May 19 21:49:26 2023, max compression
+gzip compressed data, was "pyllms-0.3.0.tar", last modified: Thu Jul 20 09:54:53 2023, max compression
```

## Comparing `pyllms-0.2.5.tar` & `pyllms-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 21:49:26.306997 pyllms-0.2.5/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.2.5/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    38271 2023-05-19 21:49:26.306713 pyllms-0.2.5/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    36916 2023-05-19 21:24:06.000000 pyllms-0.2.5/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 21:49:26.301324 pyllms-0.2.5/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.2.5/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    20934 2023-05-19 21:40:32.000000 pyllms-0.2.5/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 21:49:26.304687 pyllms-0.2.5/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      263 2023-05-13 02:47:09.000000 pyllms-0.2.5/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2108 2023-05-13 03:43:25.000000 pyllms-0.2.5/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3970 2023-05-19 21:15:15.000000 pyllms-0.2.5/llms/providers/aleph.py
--rw-r--r--   0 prelovac   (502) staff       (20)     8999 2023-05-13 10:20:16.000000 pyllms-0.2.5/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1618 2023-05-13 03:43:25.000000 pyllms-0.2.5/llms/providers/base_provider.py
--rw-r--r--   0 prelovac   (502) staff       (20)     4582 2023-05-19 21:16:49.000000 pyllms-0.2.5/llms/providers/cohere.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2632 2023-05-17 23:38:37.000000 pyllms-0.2.5/llms/providers/google.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3465 2023-05-13 03:43:25.000000 pyllms-0.2.5/llms/providers/huggingface.py
--rw-r--r--   0 prelovac   (502) staff       (20)     7452 2023-05-13 08:50:17.000000 pyllms-0.2.5/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 21:49:26.306323 pyllms-0.2.5/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    38271 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      444 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)      109 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-05-19 21:49:26.307068 pyllms-0.2.5/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1962 2023-05-19 21:48:21.000000 pyllms-0.2.5/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-07-20 09:54:53.453430 pyllms-0.3.0/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.3.0/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    38742 2023-07-20 09:54:53.453147 pyllms-0.3.0/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    37387 2023-06-05 05:17:53.000000 pyllms-0.3.0/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-07-20 09:54:53.446923 pyllms-0.3.0/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.3.0/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    21082 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-07-20 09:54:53.450194 pyllms-0.3.0/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      263 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1910 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3008 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/aleph.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     8126 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1750 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/base_provider.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3655 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/cohere.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3177 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/google.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3472 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/huggingface.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     9396 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-07-20 09:54:53.450790 pyllms-0.3.0/llms/results/
+-rw-r--r--   0 prelovac   (502) staff       (20)        0 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/results/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     8993 2023-07-20 09:50:47.000000 pyllms-0.3.0/llms/results/result.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-07-20 09:54:53.452604 pyllms-0.3.0/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    38742 2023-07-20 09:54:53.000000 pyllms-0.3.0/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      492 2023-07-20 09:54:53.000000 pyllms-0.3.0/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-07-20 09:54:53.000000 pyllms-0.3.0/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)      134 2023-07-20 09:54:53.000000 pyllms-0.3.0/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-07-20 09:54:53.000000 pyllms-0.3.0/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-07-20 09:54:53.453618 pyllms-0.3.0/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     2009 2023-07-20 09:52:00.000000 pyllms-0.3.0/setup.py
```

### Comparing `pyllms-0.2.5/LICENSE` & `pyllms-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.2.5/PKG-INFO` & `pyllms-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.2.5
+Version: 0.3.0
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, Google Palm2/Vertex, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub,vertex ai,palm,palm2
@@ -35,30 +35,30 @@
 - Connect to top LLMs in a few lines of code
 - Response meta includes tokens processed, cost and latency standardized across the models
 - Multi-model support: Get completions from different models at the same time
 - LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
-## Installation
+# Installation
 
 Install the package using pip:
 
 ```
 pip install pyllms
 ```
 
 
-## Usage
+# Usage
 
 
 ```
 import llms
 
-model = llms.init()
+model = llms.init('gpt-4')
 result = model.complete("what is 5+5")
 
 print(result.text)  
 
 ```
 
 Library will attempt to read the API keys and the default model from environment variables, which you can set like this (for the provider you are using):
@@ -107,14 +107,15 @@
   'tokens_completion': 14, 
   'cost': '0.00007', 
   'latency': 1.4
 }
 ```
 
 
+
 ## Multi-model usage
 
 You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
@@ -156,23 +157,43 @@
 
 Tip: if you are testing this in python3 CLI, run it with -u parameter to disable buffering:
 
 ```
 python3 -u
 ```
 
+## Chat history and system message
+
+You can pass the history of conversation in a list using the following format:
+
+```
+history=[]
+history.append({"role": "user", "content": user_input})
+history.append({"role": "assistant", "content": result.text})  
+
+model.complete(prompt=prompt, history=history)
+
+```
+
+In addition, OpenAI chat models support system message:
+
+```
+model.complete(prompt=prompt, system_message=system, history=history)
+
+```
+
 ## Other methods
 
 You can count tokens using the model's tokenizer:
 
 ```
 count=model.count_tokens('the quick brown fox jumped over the lazy dog')
 ```
 
-## Model Benchmarks
+# Model Benchmarks
 
 Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
 
@@ -183,14 +204,16 @@
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1'])
 
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 
 models.benchmark(evaluator=gpt4)
 ```
 
+![](./llm_benchmark.png)
+
 ```
 +---------------------------------------+--------------------+---------------------+----------------------+--------------------------+------------------+
 |                 Model                 |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)    |    Evaluation    |
 +---------------------------------------+--------------------+---------------------+----------------------+--------------------------+------------------+
 | AnthropicProvider (claude-instant-v1) |        211         |       0.00104       |         2.85         |          74.04           |        0         |
 | AnthropicProvider (claude-instant-v1) |        204         |       0.00103       |         2.02         |          100.99          |        3         |
 | AnthropicProvider (claude-instant-v1) |        139         |       0.00068       |         1.57         |          88.54           |        3         |
@@ -388,15 +411,15 @@
 
 To evaluate models on your own prompts, simply pass a list of questions and optional answers as tuple. The evaluator will automatically evaluate the responses:
 
 ```
 models.benchmark(prompts=[("what is the capital of finland", "helsinki")], evaluator=gpt4)
 ```
 
-## Supported Models
+# Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
 
 >>> model.list()
@@ -444,11 +467,11 @@
 3. Now you should be able to init Google LLM 
 
 ```
 model = llms.init('chat-bison')
 result = model.complete("hello!")
 ```
 
-## License
+# License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.2.5/README.md` & `pyllms-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 - Connect to top LLMs in a few lines of code
 - Response meta includes tokens processed, cost and latency standardized across the models
 - Multi-model support: Get completions from different models at the same time
 - LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
-## Installation
+# Installation
 
 Install the package using pip:
 
 ```
 pip install pyllms
 ```
 
 
-## Usage
+# Usage
 
 
 ```
 import llms
 
-model = llms.init()
+model = llms.init('gpt-4')
 result = model.complete("what is 5+5")
 
 print(result.text)  
 
 ```
 
 Library will attempt to read the API keys and the default model from environment variables, which you can set like this (for the provider you are using):
@@ -81,14 +81,15 @@
   'tokens_completion': 14, 
   'cost': '0.00007', 
   'latency': 1.4
 }
 ```
 
 
+
 ## Multi-model usage
 
 You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
@@ -130,23 +131,43 @@
 
 Tip: if you are testing this in python3 CLI, run it with -u parameter to disable buffering:
 
 ```
 python3 -u
 ```
 
+## Chat history and system message
+
+You can pass the history of conversation in a list using the following format:
+
+```
+history=[]
+history.append({"role": "user", "content": user_input})
+history.append({"role": "assistant", "content": result.text})  
+
+model.complete(prompt=prompt, history=history)
+
+```
+
+In addition, OpenAI chat models support system message:
+
+```
+model.complete(prompt=prompt, system_message=system, history=history)
+
+```
+
 ## Other methods
 
 You can count tokens using the model's tokenizer:
 
 ```
 count=model.count_tokens('the quick brown fox jumped over the lazy dog')
 ```
 
-## Model Benchmarks
+# Model Benchmarks
 
 Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
 
@@ -157,14 +178,16 @@
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1'])
 
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 
 models.benchmark(evaluator=gpt4)
 ```
 
+![](./llm_benchmark.png)
+
 ```
 +---------------------------------------+--------------------+---------------------+----------------------+--------------------------+------------------+
 |                 Model                 |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)    |    Evaluation    |
 +---------------------------------------+--------------------+---------------------+----------------------+--------------------------+------------------+
 | AnthropicProvider (claude-instant-v1) |        211         |       0.00104       |         2.85         |          74.04           |        0         |
 | AnthropicProvider (claude-instant-v1) |        204         |       0.00103       |         2.02         |          100.99          |        3         |
 | AnthropicProvider (claude-instant-v1) |        139         |       0.00068       |         1.57         |          88.54           |        3         |
@@ -362,15 +385,15 @@
 
 To evaluate models on your own prompts, simply pass a list of questions and optional answers as tuple. The evaluator will automatically evaluate the responses:
 
 ```
 models.benchmark(prompts=[("what is the capital of finland", "helsinki")], evaluator=gpt4)
 ```
 
-## Supported Models
+# Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
 
 >>> model.list()
@@ -418,11 +441,11 @@
 3. Now you should be able to init Google LLM 
 
 ```
 model = llms.init('chat-bison')
 result = model.complete("hello!")
 ```
 
-## License
+# License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.2.5/llms/llms.py` & `pyllms-0.3.0/llms/llms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,146 +1,91 @@
 import asyncio
 import os
 import re
 import statistics
+from dataclasses import dataclass
 from prettytable import PrettyTable
 from .providers import OpenAIProvider
 from .providers import AnthropicProvider
 from .providers import AI21Provider
 from .providers import CohereProvider
 from .providers import AlephAlphaProvider
 from .providers import HuggingfaceHubProvider
 from .providers import GoogleProvider
+from .providers.base_provider import BaseProvider
+from .results.result import AsyncStreamResult, Result, Results, StreamResult
 import concurrent.futures
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Type, Union
 
 
-class Result:
-    def __init__(self, results):
-        self._results = results
-
-    @property
-    def text(self):
-        if isinstance(self._results, list):
-            return [result["text"] for result in self._results]
-        else:
-            return self._results["text"]
-
-    @property
-    def meta(self):
-        if isinstance(self._results, list):
-            return [result["meta"] for result in self._results]
-        else:
-            return self._results["meta"]
+@dataclass
+class Provider:
+    provider: Type[BaseProvider]
+    api_key_name: Optional[str] = None
+    api_key: Optional[str] = None
+    needs_api_key: bool = True
 
 
 class LLMS:
-    def __init__(
-        self,
-        model=None,
-        openai_api_key=None,
-        anthropic_api_key=None,
-        ai21_api_key=None,
-        cohere_api_key=None,
-        alephalpha_api_key=None,
-        huggingfacehub_api_key=None,
-    ):
-        if openai_api_key is None:
-            openai_api_key = os.getenv("OPENAI_API_KEY")
-
-        if anthropic_api_key is None:
-            anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
-
-        if ai21_api_key is None:
-            ai21_api_key = os.getenv("AI21_API_KEY")
-
-        if cohere_api_key is None:
-            cohere_api_key = os.getenv("COHERE_API_KEY")
-
-        if alephalpha_api_key is None:
-            alephalpha_api_key = os.getenv("ALEPHALPHA_API_KEY")
-
-        if huggingfacehub_api_key is None:
-            huggingfacehub_api_key = os.getenv("HUGGINFACEHUB_API_KEY")
-
-        if model is None:
-            model = os.getenv("LLMS_DEFAULT_MODEL")
-            if model is None:
-                model = ["gpt-3.5-turbo"]
-            else:
-                model = [model]
-        elif isinstance(model, str):
-            model = [model]
+    _possible_providers: List[Provider] = [
+        Provider(OpenAIProvider, api_key_name="OPENAI_API_KEY"),
+        Provider(AnthropicProvider, api_key_name="ANTHROPIC_API_KEY"),
+        Provider(AI21Provider, api_key_name="AI21_API_KEY"),
+        Provider(CohereProvider, api_key_name="COHERE_API_KEY"),
+        Provider(AlephAlphaProvider, api_key_name="ALEPHALPHA_API_KEY"),
+        Provider(HuggingfaceHubProvider, api_key_name="HUGGINFACEHUB_API_KEY"),
+        Provider(GoogleProvider, needs_api_key=False),
+    ]
+    _providers: List[BaseProvider] = []
+    _models: List[str] = []
+
+    def __init__(self,
+                 model: Union[str, List[str], None] = None,
+                 **kwargs
+                 ):
+        """Programmatically load api keys and instantiate providers."""
+        for provider in [p for p in self._possible_providers if p.api_key_name]:
+            assert provider.api_key_name  # for static type checking only
+            api_key = None
+            if provider.api_key_name.lower() in kwargs:  # get api key from kwargs
+                api_key = kwargs.pop(provider.api_key_name.lower())
+            elif provider.api_key_name in os.environ:  # otherwise, get it from environment variable
+                api_key = os.getenv(provider.api_key_name)
+            provider.api_key = api_key
+
+        if model is None:  # if no model is specified, use default: from environment variable or gpt-3.5-turbo
+            default_model = os.getenv("LLMS_DEFAULT_MODEL") or "gpt-3.5-turbo"
+            self._models = [default_model]
+        else:
+            self._models = [model] if isinstance(model, str) else model
 
         self._providers = []
-        for single_model in model:
-            if openai_api_key is not None and single_model in OpenAIProvider.MODEL_INFO:
-                self._providers.append(
-                    OpenAIProvider(api_key=openai_api_key, model=single_model)
-                )
-            elif (
-                anthropic_api_key is not None
-                and single_model in AnthropicProvider.MODEL_INFO
-            ):
-                self._providers.append(
-                    AnthropicProvider(api_key=anthropic_api_key, model=single_model)
-                )
-            elif ai21_api_key is not None and single_model in AI21Provider.MODEL_INFO:
-                self._providers.append(
-                    AI21Provider(api_key=ai21_api_key, model=single_model)
-                )
-            elif (
-                cohere_api_key is not None and single_model in CohereProvider.MODEL_INFO
-            ):
-                self._providers.append(
-                    CohereProvider(api_key=cohere_api_key, model=single_model)
-                )
-            elif (
-                alephalpha_api_key is not None
-                and single_model in AlephAlphaProvider.MODEL_INFO
-            ):
-                self._providers.append(
-                    AlephAlphaProvider(api_key=alephalpha_api_key, model=single_model)
-                )
-            elif (
-                huggingfacehub_api_key is not None
-                and single_model in HuggingfaceHubProvider.MODEL_INFO
-            ):
-                self._providers.append(
-                    HuggingfaceHubProvider(
-                        api_key=huggingfacehub_api_key, model=single_model
-                    )
-                )
-            elif single_model in GoogleProvider.MODEL_INFO:
-                self._providers.append(GoogleProvider(model=single_model))
-            else:
-                raise ValueError("Invalid API key and model combination", single_model)
+        for single_model in self._models:
+            for provider in self._possible_providers:
+                if single_model in provider.provider.MODEL_INFO:
+                    print(f"Found {single_model} in {provider.provider.__name__}")
+                    if provider.api_key:
+                        self._providers.append(provider.provider(api_key=provider.api_key, model=single_model))
+                    elif not provider.needs_api_key:
+                        self._providers.append(provider.provider(model=single_model))
+                    else:
+                        raise ValueError("Invalid API key and model combination", single_model)
 
     def __repr__(self) -> str:
-        return f"LLMS({self.model})"
+        return f"LLMS({','.join(self._models)})"
 
     @property
     def n_provider(self):
         return len(self._providers)
 
     def list(self, query=None):
         model_info_list = []
 
-        all_providers = [
-            OpenAIProvider,
-            AI21Provider,
-            AnthropicProvider,
-            CohereProvider,
-            AlephAlphaProvider,
-            HuggingfaceHubProvider,
-            GoogleProvider,
-        ]
-
-        for provider in all_providers:
+        for provider in [p.provider for p in self._possible_providers]:
             for model, cost in provider.MODEL_INFO.items():
                 if query and (
                     (query.lower() not in model.lower())
                     and (query.lower() not in provider.__name__.lower())
                 ):
                     continue
                 model_info = {
@@ -160,62 +105,62 @@
         for provider in self._providers:
             results.append(provider.count_tokens(content))
         if self.n_provider > 1:
             return results
         else:
             return results[0]
 
-    def complete(self, prompt, **kwargs):
+    def complete(self, prompt: str, **kwargs) -> Union[Result, Results]:
         def _generate(provider):
             result = provider.complete(prompt, **kwargs)
             return result
 
         if self.n_provider > 1:
             results = []
             with ThreadPoolExecutor() as executor:
                 futures = {
                     executor.submit(_generate, provider): provider
                     for provider in self._providers
                 }
                 for future in as_completed(futures):
                     results.append(future.result())
 
-            return Result(results)
+            return Results(results)
         else:
-            result = self._providers[0].complete(prompt, **kwargs)
-            return Result(result)
+            return self._providers[0].complete(prompt, **kwargs)
 
     async def acomplete(
         self,
         prompt: str,
         **kwargs,
-    ):
+    ) -> Union[Result, Results]:
         if self.n_provider > 1:
             tasks = [
                 provider.acomplete(prompt, **kwargs) for provider in self._providers
             ]
             results = await asyncio.gather(*tasks, return_exceptions=False)
-            return Result(results)
+            return Results(results)
 
         else:
             provider = self._providers[0]
-            result = await provider.acomplete(prompt, **kwargs)
-            return Result(result)
+            return await provider.acomplete(prompt, **kwargs)
 
-    def complete_stream(self, prompt, **kwargs):
-        if len(self._providers) > 1:
+    def complete_stream(self, prompt, **kwargs) -> StreamResult:
+        if self.n_provider > 1:
             raise ValueError("Streaming is possible only with a single model")
+        return self._providers[0].complete_stream(prompt, **kwargs)
 
-        yield from self._providers[0].complete_stream(prompt, **kwargs)
+    async def acomplete_stream(self, prompt, **kwargs) -> AsyncStreamResult:
+        if self.n_provider > 1:
+            raise ValueError("Streaming is possible only with a single model")
+        return await self._providers[0].acomplete_stream(prompt, **kwargs)
 
     def benchmark(self, problems=None, evaluator=None, show_outputs=False, html=False):
         if not problems:
-          
             problems = [
-               
                 (
                     "A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?",
                     "pull",
                 ),
                 ("Solve the quadratic equation: x^2 - 5x + 6 = 0", "x=2, x=3"),
                 ("How much is 7! * 3! -1234.5 ?", "29005.5"),
                 (
@@ -276,21 +221,51 @@
                 ),
                 (
                     "two workers paint the fence in 8 hours. how long will it take one worker paint the same fence if they are injured and need to take a 30 min break after every hour of work?",
                     "5.5 hours",
                 ),
                 ("5+55+555+5555+55555-1725=", "60000"),
                 ("-2-2-2-2-2-2*-2*-2=", "-18"),
-                ('what is the 13th letter of the word "supralapsarian"', 'a'),
-                ('Vlad\'s uncle can still beat him in sprinting although he is 30 years younger. who is "he" referring to?', 'Vlad'),
-                ("Belgium uses 160 million litres of petrol each day. Three is enough petrol stored to last 60 days. how much more petrol does Belgium need to buy to have enough stored for 90 days. A) 4 million litres, B) 4,8 million litres, C) 480 million litres D) 160 million litres E) 4800 million litres", "E) 4800 million litres"),
-                ("The sum of three numbers is 96. The first number is 6 times the third number, and the third number is 40 less than the second number. What is the absolute value of the difference between the first and second numbers?", "5"),
-                ("The least common multiple of a positive integer n and 18 is 180, and the greatest common divisor of n and 45 is 15. What is the sum of the digits of n?", "n = 60 thus the answer is 6"),
-                ("what square is the black king on in this chess position: 1Bb3BN/R2Pk2r/1Q5B/4q2R/2bN4/4Q1BK/1p6/1bq1R1rb w - - 0 1", "e7")
-
+                ('what is the 13th letter of the word "supralapsarian"', "a"),
+                (
+                    'Vlad\'s uncle can still beat him in sprinting although he is 30 years younger. who is "he" referring to?',
+                    "Vlad",
+                ),
+                (
+                    "Belgium uses 160 million litres of petrol each day. Three is enough petrol stored to last 60 days. how much more petrol does Belgium need to buy to have enough stored for 90 days. A) 4 million litres, B) 4,8 million litres, C) 480 million litres D) 160 million litres E) 4800 million litres",
+                    "E) 4800 million litres",
+                ),
+                (
+                    "The sum of three numbers is 96. The first number is 6 times the third number, and the third number is 40 less than the second number. What is the absolute value of the difference between the first and second numbers?",
+                    "5",
+                ),
+                (
+                    "The least common multiple of a positive integer n and 18 is 180, and the greatest common divisor of n and 45 is 15. What is the sum of the digits of n?",
+                    "n = 60 thus the answer is 6",
+                ),
+                (
+                    "what square is the black king on in this chess position: 1Bb3BN/R2Pk2r/1Q5B/4q2R/2bN4/4Q1BK/1p6/1bq1R1rb w - - 0 1",
+                    "e7",
+                ),
+                (
+                    "is 9677 a prime number?",
+                    "yes",
+                ),
+                ("Current flight information (the following flights are one-way only, and all the flights available are included below):\
+There is a flight from city G to city B\
+There is a flight from city H to city K\
+There is a flight from city L to city M\
+There is a flight from city F to city H\
+There is a flight from city G to city J\
+There is a flight from city B to city I\
+There is a flight from city L to city A\
+There is a flight from city H to city N\
+There is a flight from city B to city D\
+There is a flight from city J to city C\
+Question: Is there a series of flights that goes from city F to city I?", "No"),
             ]
 
         def evaluate_answers(
             evaluator, query_answer_pairs: List[Tuple[str, str]]
         ) -> List[int]:
             system = """
 You are given a problem and answer by a student. Sometimes the correct solution will be provided with the problem as a hint, but if it is not, then first think about the solution yourself, then score the solution of the student's solution with one of these scores:
@@ -302,38 +277,36 @@
 """
             scores = []
             for i, (query, hint, answer) in enumerate(query_answer_pairs, start=1):
                 if not len(hint):
                     prompt = f"Problem: {query}\nStudent solution: {answer}"
                 else:
                     prompt = f"Problem: {query}\nHint (correct answer): {hint}\nStudent solution: {answer}"
-#                print(prompt)
+                #                print(prompt)
                 evaluator_result = evaluator.complete(
                     prompt, system_message=system
                 ).text
-#                print(evaluator_result)
                 found = re.search(r"Score: (\d+)", evaluator_result)
                 if found:
                     scores.append(int(found.group(1)))
                 else:
                     print("No score found!", evaluator_result)
 
-#            print(scores)
             return scores
 
         model_results = {}
 
         def process_prompt(model, prompt, index):
             print(model, index)
             result = model.complete(prompt, max_tokens=1000, temperature=0)
             output_data = {
-                "text": result["text"],
-                "tokens": result["meta"]["tokens"],
-                "latency": result["meta"]["latency"],
-                "cost": result["meta"]["cost"],
+                "text": result.text,
+                "tokens": result.meta["tokens"],
+                "latency": result.meta["latency"],
+                "cost": result.meta["cost"],
                 "prompt_index": index,
             }
             return output_data
 
         def process_prompts_sequentially(model, prompts):
             results = []
             with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
@@ -463,15 +436,15 @@
                     str(model),
                     f"Total Tokens: {total_tokens}",
                     f"Total Cost: {model_data['total_cost']:.5f}",
                     f"Median Latency: {model_data['median_latency']:.2f}",
                     f"Aggregated speed: {total_tokens/model_data['total_latency']:.2f}",
                 ]
             if evaluator:
-                acc=100*total_score/(3*len(model_data["evaluation"]))
+                acc = 100 * total_score / (3 * len(model_data["evaluation"]))
                 row_data.append(f"Accuracy: {acc:.2f}%")
 
             table.add_row(row_data)
 
         if not html:
             return table
         else:
```

### Comparing `pyllms-0.2.5/llms/providers/ai21.py` & `pyllms-0.3.0/llms/providers/ai21.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # llms/providers/ai21.py
 
 import ai21
 
+from ..results.result import Result
 from .base_provider import BaseProvider
 
 
 class AI21Provider(BaseProvider):
     # per million tokens
     MODEL_INFO = {
         "j2-grande-instruct": {"prompt": 10.0, "completion": 10.0, "token_limit": 8192},
@@ -14,60 +15,55 @@
 
     def __init__(self, api_key, model=None):
         ai21.api_key = api_key
         if model is None:
             model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
-    def _prepare_model_input(
+    def _prepare_model_inputs(
         self,
         prompt: str,
         temperature: float = 0,
         max_tokens: int = 300,
         **kwargs,
     ):
         maxTokens = kwargs.pop("maxTokens", max_tokens)
-        model_input = {
+        model_inputs = {
             "prompt": prompt,
             "temperature": temperature,
             "maxTokens": maxTokens,
             **kwargs,
         }
-        return model_input
+        return model_inputs
 
     def complete(
         self,
         prompt: str,
         temperature: float = 0,
         max_tokens: int = 300,
         **kwargs,
-    ):
-        model_input = self._prepare_model_input(
+    ) -> Result:
+        model_inputs = self._prepare_model_inputs(
             prompt=prompt,
             temperature=temperature,
             max_tokens=max_tokens,
             **kwargs,
         )
         with self.track_latency():
-            response = ai21.Completion.execute(model=self.model, **model_input)
+            response = ai21.Completion.execute(model=self.model, **model_inputs)
 
         completion = response.completions[0].data.text.strip()
-        prompt_tokens = len(response.prompt.tokens)
-        completion_tokens = len(response.completions[0].data.tokens)
-        total_tokens = prompt_tokens + completion_tokens
-
-        cost = self.compute_cost(
-            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
-        )
+        tokens_prompt = len(response.prompt.tokens)
+        tokens_completion = len(response.completions[0].data.tokens)
 
-        return {
-            "text": completion,
-            "meta": {
-                "model": self.model,
-                "tokens": total_tokens,
-                "tokens_prompt": prompt_tokens,
-                "tokens_completion": completion_tokens,
-                "cost": cost,
-                "latency": self.latency,
-            },
-            "provider": str(self),
+        meta = {
+            "tokens_prompt": tokens_prompt,
+            "tokens_completion": tokens_completion,
+            "latency": self.latency,
         }
+
+        return Result(
+            text=completion,
+            model_inputs=model_inputs,
+            provider=self,
+            meta=meta,
+        )
```

### Comparing `pyllms-0.2.5/llms/providers/aleph.py` & `pyllms-0.3.0/llms/providers/google.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,99 @@
-# llms/providers/aleph.py
+# we could switch to genai  https://developers.generativeai.google/api/python/google/generativeai
 
-import os
 
-from aleph_alpha_client import AsyncClient, Client, CompletionRequest, Prompt
+from typing import Dict
 
+import vertexai
+from vertexai.preview.language_models import TextGenerationModel, ChatModel
+
+from ..results.result import Result
 from .base_provider import BaseProvider
-import tiktoken
 
-class AlephAlphaProvider(BaseProvider):
+
+class GoogleProvider(BaseProvider):
+    # cost is per million tokens
     MODEL_INFO = {
-        "luminous-base": {"prompt": 6.6, "completion": 7.6, "token_limit": 2048},
-        "luminous-extended": {"prompt": 9.9, "completion": 10.9, "token_limit": 2048},
-        "luminous-supreme": {"prompt": 38.5, "completion": 42.5, "token_limit": 2048},
-        "luminous-supreme-control": {
-            "prompt": 48.5,
-            "completion": 53.6,
-            "token_limit": 2048,
-        },
+        # no support for "textembedding-gecko"
+        "chat-bison": {"prompt": 0.5, "completion": 0.5, "token_limit": 0, "uses_characters": True},
+        "text-bison": {"prompt": 1.0, "completion": 1.0, "token_limit": 0, "uses_characters": True},
     }
-
-    def __init__(self, api_key=None, model=None):
-        if api_key is None:
-            api_key = os.getenv("ALEPHALPHA_API_KEY")
-        self.client = Client(api_key)
-        self.async_client = AsyncClient(api_key)
-
+    
+    def __init__(self, model=None, **kwargs):
         if model is None:
             model = list(self.MODEL_INFO.keys())[0]
-        self.model = model
 
-    def count_tokens(self, content: str):
-        enc = tiktoken.encoding_for_model("gpt-3.5-turbo")
-        return len(enc.encode(content))
+        self.model = model
+        self.client = TextGenerationModel.from_pretrained(model) if model.startswith('text-') \
+            else ChatModel.from_pretrained(model)
+        
+        vertexai.init(**kwargs)
 
-    def _prepare_model_input(
+    def _prepare_model_inputs(
         self,
         prompt: str,
-        temperature: float = 0,
+        temperature: float = 0.01,
         max_tokens: int = 300,
         **kwargs,
-    ) -> CompletionRequest:
-        prompt = Prompt.from_text(prompt)
-        maximum_tokens = kwargs.pop("maximum_tokens", max_tokens)
-
-        model_input = CompletionRequest(
-            prompt=prompt,
-            temperature=temperature,
-            maximum_tokens=maximum_tokens,
+    ) -> Dict:
+        temperature = max(temperature, 0.01)
+        max_output_tokens = kwargs.pop("max_output_tokens", max_tokens)
+        model_inputs = {
+            "prompt": prompt,
+            "temperature": temperature,
+            "max_output_tokens": max_output_tokens,
             **kwargs,
-        )
-        return model_input
+        }
+        return model_inputs
 
     def complete(
         self,
         prompt: str,
-        temperature: float = 0,
+        temperature: float = 0.01,
         max_tokens: int = 300,
+        context: str = None,
+        examples: dict = {},
         **kwargs,
-    ):
-        model_input = self._prepare_model_input(
-            prompt=prompt, temperature=temperature, max_tokens=max_tokens, **kwargs
+    ) -> Result:
+        model_inputs = self._prepare_model_inputs(
+            prompt=prompt,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            **kwargs,
         )
         with self.track_latency():
-            response = self.client.complete(request=model_input, model=self.model)
-
-        completion = response.completions[0].completion.strip()
+            if isinstance(self.client, ChatModel):
+                chat = self.client.start_chat(context=context, examples=examples)
+                response = chat.send_message(prompt, **model_inputs)
+            elif isinstance(self.client, TextGenerationModel):
+                response = self.client.predict(prompt=prompt, **model_inputs)
+        
+        completion = response.text
 
         # Calculate tokens and cost
-        prompt_tokens = self.count_tokens(prompt)
-        completion_tokens = self.count_tokens(completion)
-
-        total_tokens = prompt_tokens + completion_tokens
-
-        cost = self.compute_cost(
-            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
-        )
-
-        return {
-            "text": completion,
-            "meta": {
-                "model": self.model,
-                "tokens": total_tokens,
-                "tokens_prompt": prompt_tokens,
-                "tokens_completion": completion_tokens,
-                "cost": cost,
-                "latency": self.latency,
-            },
-            "provider": str(self),
-        }
-
-    async def acomplete(
-        self,
-        prompt: str,
-        temperature: float = 0,
-        max_tokens: int = 300,
-        **kwargs,
-    ):
-        model_input = self._prepare_model_input(
-            prompt=prompt, temperature=temperature, max_tokens=max_tokens, **kwargs
-        )
-        with self.track_latency() as latency:
-            async with self.async_client as client:
-                response = await client.complete(request=model_input, model=self.model)
-
-        completion = response.completions[0].completion.strip()
+        prompt_tokens = len(prompt)
+        completion_tokens = len(completion)
 
-        # Calculate tokens and cost
-        prompt_tokens = -1
-        completion_tokens = -1
+        cost_per_token = self.MODEL_INFO[self.model]
+        cost = (
+            (prompt_tokens * cost_per_token["prompt"])
+            + (completion_tokens * cost_per_token["completion"])
+        ) / 1_000_000
 
+        prompt_tokens = prompt_tokens / 4
+        completion_tokens = completion_tokens / 4
         total_tokens = prompt_tokens + completion_tokens
 
-        cost = self.compute_cost(
-            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
-        )
-
-        return {
-            "text": completion,
-            "meta": {
-                "model": self.model,
-                "tokens": total_tokens,
-                "tokens_prompt": prompt_tokens,
-                "tokens_completion": completion_tokens,
-                "cost": cost,
-                "latency": latency,
-            },
-            "provider": str(self),
+        meta = {
+            "model": self.model,
+            "tokens": total_tokens,
+            "tokens_prompt": prompt_tokens,
+            "tokens_completion": completion_tokens,
+            "cost": cost,
+            "latency": self.latency,
         }
+        return Result(
+            text=completion,
+            model_inputs=model_inputs,
+            provider=self,
+            meta=meta,
+        )
```

### Comparing `pyllms-0.2.5/llms/providers/anthropic.py` & `pyllms-0.3.0/llms/providers/anthropic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,64 @@
 # llms/providers/anthropic.py
 
-import json
 import os
-import aiohttp
+from typing import AsyncGenerator, Dict, Generator, List, Optional
+
 import anthropic
 
-from typing import Dict, List, Optional, Tuple, Union
-from anthropic.api import _process_request_error
+from ..results.result import AsyncStreamResult, Result, StreamResult
 from .base_provider import BaseProvider
 
 
-class AnthropicClient(anthropic.Client):
-    """Extend Anthropic Client class to accept aiosession"""
-
-    async def _arequest_as_json(
-        self,
-        method: str,
-        path: str,
-        headers: Optional[Dict[str, str]] = None,
-        request_timeout: Optional[Union[float, Tuple[float, float]]] = None,
-        aiosession: Optional[aiohttp.ClientSession] = None,
-        **params: dict,
-    ) -> dict:
-        if aiosession is None:
-            return await super()._arequest_as_json(
-                method=method,
-                path=path,
-                params=params,
-                headers=headers,
-                request_timeout=request_timeout,
-            )
-        else:
-            request = self._request_params(
-                headers, method, params, path, request_timeout
-            )
-            async with aiosession.request(
-                request.method,
-                request.url,
-                headers=request.headers,
-                data=request.data,
-                timeout=request.timeout,
-            ) as result:
-                content = await result.text()
-                if result.status != 200:
-                    _process_request_error(method, content, result.status)
-                json_body = json.loads(content)
-                return json_body
-
-    async def acompletion(self, **kwargs):
-        # Override original method which pass kwargs as params.
-        # We will pass kwargs in
-        # _arequest_as_json will strips-off the keyword arguments that it needs
-        # and pass the rest as params
-        return await self._arequest_as_json("post", "/v1/complete", **kwargs)
-
-
 class AnthropicProvider(BaseProvider):
     MODEL_INFO = {
         "claude-instant-v1.1": {
             "prompt": 1.63,
             "completion": 5.51,
             "token_limit": 9000,
         },
         "claude-instant-v1": {"prompt": 1.63, "completion": 5.51, "token_limit": 9000},
         "claude-v1": {"prompt": 11.02, "completion": 32.68, "token_limit": 9000},
-        "claude-v1-100k": {"prompt": 11.02, "completion": 32.68, "token_limit": 100000},
+        "claude-v1-100k": {
+            "prompt": 11.02,
+            "completion": 32.68,
+            "token_limit": 100_000,
+        },
+        "claude-instant-1": {
+            "prompt": 1.63,
+            "completion": 5.51,
+            "token_limit": 100_000,
+        },
+        "claude-2": {"prompt": 11.02, "completion": 32.68, "token_limit": 100_000},
     }
 
-    def __init__(self, api_key=None, model=None):
+    def __init__(self, api_key: Optional[str] = None, model: Optional[str] = None):
         if model is None:
             model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
         if api_key is None:
             api_key = os.getenv("ANTHROPIC_API_KEY")
-        self.client = AnthropicClient(api_key)
+        self.client = anthropic.Anthropic(api_key=api_key)
+        self.async_client = anthropic.AsyncAnthropic(api_key=api_key)
 
-    def count_tokens(self, content: str):
-        return anthropic.count_tokens(content)
+    def count_tokens(self, content: str) -> int:
+        return self.client.count_tokens(content)
 
-    def _prepare_model_input(
+    def _prepare_model_inputs(
         self,
         prompt: str,
         history: Optional[List[dict]] = None,
         temperature: float = 0,
         max_tokens: int = 300,
         stop_sequences: Optional[List[str]] = None,
         ai_prompt: str = "",
         stream: bool = False,
         **kwargs,
-    ):
+    ) -> Dict:
         formatted_prompt = (
             f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}{ai_prompt}"
         )
 
         if history is not None:
             history_text_list = []
             for message in history:
@@ -114,77 +79,63 @@
             history_prompt = "".join(history_text_list)
             formatted_prompt = f"{history_prompt}{formatted_prompt}"
 
         max_tokens_to_sample = kwargs.pop("max_tokens_to_sample", max_tokens)
 
         if stop_sequences is None:
             stop_sequences = [anthropic.HUMAN_PROMPT]
-        model_input = {
+        model_inputs = {
             "prompt": formatted_prompt,
             "temperature": temperature,
             "max_tokens_to_sample": max_tokens_to_sample,
             "stop_sequences": stop_sequences,
             "stream": stream,
             **kwargs,
         }
-        return model_input
+        return model_inputs
 
     def complete(
         self,
         prompt: str,
         history: Optional[List[dict]] = None,
         temperature: float = 0,
         max_tokens: int = 300,
         stop_sequences: Optional[List[str]] = None,
         ai_prompt: str = "",
         **kwargs,
-    ):
+    ) -> Result:
         """
         Args:
             history: messages in OpenAI format,
               each dict must include role and content key.
             ai_prompt: prefix of AI response, for finer control on the output.
         """
 
-        model_input = self._prepare_model_input(
+        model_inputs = self._prepare_model_inputs(
             prompt=prompt,
             history=history,
             temperature=temperature,
             max_tokens=max_tokens,
             stop_sequences=stop_sequences,
             ai_prompt=ai_prompt,
             **kwargs,
         )
 
         with self.track_latency():
-            response = self.client.completion(model=self.model, **model_input)
+            response = self.client.completions.create(model=self.model, **model_inputs)
 
-        completion = response["completion"].strip()
+        completion = response.completion.strip()
 
-        # Calculate tokens and cost
-        prompt_tokens = anthropic.count_tokens(model_input["prompt"])
-        completion_tokens = anthropic.count_tokens(response["completion"])
-        total_tokens = prompt_tokens + completion_tokens
-        cost = self.compute_cost(
-            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        return Result(
+            text=completion,
+            model_inputs=model_inputs,
+            provider=self,
+            meta={"latency": self.latency},
         )
 
-        return {
-            "text": completion,
-            "meta": {
-                "model": self.model,
-                "tokens": total_tokens,
-                "tokens_prompt": prompt_tokens,
-                "tokens_completion": completion_tokens,
-                "cost": cost,
-                "latency": self.latency,
-            },
-            "provider": str(self),
-        }
-
     async def acomplete(
         self,
         prompt: str,
         history: Optional[List[dict]] = None,
         temperature: float = 0,
         max_tokens: int = 300,
         stop_sequences: Optional[List[str]] = None,
@@ -193,78 +144,110 @@
     ):
         """
         Args:
             history: messages in OpenAI format,
               each dict must include role and content key.
             ai_prompt: prefix of AI response, for finer control on the output.
         """
-        model_input = self._prepare_model_input(
+        model_inputs = self._prepare_model_inputs(
             prompt=prompt,
             history=history,
             temperature=temperature,
             max_tokens=max_tokens,
             stop_sequences=stop_sequences,
             ai_prompt=ai_prompt,
             **kwargs,
         )
         with self.track_latency():
-            response = await self.client.acompletion(model=self.model, **model_input)
-        completion = response["completion"].strip()
-
-        # Calculate tokens and cost
-        prompt_tokens = anthropic.count_tokens(model_input["prompt"])
-        completion_tokens = anthropic.count_tokens(response["completion"])
-        total_tokens = prompt_tokens + completion_tokens
+            response = await self.async_client.completions.create(
+                model=self.model, **model_inputs
+            )
+        completion = response.completion.strip()
 
-        cost = self.compute_cost(
-            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        return Result(
+            text=completion,
+            model_inputs=model_inputs,
+            provider=self,
+            meta={"latency": self.latency},
         )
-        return {
-            "text": completion,
-            "meta": {
-                "model": self.model,
-                "tokens": total_tokens,
-                "tokens_prompt": prompt_tokens,
-                "tokens_completion": completion_tokens,
-                "cost": cost,
-                "latency": self.latency,
-            },
-            "provider": str(self),
-        }
 
     def complete_stream(
         self,
         prompt: str,
         history: Optional[List[dict]] = None,
         temperature: float = 0,
         max_tokens: int = 300,
         stop_sequences: Optional[List[str]] = None,
         ai_prompt: str = "",
         **kwargs,
-    ):
+    ) -> StreamResult:
         """
         Args:
             history: messages in OpenAI format,
               each dict must include role and content key.
             ai_prompt: prefix of AI response, for finer control on the output.
         """
-        model_input = self._prepare_model_input(
+        model_inputs = self._prepare_model_inputs(
             prompt=prompt,
             history=history,
             temperature=temperature,
             max_tokens=max_tokens,
             stop_sequences=stop_sequences,
             ai_prompt=ai_prompt,
             stream=True,
             **kwargs,
         )
+        response = self.client.completions.create(model=self.model, **model_inputs)
+        stream = self._process_stream(response)
 
-        response = self.client.completion_stream(model=self.model, **model_input)
+        return StreamResult(stream=stream, model_inputs=model_inputs, provider=self)
 
-        first_completion = next(response)["completion"]
+    def _process_stream(self, response: Generator) -> Generator:
+        first_completion = next(response).completion
         yield first_completion.lstrip()
 
-        last_completion = first_completion
         for data in response:
-            new_chunk = data["completion"][len(last_completion) :]
-            last_completion = data["completion"]
-            yield (new_chunk)
+            yield data.completion
+
+    async def acomplete_stream(
+        self,
+        prompt: str,
+        history: Optional[List[dict]] = None,
+        temperature: float = 0,
+        max_tokens: int = 300,
+        stop_sequences: Optional[List[str]] = None,
+        ai_prompt: str = "",
+        **kwargs,
+    ) -> AsyncStreamResult:
+        """
+        Args:
+            history: messages in OpenAI format,
+              each dict must include role and content key.
+            ai_prompt: prefix of AI response, for finer control on the output.
+        """
+        model_inputs = self._prepare_model_inputs(
+            prompt=prompt,
+            history=history,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            stop_sequences=stop_sequences,
+            ai_prompt=ai_prompt,
+            stream=True,
+            **kwargs,
+        )
+
+        response = await self.async_client.completions.create(
+            model=self.model, **model_inputs
+        )
+
+        stream = self._aprocess_stream(response)
+
+        return AsyncStreamResult(
+            stream=stream, model_inputs=model_inputs, provider=self
+        )
+
+    async def _aprocess_stream(self, response: AsyncGenerator) -> AsyncGenerator:
+        first_completion = (await response.__anext__()).completion
+        yield first_completion.lstrip()
+
+        async for data in response:
+            yield data.completion
```

### Comparing `pyllms-0.2.5/llms/providers/base_provider.py` & `pyllms-0.3.0/llms/providers/base_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 
 
 class BaseProvider:
     """Base class for all providers.
     Methods will raise NotImplementedError if they are not overwritten.
     """
 
-    def __init__(self):
+    MODEL_INFO = {}
+
+    def __init__(self, model=None, api_key=None, **kwargs):
         self.latency = None
+        # to be overwritten by subclasses
+        self.api_key = api_key
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__} ({self.model})"
+        return f"{self.__class__.__name__}('{self.model}')"
 
     def __str__(self):
-        return f"{self.__class__.__name__} ({self.model})"
+        return f"{self.__class__.__name__}('{self.model}')"
 
     @contextmanager
     def track_latency(self):
         start = time.perf_counter()
         try:
             yield
         finally:
```

### Comparing `pyllms-0.2.5/llms/providers/google.py` & `pyllms-0.3.0/llms/providers/huggingface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,95 +1,126 @@
-# we could switch to genai  https://developers.generativeai.google/api/python/google/generativeai
+# llms/providers/huggingface.py
 
+import os
 
-import vertexai
-from vertexai.preview.language_models import ChatModel
-
-from typing import List, Optional
-
+from huggingface_hub.inference_api import InferenceApi
 
+from ..results.result import Result
 from .base_provider import BaseProvider
 
-class GoogleProvider(BaseProvider):
-    # cost is per million tokens
+
+class HuggingfaceHubProvider(BaseProvider):
     MODEL_INFO = {
-        "chat-bison": {
-            "prompt": 0.5,
-            "completion": 0.5,
-            "token_limit": 0,
-            "uses_characters": True,
+        "hf_pythia": {
+            "full": "OpenAssistant/oasst-sft-4-pythia-12b-epoch-3.5",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": 2048,
+        },
+         "hf_falcon40b": {
+            "full": "tiiuae/falcon-40b-instruct",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": 2048,
+            "local": True
+        },
+        "hf_falcon7b": {         
+            "full": "tiiuae/falcon-7b-instruct",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": 2048,
+            "local": True
+        },
+        "hf_mptinstruct": {
+            "full": "mosaicml/mpt-7b-instruct",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": 2048,
+            "local": True
+        },
+        "hf_mptchat": {
+            "full": "mosaicml/mpt-7b-chat",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": 2048,
+           "local": True
+        },
+        "hf_llava": {
+            "full": "liuhaotian/LLaVA-Lightning-MPT-7B-preview",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": 2048,
+            "local": True
+        },
+        "hf_dolly": {
+            "full": "databricks/dolly-v2-12b",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": -1,
+            "local": True
+        },
+        "hf_vicuna": {
+            "full": "CarperAI/stable-vicuna-13b-delta",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": -1,
         },
     }
 
-    def __init__(self, model=None):
+    def __init__(self, api_key=None, model=None):
         if model is None:
             model = list(self.MODEL_INFO.keys())[0]
 
         self.model = model
 
-        self.client = ChatModel.from_pretrained(model)
+        if api_key is None:
+            api_key = os.getenv("HUGGINFACEHUB_API_KEY")
 
-        vertexai.init()
+        self.client = InferenceApi(
+            repo_id=self.MODEL_INFO[model]["full"], token=api_key
+        )
 
-    def _prepare_model_input(
+    def _prepare_model_inputs(
         self,
         prompt: str,
-        temperature: float = 0.01,
+        temperature: float = 1.0,
         max_tokens: int = 300,
         **kwargs,
     ):
-        temperature = max(temperature, 0.01)
-        max_output_tokens = kwargs.pop("max_output_tokens", max_tokens)
+        if self.model == "hf_pythia":
+            prompt = "<|prompter|" + prompt + "<|endoftext|><|assistant|>"
+        max_new_tokens = kwargs.pop("max_length", max_tokens)
         params = {
             "temperature": temperature,
-            "max_output_tokens": max_output_tokens,
+            "max_length": max_new_tokens,
             **kwargs,
         }
         return prompt, params
 
     def complete(
         self,
         prompt: str,
         temperature: float = 0.01,
         max_tokens: int = 300,
-        context: str = None,
-        examples: dict = {},
         **kwargs,
-    ):
-        prompt, params = self._prepare_model_input(
+    ) -> Result:
+        prompt, params = self._prepare_model_inputs(
             prompt=prompt,
             temperature=temperature,
             max_tokens=max_tokens,
             **kwargs,
         )
         with self.track_latency():
-            chat = self.client.start_chat(context=context, examples=examples)
-            response = chat.send_message(prompt, **params)
-
-        completion = response.text
+            response = self.client(inputs=prompt, params=params)
 
-        # Calculate tokens and cost
-        prompt_tokens = len(prompt)
-        completion_tokens = len(completion)
-
-        cost_per_token = self.MODEL_INFO[self.model]
-        cost = (
-            (prompt_tokens * cost_per_token["prompt"])
-            + (completion_tokens * cost_per_token["completion"])
-        ) / 1_000_000
-
-        prompt_tokens = prompt_tokens / 4
-        completion_tokens = completion_tokens / 4
-        total_tokens = prompt_tokens + completion_tokens
-
-        return {
-            "text": completion,
-            "meta": {
-                "model": self.model,
-                "tokens": total_tokens,
-                "tokens_prompt": prompt_tokens,
-                "tokens_completion": completion_tokens,
-                "cost": cost,
-                "latency": self.latency,
-            },
-            "provider": str(self),
+        completion = response[0]["generated_text"][len(prompt) :]
+        meta = {
+            "tokens_prompt": -1,
+            "tokens_completion": -1,
+            "latency": self.latency,
         }
+        return Result(
+            text=completion,
+            model_inputs={"prompt": prompt, **params},
+            provider=self,
+            meta=meta,
+        )
```

### Comparing `pyllms-0.2.5/pyllms.egg-info/PKG-INFO` & `pyllms-0.3.0/pyllms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.2.5
+Version: 0.3.0
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, Google Palm2/Vertex, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub,vertex ai,palm,palm2
@@ -35,30 +35,30 @@
 - Connect to top LLMs in a few lines of code
 - Response meta includes tokens processed, cost and latency standardized across the models
 - Multi-model support: Get completions from different models at the same time
 - LLM benchmark: Evaluate models on quality, speed and cost
 
 Feel free to reuse and expand. Pull requests are welcome.
 
-## Installation
+# Installation
 
 Install the package using pip:
 
 ```
 pip install pyllms
 ```
 
 
-## Usage
+# Usage
 
 
 ```
 import llms
 
-model = llms.init()
+model = llms.init('gpt-4')
 result = model.complete("what is 5+5")
 
 print(result.text)  
 
 ```
 
 Library will attempt to read the API keys and the default model from environment variables, which you can set like this (for the provider you are using):
@@ -107,14 +107,15 @@
   'tokens_completion': 14, 
   'cost': '0.00007', 
   'latency': 1.4
 }
 ```
 
 
+
 ## Multi-model usage
 
 You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
@@ -156,23 +157,43 @@
 
 Tip: if you are testing this in python3 CLI, run it with -u parameter to disable buffering:
 
 ```
 python3 -u
 ```
 
+## Chat history and system message
+
+You can pass the history of conversation in a list using the following format:
+
+```
+history=[]
+history.append({"role": "user", "content": user_input})
+history.append({"role": "assistant", "content": result.text})  
+
+model.complete(prompt=prompt, history=history)
+
+```
+
+In addition, OpenAI chat models support system message:
+
+```
+model.complete(prompt=prompt, system_message=system, history=history)
+
+```
+
 ## Other methods
 
 You can count tokens using the model's tokenizer:
 
 ```
 count=model.count_tokens('the quick brown fox jumped over the lazy dog')
 ```
 
-## Model Benchmarks
+# Model Benchmarks
 
 Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
 
@@ -183,14 +204,16 @@
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1'])
 
 gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 
 models.benchmark(evaluator=gpt4)
 ```
 
+![](./llm_benchmark.png)
+
 ```
 +---------------------------------------+--------------------+---------------------+----------------------+--------------------------+------------------+
 |                 Model                 |       Tokens       |       Cost ($)      |     Latency (s)      |    Speed (tokens/sec)    |    Evaluation    |
 +---------------------------------------+--------------------+---------------------+----------------------+--------------------------+------------------+
 | AnthropicProvider (claude-instant-v1) |        211         |       0.00104       |         2.85         |          74.04           |        0         |
 | AnthropicProvider (claude-instant-v1) |        204         |       0.00103       |         2.02         |          100.99          |        3         |
 | AnthropicProvider (claude-instant-v1) |        139         |       0.00068       |         1.57         |          88.54           |        3         |
@@ -388,15 +411,15 @@
 
 To evaluate models on your own prompts, simply pass a list of questions and optional answers as tuple. The evaluator will automatically evaluate the responses:
 
 ```
 models.benchmark(prompts=[("what is the capital of finland", "helsinki")], evaluator=gpt4)
 ```
 
-## Supported Models
+# Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
 
 >>> model.list()
@@ -444,11 +467,11 @@
 3. Now you should be able to init Google LLM 
 
 ```
 model = llms.init('chat-bison')
 result = model.complete("hello!")
 ```
 
-## License
+# License
 
 This project is licensed under the MIT License.
```

### Comparing `pyllms-0.2.5/setup.py` & `pyllms-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,34 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.2.5",
+    version="0.3.0",
     description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, Google Palm2/Vertex, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
         "openai",
         "tiktoken",
-        "anthropic",
+        "anthropic==0.3.5",
         "ai21",
         "cohere",
         "aleph-alpha-client",
         "huggingface_hub",
         "google-cloud-aiplatform",
         "prettytable",
+        "einops",
+        "accelerate"
+
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

