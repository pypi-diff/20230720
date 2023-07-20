# Comparing `tmp/easycompletion-0.2.5.tar.gz` & `tmp/easycompletion-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.2.5.tar", last modified: Tue Jul 18 14:21:26 2023, max compression
+gzip compressed data, was "easycompletion-0.2.6.tar", last modified: Thu Jul 20 13:29:23 2023, max compression
```

## Comparing `easycompletion-0.2.5.tar` & `easycompletion-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:26.096496 easycompletion-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 14:21:14.000000 easycompletion-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-18 14:21:26.096496 easycompletion-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-18 14:21:14.000000 easycompletion-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:26.096496 easycompletion-0.2.5/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-18 14:21:14.000000 easycompletion-0.2.5/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 14:21:14.000000 easycompletion-0.2.5/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-07-18 14:21:14.000000 easycompletion-0.2.5/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-18 14:21:14.000000 easycompletion-0.2.5/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:26.096496 easycompletion-0.2.5/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-18 14:21:26.000000 easycompletion-0.2.5/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-18 14:21:26.000000 easycompletion-0.2.5/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:21:26.000000 easycompletion-0.2.5/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 14:21:26.000000 easycompletion-0.2.5/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 14:21:26.000000 easycompletion-0.2.5/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:21:26.096496 easycompletion-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-18 14:21:14.000000 easycompletion-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:29:23.053725 easycompletion-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-20 13:29:10.000000 easycompletion-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-20 13:29:23.053725 easycompletion-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-20 13:29:10.000000 easycompletion-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:29:23.049725 easycompletion-0.2.6/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-20 13:29:10.000000 easycompletion-0.2.6/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-20 13:29:10.000000 easycompletion-0.2.6/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-07-20 13:29:10.000000 easycompletion-0.2.6/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-20 13:29:10.000000 easycompletion-0.2.6/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:29:23.053725 easycompletion-0.2.6/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:29:23.053725 easycompletion-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-20 13:29:10.000000 easycompletion-0.2.6/setup.py
```

### Comparing `easycompletion-0.2.5/LICENSE` & `easycompletion-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.5/PKG-INFO` & `easycompletion-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.5
+Version: 0.2.6
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.2.5/README.md` & `easycompletion-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.5/easycompletion/__init__.py` & `easycompletion-0.2.6/easycompletion/__init__.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.5/easycompletion/model.py` & `easycompletion-0.2.6/easycompletion/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,19 @@
 
     Returns:
         True if function call matches with the response, False otherwise.
 
     Usage:
         isValid = validate_functions(response, functions, function_call)
     """
-    # Extract the function call from the response
-    response_function_call = response["choices"][0]["message"]["function_call"]
+    response_function_call = response["choices"][0]["message"].get(
+        "function_call", None
+    )
+    if response_function_call is None:
+        return False
 
     # If function_call is not "auto" and the name does not match with the response, return False
     if (
         function_call != "auto"
         and response_function_call["name"] != function_call["name"]
     ):
         return False
@@ -189,15 +192,17 @@
     # Count tokens in the input text
     total_tokens = count_tokens(text, model=model)
 
     # If text is longer than chunk_length and model is not for long texts, switch to the long text model
     if total_tokens > chunk_length and "16k" not in model:
         model = long_text_model
         if not os.environ.get("SUPPRESS_WARNINGS"):
-            print("Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)")
+            print(
+                "Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)"
+            )
 
     # If text is too long even for long text model, return None
     if total_tokens > (16384 - chunk_length):
         print("Error: Message too long")
         return {
             "text": None,
             usage: None,
@@ -337,15 +342,17 @@
         function_call_tokens = count_tokens(functions, model=model)
         total_tokens += function_call_tokens + 3  # Additional tokens for the user
 
     # Switch to a larger model if the message is too long for the default model
     if total_tokens > chunk_length and "16k" not in model:
         model = long_text_model
         if not os.environ.get("SUPPRESS_WARNINGS"):
-            print("Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)")
+            print(
+                "Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)"
+            )
 
     # Check if the total number of tokens exceeds the maximum allowable tokens for the model
     if total_tokens > (16384 - chunk_length):
         return {"error": "Message too long"}
 
     # Prepare the messages to be sent to the API
     messages = [{"role": "user", "content": text}]
```

### Comparing `easycompletion-0.2.5/easycompletion/prompt.py` & `easycompletion-0.2.6/easycompletion/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,24 +141,30 @@
         compose_prompt("Hello {{name}}!", {"name": "John"})
         Output: "Hello John!"
     """
     prompt = prompt_template  # Initial prompt template.
 
     # Replacing placeholders in the template with the actual values from the parameters.
     for key, value in parameters.items():
-        if isinstance(value, str):
-            prompt = prompt.replace("{{" + key + "}}", value)
-        elif isinstance(value, int):
-            prompt = prompt.replace("{{" + key + "}}", str(value))
-        elif isinstance(value, dict):
-            for k, v in value.items():
-                prompt = prompt.replace("{{" + key + "}}", k + "::" + v)
-        elif isinstance(value, list):
-            for item in value:
-                prompt = prompt.replace("{{" + key + "}}", item + "\n")
-        elif value is None:
-            prompt = prompt.replace("{{" + key + "}}", "None")
-        else:
-            print("ERROR PARSING")
-            sys.exit(1)
+            # check if "{{" + key + "}}" is in prompt
+            # if not, continue
+            if "{{" + key + "}}" not in prompt:
+                continue
+            try:
+                if isinstance(value, str):
+                    prompt = prompt.replace("{{" + key + "}}", value)
+                elif isinstance(value, int):
+                    prompt = prompt.replace("{{" + key + "}}", str(value))
+                elif isinstance(value, dict):
+                    for k, v in value.items():
+                        prompt = prompt.replace("{{" + key + "}}", k + "::" + v)
+                elif isinstance(value, list):
+                    for item in value:
+                        prompt = prompt.replace("{{" + key + "}}", item + "\n")
+                elif value is None:
+                    prompt = prompt.replace("{{" + key + "}}", "None")
+                else:
+                    raise Exception(f"ERROR PARSING:\n{key}\n{value}")
+            except:
+                raise Exception(f"ERROR PARSING:\n{key}\n{value}")
 
     return prompt
```

### Comparing `easycompletion-0.2.5/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.2.6/easycompletion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.5
+Version: 0.2.6
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.2.5/setup.py` & `easycompletion-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.2.5',
+    version='0.2.6',
     description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

