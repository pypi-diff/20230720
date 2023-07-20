# Comparing `tmp/llfn-0.1.0.tar.gz` & `tmp/llfn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llfn-0.1.0.tar", max compression
+gzip compressed data, was "llfn-0.1.1.tar", max compression
```

## Comparing `llfn-0.1.0.tar` & `llfn-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1264 2023-07-19 09:18:10.103949 llfn-0.1.0/README.md
--rw-r--r--   0        0        0       93 2023-07-19 09:14:19.148491 llfn-0.1.0/llfn/__init__.py
--rw-r--r--   0        0        0     1267 2023-07-19 09:34:08.324835 llfn-0.1.0/llfn/llfn.py
--rw-r--r--   0        0        0      342 2023-07-20 10:38:52.607092 llfn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1787 1970-01-01 00:00:00.000000 llfn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1187 2023-07-20 10:51:32.176634 llfn-0.1.1/README.md
+-rw-r--r--   0        0        0       43 2023-07-20 10:49:19.230094 llfn-0.1.1/llfn/__init__.py
+-rw-r--r--   0        0        0     1334 2023-07-20 10:49:48.534775 llfn-0.1.1/llfn/llfn.py
+-rw-r--r--   0        0        0      342 2023-07-20 10:51:52.819654 llfn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 llfn-0.1.1/PKG-INFO
```

### Comparing `llfn-0.1.0/README.md` & `llfn-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,31 @@
 TBD
 
 ## How to use
 
 ````py
 import dotenv
 import os
-from llfn import prompt_function, global_bind
+from llfn import LLFn
 from langchain.chat_models import ChatOpenAI
 
+
+prompt_function = LLFn()
+
+
 @prompt_function
 def translate(text: str, to_language: str) -> str:
     return f"""
 You must automatically detect the language of the following text and tranlate it to {to_language}
 ```
 {text}
 ```
 """
 
+
 @prompt_function
 def summarize(text: str, length: int) -> str:
     return f"""
 You must summarize the following text to a smaller text approximately {length} words long
 ```
 {text}
 ```
@@ -31,18 +36,17 @@
 if __name__ == "__main__":
     dotenv.load_dotenv()
     llm = ChatOpenAI(
         temperature=0.8,
         model=os.getenv("OPENAI_MODEL"),
         openai_api_key=os.getenv("OPENAI_API_KEY"),
     )  # type: ignore
-    global_bind(llm)
+    prompt_function.bind(llm)
     print(translate("สวัสดีตอนเช้าครับ อยากรับประทานอะไรดีครับเช้าวันนี้", "english"))
     print(summarize("I love my dogs. They are corgis. They love nuggets", 4))
 ````
 
 ```sh
-$ poetry run python example.py                                                                                [16:15:28]
-
+$ poetry run python example.py
 # Good morning, what would you like to have for breakfast today?
 # I love corgi dogs
 ```
```

### Comparing `llfn-0.1.0/llfn/llfn.py` & `llfn-0.1.1/llfn/llfn.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import json
-from functools import update_wrapper
+from functools import update_wrapper, wraps
 from langchain.chat_models import ChatOpenAI
 from langchain.schema import HumanMessage, SystemMessage
 
 
-llm: None | ChatOpenAI = None
-
-
-def global_bind(llm_: ChatOpenAI):
-    global llm
-    llm = llm_
-
-
-class prompt_function:
-    def __init__(self, f):
-        self.f = f
-        update_wrapper(self, f)
-
-    def __call__(self, *args, **kwargs):
-        prompt = self.f(*args, **kwargs)
-        if llm is None:
-            raise ValueError("You must call global_bind before calling prompt_function")
-        output = llm.predict_messages(
-            [
-                SystemMessage(
-                    content=f"""
+class LLFn:
+    def __init__(self):
+        self.llm = None
+
+    def bind(self, llm):
+        self.llm = llm
+
+    def __call__(self, f):
+        @wraps(f)
+        def wrapper(*args, **kwargs):
+            prompt = f(*args, **kwargs)
+            if self.llm is None:
+                raise ValueError(
+                    "You must call global_bind before calling prompt_function"
+                )
+            output = self.llm.predict_messages(
+                [
+                    SystemMessage(
+                        content=f"""
 - You must execute the user command and convert it to exactly one single output. Let's call it X
-- X MUST have Python type of `{self.f.__annotations__['return']}`
+- X MUST have Python type of `{f.__annotations__['return']}`
 - You then MUST output the JSON of X using Python's `json.dumps`
 - Executing `json.loads` on the output of your function MUST give exactly X
 - You MUST NOT output anything else. No need to provide output context
 
 - For example, if type is `str` you can output `"Hello"` BUT NOT `{{"result": "Hello"}}`
 """
-                ),
-                HumanMessage(content=prompt),
-            ]
-        )
+                    ),
+                    HumanMessage(content=prompt),
+                ]
+            )
+            return json.loads(output.content)
 
-        return json.loads(output.content)
+        return wrapper
```

### Comparing `llfn-0.1.0/PKG-INFO` & `llfn-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llfn
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,26 +19,31 @@
 TBD
 
 ## How to use
 
 ````py
 import dotenv
 import os
-from llfn import prompt_function, global_bind
+from llfn import LLFn
 from langchain.chat_models import ChatOpenAI
 
+
+prompt_function = LLFn()
+
+
 @prompt_function
 def translate(text: str, to_language: str) -> str:
     return f"""
 You must automatically detect the language of the following text and tranlate it to {to_language}
 ```
 {text}
 ```
 """
 
+
 @prompt_function
 def summarize(text: str, length: int) -> str:
     return f"""
 You must summarize the following text to a smaller text approximately {length} words long
 ```
 {text}
 ```
@@ -47,18 +52,17 @@
 if __name__ == "__main__":
     dotenv.load_dotenv()
     llm = ChatOpenAI(
         temperature=0.8,
         model=os.getenv("OPENAI_MODEL"),
         openai_api_key=os.getenv("OPENAI_API_KEY"),
     )  # type: ignore
-    global_bind(llm)
+    prompt_function.bind(llm)
     print(translate("สวัสดีตอนเช้าครับ อยากรับประทานอะไรดีครับเช้าวันนี้", "english"))
     print(summarize("I love my dogs. They are corgis. They love nuggets", 4))
 ````
 
 ```sh
-$ poetry run python example.py                                                                                [16:15:28]
-
+$ poetry run python example.py
 # Good morning, what would you like to have for breakfast today?
 # I love corgi dogs
 ```
```

