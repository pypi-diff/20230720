# Comparing `tmp/litechain-0.1.3.tar.gz` & `tmp/litechain-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litechain-0.1.3.tar", last modified: Wed Jul 19 10:02:44 2023, max compression
+gzip compressed data, was "litechain-0.1.4.tar", last modified: Thu Jul 20 20:03:42 2023, max compression
```

## Comparing `litechain-0.1.3.tar` & `litechain-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 10:02:32.000000 litechain-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 10:02:32.000000 litechain-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-19 10:02:44.139620 litechain-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-07-19 10:02:32.000000 litechain-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/contrib/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/contrib/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/contrib/llms/gpt4all_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/contrib/llms/open_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/core/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/utils/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/utils/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-19 10:02:32.000000 litechain-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 10:02:44.139620 litechain-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-19 10:02:32.000000 litechain-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:32.000000 litechain-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 20:03:30.000000 litechain-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 20:03:30.000000 litechain-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-20 20:03:42.057260 litechain-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-20 20:03:30.000000 litechain-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.053260 litechain-0.1.4/litechain/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/litechain/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/litechain/contrib/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/contrib/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/contrib/llms/gpt4all_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/contrib/llms/open_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/litechain/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/core/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/litechain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/utils/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/utils/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.053260 litechain-0.1.4/litechain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 20:03:30.000000 litechain-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:03:42.057260 litechain-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-20 20:03:30.000000 litechain-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:30.000000 litechain-0.1.4/tests/__init__.py
```

### Comparing `litechain-0.1.3/LICENSE` & `litechain-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `litechain-0.1.3/PKG-INFO` & `litechain-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.3
+Version: 0.1.4
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
@@ -147,15 +147,14 @@
 [![Join our Discord community](https://img.shields.io/badge/Join-Discord-7289DA.svg)](https://discord.gg/AmEMWmFG)
 
 # 🚙 Roadmap
 
 - [ ] Add an example for document retrieval using vector search
 - [ ] Add a `filter` function
 - [ ] Add docs for debugging
-- [ ] Add default error handling
 - [ ] Add a simple default memory mechanism
 
 # 🙋 Contributing
 
 As a very new project in a rapidly developing field LiteChain is extremely open to contributions, we need a lot of help with integrations, documentation and guides content, feel free to send MRs and open issues. The project is very easy to run (check out the Makefile, it's all you need), but more complete contibuting guidelines to be written (we need help with that too!)
 
 If you want to help me pay the bills and keep developing this project, you can:
```

### Comparing `litechain-0.1.3/README.md` & `litechain-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
 [![Join our Discord community](https://img.shields.io/badge/Join-Discord-7289DA.svg)](https://discord.gg/AmEMWmFG)
 
 # 🚙 Roadmap
 
 - [ ] Add an example for document retrieval using vector search
 - [ ] Add a `filter` function
 - [ ] Add docs for debugging
-- [ ] Add default error handling
 - [ ] Add a simple default memory mechanism
 
 # 🙋 Contributing
 
 As a very new project in a rapidly developing field LiteChain is extremely open to contributions, we need a lot of help with integrations, documentation and guides content, feel free to send MRs and open issues. The project is very easy to run (check out the Makefile, it's all you need), but more complete contibuting guidelines to be written (we need help with that too!)
 
 If you want to help me pay the bills and keep developing this project, you can:
```

### Comparing `litechain-0.1.3/litechain/__init__.py` & `litechain-0.1.4/litechain/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.3/litechain/contrib/__init__.py` & `litechain-0.1.4/litechain/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.3/litechain/contrib/llms/gpt4all_chain.py` & `litechain-0.1.4/litechain/contrib/llms/gpt4all_chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.3/litechain/contrib/llms/open_ai.py` & `litechain-0.1.4/litechain/contrib/llms/open_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,16 +240,16 @@
     ...                         },
     ...                         "format": {
     ...                             "description": "A string with the full content of what the given role said",
     ...                             "type": "string",
     ...                             "enum": ("celsius", "fahrenheit"),
     ...                         },
     ...                     },
+    ...                     "required": ["location"],
     ...                 },
-    ...                 "required": ["location"],
     ...             }
     ...         ],
     ...         temperature=0,
     ...     ).map(
     ...         lambda delta: get_current_weather(**json.loads(delta.content))
     ...         if delta.role == "function" and delta.name == "get_current_weather"
     ...         else delta
@@ -275,15 +275,15 @@
         temperature: Optional[float] = 0,
         max_tokens: Optional[int] = None,
     ) -> None:
         self.name = name
 
         async def chat_completion(
             messages: List[OpenAIChatMessage],
-        ) -> AsyncGenerator[ChainOutput[Union[OpenAIChatDelta, V], Any], Any]:
+        ) -> AsyncGenerator[ChainOutput[Union[OpenAIChatDelta, V]], Any]:
             loop = asyncio.get_event_loop()
 
             def get_completions():
                 function_kwargs = {}
                 if functions is not None:
                     function_kwargs["functions"] = functions
                 if function_call is not None:
```

### Comparing `litechain-0.1.3/litechain/core/chain.py` & `litechain-0.1.4/litechain/core/chain.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,29 +23,30 @@
 U = TypeVar("U")
 V = TypeVar("V")
 W = TypeVar("W")
 X = TypeVar("X")
 
 
 @dataclass
-class ChainOutput(Generic[T, V]):
+class ChainOutput(Generic[T]):
     """
     ChainOutput is a data class that represents the output of a Chain at each step.
 
     Attributes
     ----------
     chain : str
         The name of the chain that produced this output. This helps in identifying
         which part of the processing pipeline the output is coming from.
 
-    output : V
-        The actual output data produced by the Chain. This can be of any type produced by any step of the whole Chain.
+    output : Union[T, Any]
+        The actual output data produced by the chain. This will be type T for final chain output,
+        but can be also be of any type produced by any step of the whole chain.
 
     final : bool
-        A boolean flag indicating whether this output is the final output of the Chain.
+        A boolean flag indicating whether this output is the final output of the chain.
         Only the outputs at the end of the chain are marked as "final".
 
     Example
     -------
 
     >>> from litechain import Chain
     >>> import asyncio
@@ -60,74 +61,70 @@
     ...
     >>> asyncio.run(example())
     ChainOutput(chain='GreetingChain', data='Hello, Alice!', final=False)
     ChainOutput(chain='GreetingChain@map', data='Hello, Alice! How are you?', final=True)
     """
 
     chain: str
-    data: V
+    data: Union[T, Any]
     final: bool
 
 
 class Chain(Generic[T, U]):
     """"""
 
     _call: Callable[
-        [T], Union[AsyncGenerator[ChainOutput[U, Any], Any], AsyncGenerator[U, Any], U]
+        [T], Union[AsyncGenerator[ChainOutput[U], Any], AsyncGenerator[U, Any], U]
     ]
 
     def __init__(
         self,
         name: str,
         call: Callable[
             [T],
-            Union[AsyncGenerator[ChainOutput[U, W], Any], AsyncGenerator[U, Any], U],
+            Union[AsyncGenerator[ChainOutput[U], Any], AsyncGenerator[U, Any], U],
         ],
     ) -> None:
         self.name = name
         self._call = call
 
-    def __call__(self, input: T) -> AsyncGenerator[ChainOutput[U, Union[U, Any]], Any]:
+    def __call__(self, input: T) -> AsyncGenerator[ChainOutput[U], Any]:
         result = self._call(input)
         return self._wrap(result)
 
     def _wrap(
         self,
-        value: Union[AsyncGenerator[ChainOutput[V, W], Any], AsyncGenerator[V, Any], V],
+        value: Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
         name: Optional[str] = None,
-    ) -> AsyncGenerator[ChainOutput[V, Union[V, W]], Any]:
+    ) -> AsyncGenerator[ChainOutput[V], Any]:
         async def _wrap(
-            values: Union[
-                AsyncGenerator[ChainOutput[V, W], Any], AsyncGenerator[V, Any]
-            ],
-        ) -> AsyncGenerator[ChainOutput[V, Union[V, W]], Any]:
+            values: Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any]],
+        ) -> AsyncGenerator[ChainOutput[V], Any]:
             async for value in values:
                 yield self._output_wrap(value, name=name)
 
         if isinstance(value, AsyncGenerator):
             return _wrap(value)
         return _wrap(as_async_generator(value))
 
     def _output_wrap(
-        self, value: Union[ChainOutput[V, W], V], final=None, name=None
-    ) -> ChainOutput[V, Union[V, W]]:
+        self, value: Union[ChainOutput[V], V], final=None, name=None
+    ) -> ChainOutput[V]:
         if isinstance(value, ChainOutput):
             final = final if final is not None else value.final
-            return ChainOutput[V, Union[V, W]](
-                chain=value.chain, data=value.data, final=final
-            )
+            return ChainOutput[V](chain=value.chain, data=value.data, final=final)
 
         final = final if final is not None else True
-        return ChainOutput[V, Union[V, W]](
+        return ChainOutput[V](
             chain=self.name if name is None else name, data=value, final=final
         )
 
     async def _reyield(
-        self, async_iterable: AsyncGenerator[ChainOutput[U, U], Any]
-    ) -> AsyncGenerator[Tuple[List[U], ChainOutput[U, U]], Any]:
+        self, async_iterable: AsyncGenerator[ChainOutput[U], Any]
+    ) -> AsyncGenerator[Tuple[List[U], ChainOutput[U]], Any]:
         values: List[U] = []
         async for u in async_iterable:
             u_rewrapped = self._output_wrap(u, final=False)
             if u.final:
                 values.append(u.data)
             yield (values, u_rewrapped)
 
@@ -163,30 +160,32 @@
         ...     accronym_chain = words_chain.map(lambda word: word.upper()[0]) # uppercases each word and take the first letter
         ...     return await join_final_output(accronym_chain("as soon as possible"))
         ...
         >>> asyncio.run(example())
         'ASAP'
         """
 
-        async def map(input: T) -> AsyncGenerator[ChainOutput[V, Union[U, V]], Any]:
+        next_name = f"{self.name}@map"
+
+        async def map(input: T) -> AsyncGenerator[ChainOutput[V], Any]:
             # Reyield previous chain so we never block the stream, and at the same time yield mapped values
             prev_len_values = 0
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[V, Union[U, V]], to_reyield)
+                yield cast(ChainOutput[V], to_reyield)
                 if len(values) > prev_len_values:  # as soon as there is a new value
                     prev_len_values = len(values)
-                    yield cast(ChainOutput[V, Union[U, V]], fn(values[-1]))
+                    yield self._output_wrap(fn(values[-1]), name=next_name)
 
-        return Chain[T, V](f"{self.name}@map", lambda input: map(input))
+        return Chain[T, V](next_name, lambda input: map(input))
 
     def and_then(
         self,
         next: Callable[
             [Iterable[U]],
-            Union[AsyncGenerator[ChainOutput[V, W], Any], AsyncGenerator[V, Any], V],
+            Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
         ],
     ) -> "Chain[T, V]":
         """
         Processes the output of the current chain through a transformation function or another chain.
 
         Unlike the map method, which applies transformations to outputs as they arrive,
         the and_then method first collects all the outputs and then passes them to the transformation function or the next chain.
@@ -227,25 +226,25 @@
 
         next_name = f"{self.name}@and_then"
         if hasattr(next, "name"):
             next_name = next.name
 
         async def and_then(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[V, Union[U, V]], Any]:
+        ) -> AsyncGenerator[ChainOutput[V], Any]:
             # First, reyield previous chain so we never block the stream, and collect the results until they are done
             iter_u: Iterable[U] = []
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[V, Union[U, V]], to_reyield)
+                yield cast(ChainOutput[V], to_reyield)
                 iter_u = values
 
             # Then, call in the next chain
             iter_v = self._wrap(next(iter_u), name=next_name)
             async for v in iter_v:
-                yield cast(ChainOutput[V, Union[U, V]], v)
+                yield v
 
         return Chain[T, V](next_name, and_then)
 
     def collect(self: "Chain[T, U]") -> "SingleOutputChain[T, List[U]]":
         """
         Collects all the outputs produced by the chain and returns them as a list.
 
@@ -263,27 +262,29 @@
         ...     ).collect()
         ...     return await collect_final_output(word_chain("Hi"))
         ...
         >>> asyncio.run(example())
         [['Hi', '!']]
         """
 
+        next_name = f"{self.name}@collect"
+
         async def _collect(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[List[U], Union[U, List[U]]], Any]:
+        ) -> AsyncGenerator[ChainOutput[List[U]], Any]:
             # First, reyield previous chain so we never block the stream, and collect the results until they are done
             iter_u: Iterable[U] = []
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[List[U], Union[U, List[U]]], to_reyield)
+                yield cast(ChainOutput[List[U]], to_reyield)
                 iter_u = values
 
             # Then, yield the collected results
-            yield cast(ChainOutput[List[U], Union[U, List[U]]], iter_u)
+            yield self._output_wrap(iter_u, name=next_name)
 
-        return SingleOutputChain[T, List[U]](f"{self.name}@collect", _collect)
+        return SingleOutputChain[T, List[U]](next_name, _collect)
 
     def join(self: "Chain[T, str]", separator="") -> "SingleOutputChain[T, str]":
         """
         Joins the output of a string-producing chain into a single string.
 
         The `join` method concatenates each item in the output of the chain, using the
         provided separator between each element. This is particularly useful when working
@@ -308,31 +309,33 @@
         ...     joined_chain = capitalized_chain.join(" ")
         ...     return await join_final_output(joined_chain("this is an example"))
         ...
         >>> asyncio.run(example())
         'This Is An Example'
         """
 
+        next_name = f"{self.name}@join"
+
         async def _join(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[str, Union[U, str]], Any]:
+        ) -> AsyncGenerator[ChainOutput[str], Any]:
             # First, reyield previous chain so we never block the stream, and collect the results until they are done
             iter_u: Iterable[str] = []
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[str, Union[U, str]], to_reyield)
+                yield cast(ChainOutput[str], to_reyield)
                 iter_u = values
 
             # Then, return the joined result
             output: str = separator.join(iter_u)
-            yield cast(ChainOutput[str, Union[U, str]], output)
+            yield self._output_wrap(output, name=next_name)
 
-        return SingleOutputChain[T, str](f"{self.name}@join", _join)
+        return SingleOutputChain[T, str](next_name, _join)
 
     def gather(
-        self: "Union[Chain[T, AsyncGenerator[ChainOutput[V, W], Any]], Chain[T, AsyncGenerator[V, Any]]]",
+        self: "Union[Chain[T, AsyncGenerator[ChainOutput[V], Any]], Chain[T, AsyncGenerator[V, Any]]]",
     ) -> "SingleOutputChain[T, List[List[V]]]":
         """
         Gathers results from multiple chains and processes them in parallel.
 
         The `gather` method is used to process several chains concurrently, and it waits until all of
         them are complete before continuing. This is similar to `asyncio.gather`, and is useful when you
         want to run multiple asynchronous tasks in parallel and wait for all of them to complete.
@@ -358,25 +361,78 @@
         ...     return await collect_final_output(gathered_chain(3))
         ...
         >>> asyncio.run(example()) # will take 0.1s to finish, not 0.3s, because it runs in parallel
         ['Number: 0', 'Number: 1', 'Number: 2']
         """
         return self.collect().gather()
 
+    def on_error(
+        self,
+        handler: Callable[[Exception], Union[AsyncGenerator[ChainOutput[V], Any], V]],
+    ) -> "Chain[T, Union[U, V]]":
+        """
+        Handles any uncaught exceptions that might occur during the execution of the current chain.
+
+        The `handler` function takes an exception as its argument and returns a new value that
+        will be used as the output of the chain instead of the exception. The function can also re-raise
+        the exception or raise a new one, which will then be propagated further up the chain.
+
+        If an exception occurs in the `handler` function itself, it will be propagated without any
+        further handling.
+
+        Example:
+
+        >>> from litechain import Chain, join_final_output
+        >>> import asyncio
+        ...
+        >>> def failed_greeting(name: str):
+        ...     raise Exception(f"Giving {name} a cold shoulder")
+        ...
+        >>> async def example():
+        ...     greet_chain = Chain[str, str](
+        ...         "GreetingChain",
+        ...         failed_greeting
+        ...     ).on_error(lambda e: f"Sorry, an error occurred: {str(e)}")
+        ...
+        ...     async for output in greet_chain("Alice"):
+        ...         print(output)
+        ...
+        >>> asyncio.run(example())
+        ChainOutput(chain='GreetingChain', data=Exception('Giving Alice a cold shoulder'), final=False)
+        ChainOutput(chain='GreetingChain@on_error', data='Sorry, an error occurred: ...', final=True)
+        """
+
+        next_name = f"{self.name}@on_error"
+        if hasattr(next, "name"):
+            next_name = next.name
+
+        async def on_error(
+            input: T,
+        ) -> AsyncGenerator[ChainOutput[Union[U, V]], Any]:
+            try:
+                async for output in self(input):
+                    yield cast(ChainOutput[Union[U, V]], output)
+            except Exception as e:
+                yield cast(ChainOutput[Union[U, V]], self._output_wrap(e, final=False))
+                async for output in self._wrap(handler(e), name=next_name):
+                    yield cast(ChainOutput[Union[U, V]], output)
+
+        return Chain[T, Union[U, V]](next_name, lambda input: on_error(input))
+
 
 class SingleOutputChain(Chain[T, U]):
     """"""
 
     _call: Callable[
-        [T], Union[AsyncGenerator[ChainOutput[U, Any], Any], AsyncGenerator[U, Any], U]
+        [T], Union[AsyncGenerator[ChainOutput[U], Any], AsyncGenerator[U, Any], U]
     ]
 
     async def _reyield(
-        self, async_iterable: AsyncGenerator[ChainOutput[U, U], Any], at: str
-    ) -> AsyncGenerator[Tuple[Optional[U], ChainOutput[U, U]], Any]:
+        self, async_iterable: AsyncGenerator[ChainOutput[U], Any], at: str
+    ) -> AsyncGenerator[Tuple[Optional[U], ChainOutput[U]], Any]:
         final_value: Optional[U] = None
         async for u in async_iterable:
             u_rewrapped = self._output_wrap(u, final=False)
             if u.final:
                 if final_value is not None:
                     # TODO: try to make this happen with a bad use case, is it even breakable?
                     raise Exception(
@@ -390,95 +446,97 @@
         Similar to `Chain.map`, this method applies a function to the final output of the chain, but returns a SingleOutputChain.
 
         The `fn` parameter is a function that takes a value of type U and returns a value of type V.
 
         For detailed examples, refer to the documentation of `Chain.map`.
         """
 
-        async def map(input: T) -> AsyncGenerator[ChainOutput[V, Union[U, V]], Any]:
+        next_name = f"{self.name}@map"
+
+        async def map(input: T) -> AsyncGenerator[ChainOutput[V], Any]:
             # Reyield previous chain so we never block the stream, and at the same time yield mapped values
             final_u: Optional[U] = None
             async for value, to_reyield in self._reyield(self(input), "map"):
-                yield cast(ChainOutput[V, Union[U, V]], to_reyield)
+                yield cast(ChainOutput[V], to_reyield)
                 final_u = value
 
             if final_u is None:
                 # TODO: try to make this happen with a bad use case, is it even breakable?
                 raise Exception(
                     f"Expected item at the end of the chain, found None for {self.name}@map"
                 )
-            yield cast(ChainOutput[V, Union[U, V]], fn(final_u))
+            yield self._output_wrap(fn(final_u), name=next_name)
 
-        return SingleOutputChain[T, V](f"{self.name}@map", lambda input: map(input))
+        return SingleOutputChain[T, V](next_name, lambda input: map(input))
 
     def and_then(
         self,
         next: Callable[
             [U],
-            Union[AsyncGenerator[ChainOutput[V, W], Any], AsyncGenerator[V, Any], V],
+            Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
         ],
     ) -> "Chain[T, V]":
         """
         Similar to `Chain.and_then`, this method takes a function that receives the final output of this chain as its input and returns a new Chain.
 
         For detailed examples, refer to the documentation of `Chain.and_then`.
         """
         next_name = f"{self.name}@and_then"
         if hasattr(next, "name"):
             next_name = next.name
 
         async def and_then(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[V, Union[U, V]], Any]:
+        ) -> AsyncGenerator[ChainOutput[V], Any]:
             # First, reyield previous chain so we never block the stream, and collect the last result when it is done
             final_u: Optional[U] = None
             async for value, to_reyield in self._reyield(self(input), "and_then"):
-                yield cast(ChainOutput[V, Union[U, V]], to_reyield)
+                yield cast(ChainOutput[V], to_reyield)
                 final_u = value
 
             if final_u is None:
                 # TODO: try to make this happen with a bad use case, is it even breakable?
                 raise Exception(
                     f"Expected item at the end of the chain, found None for {self.name}@and_then"
                 )
 
             # Then, call in the next chain
             iter_v = self._wrap(next(final_u), name=next_name)
             async for v in iter_v:
-                yield cast(ChainOutput[V, Union[U, V]], v)
+                yield v
 
         return Chain[T, V](next_name, and_then)
 
     def gather(
-        self: "Union[SingleOutputChain[T, List[AsyncGenerator[ChainOutput[V, W], Any]]], SingleOutputChain[T, List[AsyncGenerator[V, Any]]]]",
+        self: "Union[SingleOutputChain[T, List[AsyncGenerator[ChainOutput[V], Any]]], SingleOutputChain[T, List[AsyncGenerator[V, Any]]]]",
     ) -> "SingleOutputChain[T, List[List[V]]]":
         """
         Similar to `Chain.gather`, this method waits for all the async generators in the list returned by the chain to finish and gathers their results in a list.
 
         For detailed examples, refer to the documentation of `Chain.gather`.
         """
 
+        next_name = f"{self.name}@gather"
+
         async def gather(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[List[List[V]], Union[U, List[List[V]]]], Any]:
+        ) -> AsyncGenerator[ChainOutput[List[List[V]]], Any]:
             # First, reyield previous chain so we never block the stream, and collect the last result when it is done
             final_u: Optional[
                 Union[
-                    List[AsyncGenerator[ChainOutput[V, W], Any]],
+                    List[AsyncGenerator[ChainOutput[V], Any]],
                     List[AsyncGenerator[V, Any]],
                 ]
             ] = None
 
             # TODO: try to work out why the type signature of self(input) is not fitting in there, it should
             async for value, to_reyield in self._reyield(
                 cast(Any, self(input)), "gather"
             ):
-                yield cast(
-                    ChainOutput[List[List[V]], Union[U, List[List[V]]]], to_reyield
-                )
+                yield cast(ChainOutput[List[List[V]]], to_reyield)
                 final_u = value
 
             if final_u is None:
                 # TODO: try to make this happen with a bad use case, is it even breakable?
                 raise Exception(
                     f"Expected item at the end of the chain, found None for {self.name}@gather"
                 )
@@ -486,29 +544,57 @@
             async def consume_async_generator(
                 generator: AsyncGenerator[X, Any],
             ) -> Iterable[X]:
                 return [item async for item in generator]
 
             # TODO: should we really wait for everything to arrive before calling asyncio gather? Can we call it during the previous reyield?
             vss: Union[
-                List[List[ChainOutput[V, W]]], List[List[V]]
+                List[List[ChainOutput[V]]], List[List[V]]
             ] = await asyncio.gather(*(consume_async_generator(gen) for gen in final_u))
 
-            clean_vss = []
+            clean_vss: List[List[V]] = []
             for vs in vss:
-                clean_vs = []
+                clean_vs: List[V] = []
                 for v in vs:
                     v_rewrapped = cast(
-                        ChainOutput[List[List[V]], Union[U, List[List[V]]]],
+                        ChainOutput[List[List[V]]],
                         self._output_wrap(v, final=False),
                     )
                     if isinstance(v, ChainOutput):
                         yield v_rewrapped
                         if v.final:
                             clean_vs.append(v.data)
                     else:
                         clean_vs.append(v)
                 clean_vss.append(clean_vs)
 
-            yield cast(ChainOutput[List[List[V]], Union[U, List[List[V]]]], clean_vss)
+            yield self._output_wrap(clean_vss, name=next_name)
+
+        return SingleOutputChain[T, List[List[V]]](next_name, gather)
 
-        return SingleOutputChain[T, List[List[V]]](f"{self.name}@gather", gather)
+    def on_error(
+        self,
+        handler: Callable[[Exception], Union[AsyncGenerator[ChainOutput[V], Any], V]],
+    ) -> "SingleOutputChain[T, Union[U, V]]":
+        """
+        Similar to `Chain.on_error`, this method handles any uncaught exceptions that might occur during the execution of the current chain.
+
+        For detailed examples, refer to the documentation of `Chain.gather`.
+        """
+
+        next_name = f"{self.name}@on_error"
+        if hasattr(next, "name"):
+            next_name = next.name
+
+        async def on_error(
+            input: T,
+        ) -> AsyncGenerator[ChainOutput[Union[U, V]], Any]:
+            try:
+                async for output in self(input):
+                    yield cast(ChainOutput[Union[U, V]], output)
+            except Exception as e:
+                async for output in self._wrap(handler(e), name=next_name):
+                    yield cast(ChainOutput[Union[U, V]], output)
+
+        return SingleOutputChain[T, Union[U, V]](
+            next_name, lambda input: on_error(input)
+        )
```

### Comparing `litechain-0.1.3/litechain/utils/async_generator.py` & `litechain-0.1.4/litechain/utils/async_generator.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.3/litechain/utils/chain.py` & `litechain-0.1.4/litechain/utils/chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from litechain.utils.async_generator import collect, join
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 def debug(
-    chain: Callable[[T], AsyncGenerator[ChainOutput[U, Any], Any]]
+    chain: Callable[[T], AsyncGenerator[ChainOutput[U], Any]]
 ) -> Chain[T, U]:
     """
     A helper for helping you debugging chains. Simply wrap any piece of the chain or the whole chain together
     with the `debug` function to print out everything that goes through it and its nested chains.
 
     For example, you can wrap the whole chain to debug everything:
     >>> from litechain import Chain, join_final_output
@@ -34,18 +34,14 @@
     >>> asyncio.run(debug_whole_chain())
     <BLANKLINE>
     <BLANKLINE>
     \x1b[32m> GreetingChain\x1b[39m
     <BLANKLINE>
     Hello, Alice!
     <BLANKLINE>
-    \x1b[32m> GreetingChain@join\x1b[39m
-    <BLANKLINE>
-    Hello, Alice!
-    <BLANKLINE>
     \x1b[32m> PoliteChain\x1b[39m
     <BLANKLINE>
     Hello, Alice! How are you?
 
     Or, alternatively, you can debug just a piece of it:
     >>> from litechain import Chain, join_final_output
     >>> import asyncio
@@ -60,39 +56,47 @@
     <BLANKLINE>
     <BLANKLINE>
     \x1b[32m> GreetingChain\x1b[39m
     <BLANKLINE>
     Hello, Alice!
     """
 
-    async def debug(input: T) -> AsyncGenerator[ChainOutput[U, Any], Any]:
+    async def debug(input: T) -> AsyncGenerator[ChainOutput[U], Any]:
         last_chain = ""
+        last_output = ""
         async for output in chain(input):
+            if output.chain != last_chain and last_output == output.data:
+                yield output
+                continue
+
             if output.chain != last_chain:
                 print("\n", end="", flush=True)
                 last_chain = output.chain
                 print(f"\n{Fore.GREEN}> {output.chain}{Fore.RESET}\n")
             if hasattr(output.data, "__chain_debug__"):
-                output.data.__chain_debug__()
+                output.data.__chain_debug__() # type: ignore
+            elif isinstance(output.data, Exception):
+                print(f"{Fore.RED}Exception:{Fore.RESET} {output.data}", end="")
             else:
                 print(
                     output.data,
                     end=("" if isinstance(output.data, str) else ", "),
                     flush=True,
                 )
+            last_output = output.data
             yield output
 
     next_name = f"@debug"
     if hasattr(next, "name"):
         next_name = f"{next.name}@debug"
     return Chain[T, U](next_name, debug)
 
 
 async def filter_final_output(
-    async_iterable: AsyncGenerator[ChainOutput[T, Any], Any]
+    async_iterable: AsyncGenerator[ChainOutput[T], Any]
 ) -> AsyncGenerator[T, Any]:
     """
     Filters only the final output values of a Chain's outputs.
 
     Example
     -------
     >>> from litechain import Chain, filter_final_output
@@ -118,15 +122,15 @@
     """
     async for output in async_iterable:
         if output.final:
             yield cast(T, output.data)
 
 
 async def collect_final_output(
-    async_iterable: AsyncGenerator[ChainOutput[T, Any], Any]
+    async_iterable: AsyncGenerator[ChainOutput[T], Any]
 ) -> Iterable[T]:
     """
     Blocks the chain until it is done, then joins the final output values into a single list.
 
     Example
     -------
     >>> from litechain import Chain, as_async_generator, collect_final_output
@@ -149,15 +153,15 @@
     >>> asyncio.run(collected_outputs())
     ['Hello, ', 'Alice', '!']
     """
     return await collect(filter_final_output(async_iterable))
 
 
 async def join_final_output(
-    async_iterable: AsyncGenerator[ChainOutput[str, Any], Any]
+    async_iterable: AsyncGenerator[ChainOutput[str], Any]
 ) -> str:
     """
     Blocks a string producing chain until it is done, then joins the final output values into a single string.
 
     Example
     -------
     >>> from litechain import Chain, as_async_generator, join_final_output
```

### Comparing `litechain-0.1.3/litechain.egg-info/PKG-INFO` & `litechain-0.1.4/litechain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.3
+Version: 0.1.4
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
@@ -147,15 +147,14 @@
 [![Join our Discord community](https://img.shields.io/badge/Join-Discord-7289DA.svg)](https://discord.gg/AmEMWmFG)
 
 # 🚙 Roadmap
 
 - [ ] Add an example for document retrieval using vector search
 - [ ] Add a `filter` function
 - [ ] Add docs for debugging
-- [ ] Add default error handling
 - [ ] Add a simple default memory mechanism
 
 # 🙋 Contributing
 
 As a very new project in a rapidly developing field LiteChain is extremely open to contributions, we need a lot of help with integrations, documentation and guides content, feel free to send MRs and open issues. The project is very easy to run (check out the Makefile, it's all you need), but more complete contibuting guidelines to be written (we need help with that too!)
 
 If you want to help me pay the bills and keep developing this project, you can:
```

### Comparing `litechain-0.1.3/litechain.egg-info/SOURCES.txt` & `litechain-0.1.4/litechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litechain-0.1.3/setup.py` & `litechain-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="litechain",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=requirements,
     author="Rogerio Chaves",
     author_email="rogeriocfj@gmail.com",
     description="Build robust LLM applications with true composability 🔗",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

