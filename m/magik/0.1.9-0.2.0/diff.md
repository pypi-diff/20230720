# Comparing `tmp/magik-0.1.9.tar.gz` & `tmp/magik-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.1.9.tar", last modified: Wed Jul 19 22:33:08 2023, max compression
+gzip compressed data, was "magik-0.2.0.tar", last modified: Thu Jul 20 20:10:31 2023, max compression
```

## Comparing `magik-0.1.9.tar` & `magik-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-19 22:33:08.653221 magik-0.1.9/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6687 2023-07-19 22:33:08.653096 magik-0.1.9/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6261 2023-07-18 19:16:46.000000 magik-0.1.9/README.md
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-19 22:33:08.651775 magik-0.1.9/magik/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.1.9/magik/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2478 2023-07-18 22:08:35.000000 magik-0.1.9/magik/cli.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-18 22:08:46.000000 magik-0.1.9/magik/config.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      587 2023-07-18 19:22:52.000000 magik-0.1.9/magik/constants.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      617 2023-07-19 22:20:55.000000 magik-0.1.9/magik/decorators.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1403 2023-07-18 22:08:54.000000 magik-0.1.9/magik/deploy.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)    11036 2023-07-18 22:46:27.000000 magik-0.1.9/magik/evaluators.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-19 22:33:08.652838 magik-0.1.9/magik/examples/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.1.9/magik/examples/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1295 2023-07-19 21:31:34.000000 magik-0.1.9/magik/examples/assertions.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1385 2023-07-19 21:29:31.000000 magik-0.1.9/magik/generate.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2161 2023-07-18 22:09:06.000000 magik-0.1.9/magik/initialize.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.1.9/magik/internal_logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      608 2023-07-18 22:09:18.000000 magik-0.1.9/magik/logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.9/magik/matchers.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1043 2023-07-18 22:09:25.000000 magik-0.1.9/magik/openai_helper.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     8190 2023-07-18 22:22:50.000000 magik-0.1.9/magik/run.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-18 22:09:43.000000 magik-0.1.9/magik/sys_exec.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1539 2023-07-18 22:13:16.000000 magik-0.1.9/magik/utils.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-19 22:33:08.652635 magik-0.1.9/magik.egg-info/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6687 2023-07-19 22:33:08.000000 magik-0.1.9/magik.egg-info/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      538 2023-07-19 22:33:08.000000 magik-0.1.9/magik.egg-info/SOURCES.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-19 22:33:08.000000 magik-0.1.9/magik.egg-info/dependency_links.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-19 22:33:08.000000 magik-0.1.9/magik.egg-info/entry_points.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-19 22:33:08.000000 magik-0.1.9/magik.egg-info/requires.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-19 22:33:08.000000 magik-0.1.9/magik.egg-info/top_level.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-19 22:33:08.653258 magik-0.1.9/setup.cfg
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-19 22:32:29.000000 magik-0.1.9/setup.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-20 20:10:31.270813 magik-0.2.0/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6006 2023-07-20 20:10:31.270652 magik-0.2.0/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     5580 2023-07-19 22:37:02.000000 magik-0.2.0/README.md
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-20 20:10:31.269606 magik-0.2.0/magik/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.2.0/magik/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1844 2023-07-20 17:04:56.000000 magik-0.2.0/magik/classifier.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2478 2023-07-19 22:36:56.000000 magik-0.2.0/magik/cli.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-20 08:24:46.000000 magik-0.2.0/magik/config.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      587 2023-07-18 19:22:52.000000 magik-0.2.0/magik/constants.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      617 2023-07-19 22:36:56.000000 magik-0.2.0/magik/decorators.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1403 2023-07-19 22:36:56.000000 magik-0.2.0/magik/deploy.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)    12700 2023-07-20 19:58:37.000000 magik-0.2.0/magik/evaluators.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-20 20:10:31.270496 magik-0.2.0/magik/examples/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.2.0/magik/examples/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1295 2023-07-19 22:36:56.000000 magik-0.2.0/magik/examples/assertions.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1385 2023-07-19 22:36:56.000000 magik-0.2.0/magik/generate.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2161 2023-07-19 22:36:56.000000 magik-0.2.0/magik/initialize.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.2.0/magik/internal_logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      895 2023-07-20 20:01:05.000000 magik-0.2.0/magik/logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.2.0/magik/matchers.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1248 2023-07-20 12:39:03.000000 magik-0.2.0/magik/openai_helper.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     8190 2023-07-20 20:02:29.000000 magik-0.2.0/magik/run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      897 2023-07-20 12:53:40.000000 magik-0.2.0/magik/similarity.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-19 22:36:56.000000 magik-0.2.0/magik/sys_exec.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1539 2023-07-19 22:36:56.000000 magik-0.2.0/magik/utils.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-20 20:10:31.270301 magik-0.2.0/magik.egg-info/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6006 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      578 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/SOURCES.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/dependency_links.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/entry_points.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/requires.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-20 20:10:31.000000 magik-0.2.0/magik.egg-info/top_level.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-20 20:10:31.270850 magik-0.2.0/setup.cfg
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-20 20:08:26.000000 magik-0.2.0/setup.py
```

### Comparing `magik-0.1.9/PKG-INFO` & `magik-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.9
+Version: 0.2.0
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -72,15 +72,15 @@
 ---
 
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
 For example, assuming your prompt looks like this:
 
 ```
-Create some marketing copy for a tweet of less than {num_chars} characters for my app {name}.
+Create some marketing copy for a tweet of less than 280 characters for my app {app_name}.
 
 My app helps people generate sales emails using AI. 
 
 Make sure the marketing copy contains a complete and valid link to my app. 
 
 Here is the link to my app: https://magiklabs.app.
 ```
@@ -88,80 +88,59 @@
 You can write tests like this:
 
 ```python
 from magik.evaluators import (
     contains_none,
     contains_link,
     contains_valid_link,
-    not_contains_pii,
     is_positive_sentiment,
     length_less_than,
-    contains,
-    negate,
 )
 
 
-def is_hallucination(output):
-    return {"result": False, "reason": "Custom reason for is_hallucination"}
-
 
 # Define tests here
 tests = [
     {
-        # contains_link(output)
         "description": "output contains a link",
-        "eval_function": contains_link,
-        "eval_function_args": [],
+        "eval": contains_link(),
         "prompt_vars": {
-            "name": "Uber",
-            "num_chars": 280,
+            "app_name": "Uber",
         },
         "failure_labels": ["bad_response_format"],
     },
     {
-        # contains_valid_link(output)
         "description": "output contains a valid link",
-        "eval_function": contains_valid_link,
-        "eval_function_args": [],
+        "eval": contains_valid_link(),
         "prompt_vars": {
-            "name": "Magik",
-            "num_chars": 280,
+            "app_name": "Magik",
         },
         "failure_labels": ["bad_response_format"],
     },
     {
-        # is_positive_sentiment(output)
         "description": "output sentiment is positive",
-        "eval_function": is_positive_sentiment,
-        "eval_function_args": [],
+        "eval": is_positive_sentiment(),
         "prompt_vars": {
-            "name": "Lyft",
-            "num_chars": 280,
+            "app_name": "Lyft",
         },
         "failure_labels": ["negative_sentiment"],
     },
     {
-        # length_less_than(output, 280)
         "description": "output length is less than 280 characters",
-        "eval_function": length_less_than,
-        "eval_function_args": [280],
+        "eval": length_less_than(280),
         "prompt_vars": {
-            "name": "Facebook",
-            "num_chars": 280,
+            "app_name": "Facebook",
         },
         "failure_labels": ["negative_sentiment", "critical"],
     },
     {
-        # contains_all(output, ["#"])
         "description": "output does not contain hashtags",
-        "eval_function": contains_none,
-        "eval_function_args": ["#"],
+        "eval": contains_none(['#']),
         "prompt_vars": {
-            "name": "Datadog",
-            "num_chars": 280,
+            "app_name": "Datadog",
         },
         "failure_labels": ["bad_response_format"],
     },
 ]
 ```
 
 <br /><br />
```

### Comparing `magik-0.1.9/README.md` & `magik-0.2.0/magik.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: magik
+Version: 0.2.0
+Summary: SDK to write and run tests for your LLM app
+Home-page: UNKNOWN
+Author: Magik Labs Team
+Author-email: hello@magiklabs.app
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 _Magik is an LLM output testing SDK + observability platform that helps you write tests and monitor your app in production_.
 <br /><br />
 
 # Overview
 
 Reliability of output is one of the biggest challenges for people trying to use LLM apps in production.<br />
 
@@ -57,15 +72,15 @@
 ---
 
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
 For example, assuming your prompt looks like this:
 
 ```
-Create some marketing copy for a tweet of less than {num_chars} characters for my app {name}.
+Create some marketing copy for a tweet of less than 280 characters for my app {app_name}.
 
 My app helps people generate sales emails using AI. 
 
 Make sure the marketing copy contains a complete and valid link to my app. 
 
 Here is the link to my app: https://magiklabs.app.
 ```
@@ -73,80 +88,59 @@
 You can write tests like this:
 
 ```python
 from magik.evaluators import (
     contains_none,
     contains_link,
     contains_valid_link,
-    not_contains_pii,
     is_positive_sentiment,
     length_less_than,
-    contains,
-    negate,
 )
 
 
-def is_hallucination(output):
-    return {"result": False, "reason": "Custom reason for is_hallucination"}
-
 
 # Define tests here
 tests = [
     {
-        # contains_link(output)
         "description": "output contains a link",
-        "eval_function": contains_link,
-        "eval_function_args": [],
+        "eval": contains_link(),
         "prompt_vars": {
-            "name": "Uber",
-            "num_chars": 280,
+            "app_name": "Uber",
         },
         "failure_labels": ["bad_response_format"],
     },
     {
-        # contains_valid_link(output)
         "description": "output contains a valid link",
-        "eval_function": contains_valid_link,
-        "eval_function_args": [],
+        "eval": contains_valid_link(),
         "prompt_vars": {
-            "name": "Magik",
-            "num_chars": 280,
+            "app_name": "Magik",
         },
         "failure_labels": ["bad_response_format"],
     },
     {
-        # is_positive_sentiment(output)
         "description": "output sentiment is positive",
-        "eval_function": is_positive_sentiment,
-        "eval_function_args": [],
+        "eval": is_positive_sentiment(),
         "prompt_vars": {
-            "name": "Lyft",
-            "num_chars": 280,
+            "app_name": "Lyft",
         },
         "failure_labels": ["negative_sentiment"],
     },
     {
-        # length_less_than(output, 280)
         "description": "output length is less than 280 characters",
-        "eval_function": length_less_than,
-        "eval_function_args": [280],
+        "eval": length_less_than(280),
         "prompt_vars": {
-            "name": "Facebook",
-            "num_chars": 280,
+            "app_name": "Facebook",
         },
         "failure_labels": ["negative_sentiment", "critical"],
     },
     {
-        # contains_all(output, ["#"])
         "description": "output does not contain hashtags",
-        "eval_function": contains_none,
-        "eval_function_args": ["#"],
+        "eval": contains_none(['#']),
         "prompt_vars": {
-            "name": "Datadog",
-            "num_chars": 280,
+            "app_name": "Datadog",
         },
         "failure_labels": ["bad_response_format"],
     },
 ]
 ```
 
 <br /><br />
@@ -183,7 +177,9 @@
 - Set up alerts to notify you about critical errors in production.
 
 <br /><br />
 
 # Platform
 
 Contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app) to get access to our LLM observability platform where you can run the tests you've defined here against your LLM responses in production.
+
+
```

### Comparing `magik-0.1.9/magik/cli.py` & `magik-0.2.0/magik/cli.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/constants.py` & `magik-0.2.0/magik/constants.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/decorators.py` & `magik-0.2.0/magik/decorators.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/deploy.py` & `magik-0.2.0/magik/deploy.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/evaluators.py` & `magik-0.2.0/magik/evaluators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Contains functions to evaluate assertions.
 import requests
 import json
 import re
 import ast
+import numpy as np
 from magik.openai_helper import OpenAI
 from magik.utils import standardize_url, generate_grading_prompt
 from magik.constants import OPEN_AI_DEFAULT_MODEL
 from magik.decorators import magik_eval
+from magik.similarity import similarity_score
+from magik.classifier import classify_output
 
 
 @magik_eval
 def equals(expected_output, case_sensitive=False, output_to_test=None):
     if case_sensitive == False:
         output_to_test = output_to_test.lower()
         expected_output = expected_output.lower()
@@ -332,7 +335,60 @@
             "reason": "Output contains JSON",
         }
     else:
         return {
             "result": False,
             "reason": "Output does not contain JSON",
         }
+
+
+@magik_eval
+def cosine_similarity_above_threshold(
+    compare_against: str,
+    threshold: float,
+    model="text-embedding-ada-002",
+    output_to_test=None,
+):
+    score = similarity_score(output_to_test, compare_against, model)
+    print(f"score is {score}")
+    result = score > threshold
+    return {
+        "result": result,
+        "reason": f"cosine similarity score is {score} and is above threshold {threshold}",
+    }
+
+
+@magik_eval
+def cosine_similarity_below_threshold(
+    compare_against: str,
+    threshold: float,
+    model="text-embedding-ada-002",
+    output_to_test=None,
+):
+    score = similarity_score(output_to_test, compare_against, model)
+    print(f"score is {score}")
+    result = score < threshold
+    return {
+        "result": result,
+        "reason": f"cosine similarity score is {score} and is below threshold {threshold}",
+    }
+
+
+@magik_eval
+def matches_desired_classification(
+    classification_labels_and_descriptions: list[dict],
+    input_description: str,
+    task_description: str,
+    desired_classification_label: str,
+    output_to_test=None,
+):
+    label = classify_output(
+        classification_labels_and_descriptions=classification_labels_and_descriptions,
+        input_description=input_description,
+        task_description=task_description,
+        output_to_test=output_to_test,
+    )
+    result = label == desired_classification_label
+    return {
+        "result": result,
+        "reason": f"output is classified as {label} and desired classification is {desired_classification_label}",
+    }
```

### Comparing `magik-0.1.9/magik/examples/assertions.py` & `magik-0.2.0/magik/examples/assertions.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/generate.py` & `magik-0.2.0/magik/generate.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/initialize.py` & `magik-0.2.0/magik/initialize.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/internal_logger.py` & `magik-0.2.0/magik/internal_logger.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/openai_helper.py` & `magik-0.2.0/magik/openai_helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,7 +25,12 @@
     def openai_chat_completion_message(self, model, prompt):
         """
         Call the OpenAI API to generate a chat completion for models like GPT 3.5 turbo and GPT 4
         Returns just the message content string
         """
         response = self.openai_chat_completion(model, prompt)
         return response.choices[0].message.content
+
+    def get_embedding(self, text: str, model="text-embedding-ada-002") -> list[float]:
+        return self.openai.Embedding.create(input=[text], model=model)["data"][0][
+            "embedding"
+        ]
```

### Comparing `magik-0.1.9/magik/run.py` & `magik-0.2.0/magik/run.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/sys_exec.py` & `magik-0.2.0/magik/sys_exec.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik/utils.py` & `magik-0.2.0/magik/utils.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.9/magik.egg-info/PKG-INFO` & `magik-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: magik
-Version: 0.1.9
-Summary: SDK to write and run tests for your LLM app
-Home-page: UNKNOWN
-Author: Magik Labs Team
-Author-email: hello@magiklabs.app
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 _Magik is an LLM output testing SDK + observability platform that helps you write tests and monitor your app in production_.
 <br /><br />
 
 # Overview
 
 Reliability of output is one of the biggest challenges for people trying to use LLM apps in production.<br />
 
@@ -72,15 +57,15 @@
 ---
 
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
 For example, assuming your prompt looks like this:
 
 ```
-Create some marketing copy for a tweet of less than {num_chars} characters for my app {name}.
+Create some marketing copy for a tweet of less than 280 characters for my app {app_name}.
 
 My app helps people generate sales emails using AI. 
 
 Make sure the marketing copy contains a complete and valid link to my app. 
 
 Here is the link to my app: https://magiklabs.app.
 ```
@@ -88,80 +73,59 @@
 You can write tests like this:
 
 ```python
 from magik.evaluators import (
     contains_none,
     contains_link,
     contains_valid_link,
-    not_contains_pii,
     is_positive_sentiment,
     length_less_than,
-    contains,
-    negate,
 )
 
 
-def is_hallucination(output):
-    return {"result": False, "reason": "Custom reason for is_hallucination"}
-
 
 # Define tests here
 tests = [
     {
-        # contains_link(output)
         "description": "output contains a link",
-        "eval_function": contains_link,
-        "eval_function_args": [],
+        "eval": contains_link(),
         "prompt_vars": {
-            "name": "Uber",
-            "num_chars": 280,
+            "app_name": "Uber",
         },
         "failure_labels": ["bad_response_format"],
     },
     {
-        # contains_valid_link(output)
         "description": "output contains a valid link",
-        "eval_function": contains_valid_link,
-        "eval_function_args": [],
+        "eval": contains_valid_link(),
         "prompt_vars": {
-            "name": "Magik",
-            "num_chars": 280,
+            "app_name": "Magik",
         },
         "failure_labels": ["bad_response_format"],
     },
     {
-        # is_positive_sentiment(output)
         "description": "output sentiment is positive",
-        "eval_function": is_positive_sentiment,
-        "eval_function_args": [],
+        "eval": is_positive_sentiment(),
         "prompt_vars": {
-            "name": "Lyft",
-            "num_chars": 280,
+            "app_name": "Lyft",
         },
         "failure_labels": ["negative_sentiment"],
     },
     {
-        # length_less_than(output, 280)
         "description": "output length is less than 280 characters",
-        "eval_function": length_less_than,
-        "eval_function_args": [280],
+        "eval": length_less_than(280),
         "prompt_vars": {
-            "name": "Facebook",
-            "num_chars": 280,
+            "app_name": "Facebook",
         },
         "failure_labels": ["negative_sentiment", "critical"],
     },
     {
-        # contains_all(output, ["#"])
         "description": "output does not contain hashtags",
-        "eval_function": contains_none,
-        "eval_function_args": ["#"],
+        "eval": contains_none(['#']),
         "prompt_vars": {
-            "name": "Datadog",
-            "num_chars": 280,
+            "app_name": "Datadog",
         },
         "failure_labels": ["bad_response_format"],
     },
 ]
 ```
 
 <br /><br />
@@ -198,9 +162,7 @@
 - Set up alerts to notify you about critical errors in production.
 
 <br /><br />
 
 # Platform
 
 Contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app) to get access to our LLM observability platform where you can run the tests you've defined here against your LLM responses in production.
-
-
```

### Comparing `magik-0.1.9/magik.egg-info/SOURCES.txt` & `magik-0.2.0/magik.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 README.md
 setup.py
 magik/__init__.py
+magik/classifier.py
 magik/cli.py
 magik/config.py
 magik/constants.py
 magik/decorators.py
 magik/deploy.py
 magik/evaluators.py
 magik/generate.py
 magik/initialize.py
 magik/internal_logger.py
 magik/logger.py
 magik/matchers.py
 magik/openai_helper.py
 magik/run.py
+magik/similarity.py
 magik/sys_exec.py
 magik/utils.py
 magik.egg-info/PKG-INFO
 magik.egg-info/SOURCES.txt
 magik.egg-info/dependency_links.txt
 magik.egg-info/entry_points.txt
 magik.egg-info/requires.txt
```

### Comparing `magik-0.1.9/setup.py` & `magik-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="magik",
-    version="0.1.9",
+    version="0.2.0",
     author="Magik Labs Team",
     author_email="hello@magiklabs.app",
     description="SDK to write and run tests for your LLM app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

